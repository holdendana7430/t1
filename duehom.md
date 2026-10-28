代发 wailian999

Ruby: File.delete("a.txt")
来源：http://hz.chenzaomai.com/gtnmisytvb.html

C#:   File.Delete("a.txt");
来源：http://hz.ehwqpu.com/gtncmajvmp.html

[F07] 创建目录（含多级）
来源：http://hz.wangdashe.top/gtugetiqbp.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.guowangkeji.top/gtgfgfjsoq.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.jqgfzy.top/gtdbbwyjoy.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.smart0.xyz/gtyngcepun.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.yangfankeji.com/gteerwotob.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.fengsongda.top/gtjlwjduge.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.svipenyu.cn/gtuifnoagf.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.haohaochexian.top/gtbdsjfqnr.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.ydzc1.top/gtmtdjulzf.html

[F08] 遍历目录
来源：http://hz.shangyingyoupin.top/gttnmevhgi.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.hongshengwenyu.top/gtgcvmdkis.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.jinqigufen.top/gtgtsiqhhc.html

JS:   fs.readdirSync("dir")
来源：http://hz.aibaodan.cn/gtkyxcjvrj.html

TS:   fs.readdirSync("dir")
来源：http://hz.bjfxy.top/gtzuaixptv.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.gotoacloud.top/gtlqzxqaep.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.haohaochexian.top/gtlpfefqed.html

Ruby: Dir.children("dir")
来源：http://hz.zhiwuduotai.top/gtkwjszuwi.html

C#:   Directory.GetFiles("dir")
来源：http://hz.wangshuangyany.cn/gtpfnyhkax.html

[F09] 获取文件大小
来源：http://hz.chenlongwang.top/gtbdhhjrnr.html

Py:   os.path.getsize("a.txt")
来源：http://hz.yj202588.top/gtwezcyous.html

PHP:  filesize("a.txt");
来源：http://hz.hfpthk.cn/gtfojlhshd.html

JS:   fs.statSync("a.txt").size
来源：http://hz.gzhubu.top/gtzdbqpszv.html

TS:   fs.statSync("a.txt").size
来源：http://hz.xinyue.icu/gtrfyuzftc.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.cqqwz.cn/gtquuwetnf.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.xinyue.icu/gtpdfxouqn.html

Ruby: File.size("a.txt")
来源：http://hz.yuanzhike.top/gtzphqxaih.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.hammf.cn/gtlweodmrk.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.hnxiangtu.top/gtpcpvurnp.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.mhx1999.top/gtpnpgwvjo.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.pengpengdd.cyou/gtrnubjibw.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.xingfuxueyuan.xyz/gtufrsarms.html

TS:   path.extname("a.txt")
来源：http://hz.chenlongwang.top/gtwwnzlsrr.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.xingfuxueyuan.xyz/gtpoqongtr.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.xinyue.icu/gtlvudzitf.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.zhoulong.xyz/gtipcuzpbr.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.sysykeji.top/gthghecgoi.html

[F11] 复制与移动文件
来源：http://hz.yueranfly.top/gtqzhokuqu.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.iojbl.cn/gtyqmcuomn.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.yj20258888.top/gtxucwtidf.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.shanyushiyangkeji.top/gtmbhccigr.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.jyoumei.cn/gtkcxhkxma.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.jqgfzy.top/gtlnlzceoz.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.gogol.net.cn/gtjqyodkek.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.yvedp.cn/gtojkgsiga.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.9152youxi.cn/gtijzjvmsw.html

[F12] CSV 读写
来源：http://hz.andypj.xyz/gtlwyszykb.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.chenlongwang.top/gtfgrgpmjw.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.xuanzx.com/gtkfdtagml.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.pycfn.com/gtvjfxmcbk.html

TS:   // 同上
来源：http://hz.gotoacloud.top/gtxqiscvtn.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.shuidangran.top/gtabvrzcaj.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.zhoulong.xyz/gtnzlxjxqu.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.xinyue.icu/gtqyoafjfq.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.yongpay.top/gtalittvqo.html

================================================================================
来源：http://hz.yuanzhike.top/gtsbzrvvfg.html

G. 面向对象
来源：http://hz.gotoacloud.top/gtbuzazwut.html

================================================================================
来源：http://hz.xuanzx.com/gtykxdoqbo.html

[G01] 定义类
来源：http://hz.jiagoushi.top/gtneapxrds.html

Py:   class User: pass
来源：http://hz.quarkkingdee.top/gtmfinzrhs.html

PHP:  class User {}
来源：http://hz.tian-w.cn/gthylagoaj.html

JS:   class User {}
来源：http://hz.ywan-chungtsiang.top/gtdbenvbgn.html

TS:   class User { name: string = ""; }
来源：http://hz.zhaomingkeji.xyz/gtjzwkbodk.html

Java: class User {}
来源：http://hz.fzhhl.top/gtblxwglkc.html

Go:   type User struct { Name string }
来源：http://hz.316326.xyz/gtyojaecag.html

Ruby: class User; end
来源：http://hz.yongpay.top/gtucsgjifp.html

C#:   class User {}
来源：http://hz.mhx1999.top/gtzzwnyfci.html

[G02] 构造函数
来源：http://hz.smart0.xyz/gtedasltwj.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.yj20258.top/gtbvltesse.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.yj20258.top/gtycbhbgot.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.jyoumei.cn/gtuzykaeqb.html

TS:   constructor(public name: string) {}
来源：http://hz.tianlin.xyz/gtydhryooi.html

Java: User(String name) { this.name = name; }
来源：http://hz.hnxiangtu.top/gtwmsoronl.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.xinyue.icu/gtatyxvekt.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.yj202588.top/gtbawjlkfm.html

C#:   public User(string name) { Name = name; }
来源：http://hz.zhaomingkeji.xyz/gterivrnrs.html

[G03] 实例属性
来源：http://hz.havefunace.top/gtrgnxuthq.html

Py:   self.name = "x"
来源：http://hz.kuanghao11.cn/gtxvsxortb.html

PHP:  public string $name = "x";
来源：http://hz.cdnleiting.top/gtxotnhzxm.html

JS:   this.name = "x";
来源：http://hz.jlsjyb.cn/gtlrsckqeh.html

TS:   name: string = "x";
来源：http://hz.yongpay.top/gtvyzucpxq.html

Java: private String name;
来源：http://hz.tian-w.cn/gtdllnvsrw.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.mhx1999.top/gtikvveqei.html

Ruby: @name = "x"
来源：http://hz.vqdsnc.cn/gtepepfeod.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.iojbl.cn/gtqvmmxncb.html

[G04] 定义方法
来源：http://hz.hywenlv.cn/gtvopwfxza.html

Py:   def greet(self): return self.name
来源：http://hz.hammf.cn/gtchhhjtxy.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.tianlin.xyz/gtqthyzerx.html

JS:   greet() { return this.name; }
来源：http://hz.kuanghao11.cn/gtkqxlsyio.html

TS:   greet(): string { return this.name; }
来源：http://hz.hnqzz.top/gtzxwvammg.html

Java: String greet() { return name; }
来源：http://hz.cdnleiting.top/gtfblavfro.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.nanxuanxn.top/gtxuszycnb.html

Ruby: def greet; @name; end
来源：http://hz.daxiang520.top/gtlotjcpkt.html

C#:   public string Greet() => Name;
来源：http://hz.jyoumei.cn/gthayghmlj.html

[G05] 继承
来源：http://hz.yonumen.top/gtinlygusw.html

Py:   class Admin(User): pass
来源：http://hz.dashuyun.cn/gtpnapwfck.html

PHP:  class Admin extends User {}
来源：http://hz.tianlin.xyz/gttdfzxhsr.html

JS:   class Admin extends User {}
来源：http://hz.redwolf501.top/gthfnqebqu.html

TS:   class Admin extends User {}
来源：http://hz.cqqwz.cn/gtkwzcbtec.html

Java: class Admin extends User {}
来源：http://hz.shzxlz.cn/gtbalwsfjy.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.pengpengdd.cyou/gtuyymambw.html

Ruby: class Admin < User; end
来源：http://hz.52xcode.cn/gtspzjhhpd.html

C#:   class Admin : User {}
来源：http://hz.daria6918.cn/gtuhvhimph.html

[G06] 重写方法
来源：http://hz.zhaomingkeji.xyz/gteqbshzwm.html

Py:   def greet(self): return "admin"
来源：http://hz.ybcxt.top/gtxfppiujw.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.nanxuanxn.top/gtnuzaszei.html

JS:   greet() { return "admin"; }
来源：http://hz.yvedp.cn/gthfycbede.html

TS:   greet(): string { return "admin"; }
来源：http://hz.jlsjyb.cn/gtinthgqtx.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.yuxming.cn/gtqehyreuj.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.yuxming.cn/gtaqqbxvmw.html

Ruby: def greet; "admin"; end
来源：http://hz.xuanzx.com/gtsxgaznjz.html

C#:   public override string Greet() => "admin";
来源：http://hz.nanxuanxn.top/gtvneowixj.html

[G07] 调用父类方法
来源：http://hz.feifeiyinyue.top/gtitqebwny.html

Py:   super().greet()
来源：http://hz.ivvv.top/gtavosvpqi.html

PHP:  parent::greet();
来源：http://hz.gotoacloud.top/gtvyfhvlcr.html

JS:   super.greet();
来源：http://hz.fengsongda.top/gttkecthey.html

TS:   super.greet();
来源：http://hz.haohaochexian.top/gtkjjanewp.html

Java: super.greet();
来源：http://hz.xuanzx.com/gtscopoozc.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.9152youxi.cn/gtnsxrigzc.html

Ruby: super
来源：http://hz.wangdashe.top/gtttmbbyzo.html

C#:   base.Greet();
来源：http://hz.bjfxy.top/gtjikeufhd.html

[G08] 静态方法与属性
来源：http://hz.kuanghao11.cn/gtydolvqlq.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.sweek.top/gtpkepywvr.html

PHP:  public static function f() {}
来源：http://hz.yuanzhike.top/gtetjmwnin.html

JS:   static f() {}
来源：http://hz.xingfuxueyuan.xyz/gtvfofpnlj.html

TS:   static f(): void {}
来源：http://hz.dashuyun.cn/gtozfitrvl.html

Java: static void f() {}
来源：http://hz.dashuyun.cn/gtgnqcerlv.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.vqdsnc.cn/gtkjbmksny.html

Ruby: def self.f; end
来源：http://hz.chenlongwang.top/gtdpolsgti.html

C#:   public static void F() {}
来源：http://hz.shanyushiyangtech.top/gtvwiotbul.html

[G09] 接口 / 抽象类
来源：http://hz.feifeiyinyue.top/gticncleqp.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.jlsjyb.cn/gtmzizhgga.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.guannengcc.top/gtsdkdkpqv.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.sysykeji.top/gtadqxqela.html

TS:   interface Shape { area(): number; }
来源：http://hz.yangfankeji.com/gtvrxyiqfj.html

Java: interface Shape { double area(); }
来源：http://hz.gzhubu.top/gtrnfszbhh.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.xuetiantiany.cn/gtkjihkifl.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.yj20258.top/gtmvieofex.html

C#:   interface IShape { double Area(); }
来源：http://hz.zhoulong.xyz/gtqcbjhvsp.html

[G10] 访问控制
来源：http://hz.shanyushiyangkeji.top/gtvdmqnttv.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.wangdashe.top/gtqapybvje.html

PHP:  public / protected / private
来源：http://hz.yj20258.top/gtdmwamzgz.html

JS:   #private 字段；其余公开
来源：http://hz.jinghuilouyu.cn/gtgraavoqu.html

TS:   public / protected / private
来源：http://hz.ydzc1.top/gtevtqhubr.html

Java: public / protected / private / 默认包级
来源：http://hz.nanxinkj.top/gteuukgjpu.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.hammf.cn/gtqzmqhwey.html

Ruby: public / protected / private
来源：http://hz.cqqwz.cn/gtgelnyglb.html

C#:   public / protected / private / internal
来源：http://hz.gaohongyu789.top/gthrteyzqd.html

[G11] getter / setter
来源：http://hz.jianghu66.top/gtswdbnnyb.html

Py:   @property 与 @x.setter
来源：http://hz.zhijiandao.cn/gtrkcrfyjv.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.tanke756.top/gtrwepsesn.html

JS:   get name() { return this._name; }
来源：http://hz.xylfe.cn/gtdcwwfhfi.html

TS:   get name(): string { return this._name; }
来源：http://hz.zhoulong.xyz/gtznwjdtgr.html

Java: public String getName() { return name; }
来源：http://hz.sufxvd.cn/gtdvdgfnch.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.yangfankeji.com/gtychobyci.html

Ruby: attr_accessor :name
来源：http://hz.hywenlv.cn/gtyioeydvs.html

C#:   public string Name { get; set; }
来源：http://hz.yj20258888.top/gtudhgimpp.html

[G12] 对象转字符串
来源：http://hz.0kj1m.cn/gtxyvaxzps.html

Py:   def __str__(self): return self.name
来源：http://hz.zhaomingkeji.xyz/gtumsytdiq.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.xingfuxueyuan.xyz/gttsflnnqz.html

JS:   toString() { return this.name; }
来源：http://hz.haohaochexian.top/gtmebdvhwr.html

TS:   toString(): string { return this.name; }
来源：http://hz.birdmap.top/gtutufvrco.html

Java: @Override public String toString() { return name; }
来源：http://hz.yj202588.top/gtsewebbnu.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.bjfxy.top/gtlotxydzx.html

Ruby: def to_s; @name; end
来源：http://hz.fengsongda.top/gtdjmeqpai.html

C#:   public override string ToString() => Name;
来源：http://hz.yongpay.top/gtgshnhciw.html

[G13] 判断对象类型
来源：http://hz.xuetiantiany.cn/gtmrdmxwne.html

Py:   isinstance(u, User)
来源：http://hz.yvedp.cn/gtvinaqosc.html

PHP:  $u instanceof User
来源：http://hz.ywan-chungtsiang.top/gtxnkvdibs.html

JS:   u instanceof User
来源：http://hz.cucudq.cn/gtepibkjng.html

TS:   u instanceof User
来源：http://hz.vqdsnc.cn/gtskbunmhp.html

Java: u instanceof User
来源：http://hz.hywenlv.cn/gtzfmgpqkp.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.zhaomingkeji.xyz/gtgduuepul.html

Ruby: u.is_a?(User)
来源：http://hz.jqgufenzy.top/gtrndzrnzv.html

C#:   u is User
来源：http://hz.gaohongyu789.top/gtcbktnkjb.html

[G14] 数据类 / record
来源：http://hz.yuxming.cn/gtxfznkuic.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.iojbl.cn/gtuodhzcax.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.jinghuilouyu.cn/gtvrzpfoet.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.hysaishi.cn/gtvulapvwc.html

TS:   type User = { name: string; age: number };
来源：http://hz.nanxinkj.top/gtsjxpghqh.html

Java: record User(String name, int age) {}
来源：http://hz.sxryk.cn/gtyljarhdd.html

Go:   type User struct { Name string; Age int }
来源：http://hz.kuanghao11.cn/gtnqgemxlu.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.yj20258888.top/gtayjqorqo.html

C#:   record User(string Name, int Age);
来源：http://hz.hongshengwenyu.top/gtkmrzuvdf.html

[G15] 枚举
来源：http://hz.havefunace.top/gtbnphxjnw.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.vqdsnc.cn/gtbtonbgxs.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.guannengcc.top/gtydboyhoy.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.hongshengwenyu.top/gtcibtnmju.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.yanxiufei.cn/gtwlpjipgp.html

Java: enum Color { RED, GREEN }
来源：http://hz.mhx1999.top/gtwrklezrs.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.chenzaomai.com/gtcgwshvuj.html

Ruby: Color = %i[red green].freeze
来源：http://hz.snrcjt.cn/gtjmfotxxm.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.daria6918.cn/gtqkdspspu.html

[G16] 对象转数组 / 字典
来源：http://hz.tianlin.xyz/gtnznwelvc.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.jiagoushi.top/gtrvknebdi.html

PHP:  get_object_vars($obj);
来源：http://hz.zhiwuduotai.top/gtxqtgmklr.html

JS:   Object.entries(obj)
来源：http://hz.chenzaomai.com/gtcwkoppoq.html

TS:   Object.entries(obj)
来源：http://hz.tianlin.xyz/gtrqjpusad.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.daxiang520.top/gtuffpmpdu.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.zycfv.cn/gtwedolvvn.html

Ruby: obj.instance_variables
来源：http://hz.yanxiufei.cn/gtnwweqvxf.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.hammf.cn/gtldzvjklz.html

================================================================================
来源：http://hz.sxryk.cn/gtjtoegjll.html

H. 异常与错误处理
来源：http://hz.9152youxi.cn/gtfvuwnydh.html

================================================================================
来源：http://hz.haohaochexian.top/gtheizqmun.html

[H01] try / catch 基础
来源：http://hz.yvedp.cn/gtnwypmnlk.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.daria6918.cn/gtbsajnjlo.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.zhongyouzk.top/gtzmjqmrig.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.fzhhl.top/gtkfdewott.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.zhaomingkeji.xyz/gtzxpyajwv.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.cashguo.top/gtqovdnejr.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.cucudq.cn/gtnxpgrwju.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.cheryme.top/gtyfgkctrr.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.hammf.cn/gtrywofbth.html

[H02] finally / ensure 收尾
来源：http://hz.cheryme.top/gtauylrbfb.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.redwolf501.top/gtzhyurgyb.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.quarkkingdee.top/gtxgwkylck.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.jlsjyb.cn/gtqwbpyooy.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.svipenyu.cn/gteieczhju.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.yvedp.cn/gtzalqzkli.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.sxryk.cn/gtrzvaioon.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.nanxuanxn.top/gtuiykmann.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.yj20258.top/gtjtwtbzje.html

[H03] 主动抛出异常
来源：http://hz.wangdashe.top/gtpljhtwdk.html

Py:   raise ValueError("错误信息")
来源：http://hz.hnxiangtu.top/gtrsaehqpg.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.daxiang520.top/gtavyyjfed.html

JS:   throw new Error("错误信息");
来源：http://hz.jinqigufen.top/gtpuofvyho.html

TS:   throw new Error("错误信息");
来源：http://hz.yuanzhike.top/gtpakvsvib.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.tian-w.cn/gtfanetoor.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.ybcxt.top/gtwgmcbgxb.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.316326.xyz/gttqqucyxe.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.daria6918.cn/gtgdcplayr.html

[H04] 自定义异常类型
来源：http://hz.yongpay.top/gtxjsnieyj.html

Py:   class MyError(Exception): pass
来源：http://hz.xuetiantiany.cn/gtcnalygmd.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.hnqzz.top/gthihezfsr.html

JS:   class MyError extends Error {}
来源：http://hz.meibo888.top/gtzdbtraoq.html

TS:   class MyError extends Error {}
来源：http://hz.svipenyu.cn/gtupuqhxaz.html

Java: class MyException extends RuntimeException {}
来源：http://hz.yanxiufei.cn/gtmadjadgy.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.zhaomingkeji.xyz/gtcvdsefps.html

Ruby: class MyError < StandardError; end
来源：http://hz.hfpthk.cn/gtakstudcs.html

C#:   class MyException : Exception {}
来源：http://hz.dashuyun.cn/gtqhiqmhph.html

[H05] 捕获特定类型
来源：http://hz.guowangkeji.top/gtqsghpppl.html

Py:   except ValueError as e:
来源：http://hz.nwbrower.top/gtgatsnkgq.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.gotoacloud.top/gtvawtczkz.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.hnxiangtu.top/gtcvhjgwcp.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.daria6918.cn/gtgygzypyo.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.yj202588.top/gtdyttyhzp.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.chenjidiqi.icu/gtkrmqgstc.html

Ruby: rescue ArgumentError => e
来源：http://hz.chenlongwang.top/gtouexskhx.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.dashuyun.cn/gtflqmdbsw.html

[H06] 可选值 / 空值安全访问
来源：http://hz.zycfv.cn/gttrrzsbdn.html

Py:   value = d.get("k") or default
来源：http://hz.yj20258888.top/gtilcuuwxq.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.yongpay.top/gtqfkmsgta.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.ivvv.top/gtpojvtvln.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.jinqigufen.top/gtkqsmzlea.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.hnxiangtu.top/gtcntaisct.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.yuxming.cn/gtgqlefmlr.html

Ruby: d&.dig(:a, :b)
来源：http://hz.shangyingyoupin.top/gtwruogczc.html

C#:   obj?.A?.B ?? default
来源：http://hz.daxiang520.top/gtdmgrpfqf.html

[H07] 断言
来源：http://hz.gaohongyu789.top/gteyalsoyi.html

Py:   assert x > 0, "必须为正"
来源：http://hz.yanxiufei.cn/gtjdopfzdf.html

PHP:  assert($x > 0);
来源：http://hz.hfpthk.cn/gtsrtdduyq.html

JS:   console.assert(x > 0);
来源：http://hz.yuanzhike.top/gtujthryqa.html

TS:   console.assert(x > 0);
来源：http://hz.ywan-chungtsiang.top/gtcxtzvpbq.html

Java: assert x > 0 : "必须为正";
来源：http://hz.tian-w.cn/gttnavxqkv.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.cheryme.top/gtigafiozm.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.yvedp.cn/gtlbwfctwk.html

C#:   Debug.Assert(x > 0);
来源：http://hz.ybcxt.top/gtrhpwqknk.html

[H08] 获取错误信息与堆栈
来源：http://hz.fengsongda.top/gtpzvbanzc.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.cashguo.top/gtpcwaidhm.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.yangfankeji.com/gtyqqcbcyz.html

JS:   e.message;  e.stack
来源：http://hz.316326.xyz/gtoizjczzy.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.chenjidiqi.icu/gtvidqttph.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.hnxiangtu.top/gtmabjfxct.html

Go:   err.Error()
来源：http://hz.bjfxy.top/gthgijphpe.html

Ruby: e.message;  e.backtrace
来源：http://hz.jqgufenzy.top/gtaoksujmk.html

C#:   e.Message;  e.StackTrace
来源：http://hz.guannengcc.top/gtwlpkqcsk.html

[H09] 带错误码的异常
来源：http://hz.jinqigufen.top/gtfcuhlrqb.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.nwbrower.top/gtbxqbduxv.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.jlsjyb.cn/gtftbwbljg.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.jinyuanbaomall.cn/gtesyvqaib.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.jinyuanbaomall.cn/gtgetrwioy.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.52xcode.cn/gtboiinksw.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.smart0.xyz/gthtqxrrvk.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.shuidangran.top/gttnkalelx.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.chenzaomai.com/gtlmpfviws.html

[H10] 资源自动释放
来源：http://hz.smart0.xyz/gtswylqmbq.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.smart0.xyz/gtxzqgoaze.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.gaohongyu789.top/gteudumsft.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.feifeiyinyue.top/gtvpydzael.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.zdqjudy.top/gtwtffxwfp.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.snrcjt.cn/gtgktmppyz.html

Go:   defer f.Close()
来源：http://hz.shzxlz.cn/gtqhgdabjs.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.pengpengdd.cyou/gtyhehuupd.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.yueranfly.top/gtpowvgfnx.html

================================================================================
来源：http://hz.kuanghao11.cn/gtlbrvgvyl.html

I. 正则表达式
来源：http://hz.hnxiangtu.top/gtbvbgmyem.html

================================================================================
来源：http://hz.cucudq.cn/gtbmojinuf.html

[I01] 判断是否匹配
来源：http://hz.cdnleiting.top/gtyxtahrxy.html


<!-- 参考信息 -->