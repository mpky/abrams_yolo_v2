# YOLO v2 Applied to M1 Abrams Tanks

#### Project Goal

Using [thrieu's darkflow](https://github.com/thtrieu/darkflow) and following [markjay4k's walkthrough](https://github.com/markjay4k/YOLO-series), train a custom set of YOLO v2 weights to detect and highlight M1 Abrams tanks in a given image or video. This is a continuation of my [previous project](https://github.com/mpky/abrams_project) where I built an image classifier to detect M1 Abrams tanks in a given image.

#### Motivation

The massive amount of photos and videos uploaded to social media today from conflict zones has provided opportunities for creative and new types of research and analysis. Experts such as those at Bellingcat and Armament Research Services have proven the power of this new type of open-source information in their analysis on everything from chemical weapons attacks to the capabilities of various armed opposition groups in Syria.

In some cases, these arms control experts spend hours sifting through battlefield footage and pictures to assess what types of weapons each combatant is using. This work is extremely important in ensuring that weapons legally sold or transferred from one country to another are not then sold or otherwise transferred to potentially unintended third-party users.

One of the more alarming [such incidents](https://www.longwarjournal.org/archives/2015/01/video-shows-hezbollah-brigades-convoy-transporting-american-m1-tank.php) occurred in Iraq in 2015 when Kata'ib Hezbollah, an Iraqi Shia militia group sanctioned as a terrorist organization by the US Treasury, uploaded a video to YouTube showing that an M1 Abrams tank had come into their possession. These main battle tanks had been sold by the United States to the Iraqi Army over the past decade, but it is unclear then how Kata'ib Hezbollah came to be in possession of one of them.

A YOLO model trained on images of high-risk weapons systems, in this case M1 Abrams tanks, can help open source arms trackers monitor end-use issues and accelerate their research process.

#### Data

I used the [Fatkun Batch Download Image](https://chrome.google.com/webstore/detail/fatkun-batch-download-ima/nnjjahlikiabnchcpehcpkdeckfgnohf?hl=en) extension for Google Chrome to download results of a Google Image search. The resulting dataset required manual cleaning as the downloader is fairly brute force and Google Image searches were sometimes polluted with images of non-Abrams tanks.  In total, I have 1291 images of M1 Abrams tanks that I manually annotated with the [RectLabel app](https://rectlabel.com/).

#### Training

I trained the model for 5125 steps/64 epochs using Google Colaboratory's free GPU compute. The model's loss leveled off around 1.5.

#### Results

The model is able to detect M1 Abrams in all of the test photos, although with a low degree of confidence.

Video Results:

https://youtu.be/TGagMXkKJ4E

https://youtu.be/S9IXBASPzag

Image Results:

![download (5)](https://user-images.githubusercontent.com/31871105/57265597-6a014300-7046-11e9-81ee-00c5f3886eb2.png)

![download (2)](https://user-images.githubusercontent.com/31871105/57265613-81d8c700-7046-11e9-992c-a02bb62b2e0b.png)
