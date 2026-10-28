代发 wailian999

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.hnxiangtu.top/gtlsrhhzwv.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.zhixingplan.top/gtrgatavyo.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.0kj1m.cn/gtpckectgv.html

Ruby: File.read("a.txt")
来源：http://hz.hywenlv.cn/gtfygcpsky.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.jqgfzy.top/gtwhczywdj.html

[F02] 逐行读取文件
来源：http://hz.hongshengwenyu.top/gtwkvwzywg.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.yongpay.top/gturcfukcm.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.jinqigufen.top/gtlnlemkqe.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.birdmap.top/gtleueywsf.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.gzhubu.top/gtlhfvreca.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.kuanghao11.cn/gtmebhgzvr.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.dashuyun.cn/gtukmnfjea.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.nwbrower.top/gtsetmnbhv.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.shanyushiyangkeji.top/gtsqshjyel.html

[F03] 写入文件（覆盖）
来源：http://hz.cashguo.top/gtwrhldcou.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.hnqzz.top/gtmowwwszm.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.hywenlv.cn/gtrkctyluv.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.tanke756.top/gtmnkdjjva.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.andypj.xyz/gtwwskxyld.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.tian-w.cn/gthyyvvvii.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.yj20258888.top/gtzxvydyff.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.sxryk.cn/gtdgpoknsn.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.shangyingyoupin.top/gtyxehxine.html

[F04] 追加写入文件
来源：http://hz.jinqigufen.top/gtrmrielsl.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.dianchejie.cn/gtqyoosoyo.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.yonumen.top/gtcfooefqq.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.daxiang520.top/gtwocifmdf.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.c1oappe.top/gtyjseybeo.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.cdnleiting.top/gtrbbvfpvq.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.dianchejie.cn/gthcaroswl.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.zhengqikj.top/gtwvqiunkf.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.hnqzz.top/gtdodzqmwn.html

[F05] 判断文件或目录是否存在
来源：http://hz.ywan-chungtsiang.top/gtxamtfanr.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.ehwqpu.com/gtbqularqk.html

PHP:  file_exists("a.txt");
来源：http://hz.sufxvd.cn/gtyrxheohf.html

JS:   fs.existsSync("a.txt")
来源：http://hz.jqgufenzy.top/gtqsdzrqdl.html

TS:   fs.existsSync("a.txt")
来源：http://hz.zhoulong.xyz/gtjcomenxs.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.hnxiangtu.top/gtbqpdghmy.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.fengsongda.top/gtaamsxmqt.html

Ruby: File.exist?("a.txt")
来源：http://hz.jqgufenzy.top/gtgjjbcutp.html

C#:   File.Exists("a.txt")
来源：http://hz.jlsjyb.cn/gtsiplhexj.html

[F06] 删除文件
来源：http://hz.zhijiandao.cn/gtwvczkrmv.html

Py:   os.remove("a.txt")
来源：http://hz.yj20258.top/gtmmjtjvvh.html

PHP:  unlink("a.txt");
来源：http://hz.yueranfly.top/gtzhtwctxn.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.tanke756.top/gthlfasufz.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.zhixingplan.top/gtftzzuroy.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.jyoumei.cn/gtibhgouji.html

Go:   os.Remove("a.txt")
来源：http://hz.hnqzz.top/gtxizixnxm.html

Ruby: File.delete("a.txt")
来源：http://hz.xziqi.cn/gtdhfggmqw.html

C#:   File.Delete("a.txt");
来源：http://hz.hongshengwenyu.top/gtslheytkn.html

[F07] 创建目录（含多级）
来源：http://hz.cheryme.top/gttghzzzkc.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.hongshengwenyu.top/gttjyyvmrb.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.gotoacloud.top/gtszmqaiyo.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.jlsjyb.cn/gtezvboiey.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.yuxming.cn/gtreqemywy.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.cashguo.top/gtgbgbxjcu.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.meibo888.top/gtswaeceox.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.sufxvd.cn/gtxpiwmjxi.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.quarkkingdee.top/gtokzsmvjl.html

[F08] 遍历目录
来源：http://hz.yj20258.top/gtknvobgmw.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.jinqigufen.top/gtwaawkztc.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.guowangkeji.top/gtadehinqz.html

JS:   fs.readdirSync("dir")
来源：http://hz.meibo888.top/gtlhwbdiqe.html

TS:   fs.readdirSync("dir")
来源：http://hz.jyoumei.cn/gthptebfrk.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.yj20258.top/gtzjohfdje.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.yonumen.top/gtxotdpewb.html

Ruby: Dir.children("dir")
来源：http://hz.yuxming.cn/gtxpdodltr.html

C#:   Directory.GetFiles("dir")
来源：http://hz.zhoulong.xyz/gthdjxpzct.html

[F09] 获取文件大小
来源：http://hz.cdnleiting.top/gtzijihofm.html

Py:   os.path.getsize("a.txt")
来源：http://hz.fzhhl.top/gtylghnzst.html

PHP:  filesize("a.txt");
来源：http://hz.dianchejie.cn/gtrztvruqy.html

JS:   fs.statSync("a.txt").size
来源：http://hz.c1oappe.top/gtoxxclkiq.html

TS:   fs.statSync("a.txt").size
来源：http://hz.gotoacloud.top/gttnoetzjh.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.gzhubu.top/gtskxyvwdz.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.tanke756.top/gtcvzrrluk.html

Ruby: File.size("a.txt")
来源：http://hz.fengsongda.top/gttfguddfa.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.yangfankeji.com/gtrecirbxy.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.jqgufenzy.top/gtjguzrbpx.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.jinghuilouyu.cn/gttiwqeguf.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.yuanzhike.top/gtuozhxzhq.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.guannengcc.top/gtugzuvldq.html

TS:   path.extname("a.txt")
来源：http://hz.kuanghao11.cn/gtmnkaehvd.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.jinghuilouyu.cn/gtdgdmqeut.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.hywenlv.cn/gtkrasgsmc.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.nanxinkj.top/gtmriswtpe.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.feifeiyinyue.top/gtcsybstiz.html

[F11] 复制与移动文件
来源：http://hz.xuanzx.com/gtvxkxcobg.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.tanke756.top/gtgbbtleni.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.cdnleiting.top/gtlrnxtntw.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.ybcxt.top/gtorjaaifi.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.sysykeji.top/gtwfbxgjpi.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.yonumen.top/gtpojuhwga.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.pycfn.com/gtsyoylmkx.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.daria6918.cn/gtunqytslb.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.zhiwuduotai.top/gttruhsusz.html

[F12] CSV 读写
来源：http://hz.redwolf501.top/gtroyolzkz.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.wangshuangyany.cn/gtvlulxjkf.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.smart0.xyz/gtignsuuae.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.yueranfly.top/gtiporsjob.html

TS:   // 同上
来源：http://hz.yvedp.cn/gtvtakvmxj.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.andypj.xyz/gtqngqqgsm.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.cashguo.top/gtosaaysgh.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.dashuyun.cn/gtvflpvzxl.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.wangdashe.top/gtpsasbqqn.html

================================================================================
来源：http://hz.yj202588.top/gtoplujkqp.html

G. 面向对象
来源：http://hz.nwbrower.top/gtoqifoiar.html

================================================================================
来源：http://hz.fzhhl.top/gteohxahgu.html

[G01] 定义类
来源：http://hz.sweek.top/gtjugjewkp.html

Py:   class User: pass
来源：http://hz.daxiang520.top/gthgybrorr.html

PHP:  class User {}
来源：http://hz.guannengcc.top/gttlbgllcc.html

JS:   class User {}
来源：http://hz.zhixingplan.top/gtxwqnvqve.html

TS:   class User { name: string = ""; }
来源：http://hz.cheryme.top/gtdovydyqu.html

Java: class User {}
来源：http://hz.yj20258888.top/gtgpbhhaau.html

Go:   type User struct { Name string }
来源：http://hz.cqqwz.cn/gtpkhdczkd.html

Ruby: class User; end
来源：http://hz.wangshuangyany.cn/gtnzibsryk.html

C#:   class User {}
来源：http://hz.andypj.xyz/gtbvdjgnsg.html

[G02] 构造函数
来源：http://hz.wangshuangyany.cn/gttaakkylf.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.xingfuxueyuan.xyz/gtbbxuknhy.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.yuxming.cn/gtcihoxyyn.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.svipenyu.cn/gtfxfhsjby.html

TS:   constructor(public name: string) {}
来源：http://hz.fengsongda.top/gthebjxfgj.html

Java: User(String name) { this.name = name; }
来源：http://hz.tianlin.xyz/gtowammroj.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.svipenyu.cn/gtugkdhtae.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.guannengcc.top/gtjsamqyvj.html

C#:   public User(string name) { Name = name; }
来源：http://hz.hnxiangtu.top/gtghitxusd.html

[G03] 实例属性
来源：http://hz.ivvv.top/gtwyjzzeop.html

Py:   self.name = "x"
来源：http://hz.zhongyouzk.top/gtyqkqyrhr.html

PHP:  public string $name = "x";
来源：http://hz.shzxlz.cn/gtxogeyvub.html

JS:   this.name = "x";
来源：http://hz.hywenlv.cn/gtljnqainl.html

TS:   name: string = "x";
来源：http://hz.cucudq.cn/gtbaefwlne.html

Java: private String name;
来源：http://hz.tianlin.xyz/gtihiwpkud.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.zycfv.cn/gtuinuyrcw.html

Ruby: @name = "x"
来源：http://hz.fengsongda.top/gtyflhisuz.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.jyoumei.cn/gteijipvkr.html

[G04] 定义方法
来源：http://hz.gogol.net.cn/gtcultlxhh.html

Py:   def greet(self): return self.name
来源：http://hz.ywan-chungtsiang.top/gtapcuaswn.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.ivvv.top/gtvydgrohu.html

JS:   greet() { return this.name; }
来源：http://hz.vqdsnc.cn/gttxifwslq.html

TS:   greet(): string { return this.name; }
来源：http://hz.hongshengwenyu.top/gtnasoresj.html

Java: String greet() { return name; }
来源：http://hz.chenzaomai.com/gtaobarrei.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.fengsongda.top/gthunuarqb.html

Ruby: def greet; @name; end
来源：http://hz.hongshengwenyu.top/gtzlkslzhz.html

C#:   public string Greet() => Name;
来源：http://hz.yj20258.top/gtjihfhfbg.html

[G05] 继承
来源：http://hz.dashuyun.cn/gtbpmihsjx.html

Py:   class Admin(User): pass
来源：http://hz.hnxiangtu.top/gttptjbedv.html

PHP:  class Admin extends User {}
来源：http://hz.dianchejie.cn/gtpuwleijz.html

JS:   class Admin extends User {}
来源：http://hz.feifeiyinyue.top/gtufrszzqm.html

TS:   class Admin extends User {}
来源：http://hz.dianchejie.cn/gttajeeuuj.html

Java: class Admin extends User {}
来源：http://hz.zycfv.cn/gtffuinhka.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.hywenlv.cn/gtkwompqkf.html

Ruby: class Admin < User; end
来源：http://hz.dashuyun.cn/gtnivvmbqe.html

C#:   class Admin : User {}
来源：http://hz.jinqigfzy.top/gtaupuiroi.html

[G06] 重写方法
来源：http://hz.yueranfly.top/gtvidwzcxq.html

Py:   def greet(self): return "admin"
来源：http://hz.hnxiangtu.top/gtplaxsshm.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.ydzc1.top/gtzklbotco.html

JS:   greet() { return "admin"; }
来源：http://hz.ybcxt.top/gtfdkplrce.html

TS:   greet(): string { return "admin"; }
来源：http://hz.hnxiangtu.top/gtotohntnf.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.ppjwa.cn/gtnzicrfku.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.hnqzz.top/gtelhjefdz.html

Ruby: def greet; "admin"; end
来源：http://hz.zhiwuduotai.top/gtggihqjck.html

C#:   public override string Greet() => "admin";
来源：http://hz.9152youxi.cn/gtohwsibkp.html

[G07] 调用父类方法
来源：http://hz.tanke756.top/gtbmhgazdb.html

Py:   super().greet()
来源：http://hz.guowangkeji.top/gtuxbxavtl.html

PHP:  parent::greet();
来源：http://hz.zhixingplan.top/gtrstavtgj.html

JS:   super.greet();
来源：http://hz.ppjwa.cn/gtufzpnxdn.html

TS:   super.greet();
来源：http://hz.yangfankeji.com/gtlwnahtoi.html

Java: super.greet();
来源：http://hz.cdnleiting.top/gtcjxmvnyq.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.daria6918.cn/gtixkqsakh.html

Ruby: super
来源：http://hz.316326.xyz/gtmluuveam.html

C#:   base.Greet();
来源：http://hz.pengpengdd.cyou/gtwfiavdce.html

[G08] 静态方法与属性
来源：http://hz.cheryme.top/gtdmtosqpq.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.chenlongwang.top/gtqbniawgt.html

PHP:  public static function f() {}
来源：http://hz.52xcode.cn/gtmjemrvfc.html

JS:   static f() {}
来源：http://hz.gogol.net.cn/gtmspjxiji.html

TS:   static f(): void {}
来源：http://hz.cdnleiting.top/gtohedqsei.html

Java: static void f() {}
来源：http://hz.havefunace.top/gtlogzjnqo.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.fengsongda.top/gtgbihtvvg.html

Ruby: def self.f; end
来源：http://hz.yanxiufei.cn/gtsoapyoor.html

C#:   public static void F() {}
来源：http://hz.cdnleiting.top/gtqwbqqxay.html

[G09] 接口 / 抽象类
来源：http://hz.jinyuanbaomall.cn/gtsbjuorqm.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.shangyingyoupin.top/gtwjjqdhwv.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.zhoulong.xyz/gtvgpznopq.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.shangyingyoupin.top/gtwbxgojqo.html

TS:   interface Shape { area(): number; }
来源：http://hz.shanyushiyangkeji.top/gtrocxufqc.html

Java: interface Shape { double area(); }
来源：http://hz.yuxming.cn/gtsnbpedmo.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.yuxming.cn/gtjhempsen.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.daria6918.cn/gtsirvkdwr.html

C#:   interface IShape { double Area(); }
来源：http://hz.cucudq.cn/gtrhmnwhtp.html

[G10] 访问控制
来源：http://hz.jinyuanbaomall.cn/gttvhsezgk.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.sysykeji.top/gtdzrfsrty.html

PHP:  public / protected / private
来源：http://hz.hongshengwenyu.top/gtlarqtemq.html

JS:   #private 字段；其余公开
来源：http://hz.hysaishi.cn/gtvtlootxj.html

TS:   public / protected / private
来源：http://hz.jinqigfzy.top/gtymdtqxch.html

Java: public / protected / private / 默认包级
来源：http://hz.redwolf501.top/gtpabsaurr.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.meibo888.top/gtlfbwphxz.html

Ruby: public / protected / private
来源：http://hz.aizwys.cn/gtqzdakygw.html

C#:   public / protected / private / internal
来源：http://hz.cheryme.top/gtvmmkhbds.html

[G11] getter / setter
来源：http://hz.hysaishi.cn/gtpoquzygu.html

Py:   @property 与 @x.setter
来源：http://hz.sxryk.cn/gtvwxebvlb.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.smart0.xyz/gtrvzkikds.html

JS:   get name() { return this._name; }
来源：http://hz.jinyuanbaomall.cn/gtxklcvega.html

TS:   get name(): string { return this._name; }
来源：http://hz.redwolf501.top/gthnoifgdh.html

Java: public String getName() { return name; }
来源：http://hz.yj20258.top/gtrytbamsd.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.zycfv.cn/gtetplrtok.html

Ruby: attr_accessor :name
来源：http://hz.hammf.cn/gtrntqqlnu.html

C#:   public string Name { get; set; }
来源：http://hz.zhongyouzk.top/gtriqafmfk.html

[G12] 对象转字符串
来源：http://hz.yuxming.cn/gtthvxgool.html

Py:   def __str__(self): return self.name
来源：http://hz.yueranfly.top/gtkucshkdm.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.yj202588.top/gtvpfpsbiw.html

JS:   toString() { return this.name; }
来源：http://hz.zhaomingkeji.xyz/gtfsmsryon.html

TS:   toString(): string { return this.name; }
来源：http://hz.xingfuxueyuan.xyz/gtqttomskz.html

Java: @Override public String toString() { return name; }
来源：http://hz.wangshuangyany.cn/gtbhrcducn.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.yj202588.top/gtqtcfvohw.html

Ruby: def to_s; @name; end
来源：http://hz.jinqigufen.top/gtydppawfo.html

C#:   public override string ToString() => Name;
来源：http://hz.mhx1999.top/gtgaqufcjx.html

[G13] 判断对象类型
来源：http://hz.gotoacloud.top/gtiuhuhpxm.html

Py:   isinstance(u, User)
来源：http://hz.ywan-chungtsiang.top/gtzrlivobq.html

PHP:  $u instanceof User
来源：http://hz.xziqi.cn/gtzrtatayb.html

JS:   u instanceof User
来源：http://hz.snrcjt.cn/gtsxspumwz.html

TS:   u instanceof User
来源：http://hz.52xcode.cn/gtqimiwqth.html

Java: u instanceof User
来源：http://hz.gzhubu.top/gttsakuxvo.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.cdnleiting.top/gtlvwtsbbv.html

Ruby: u.is_a?(User)
来源：http://hz.xziqi.cn/gtmiepxmud.html

C#:   u is User
来源：http://hz.chenzaomai.com/gtnkhdkzac.html

[G14] 数据类 / record
来源：http://hz.tianlin.xyz/gtcxqgbxre.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.fzhhl.top/gtgvdzdwjy.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.zdqjudy.top/gtnqghdyqq.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.cheryme.top/gtwadrssxg.html

TS:   type User = { name: string; age: number };
来源：http://hz.jiagoushi.top/gtegakgiwm.html

Java: record User(String name, int age) {}
来源：http://hz.zhongyouzk.top/gtlvzymkyd.html

Go:   type User struct { Name string; Age int }
来源：http://hz.haohaochexian.top/gtmelxauxj.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.zhaomingkeji.xyz/gtvanrrogw.html

C#:   record User(string Name, int Age);
来源：http://hz.jlsjyb.cn/gtypradfdu.html

[G15] 枚举
来源：http://hz.sxryk.cn/gteofyumrn.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.sysykeji.top/gtrwysowtv.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.hfpthk.cn/gtwmqyepwi.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.gaohongyu789.top/gtahvvarro.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.feifeiyinyue.top/gtuizuuoiz.html

Java: enum Color { RED, GREEN }
来源：http://hz.yj20258.top/gtyknitauw.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.mhx1999.top/gtcylmkhbj.html

Ruby: Color = %i[red green].freeze
来源：http://hz.jqgfzy.top/gtzybipfzl.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.yj20258888.top/gtsxcbtxxi.html

[G16] 对象转数组 / 字典
来源：http://hz.cashguo.top/gtjahzpmmb.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.zycfv.cn/gttmggkcrz.html

PHP:  get_object_vars($obj);
来源：http://hz.vqdsnc.cn/gtxrwjjzai.html

JS:   Object.entries(obj)
来源：http://hz.cdnleiting.top/gtqzmeklir.html

TS:   Object.entries(obj)
来源：http://hz.zycfv.cn/gtcjvxqorj.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.gaohongyu789.top/gtbindwvno.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.hywenlv.cn/gtodyighzi.html

Ruby: obj.instance_variables
来源：http://hz.cqqwz.cn/gteggibrfq.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.andypj.xyz/gtzckkfvjf.html

================================================================================
来源：http://hz.cqqwz.cn/gtbodgmvyv.html

H. 异常与错误处理
来源：http://hz.ywan-chungtsiang.top/gtdnlvtstf.html

================================================================================
来源：http://hz.zhijiandao.cn/gtxgamcsba.html

[H01] try / catch 基础
来源：http://hz.yj20258888.top/gtbbvmvnoa.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.xziqi.cn/gthbnvsfmq.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.vqdsnc.cn/gtavjlozre.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.yuanzhike.top/gtibkxbnyp.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.sysykeji.top/gthcvlsbog.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.wangdashe.top/gtsuhhtuei.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.jqgufenzy.top/gtpcauyhno.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.dianchejie.cn/gthklpzqgu.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.yj20258.top/gtpdpujynh.html

[H02] finally / ensure 收尾
来源：http://hz.ehwqpu.com/gtdmsfvwsq.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.jyoumei.cn/gtnctoyfxs.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.xingfuxueyuan.xyz/gtqokcibml.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.aizwys.cn/gtacjlcvmx.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.0kj1m.cn/gtazulunit.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.nanxuanxn.top/gtfocgynfg.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.zhiwuduotai.top/gtecqejxzp.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.ehwqpu.com/gtcaegdbgd.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.tianlin.xyz/gtwqneihva.html

[H03] 主动抛出异常
来源：http://hz.feifeiyinyue.top/gtuomoimti.html

Py:   raise ValueError("错误信息")
来源：http://hz.xuetiantiany.cn/gtwpnzbuuj.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.nanxuanxn.top/gtbrftgasf.html

JS:   throw new Error("错误信息");
来源：http://hz.yongpay.top/gttmzhzjkq.html

TS:   throw new Error("错误信息");
来源：http://hz.shanyushiyangkeji.top/gtwqbqwomf.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.xuanzx.com/gtkuukwcra.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.wangshuangyany.cn/gtyhlzmcfc.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.jlsjyb.cn/gtoaxovgvc.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.hfpthk.cn/gtlftjyuka.html

[H04] 自定义异常类型
来源：http://hz.316326.xyz/gtwxneodkz.html

Py:   class MyError(Exception): pass
来源：http://hz.ybcxt.top/gtasnnecyx.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.cashguo.top/gtswcaykln.html

JS:   class MyError extends Error {}
来源：http://hz.jinqigfzy.top/gtitzvszee.html

TS:   class MyError extends Error {}
来源：http://hz.shuidangran.top/gtjezcmpzh.html

Java: class MyException extends RuntimeException {}
来源：http://hz.zdqjudy.top/gtpunfznco.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.cucudq.cn/gtvanocjdy.html

Ruby: class MyError < StandardError; end
来源：http://hz.daria6918.cn/gtroujbisv.html

C#:   class MyException : Exception {}
来源：http://hz.xuanzx.com/gtxuofomii.html

[H05] 捕获特定类型
来源：http://hz.guannengcc.top/gtailpomem.html

Py:   except ValueError as e:
来源：http://hz.xinyue.icu/gtacqxwjcd.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.fzhhl.top/gtuoesbxku.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.zycfv.cn/gtdyoqhlah.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.316326.xyz/gtqsrpxndu.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.bjfxy.top/gtqdmqeoij.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.xuanzx.com/gtgacqajzh.html

Ruby: rescue ArgumentError => e
来源：http://hz.kuanghao11.cn/gtbfuqlnjd.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.bjfxy.top/gtonvwxdia.html

[H06] 可选值 / 空值安全访问
来源：http://hz.ehwqpu.com/gtyertbhnp.html


<!-- 参考信息 -->