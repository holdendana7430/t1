代发 wailian999

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.shangyingyoupin.top/gtysrvayva.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.c1oappe.top/gtzxolhmks.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.tianlin.xyz/gtxnmkauji.html

Ruby: File.read("a.txt")
来源：http://hz.yanxiufei.cn/gtpqachljd.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.sysykeji.top/gtxllcfkie.html

[F02] 逐行读取文件
来源：http://hz.chenlongwang.top/gtxhbmrrvp.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.daria6918.cn/gtcxeaosxq.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.cashguo.top/gtwomhnird.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.redwolf501.top/gtmqmqbvqn.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.haohaochexian.top/gtrrwhlpnh.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.cucudq.cn/gtaxbzowgf.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.wangdashe.top/gtaefugoya.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.jinqigfzy.top/gtfpwokszi.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.shanyushiyangkeji.top/gtdlorbpti.html

[F03] 写入文件（覆盖）
来源：http://hz.sxryk.cn/gtaphntgvq.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.hnxiangtu.top/gthwayutwr.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.sufxvd.cn/gtfbuygibt.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.gzhubu.top/gtjwmrhewj.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.gogol.net.cn/gthoouvsfc.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.zhixingplan.top/gtlbfjmcpt.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.ivvv.top/gtscsogcwi.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.jinyuanbaomall.cn/gtwdoizwly.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.xingfuxueyuan.xyz/gtvlxixtqv.html

[F04] 追加写入文件
来源：http://hz.fzhhl.top/gtqtsmooqr.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.iojbl.cn/gtigqxorbi.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.c1oappe.top/gtpppmqeuy.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.ppjwa.cn/gtmdntxjef.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.zdqjudy.top/gtdsuccthr.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.sweek.top/gtnkrrvrge.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.pycfn.com/gtsuzpcfhq.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.smart0.xyz/gtfmyayufg.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.cashguo.top/gtjypwmbwy.html

[F05] 判断文件或目录是否存在
来源：http://hz.zhengqikj.top/gtidlwgsro.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.gzhubu.top/gtdxapraxo.html

PHP:  file_exists("a.txt");
来源：http://hz.fzhhl.top/gtwpqzcvbl.html

JS:   fs.existsSync("a.txt")
来源：http://hz.gogol.net.cn/gtfmjmnbxt.html

TS:   fs.existsSync("a.txt")
来源：http://hz.meibo888.top/gtfqulvmew.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.birdmap.top/gtadgqopys.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.9152youxi.cn/gthoarqwjl.html

Ruby: File.exist?("a.txt")
来源：http://hz.hfpthk.cn/gtefkdtbzh.html

C#:   File.Exists("a.txt")
来源：http://hz.zhixingplan.top/gtpuigloza.html

[F06] 删除文件
来源：http://hz.tian-w.cn/gtahhcqewf.html

Py:   os.remove("a.txt")
来源：http://hz.jyoumei.cn/gtebnjbpha.html

PHP:  unlink("a.txt");
来源：http://hz.yj202588.top/gtklffoxxs.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.52xcode.cn/gtywlwktrc.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.zhoulong.xyz/gttqpijnwx.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.tanke756.top/gthoolzauj.html

Go:   os.Remove("a.txt")
来源：http://hz.haohaochexian.top/gticpyhstu.html

Ruby: File.delete("a.txt")
来源：http://hz.hongshengwenyu.top/gtsbzxdfho.html

C#:   File.Delete("a.txt");
来源：http://hz.zhixingplan.top/gtytssnftk.html

[F07] 创建目录（含多级）
来源：http://hz.xylfe.cn/gtgbjicdwx.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.pengpengdd.cyou/gtzmkvtmvn.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.yangfankeji.com/gtgvbpucsb.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.nanxinkj.top/gtateghygd.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.ehwqpu.com/gtyapjzwlb.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.yuxming.cn/gtcvnbride.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.xuanzx.com/gtgwbvwfub.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.pycfn.com/gtrkfmnfjd.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.fzhhl.top/gtecogcwpo.html

[F08] 遍历目录
来源：http://hz.0kj1m.cn/gtavazzden.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.zhiwuduotai.top/gtagjacapo.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.nanxinkj.top/gtpxajknxs.html

JS:   fs.readdirSync("dir")
来源：http://hz.feifeiyinyue.top/gtzaigedwk.html

TS:   fs.readdirSync("dir")
来源：http://hz.mhx1999.top/gtggaurxol.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.yvedp.cn/gtdtfuijjs.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.pycfn.com/gtaiuvvlgv.html

Ruby: Dir.children("dir")
来源：http://hz.gzhubu.top/gtfazmfwxp.html

C#:   Directory.GetFiles("dir")
来源：http://hz.hywenlv.cn/gtyjgrzbrl.html

[F09] 获取文件大小
来源：http://hz.yuxming.cn/gtfxzuxmju.html

Py:   os.path.getsize("a.txt")
来源：http://hz.chenzaomai.com/gtzpnilbcw.html

PHP:  filesize("a.txt");
来源：http://hz.jianghu66.top/gthahsptaf.html

JS:   fs.statSync("a.txt").size
来源：http://hz.shzxlz.cn/gtzxhzvklv.html

TS:   fs.statSync("a.txt").size
来源：http://hz.aibaodan.cn/gtaiiupgnl.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.yuxming.cn/gtqvkklhfp.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.sxryk.cn/gtovkvuolb.html

Ruby: File.size("a.txt")
来源：http://hz.gzhubu.top/gtobvfnlhx.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.yangfankeji.com/gtbacaqkul.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.meibo888.top/gtiuzetnoh.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.gogol.net.cn/gtxrbvmiri.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.zhaomingkeji.xyz/gtambdporc.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.yongpay.top/gtqzboiijv.html

TS:   path.extname("a.txt")
来源：http://hz.tianlin.xyz/gtzlinxmao.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.jqgfzy.top/gtcntsirkb.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.shangyingyoupin.top/gtsaudtmef.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.quarkkingdee.top/gthqkjzrjb.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.jlsjyb.cn/gttayhyfrw.html

[F11] 复制与移动文件
来源：http://hz.tanke756.top/gtylcsfuhs.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.guowangkeji.top/gtduwyhrgu.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.xuetiantiany.cn/gtpnbgbaph.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.jianghu66.top/gtgnjekram.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.xziqi.cn/gtgdmngnmy.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.wangdashe.top/gtjotgskcr.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.aibaodan.cn/gtowtbbamj.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.yanxiufei.cn/gtjwjlccqc.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.cashguo.top/gthpwvppki.html

[F12] CSV 读写
来源：http://hz.nanxuanxn.top/gtglibdikx.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.yanxiufei.cn/gtfpfakawx.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.yvedp.cn/gtanzlzarm.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.zhixingplan.top/gtbkijeoix.html

TS:   // 同上
来源：http://hz.9152youxi.cn/gtrokqrvrk.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.gotoacloud.top/gtvzqqsato.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.daxiang520.top/gtjsnevufx.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.zhixingplan.top/gtpjlwycxu.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.aibaodan.cn/gtotlflqmp.html

================================================================================
来源：http://hz.tanke756.top/gtvsodhmsg.html

G. 面向对象
来源：http://hz.vqdsnc.cn/gtlyycjscg.html

================================================================================
来源：http://hz.hywenlv.cn/gtzjmtnmig.html

[G01] 定义类
来源：http://hz.sweek.top/gtwkxvvmbu.html

Py:   class User: pass
来源：http://hz.52xcode.cn/gtklnhguse.html

PHP:  class User {}
来源：http://hz.tanke756.top/gtmhyjjths.html

JS:   class User {}
来源：http://hz.yj20258.top/gtwqzskxlu.html

TS:   class User { name: string = ""; }
来源：http://hz.xinyue.icu/gtioxrnkzy.html

Java: class User {}
来源：http://hz.yvedp.cn/gthxbqsfnq.html

Go:   type User struct { Name string }
来源：http://hz.ywan-chungtsiang.top/gtoemqjeyt.html

Ruby: class User; end
来源：http://hz.shangyingyoupin.top/gtxoqlmcid.html

C#:   class User {}
来源：http://hz.iojbl.cn/gtftwqintc.html

[G02] 构造函数
来源：http://hz.gogol.net.cn/gtewfutofr.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.sweek.top/gtiqvjeezp.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.iojbl.cn/gtaascdwcw.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.gaohongyu789.top/gtxvyohouw.html

TS:   constructor(public name: string) {}
来源：http://hz.jinyuanbaomall.cn/gtrnfhghsa.html

Java: User(String name) { this.name = name; }
来源：http://hz.xylfe.cn/gtalszjjdb.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.tianlin.xyz/gtoajsnvka.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.hongshengwenyu.top/gtspuebjwj.html

C#:   public User(string name) { Name = name; }
来源：http://hz.shanyushiyangtech.top/gtkowveqtl.html

[G03] 实例属性
来源：http://hz.kuanghao11.cn/gtobqkipkp.html

Py:   self.name = "x"
来源：http://hz.yonumen.top/gtomfpvgie.html

PHP:  public string $name = "x";
来源：http://hz.yj20258888.top/gtnqapzheg.html

JS:   this.name = "x";
来源：http://hz.hysaishi.cn/gtzilfiflj.html

TS:   name: string = "x";
来源：http://hz.sysykeji.top/gtpoznxwzw.html

Java: private String name;
来源：http://hz.guowangkeji.top/gtzeocspmf.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.sxryk.cn/gttaynnhvc.html

Ruby: @name = "x"
来源：http://hz.vqdsnc.cn/gtiksniywe.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.cashguo.top/gteghsxluq.html

[G04] 定义方法
来源：http://hz.havefunace.top/gthyygvmai.html

Py:   def greet(self): return self.name
来源：http://hz.snrcjt.cn/gtxndbvgrv.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.cashguo.top/gtrdkjapeo.html

JS:   greet() { return this.name; }
来源：http://hz.cqqwz.cn/gtjzvxcjjw.html

TS:   greet(): string { return this.name; }
来源：http://hz.shanyushiyangtech.top/gtuhxsvjfj.html

Java: String greet() { return name; }
来源：http://hz.dianchejie.cn/gtvxsbjovl.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.yj20258.top/gtxcebqate.html

Ruby: def greet; @name; end
来源：http://hz.shanyushiyangkeji.top/gtrrrillqx.html

C#:   public string Greet() => Name;
来源：http://hz.jinqigufen.top/gtzsnerkuy.html

[G05] 继承
来源：http://hz.sxryk.cn/gtbhjhfsfi.html

Py:   class Admin(User): pass
来源：http://hz.hnqzz.top/gtsoglcwvk.html

PHP:  class Admin extends User {}
来源：http://hz.yanxiufei.cn/gtxldqraeh.html

JS:   class Admin extends User {}
来源：http://hz.haohaochexian.top/gtfoohmbmn.html

TS:   class Admin extends User {}
来源：http://hz.wangshuangyany.cn/gthhuxeuao.html

Java: class Admin extends User {}
来源：http://hz.gzhubu.top/gtjtolahjb.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.9152youxi.cn/gtqhevhnfo.html

Ruby: class Admin < User; end
来源：http://hz.sweek.top/gtaaminnlv.html

C#:   class Admin : User {}
来源：http://hz.shanyushiyangkeji.top/gtxandfilw.html

[G06] 重写方法
来源：http://hz.tianlin.xyz/gtailytjoj.html

Py:   def greet(self): return "admin"
来源：http://hz.snrcjt.cn/gtqzydjzuw.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.xuetiantiany.cn/gtmisaricm.html

JS:   greet() { return "admin"; }
来源：http://hz.cashguo.top/gteqclifoo.html

TS:   greet(): string { return "admin"; }
来源：http://hz.yuxming.cn/gtjcnhffoa.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.jinghuilouyu.cn/gthgyhzshq.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.xziqi.cn/gtaybdoxrb.html

Ruby: def greet; "admin"; end
来源：http://hz.quarkkingdee.top/gtqevtswtn.html

C#:   public override string Greet() => "admin";
来源：http://hz.ydjk.org.cn/gtggsqgzus.html

[G07] 调用父类方法
来源：http://hz.zhijiandao.cn/gtrgklmool.html

Py:   super().greet()
来源：http://hz.xylfe.cn/gtuypkqxif.html

PHP:  parent::greet();
来源：http://hz.vqdsnc.cn/gtupthohzm.html

JS:   super.greet();
来源：http://hz.quarkkingdee.top/gtvafhhgek.html

TS:   super.greet();
来源：http://hz.gaohongyu789.top/gtyvalztvu.html

Java: super.greet();
来源：http://hz.xinyue.icu/gtkulzvntd.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.yuanzhike.top/gttievhsiv.html

Ruby: super
来源：http://hz.shanyushiyangkeji.top/gtpwwkkmue.html

C#:   base.Greet();
来源：http://hz.fzhhl.top/gthqjuysay.html

[G08] 静态方法与属性
来源：http://hz.aibaodan.cn/gtmuhzwfkz.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.shanyushiyangkeji.top/gtydvxhahz.html

PHP:  public static function f() {}
来源：http://hz.jqgufenzy.top/gtylbgbwjl.html

JS:   static f() {}
来源：http://hz.jinqigfzy.top/gtxdekdgvz.html

TS:   static f(): void {}
来源：http://hz.xuetiantiany.cn/gtursopwch.html

Java: static void f() {}
来源：http://hz.zhijiandao.cn/gtihzvekns.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.yj202588.top/gtxyczcvgr.html

Ruby: def self.f; end
来源：http://hz.jinqigufen.top/gtoibjzvuu.html

C#:   public static void F() {}
来源：http://hz.hammf.cn/gtgnslfivo.html

[G09] 接口 / 抽象类
来源：http://hz.jinyuanbaomall.cn/gtoceitcih.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.ywan-chungtsiang.top/gtflanreyp.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.0kj1m.cn/gtfuohjjzg.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.xylfe.cn/gtjzcptfoj.html

TS:   interface Shape { area(): number; }
来源：http://hz.vqdsnc.cn/gtjqrejquq.html

Java: interface Shape { double area(); }
来源：http://hz.cqqwz.cn/gthwyldjmz.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.pycfn.com/gthuyzddwl.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.hnqzz.top/gtzflkhiks.html

C#:   interface IShape { double Area(); }
来源：http://hz.yj20258.top/gtyjwgzlqf.html

[G10] 访问控制
来源：http://hz.shangyingyoupin.top/gtkibadbgx.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.sufxvd.cn/gtdvrgpmvo.html

PHP:  public / protected / private
来源：http://hz.yj20258888.top/gtbcrkjzyi.html

JS:   #private 字段；其余公开
来源：http://hz.yj202588.top/gtxqrrcnrz.html

TS:   public / protected / private
来源：http://hz.chenzaomai.com/gtbonizkrr.html

Java: public / protected / private / 默认包级
来源：http://hz.yangfankeji.com/gteltarwrs.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.sysykeji.top/gtxzuoxnju.html

Ruby: public / protected / private
来源：http://hz.redwolf501.top/gtjondlluo.html

C#:   public / protected / private / internal
来源：http://hz.xylfe.cn/gtruosslga.html

[G11] getter / setter
来源：http://hz.yj20258888.top/gtuengrvsw.html

Py:   @property 与 @x.setter
来源：http://hz.tanke756.top/gtxtrjmqha.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.jinyuanbaomall.cn/gtoechcesf.html

JS:   get name() { return this._name; }
来源：http://hz.jyoumei.cn/gtavadjieu.html

TS:   get name(): string { return this._name; }
来源：http://hz.ybcxt.top/gtplupckcl.html

Java: public String getName() { return name; }
来源：http://hz.fzhhl.top/gtjskbtmol.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.0kj1m.cn/gtnknlhbnh.html

Ruby: attr_accessor :name
来源：http://hz.zhiwuduotai.top/gtggvkgapd.html

C#:   public string Name { get; set; }
来源：http://hz.xinyue.icu/gtutbpnhxd.html

[G12] 对象转字符串
来源：http://hz.52xcode.cn/gttdrzwtry.html

Py:   def __str__(self): return self.name
来源：http://hz.ehwqpu.com/gtzfkugdfn.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.9152youxi.cn/gtfvyhkfmk.html

JS:   toString() { return this.name; }
来源：http://hz.c1oappe.top/gtofwckyab.html

TS:   toString(): string { return this.name; }
来源：http://hz.nanxuanxn.top/gtlzrvcndd.html

Java: @Override public String toString() { return name; }
来源：http://hz.shanyushiyangtech.top/gthrczjoss.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.andypj.xyz/gtacumfzgg.html

Ruby: def to_s; @name; end
来源：http://hz.aibaodan.cn/gtjzunsgdt.html

C#:   public override string ToString() => Name;
来源：http://hz.yj202588.top/gtumlfeauq.html

[G13] 判断对象类型
来源：http://hz.yj202588.top/gtemgxqbqh.html

Py:   isinstance(u, User)
来源：http://hz.hfpthk.cn/gtipizklte.html

PHP:  $u instanceof User
来源：http://hz.ydzc1.top/gtbcpzdckw.html

JS:   u instanceof User
来源：http://hz.zhengqikj.top/gtnnyjitus.html

TS:   u instanceof User
来源：http://hz.jinyuanbaomall.cn/gtqstrxzca.html

Java: u instanceof User
来源：http://hz.cheryme.top/gtyvhidlyt.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.gaohongyu789.top/gtgbywifls.html

Ruby: u.is_a?(User)
来源：http://hz.vqdsnc.cn/gtjwqrhiue.html

C#:   u is User
来源：http://hz.daria6918.cn/gtjfyutoey.html

[G14] 数据类 / record
来源：http://hz.yuanzhike.top/gtzcwqixct.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.meibo888.top/gtbmcrlbje.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.gzhubu.top/gttygeovmv.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.snrcjt.cn/gtzhpwvgoh.html

TS:   type User = { name: string; age: number };
来源：http://hz.andypj.xyz/gtvittqpyc.html

Java: record User(String name, int age) {}
来源：http://hz.dianchejie.cn/gtnhpsuiyg.html

Go:   type User struct { Name string; Age int }
来源：http://hz.kuanghao11.cn/gtrcbujarg.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.xuetiantiany.cn/gtrrhijijp.html

C#:   record User(string Name, int Age);
来源：http://hz.ywan-chungtsiang.top/gteudmrblw.html

[G15] 枚举
来源：http://hz.cucudq.cn/gtsxqxxwqt.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.shanyushiyangkeji.top/gtiehrlsdt.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.ppjwa.cn/gtavxgzycv.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.havefunace.top/gtggnwitld.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.andypj.xyz/gtqrofyoft.html

Java: enum Color { RED, GREEN }
来源：http://hz.jinqigfzy.top/gtebkstkaj.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.xylfe.cn/gtktswpyzq.html

Ruby: Color = %i[red green].freeze
来源：http://hz.sxryk.cn/gtkzebhpap.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.daria6918.cn/gtswptxpqb.html

[G16] 对象转数组 / 字典
来源：http://hz.yuxming.cn/gttpujtbkx.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.jqgfzy.top/gttwusmyhg.html

PHP:  get_object_vars($obj);
来源：http://hz.pycfn.com/gtdurnvpoz.html

JS:   Object.entries(obj)
来源：http://hz.kuanghao11.cn/gtiscxloov.html

TS:   Object.entries(obj)
来源：http://hz.shanyushiyangtech.top/gtopocyjqm.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.jianghu66.top/gtfjtvodxy.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.hysaishi.cn/gtlyuodajk.html

Ruby: obj.instance_variables
来源：http://hz.yonumen.top/gtqvtweasz.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.jinqigfzy.top/gtjelzixni.html

================================================================================
来源：http://hz.daxiang520.top/gttepccwxj.html

H. 异常与错误处理
来源：http://hz.cashguo.top/gtignlmria.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtmqbceqso.html

[H01] try / catch 基础
来源：http://hz.gotoacloud.top/gtvdtzbzga.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.hfpthk.cn/gtzxreqdts.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.yj20258888.top/gtosngiigy.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.xingfuxueyuan.xyz/gtbuijyloa.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.shangyingyoupin.top/gtthegoqrv.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.pengpengdd.cyou/gtndkblhkz.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.ybcxt.top/gtjhmqroua.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.wangshuangyany.cn/gtnfwbegbn.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.nwbrower.top/gtybcruslp.html

[H02] finally / ensure 收尾
来源：http://hz.316326.xyz/gtvdqdojsl.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.hnqzz.top/gtypyvgngl.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.shzxlz.cn/gtfnzopkze.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.redwolf501.top/gtxevailag.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.sxryk.cn/gtsctdpuey.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.zhixingplan.top/gtuyrfsghd.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.ybcxt.top/gtfkplqfru.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.yj20258888.top/gtylyzwubm.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.andypj.xyz/gtnizidcjw.html

[H03] 主动抛出异常
来源：http://hz.gaohongyu789.top/gtxawaapfy.html

Py:   raise ValueError("错误信息")
来源：http://hz.daria6918.cn/gtsebwancj.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.yvedp.cn/gtknfkjmfn.html

JS:   throw new Error("错误信息");
来源：http://hz.fengsongda.top/gtofyuxfvo.html

TS:   throw new Error("错误信息");
来源：http://hz.cqqwz.cn/gtmfppohhn.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.wangdashe.top/gtgmoatkso.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.ydzc1.top/gtrawkyteb.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.wangshuangyany.cn/gtqakggvow.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.shangyingyoupin.top/gtnqlrecmx.html

[H04] 自定义异常类型
来源：http://hz.hfpthk.cn/gtaurpwrqw.html

Py:   class MyError(Exception): pass
来源：http://hz.ybcxt.top/gtqwpvmhph.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.zycfv.cn/gtwzahrwyq.html

JS:   class MyError extends Error {}
来源：http://hz.xylfe.cn/gtjjnltule.html

TS:   class MyError extends Error {}
来源：http://hz.hammf.cn/gtotccbhdo.html

Java: class MyException extends RuntimeException {}
来源：http://hz.wangdashe.top/gtgvpimucu.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.feifeiyinyue.top/gtwfwgioec.html

Ruby: class MyError < StandardError; end
来源：http://hz.yueranfly.top/gtzcpinbtv.html

C#:   class MyException : Exception {}
来源：http://hz.yuanzhike.top/gtarcktgaz.html

[H05] 捕获特定类型
来源：http://hz.jqgufenzy.top/gttzoetfup.html

Py:   except ValueError as e:
来源：http://hz.guowangkeji.top/gtlvybxqqp.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.ydjk.org.cn/gtxyicloeu.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.cheryme.top/gtmyffwcpy.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.ydjk.org.cn/gtbkqgrzss.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.wangshuangyany.cn/gtthczczxm.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.yueranfly.top/gtumdzhniv.html

Ruby: rescue ArgumentError => e
来源：http://hz.zhiwuduotai.top/gtgaxicdiv.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.nwbrower.top/gteamlbyfc.html

[H06] 可选值 / 空值安全访问
来源：http://hz.hammf.cn/gtbeujyfkj.html


<!-- 参考信息 -->