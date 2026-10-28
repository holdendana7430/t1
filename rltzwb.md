代发 wailian999

TS:   fs.existsSync("a.txt")
来源：http://hz.yanxiufei.cn/gtpghayuci.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.meibo888.top/gtsycqhygq.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.sxryk.cn/gtldevfcpt.html

Ruby: File.exist?("a.txt")
来源：http://hz.ivvv.top/gtmszdfgwt.html

C#:   File.Exists("a.txt")
来源：http://hz.snrcjt.cn/gttfjypigi.html

[F06] 删除文件
来源：http://hz.zhixingplan.top/gthdggfqmu.html

Py:   os.remove("a.txt")
来源：http://hz.zhengqikj.top/gtexaewxft.html

PHP:  unlink("a.txt");
来源：http://hz.cdnleiting.top/gtzfqnoolw.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.feifeiyinyue.top/gtdmddtkhs.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.9152youxi.cn/gthhgueffx.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.jinqigufen.top/gtcvtmwlnb.html

Go:   os.Remove("a.txt")
来源：http://hz.jianghu66.top/gtmctyrhfk.html

Ruby: File.delete("a.txt")
来源：http://hz.jinghuilouyu.cn/gtylmozpqr.html

C#:   File.Delete("a.txt");
来源：http://hz.sysykeji.top/gtqvncudak.html

[F07] 创建目录（含多级）
来源：http://hz.yuanzhike.top/gtxxjyweqm.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.c1oappe.top/gttgkgrpwu.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.feifeiyinyue.top/gtjyqnlzob.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.cdnleiting.top/gtsfenggcj.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.yanxiufei.cn/gtrzyvqqys.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.yangfankeji.com/gtzugkmckh.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.ppjwa.cn/gtletvxaxb.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.fzhhl.top/gtoqtuxeby.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.aizwys.cn/gtdlyzbrgl.html

[F08] 遍历目录
来源：http://hz.hnxiangtu.top/gtqedjyyxy.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.shanyushiyangtech.top/gtfwwnbflq.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.yuanzhike.top/gtqlrkajrb.html

JS:   fs.readdirSync("dir")
来源：http://hz.mhx1999.top/gtmkzgeqap.html

TS:   fs.readdirSync("dir")
来源：http://hz.xingfuxueyuan.xyz/gtcawawtdw.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.kuanghao11.cn/gtzxwanccq.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.sweek.top/gtcueasmmu.html

Ruby: Dir.children("dir")
来源：http://hz.xuetiantiany.cn/gtxztdwrlf.html

C#:   Directory.GetFiles("dir")
来源：http://hz.jianghu66.top/gtoaayigeq.html

[F09] 获取文件大小
来源：http://hz.yvedp.cn/gtvwygdbfn.html

Py:   os.path.getsize("a.txt")
来源：http://hz.hnxiangtu.top/gtcnfwupas.html

PHP:  filesize("a.txt");
来源：http://hz.iojbl.cn/gtpxebnsir.html

JS:   fs.statSync("a.txt").size
来源：http://hz.jyoumei.cn/gtxpkirkst.html

TS:   fs.statSync("a.txt").size
来源：http://hz.hysaishi.cn/gtkmwvficy.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.wangdashe.top/gtvkgxwsqu.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.0kj1m.cn/gtipjnfbvn.html

Ruby: File.size("a.txt")
来源：http://hz.xylfe.cn/gtcalbpppq.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.kuanghao11.cn/gtoxhwywog.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.andypj.xyz/gtkggcfiue.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.sweek.top/gtwciqdsgv.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.snrcjt.cn/gtngnfwbpn.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.jlsjyb.cn/gtfbuutbdx.html

TS:   path.extname("a.txt")
来源：http://hz.aibaodan.cn/gtgkedmcdm.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.yj20258.top/gtvmwrbgxy.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.chenjidiqi.icu/gtspaasulq.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.daria6918.cn/gtaofcqaxx.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.gotoacloud.top/gtvyqkslvr.html

[F11] 复制与移动文件
来源：http://hz.zhixingplan.top/gthfdpcbjv.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.bjfxy.top/gtqyddamdg.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.zdqjudy.top/gttolpxnsf.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.wangshuangyany.cn/gttxxhqlhw.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.xylfe.cn/gtkvjlrmxv.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.chenzaomai.com/gtofatanpv.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.sysykeji.top/gtcwhcwjmi.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.svipenyu.cn/gtjocapsma.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.sufxvd.cn/gtsxceoxnk.html

[F12] CSV 读写
来源：http://hz.yangfankeji.com/gtinhwhhds.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.yj20258.top/gtmmmxzvvy.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.kuanghao11.cn/gtixvkothn.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.wangdashe.top/gtzaxvazlo.html

TS:   // 同上
来源：http://hz.havefunace.top/gtjfaewoxp.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.meibo888.top/gtooguzsrg.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.ybcxt.top/gtngcuiqtu.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.iojbl.cn/gtyopluyls.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.andypj.xyz/gtuqmmdssx.html

================================================================================
来源：http://hz.nanxinkj.top/gtdqadiekn.html

G. 面向对象
来源：http://hz.bjfxy.top/gtltpgkazi.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtuowtcpbs.html

[G01] 定义类
来源：http://hz.jqgufenzy.top/gtfsocnngm.html

Py:   class User: pass
来源：http://hz.zhaomingkeji.xyz/gtmlklrjar.html

PHP:  class User {}
来源：http://hz.redwolf501.top/gtbiylalfu.html

JS:   class User {}
来源：http://hz.jianghu66.top/gtrgjiowxr.html

TS:   class User { name: string = ""; }
来源：http://hz.0kj1m.cn/gtqxbdkwfm.html

Java: class User {}
来源：http://hz.xuetiantiany.cn/gtlwysvoiw.html

Go:   type User struct { Name string }
来源：http://hz.quarkkingdee.top/gtkmsdhqol.html

Ruby: class User; end
来源：http://hz.havefunace.top/gtomsfellr.html

C#:   class User {}
来源：http://hz.meibo888.top/gtebdefflc.html

[G02] 构造函数
来源：http://hz.jinyuanbaomall.cn/gtuqazmroj.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.xinyue.icu/gtfwujofyi.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.shzxlz.cn/gtbjvevzuq.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.yuxming.cn/gtlhuirypk.html

TS:   constructor(public name: string) {}
来源：http://hz.tian-w.cn/gtfuyumddv.html

Java: User(String name) { this.name = name; }
来源：http://hz.xingfuxueyuan.xyz/gtibgmzfzw.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.sysykeji.top/gtyulrtemj.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.yuxming.cn/gtgkhmomqu.html

C#:   public User(string name) { Name = name; }
来源：http://hz.nanxinkj.top/gtmqvkzghs.html

[G03] 实例属性
来源：http://hz.ivvv.top/gtahjsqpac.html

Py:   self.name = "x"
来源：http://hz.gzhubu.top/gtabpadbdy.html

PHP:  public string $name = "x";
来源：http://hz.hfpthk.cn/gtgoknfciv.html

JS:   this.name = "x";
来源：http://hz.wangshuangyany.cn/gtopvsppjz.html

TS:   name: string = "x";
来源：http://hz.ehwqpu.com/gtuvjafiyb.html

Java: private String name;
来源：http://hz.xinyue.icu/gtqxztcesh.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.jianghu66.top/gthghptamd.html

Ruby: @name = "x"
来源：http://hz.birdmap.top/gtszfnuuul.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.yueranfly.top/gtmxedvkjf.html

[G04] 定义方法
来源：http://hz.shuidangran.top/gtliuqgbfb.html

Py:   def greet(self): return self.name
来源：http://hz.xuanzx.com/gtmncoltgv.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.xylfe.cn/gtmbrqwass.html

JS:   greet() { return this.name; }
来源：http://hz.andypj.xyz/gtwstqwgxh.html

TS:   greet(): string { return this.name; }
来源：http://hz.sufxvd.cn/gtmdrlhsyf.html

Java: String greet() { return name; }
来源：http://hz.cheryme.top/gtphojapbf.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.havefunace.top/gtbvxzznde.html

Ruby: def greet; @name; end
来源：http://hz.cheryme.top/gtpyqbqtro.html

C#:   public string Greet() => Name;
来源：http://hz.zhengqikj.top/gtjekujkeu.html

[G05] 继承
来源：http://hz.shanyushiyangtech.top/gtsrahozsa.html

Py:   class Admin(User): pass
来源：http://hz.cucudq.cn/gtitypmkbp.html

PHP:  class Admin extends User {}
来源：http://hz.yj20258888.top/gtqwbycvnu.html

JS:   class Admin extends User {}
来源：http://hz.sxryk.cn/gtrcrvbdxu.html

TS:   class Admin extends User {}
来源：http://hz.gaohongyu789.top/gtfvugmvvj.html

Java: class Admin extends User {}
来源：http://hz.yvedp.cn/gtvxyrlshm.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.shangyingyoupin.top/gtvlehlhhz.html

Ruby: class Admin < User; end
来源：http://hz.ehwqpu.com/gtoxtsbodu.html

C#:   class Admin : User {}
来源：http://hz.sxryk.cn/gtorddfcuw.html

[G06] 重写方法
来源：http://hz.chenlongwang.top/gtmgwmufcu.html

Py:   def greet(self): return "admin"
来源：http://hz.cdnleiting.top/gtzdjvdvty.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.nwbrower.top/gtahgjeaty.html

JS:   greet() { return "admin"; }
来源：http://hz.feifeiyinyue.top/gtpxasprfv.html

TS:   greet(): string { return "admin"; }
来源：http://hz.dianchejie.cn/gtygcdvhrf.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.jinyuanbaomall.cn/gtpascbeia.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.yj20258.top/gtukrsbmeb.html

Ruby: def greet; "admin"; end
来源：http://hz.sufxvd.cn/gtxtmifnuc.html

C#:   public override string Greet() => "admin";
来源：http://hz.zhixingplan.top/gtsyzexykr.html

[G07] 调用父类方法
来源：http://hz.guowangkeji.top/gtzeryfbyu.html

Py:   super().greet()
来源：http://hz.hnqzz.top/gtciflowad.html

PHP:  parent::greet();
来源：http://hz.ydjk.org.cn/gtwfejcrkw.html

JS:   super.greet();
来源：http://hz.yanxiufei.cn/gtijemflzn.html

TS:   super.greet();
来源：http://hz.fengsongda.top/gtfgekhdru.html

Java: super.greet();
来源：http://hz.birdmap.top/gtuqdomnen.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.hongshengwenyu.top/gtfensrqiv.html

Ruby: super
来源：http://hz.quarkkingdee.top/gtyzngznja.html

C#:   base.Greet();
来源：http://hz.316326.xyz/gtodheqhhx.html

[G08] 静态方法与属性
来源：http://hz.yonumen.top/gtlcyrsmec.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.yj202588.top/gtpqxlnjjq.html

PHP:  public static function f() {}
来源：http://hz.ydzc1.top/gteolnccjd.html

JS:   static f() {}
来源：http://hz.jiagoushi.top/gtqfmrgcvk.html

TS:   static f(): void {}
来源：http://hz.yj202588.top/gtfytkyrfq.html

Java: static void f() {}
来源：http://hz.hnxiangtu.top/gtxdsfjvzj.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.sufxvd.cn/gtgmitrgny.html

Ruby: def self.f; end
来源：http://hz.gzhubu.top/gtbzddskqq.html

C#:   public static void F() {}
来源：http://hz.zdqjudy.top/gtdqzswyez.html

[G09] 接口 / 抽象类
来源：http://hz.0kj1m.cn/gtmxgotpwz.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.ywan-chungtsiang.top/gtiywfumbp.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.xuetiantiany.cn/gtyckeqjzq.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.0kj1m.cn/gthppkhavt.html

TS:   interface Shape { area(): number; }
来源：http://hz.jqgfzy.top/gteeuixqiu.html

Java: interface Shape { double area(); }
来源：http://hz.jinyuanbaomall.cn/gtyoecygly.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.316326.xyz/gtchntalmh.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.andypj.xyz/gthgacpadh.html

C#:   interface IShape { double Area(); }
来源：http://hz.andypj.xyz/gtpqttnhws.html

[G10] 访问控制
来源：http://hz.kuanghao11.cn/gtpijpjwdb.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.9152youxi.cn/gtdqgqenqv.html

PHP:  public / protected / private
来源：http://hz.hfpthk.cn/gthaoczgop.html

JS:   #private 字段；其余公开
来源：http://hz.jinqigufen.top/gtyqttrvfr.html

TS:   public / protected / private
来源：http://hz.feifeiyinyue.top/gtrpgpztvv.html

Java: public / protected / private / 默认包级
来源：http://hz.zdqjudy.top/gtfgedqsde.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.havefunace.top/gteypdotoe.html

Ruby: public / protected / private
来源：http://hz.tian-w.cn/gtaphfjjav.html

C#:   public / protected / private / internal
来源：http://hz.hnxiangtu.top/gthkxigumf.html

[G11] getter / setter
来源：http://hz.feifeiyinyue.top/gtvtqgncgf.html

Py:   @property 与 @x.setter
来源：http://hz.pengpengdd.cyou/gtqfoqbkvp.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.jlsjyb.cn/gtiuholxbn.html

JS:   get name() { return this._name; }
来源：http://hz.haohaochexian.top/gtwvwsjcpv.html

TS:   get name(): string { return this._name; }
来源：http://hz.fengsongda.top/gtgmurwtaw.html

Java: public String getName() { return name; }
来源：http://hz.gotoacloud.top/gtanbrujbd.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.sweek.top/gteetrnhjk.html

Ruby: attr_accessor :name
来源：http://hz.xuetiantiany.cn/gtclsbcrra.html

C#:   public string Name { get; set; }
来源：http://hz.aizwys.cn/gtpshzsxea.html

[G12] 对象转字符串
来源：http://hz.cashguo.top/gtmjnetqju.html

Py:   def __str__(self): return self.name
来源：http://hz.daria6918.cn/gtyfyvrbtv.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.hammf.cn/gtaueljjbv.html

JS:   toString() { return this.name; }
来源：http://hz.shuidangran.top/gtsnioplpd.html

TS:   toString(): string { return this.name; }
来源：http://hz.fzhhl.top/gtslvptbrh.html

Java: @Override public String toString() { return name; }
来源：http://hz.shzxlz.cn/gtejncgzwq.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.yuanzhike.top/gtbkcyqcyt.html

Ruby: def to_s; @name; end
来源：http://hz.shanyushiyangkeji.top/gtmjljxvsq.html

C#:   public override string ToString() => Name;
来源：http://hz.316326.xyz/gtqczkkozu.html

[G13] 判断对象类型
来源：http://hz.hammf.cn/gtgjpyqtvz.html

Py:   isinstance(u, User)
来源：http://hz.sufxvd.cn/gtapkognjz.html

PHP:  $u instanceof User
来源：http://hz.guannengcc.top/gtxarptgih.html

JS:   u instanceof User
来源：http://hz.yangfankeji.com/gtgzdxbqum.html

TS:   u instanceof User
来源：http://hz.fzhhl.top/gtdgpzjhit.html

Java: u instanceof User
来源：http://hz.nanxuanxn.top/gtphncsfmi.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.shanyushiyangkeji.top/gtnaomxyqb.html

Ruby: u.is_a?(User)
来源：http://hz.xuetiantiany.cn/gtkumwnpmy.html

C#:   u is User
来源：http://hz.zhengqikj.top/gtjqiehpgq.html

[G14] 数据类 / record
来源：http://hz.zhijiandao.cn/gtakjvxphw.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.pengpengdd.cyou/gtmjvnzciu.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.tanke756.top/gtttwjhnwz.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.jlsjyb.cn/gtxnrdksei.html

TS:   type User = { name: string; age: number };
来源：http://hz.jqgufenzy.top/gthhdbepzn.html

Java: record User(String name, int age) {}
来源：http://hz.hongshengwenyu.top/gtfkuoxoni.html

Go:   type User struct { Name string; Age int }
来源：http://hz.ppjwa.cn/gtlemmpgun.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.hnqzz.top/gtxjprmigz.html

C#:   record User(string Name, int Age);
来源：http://hz.zhijiandao.cn/gtvflzfqfn.html

[G15] 枚举
来源：http://hz.chenjidiqi.icu/gtiaprbgln.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.cdnleiting.top/gtoiqkelfb.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.ehwqpu.com/gtsyrxpwgx.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.nanxuanxn.top/gtadjhghjc.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.mhx1999.top/gtyzszpdaq.html

Java: enum Color { RED, GREEN }
来源：http://hz.cheryme.top/gtkfkkjpap.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.sweek.top/gtqvdoaslu.html

Ruby: Color = %i[red green].freeze
来源：http://hz.cdnleiting.top/gtldaouxpv.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.snrcjt.cn/gtwfbabigy.html

[G16] 对象转数组 / 字典
来源：http://hz.kuanghao11.cn/gtpyfewfdk.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.sysykeji.top/gtpzfdffqh.html

PHP:  get_object_vars($obj);
来源：http://hz.cqqwz.cn/gtxgwztkan.html

JS:   Object.entries(obj)
来源：http://hz.yanxiufei.cn/gtvimcssir.html

TS:   Object.entries(obj)
来源：http://hz.xuanzx.com/gtzlrrzhey.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.hywenlv.cn/gtxqunhkfr.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.shangyingyoupin.top/gtwhfuzzct.html

Ruby: obj.instance_variables
来源：http://hz.gogol.net.cn/gtzvddqydf.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.ehwqpu.com/gtbmwvtsgv.html

================================================================================
来源：http://hz.52xcode.cn/gtmiczrywv.html

H. 异常与错误处理
来源：http://hz.chenlongwang.top/gtosrasiho.html

================================================================================
来源：http://hz.tanke756.top/gtpmnokihh.html

[H01] try / catch 基础
来源：http://hz.zycfv.cn/gtxrgxyoar.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.aibaodan.cn/gthpjzcimq.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.zdqjudy.top/gtsyshkowg.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.yj20258.top/gtztjmuxiy.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.sweek.top/gtgzuiskpm.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.zhaomingkeji.xyz/gtuqdofdpp.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.gotoacloud.top/gtqppakuvw.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.cucudq.cn/gtmbeultpb.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.wangshuangyany.cn/gtnfnbcwrm.html

[H02] finally / ensure 收尾
来源：http://hz.yuanzhike.top/gtjqtcikkx.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.birdmap.top/gtojoaylqa.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.zhengqikj.top/gtmokplmno.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.quarkkingdee.top/gttnokfvan.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.yj20258888.top/gtjrecgxxz.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.hnqzz.top/gtwrqxbjge.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.jqgfzy.top/gtcdsybutu.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.jyoumei.cn/gtxpcnvhfn.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.pycfn.com/gtlufkzqif.html

[H03] 主动抛出异常
来源：http://hz.52xcode.cn/gtjwmuqrfi.html

Py:   raise ValueError("错误信息")
来源：http://hz.shangyingyoupin.top/gtiidiqmrm.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.shuidangran.top/gtpmawtcxl.html

JS:   throw new Error("错误信息");
来源：http://hz.guowangkeji.top/gtywkqtgcd.html

TS:   throw new Error("错误信息");
来源：http://hz.gaohongyu789.top/gtkeihjmga.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.daxiang520.top/gtyoglxknc.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.hnqzz.top/gtorprsznq.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.jinyuanbaomall.cn/gtdlrdlisv.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.guowangkeji.top/gtbtmeboyw.html

[H04] 自定义异常类型
来源：http://hz.nanxuanxn.top/gturfuqzbb.html

Py:   class MyError(Exception): pass
来源：http://hz.gotoacloud.top/gtfeswbdji.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.sweek.top/gtprazpnir.html

JS:   class MyError extends Error {}
来源：http://hz.hywenlv.cn/gtbidsufmp.html

TS:   class MyError extends Error {}
来源：http://hz.ydjk.org.cn/gtxdxsbmuy.html

Java: class MyException extends RuntimeException {}
来源：http://hz.xylfe.cn/gtqkoffqzk.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.tianlin.xyz/gtlkwkapgr.html

Ruby: class MyError < StandardError; end
来源：http://hz.svipenyu.cn/gtzrdimiok.html

C#:   class MyException : Exception {}
来源：http://hz.ivvv.top/gtoleubdbx.html

[H05] 捕获特定类型
来源：http://hz.jianghu66.top/gthshbcagw.html

Py:   except ValueError as e:
来源：http://hz.zdqjudy.top/gtddgmlrul.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.meibo888.top/gtrdpxjgzi.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.zhixingplan.top/gttvrxuirh.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.andypj.xyz/gtpptqcjyn.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.zhaomingkeji.xyz/gtsomjjszw.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.chenzaomai.com/gteluqpxbb.html

Ruby: rescue ArgumentError => e
来源：http://hz.ydzc1.top/gtpdsyysyo.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.ydjk.org.cn/gtowcsawgl.html

[H06] 可选值 / 空值安全访问
来源：http://hz.hnxiangtu.top/gtewsfyyay.html

Py:   value = d.get("k") or default
来源：http://hz.jlsjyb.cn/gtldfwyvkt.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.zhixingplan.top/gtqrtisred.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.shuidangran.top/gtwsdnzvak.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.fengsongda.top/gtxiareows.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.jqgufenzy.top/gtgyrliovn.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.tanke756.top/gtnfylheib.html

Ruby: d&.dig(:a, :b)
来源：http://hz.yueranfly.top/gtnpzplrfl.html

C#:   obj?.A?.B ?? default
来源：http://hz.shangyingyoupin.top/gtfgfyrvnb.html

[H07] 断言
来源：http://hz.0kj1m.cn/gtuvlxgtmk.html

Py:   assert x > 0, "必须为正"
来源：http://hz.smart0.xyz/gtdvhyxxsy.html

PHP:  assert($x > 0);
来源：http://hz.mhx1999.top/gtigsblxbt.html

JS:   console.assert(x > 0);
来源：http://hz.shanyushiyangkeji.top/gtvjzrqjzs.html

TS:   console.assert(x > 0);
来源：http://hz.bjfxy.top/gtvhfuhxbf.html

Java: assert x > 0 : "必须为正";
来源：http://hz.jiagoushi.top/gtrufnegxo.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.jqgufenzy.top/gteocwezya.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.c1oappe.top/gthwtknaly.html

C#:   Debug.Assert(x > 0);
来源：http://hz.52xcode.cn/gtzelrlgwk.html

[H08] 获取错误信息与堆栈
来源：http://hz.pycfn.com/gtmahggggs.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.redwolf501.top/gtonvvzrts.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.hysaishi.cn/gtppfqahsc.html

JS:   e.message;  e.stack
来源：http://hz.gzhubu.top/gthcrqthhj.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.gogol.net.cn/gthhvwktul.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.c1oappe.top/gtudacjomt.html

Go:   err.Error()
来源：http://hz.guannengcc.top/gtjcosbsyc.html

Ruby: e.message;  e.backtrace
来源：http://hz.xuanzx.com/gtewlapbgx.html

C#:   e.Message;  e.StackTrace
来源：http://hz.pycfn.com/gtgzbtzwyv.html

[H09] 带错误码的异常
来源：http://hz.dashuyun.cn/gtvxitmokb.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.zhengqikj.top/gtafipksce.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.fzhhl.top/gtkfnsrytx.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.dianchejie.cn/gtysqeixom.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.0kj1m.cn/gtqescffym.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.tian-w.cn/gtdfqxockn.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.cucudq.cn/gtwnutruom.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.gzhubu.top/gtqajztbqe.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.yj20258888.top/gtsemhudmp.html

[H10] 资源自动释放
来源：http://hz.gaohongyu789.top/gtfwwekrak.html


<!-- 参考信息 -->