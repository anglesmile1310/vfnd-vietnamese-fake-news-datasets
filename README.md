# VIETNAMESE FAKE NEWS DATASET - VFND

VFND là bộ dataset về các tin tức giả bằng ngôn ngữ tiếng Việt được tập hợp trong khoảng thời gian 2017-2019, các tin tức được đưa vào đây được phân loại thật giả dựa trên một số nguồn tin, tham chiếu chéo đến các nguồn tin được dẫn hoặc được phân loại bởi cộng đồng. 

Nếu muốn sử dụng, mời các bạn vui lòng liên hệ đến email: thanh.hoquangcse96@gmail.com, và vui lòng dẫn nguồn của repo này trong bài viết của bạn

## 1. Giới thiệu tổng quan và các chủ đề tin tức

Cấu trúc tên của 1 file bao gồm: VFND_{Source}\_{Label}\_{Number}. Trong đó: {Source}: Ac - nguồn bài báo từ các trang tin tức; Fb - Nguồn từ các bài viết của người dùng hoặc fanpage trên Facebook có tính chất như nguồn tin tức. {Label} thuộc tập {“Fake”, “Real”}

### Giới hạn các chủ đề tin tức trong tập dữ liệu:

Thứ 1: Các tin tức sử dụng trong bộ dataset đều là tin tức tường thuật về 1 sự kiện. Lý do: Để có thể kiểm tra chéo giữa các nguồn tin để xác định được tin tức thật hoặc giả trong trường hợp mà cộng đồng chưa hỗ trợ phân loại tin tức.

Thứ 2: Các chủ đề mà bộ dataset tập trung là: Thể thao, Văn hóa, Xã hội, Kinh tế, Pháp luật. Các tin tức sẽ được kiểm tra chéo về nguồn gốc, nội dung, sự kiện để xác định thật và giả


### Cách thức lấy dữ liệu

Các dữ liệu tin tức và nguồn dữ liệu của bộ dataset sẽ được trình bày trong các file README.md đi theo từng thư mục phân loại. Trong đó nội dung các file sẽ đưa ra nguồn tin tức và cách mà nhóm phân loại tin tức đó là giả.

Nhóm sử dụng thư viện: [news-please](https://github.com/fhamborg/news-please) 

## 2. Mô tả các thành phần trong bộ dữ liệu
### [_Article_\__Contents_](https://github.com/thanhhocse96/vfnd-vietnamese-fake-news-datasets/tree/master/Article_Contents): tập hợp các bài báo đã được phân loại 

Thư mục được cấu trúc theo từng label của tin tức: ```Fake, Real, Unclarified```, trong đó dữ liệu trong ```Unclarified``` sẽ được phân loại theo ```Fake, Real``` sau khi được xác nhận.

File ```stance.csv``` sẽ chứa stance (lập trường) của tin tức trong thư mục này. Phục vụ cho Stance Detection, nhóm tham khảo từ:
1. [FakeNewsChallenge](http://www.fakenewschallenge.org/)
2. [Emergent: a novel data-set for stance classification](http://aclweb.org/anthology/N/N16/N16-1138.pdf)
3. [Stance Detection with Bidirectional Conditional Encoding](https://arxiv.org/abs/1606.05464)
Cấu trúc của file ```stance.csv``` bao gồm 2 trường: ```filename``` - tên của các file trong tập dữ liệu về tin tức - và ```stance``` - stance của dữ liệu, bao gồm 4 nhãn: ```agrees, disagrees, discusses, unrelated``` như [FakeNewsChallenge](http://www.fakenewschallenge.org/)

### [_Facebook_](https://github.com/thanhhocse96/vfnd-vietnamese-fake-news-datasets/tree/master/Facebook): tập hợp các facebook post đã được phân loại
Cấu trúc của thư mục cũng tương tự như cấu trúc của _Article_\__Contents_, tuy nhiên, trong thư mục này nhóm tập trung vào những post được cộng đồng xác định là giả (Fake) hoặc chưa xác định thật giả (Unclarified)
### [_Utils_](): Các file hỗ trợ

# ----Draft-----
```
Give the example
```

And repeat

```
until finished
```

End with an example of getting some data out of the system or using it for a little demo

## Running the tests

Explain how to run the automated tests for this system

### Break down into end to end tests

Explain what these tests test and why

```
Give an example
```

### And coding style tests

Explain what these tests test and why

```
Give an example
```

## Deployment

Add additional notes about how to deploy this on a live system

## Built With

* [Dropwizard](http://www.dropwizard.io/1.0.2/docs/) - The web framework used
* [Maven](https://maven.apache.org/) - Dependency Management
* [ROME](https://rometools.github.io/rome/) - Used to generate RSS Feeds

## Contributing

Please read [CONTRIBUTING.md](https://gist.github.com/PurpleBooth/b24679402957c63ec426) for details on our code of conduct, and the process for submitting pull requests to us.

## Versioning

We use [SemVer](http://semver.org/) for versioning. For the versions available, see the [tags on this repository](https://github.com/your/project/tags). 

## Authors

* **Hồ Quang Thanh** - *Some one who love AI* - [thanhhocse96](https://github.com/thanhhocse96)

See also the list of [contributors](https://github.com/your/project/contributors) who participated in this project.

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details

## Acknowledgments

* Hat tip to anyone whose code was used
* Inspiration
* etc

