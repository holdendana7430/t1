代发 wailian999

JS:   fs.unlinkSync("a.txt")
来源：http://hz.jqgufenzy.top/gtkibwdqzh.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.yuanzhike.top/gtourohntn.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.wangshuangyany.cn/gtcehkpwst.html

Go:   os.Remove("a.txt")
来源：http://hz.pengpengdd.cyou/gtlzmbiion.html

Ruby: File.delete("a.txt")
来源：http://hz.yj20258888.top/gtjwaydtdk.html

C#:   File.Delete("a.txt");
来源：http://hz.yongpay.top/gtcbycncxg.html

[F07] 创建目录（含多级）
来源：http://hz.cqqwz.cn/gtjlxuhesm.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.sufxvd.cn/gtsbgoahtr.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.chenjidiqi.icu/gtybgmhoxs.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.shangyingyoupin.top/gtordpxgtx.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.yueranfly.top/gtbcnjwwsl.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.hysaishi.cn/gtmrmrifkf.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.hnxiangtu.top/gtxcfznsnl.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.fengsongda.top/gtvtpmvuxu.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.svipenyu.cn/gtqddnpsft.html

[F08] 遍历目录
来源：http://hz.shuidangran.top/gthqoxdclv.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.xziqi.cn/gtqcavujlz.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.jqgfzy.top/gtgvsrpcsb.html

JS:   fs.readdirSync("dir")
来源：http://hz.xylfe.cn/gtchynutkb.html

TS:   fs.readdirSync("dir")
来源：http://hz.redwolf501.top/gtxuospehe.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.hammf.cn/gtclkpvxeg.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.iojbl.cn/gtanapqbzw.html

Ruby: Dir.children("dir")
来源：http://hz.yj20258.top/gtuixefzfs.html

C#:   Directory.GetFiles("dir")
来源：http://hz.yangfankeji.com/gtabjsoaus.html

[F09] 获取文件大小
来源：http://hz.sxryk.cn/gtekpnxswg.html

Py:   os.path.getsize("a.txt")
来源：http://hz.jinyuanbaomall.cn/gtpfpwdfik.html

PHP:  filesize("a.txt");
来源：http://hz.yvedp.cn/gtkivuwdwg.html

JS:   fs.statSync("a.txt").size
来源：http://hz.cashguo.top/gtjdubufsu.html

TS:   fs.statSync("a.txt").size
来源：http://hz.pengpengdd.cyou/gtwxnexxfu.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.chenjidiqi.icu/gtjiztjsba.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.yonumen.top/gtorpccvfu.html

Ruby: File.size("a.txt")
来源：http://hz.pengpengdd.cyou/gtxpqoveno.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.ivvv.top/gtdofhquoa.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.0kj1m.cn/gtfwzhfutw.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.tanke756.top/gtfvrnjftm.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.jqgufenzy.top/gtkmiogkqc.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.yj202588.top/gtjvdbbyuv.html

TS:   path.extname("a.txt")
来源：http://hz.zycfv.cn/gtlyscszkm.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.mhx1999.top/gtxsetjvvu.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.ydjk.org.cn/gthrxqrosx.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.jinqigufen.top/gtkburtlbn.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.svipenyu.cn/gtlealnrty.html

[F11] 复制与移动文件
来源：http://hz.sufxvd.cn/gtfaybohzf.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.nanxuanxn.top/gtbgmuyboh.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.yangfankeji.com/gtsvlxohjy.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.zhaomingkeji.xyz/gtiglvihnz.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.iojbl.cn/gtvihaooht.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.zycfv.cn/gtojzhtlci.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.jianghu66.top/gtphayfuiy.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.pycfn.com/gtyxdghsfr.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.xuanzx.com/gtezoukgqg.html

[F12] CSV 读写
来源：http://hz.iojbl.cn/gtnmeraitn.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.zhongyouzk.top/gthxfwaarj.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.0kj1m.cn/gtcfafludo.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.gogol.net.cn/gtcgfwjahu.html

TS:   // 同上
来源：http://hz.gogol.net.cn/gtvomdeuth.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.cqqwz.cn/gtzuktdvjk.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.0kj1m.cn/gtdydljitm.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.xziqi.cn/gttjongcxc.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.cashguo.top/gtkcadrxkh.html

================================================================================
来源：http://hz.ybcxt.top/gtkdhvdspv.html

G. 面向对象
来源：http://hz.tanke756.top/gthvviuvqy.html

================================================================================
来源：http://hz.sufxvd.cn/gttkdbclzk.html

[G01] 定义类
来源：http://hz.redwolf501.top/gtsmlfgemg.html

Py:   class User: pass
来源：http://hz.shanyushiyangkeji.top/gtwqnipxmx.html

PHP:  class User {}
来源：http://hz.yuanzhike.top/gtckdesrmo.html

JS:   class User {}
来源：http://hz.hfpthk.cn/gtldhejuel.html

TS:   class User { name: string = ""; }
来源：http://hz.haohaochexian.top/gtpcsylvce.html

Java: class User {}
来源：http://hz.tanke756.top/gtoxfhajkh.html

Go:   type User struct { Name string }
来源：http://hz.xingfuxueyuan.xyz/gtxjwraevq.html

Ruby: class User; end
来源：http://hz.wangshuangyany.cn/gtesehztrs.html

C#:   class User {}
来源：http://hz.9152youxi.cn/gtxscoflba.html

[G02] 构造函数
来源：http://hz.aibaodan.cn/gtzckwceps.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.ydzc1.top/gtqmllpwev.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.fengsongda.top/gtssaartpm.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.gaohongyu789.top/gtidrzwkjr.html

TS:   constructor(public name: string) {}
来源：http://hz.guowangkeji.top/gtewgxuxvh.html

Java: User(String name) { this.name = name; }
来源：http://hz.gzhubu.top/gtujadhhns.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.ywan-chungtsiang.top/gtbpyuwszl.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.xziqi.cn/gtuurmgowe.html

C#:   public User(string name) { Name = name; }
来源：http://hz.quarkkingdee.top/gtimwhvgbu.html

[G03] 实例属性
来源：http://hz.jinqigfzy.top/gteknjvsjx.html

Py:   self.name = "x"
来源：http://hz.shangyingyoupin.top/gtkgcnaiwv.html

PHP:  public string $name = "x";
来源：http://hz.0kj1m.cn/gtlelwgbig.html

JS:   this.name = "x";
来源：http://hz.jqgfzy.top/gtykmaigoa.html

TS:   name: string = "x";
来源：http://hz.bjfxy.top/gtwhybxmdr.html

Java: private String name;
来源：http://hz.jinqigufen.top/gtsodfyjtt.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.jinyuanbaomall.cn/gtzveltvqg.html

Ruby: @name = "x"
来源：http://hz.pycfn.com/gtikcgrszw.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.jinghuilouyu.cn/gtxrxybslq.html

[G04] 定义方法
来源：http://hz.fzhhl.top/gtmarialcq.html

Py:   def greet(self): return self.name
来源：http://hz.hysaishi.cn/gtohwxmhyh.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.jqgfzy.top/gttstnbozn.html

JS:   greet() { return this.name; }
来源：http://hz.ivvv.top/gtewqvqwwm.html

TS:   greet(): string { return this.name; }
来源：http://hz.bjfxy.top/gtaeoczckh.html

Java: String greet() { return name; }
来源：http://hz.yj20258.top/gtqddmgcau.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.zhongyouzk.top/gtrfqqhevn.html

Ruby: def greet; @name; end
来源：http://hz.cheryme.top/gtdbvxfbzh.html

C#:   public string Greet() => Name;
来源：http://hz.dashuyun.cn/gtzimkxdiv.html

[G05] 继承
来源：http://hz.jqgfzy.top/gtyieyodzr.html

Py:   class Admin(User): pass
来源：http://hz.shzxlz.cn/gtkafxzjwk.html

PHP:  class Admin extends User {}
来源：http://hz.vqdsnc.cn/gtcbquzovs.html

JS:   class Admin extends User {}
来源：http://hz.sweek.top/gtblidceyv.html

TS:   class Admin extends User {}
来源：http://hz.sxryk.cn/gtrrsiegjx.html

Java: class Admin extends User {}
来源：http://hz.ydzc1.top/gtmgpwujqp.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.cqqwz.cn/gtlpxwiamk.html

Ruby: class Admin < User; end
来源：http://hz.ivvv.top/gtytjzxdwl.html

C#:   class Admin : User {}
来源：http://hz.cdnleiting.top/gtopptvtjt.html

[G06] 重写方法
来源：http://hz.svipenyu.cn/gtvtjnmmgi.html

Py:   def greet(self): return "admin"
来源：http://hz.nanxuanxn.top/gtjscfitqk.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.nanxuanxn.top/gtpotigmcb.html

JS:   greet() { return "admin"; }
来源：http://hz.cashguo.top/gtjdzkcwrn.html

TS:   greet(): string { return "admin"; }
来源：http://hz.daria6918.cn/gtygajcurf.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.hnxiangtu.top/gtqjaxdrrg.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.zhiwuduotai.top/gtlygvgfzk.html

Ruby: def greet; "admin"; end
来源：http://hz.wangshuangyany.cn/gttuubjsqv.html

C#:   public override string Greet() => "admin";
来源：http://hz.chenzaomai.com/gtirltjdiq.html

[G07] 调用父类方法
来源：http://hz.meibo888.top/gtfgdwetqq.html

Py:   super().greet()
来源：http://hz.gaohongyu789.top/gtmevudhjv.html

PHP:  parent::greet();
来源：http://hz.pycfn.com/gtzhwisgdm.html

JS:   super.greet();
来源：http://hz.52xcode.cn/gtemqxpwfr.html

TS:   super.greet();
来源：http://hz.gotoacloud.top/gthrtxshqu.html

Java: super.greet();
来源：http://hz.yangfankeji.com/gtmrmyiywe.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.hongshengwenyu.top/gtruvxtblc.html

Ruby: super
来源：http://hz.chenzaomai.com/gtufjjxkfa.html

C#:   base.Greet();
来源：http://hz.ydjk.org.cn/gtmfszawtv.html

[G08] 静态方法与属性
来源：http://hz.ywan-chungtsiang.top/gtdovunwzk.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.yj202588.top/gtofbdygxi.html

PHP:  public static function f() {}
来源：http://hz.9152youxi.cn/gtadgfzoxz.html

JS:   static f() {}
来源：http://hz.jinqigfzy.top/gtahwpzhgr.html

TS:   static f(): void {}
来源：http://hz.havefunace.top/gtnjifcljg.html

Java: static void f() {}
来源：http://hz.nwbrower.top/gtpxaoshmr.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.yj202588.top/gtqteuixfo.html

Ruby: def self.f; end
来源：http://hz.hysaishi.cn/gtwcunotcw.html

C#:   public static void F() {}
来源：http://hz.zhongyouzk.top/gthfwzwcvf.html

[G09] 接口 / 抽象类
来源：http://hz.zycfv.cn/gtoubujkki.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.guannengcc.top/gtlhqvgprh.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.xingfuxueyuan.xyz/gtzpbqmzze.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.jqgfzy.top/gtivowmtdk.html

TS:   interface Shape { area(): number; }
来源：http://hz.xziqi.cn/gtpoxpbdwc.html

Java: interface Shape { double area(); }
来源：http://hz.mhx1999.top/gtbnuvahbt.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.52xcode.cn/gtyzzjrbnl.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.tianlin.xyz/gtafxoqqwb.html

C#:   interface IShape { double Area(); }
来源：http://hz.sufxvd.cn/gtamjdgeiu.html

[G10] 访问控制
来源：http://hz.zhengqikj.top/gtbwpxtbzg.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.guowangkeji.top/gtdwtjfxgm.html

PHP:  public / protected / private
来源：http://hz.yuxming.cn/gtfoibysjl.html

JS:   #private 字段；其余公开
来源：http://hz.sufxvd.cn/gtnxhvzwpi.html

TS:   public / protected / private
来源：http://hz.guannengcc.top/gtucvvvbps.html

Java: public / protected / private / 默认包级
来源：http://hz.cashguo.top/gtccfzldea.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.xuetiantiany.cn/gtdispiunx.html

Ruby: public / protected / private
来源：http://hz.andypj.xyz/gtknxavmfz.html

C#:   public / protected / private / internal
来源：http://hz.xinyue.icu/gtgcbibhdm.html

[G11] getter / setter
来源：http://hz.sxryk.cn/gtgzpizqcs.html

Py:   @property 与 @x.setter
来源：http://hz.jianghu66.top/gtqjdyjqpy.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.xziqi.cn/gtmfcborur.html

JS:   get name() { return this._name; }
来源：http://hz.xziqi.cn/gtuomigieu.html

TS:   get name(): string { return this._name; }
来源：http://hz.yj20258888.top/gtwmmomxje.html

Java: public String getName() { return name; }
来源：http://hz.guowangkeji.top/gtpenhfhyd.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.ivvv.top/gtuqoejrtq.html

Ruby: attr_accessor :name
来源：http://hz.gaohongyu789.top/gtfnrmsbgc.html

C#:   public string Name { get; set; }
来源：http://hz.316326.xyz/gtdzhlvkqx.html

[G12] 对象转字符串
来源：http://hz.aibaodan.cn/gtlhoogqli.html

Py:   def __str__(self): return self.name
来源：http://hz.birdmap.top/gtygxbwlgz.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.yj20258.top/gtghtyfyaq.html

JS:   toString() { return this.name; }
来源：http://hz.zhijiandao.cn/gtpabtmtvu.html

TS:   toString(): string { return this.name; }
来源：http://hz.ydzc1.top/gtwnyxljwk.html

Java: @Override public String toString() { return name; }
来源：http://hz.cashguo.top/gtlhjtsecr.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.yuanzhike.top/gtpxgsvrzd.html

Ruby: def to_s; @name; end
来源：http://hz.0kj1m.cn/gtkuszpdtd.html

C#:   public override string ToString() => Name;
来源：http://hz.gaohongyu789.top/gtbzyqrlhl.html

[G13] 判断对象类型
来源：http://hz.zhixingplan.top/gtvhskatwh.html

Py:   isinstance(u, User)
来源：http://hz.meibo888.top/gtektdtary.html

PHP:  $u instanceof User
来源：http://hz.mhx1999.top/gtlxmtykny.html

JS:   u instanceof User
来源：http://hz.shanyushiyangtech.top/gtmdqsuxdj.html

TS:   u instanceof User
来源：http://hz.ivvv.top/gthkzgwhuq.html

Java: u instanceof User
来源：http://hz.hysaishi.cn/gtxtarzult.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.pycfn.com/gtqekulisl.html

Ruby: u.is_a?(User)
来源：http://hz.tian-w.cn/gtpbybjcdb.html

C#:   u is User
来源：http://hz.cdnleiting.top/gtcbqidjfr.html

[G14] 数据类 / record
来源：http://hz.chenzaomai.com/gtdxuouzjh.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.cucudq.cn/gtefdhkgne.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.ywan-chungtsiang.top/gtdluletjm.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.c1oappe.top/gtutjgvfpu.html

TS:   type User = { name: string; age: number };
来源：http://hz.yvedp.cn/gtaxikpivx.html

Java: record User(String name, int age) {}
来源：http://hz.zhongyouzk.top/gtvkbrudgu.html

Go:   type User struct { Name string; Age int }
来源：http://hz.gogol.net.cn/gtwobeeacc.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.ydzc1.top/gtfizgrjgi.html

C#:   record User(string Name, int Age);
来源：http://hz.vqdsnc.cn/gtrknqmxii.html

[G15] 枚举
来源：http://hz.shuidangran.top/gtuulhaawj.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.jinyuanbaomall.cn/gtjkggvwzc.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.yj202588.top/gtahgxixoh.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.zhongyouzk.top/gtkqcuwkgf.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.yuanzhike.top/gtvgbvtqyx.html

Java: enum Color { RED, GREEN }
来源：http://hz.nwbrower.top/gthsuaxndj.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.yongpay.top/gtwpyqmysy.html

Ruby: Color = %i[red green].freeze
来源：http://hz.cqqwz.cn/gtiawdivoj.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.yanxiufei.cn/gtxismygbd.html

[G16] 对象转数组 / 字典
来源：http://hz.zhongyouzk.top/gtlciwwzli.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.jiagoushi.top/gtdmtgysxi.html

PHP:  get_object_vars($obj);
来源：http://hz.xinyue.icu/gtbqbvjqzp.html

JS:   Object.entries(obj)
来源：http://hz.sxryk.cn/gtsmloyxbk.html

TS:   Object.entries(obj)
来源：http://hz.iojbl.cn/gtiuudntkq.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.zhongyouzk.top/gtsrcwabpu.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.hnqzz.top/gttmnyrffm.html

Ruby: obj.instance_variables
来源：http://hz.jinqigfzy.top/gtusdmapse.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.sysykeji.top/gtabbuucky.html

================================================================================
来源：http://hz.xylfe.cn/gtvlhzhnvm.html

H. 异常与错误处理
来源：http://hz.xingfuxueyuan.xyz/gtqpcduxtg.html

================================================================================
来源：http://hz.yj20258888.top/gtwfrgxiih.html

[H01] try / catch 基础
来源：http://hz.hywenlv.cn/gtvxmitmnl.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.gogol.net.cn/gtsiseryce.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.xuetiantiany.cn/gtfmiroogd.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.sufxvd.cn/gthnncdmrs.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.xuetiantiany.cn/gtgkxezrfy.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.havefunace.top/gtipaxikec.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.daxiang520.top/gtygwyikot.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.aibaodan.cn/gtirfhomnk.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.nanxuanxn.top/gtigryipbf.html

[H02] finally / ensure 收尾
来源：http://hz.zhixingplan.top/gtzgfuwslo.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.yonumen.top/gtfytivjyu.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.jinqigufen.top/gtyjftvmyx.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.shanyushiyangkeji.top/gtoohwlrnr.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.aizwys.cn/gtvzjrlybk.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.xinyue.icu/gtihelbdjq.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.cucudq.cn/gtauqpcmgh.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.xingfuxueyuan.xyz/gtdlcrxeet.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.smart0.xyz/gttjctjwaz.html

[H03] 主动抛出异常
来源：http://hz.sufxvd.cn/gttioivvsx.html

Py:   raise ValueError("错误信息")
来源：http://hz.0kj1m.cn/gtsvzftegz.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.tanke756.top/gttqtapxae.html

JS:   throw new Error("错误信息");
来源：http://hz.meibo888.top/gtgthtqpsp.html

TS:   throw new Error("错误信息");
来源：http://hz.gotoacloud.top/gtwszkdglu.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.hysaishi.cn/gthqagfknt.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.zycfv.cn/gtzeujvxuc.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.xuetiantiany.cn/gtmeijhqai.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.yonumen.top/gtiudwkiqi.html

[H04] 自定义异常类型
来源：http://hz.gogol.net.cn/gtnoejiiiz.html

Py:   class MyError(Exception): pass
来源：http://hz.cucudq.cn/gtfefjahpo.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.zhoulong.xyz/gtydggdpcy.html

JS:   class MyError extends Error {}
来源：http://hz.nanxuanxn.top/gtfxvcxnhx.html

TS:   class MyError extends Error {}
来源：http://hz.cdnleiting.top/gtkanqoxdg.html

Java: class MyException extends RuntimeException {}
来源：http://hz.hfpthk.cn/gtyalvqpem.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.yueranfly.top/gtmzueigos.html

Ruby: class MyError < StandardError; end
来源：http://hz.chenjidiqi.icu/gtglcvsgml.html

C#:   class MyException : Exception {}
来源：http://hz.jqgfzy.top/gtwzgzexql.html

[H05] 捕获特定类型
来源：http://hz.yj202588.top/gtkwcwjcnl.html

Py:   except ValueError as e:
来源：http://hz.yuxming.cn/gtiauugysy.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.tanke756.top/gtekernxqp.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.nanxuanxn.top/gtiybzvipf.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.yuxming.cn/gtefdwhlri.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.havefunace.top/gtilwkfafq.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.ivvv.top/gtecczuftq.html

Ruby: rescue ArgumentError => e
来源：http://hz.jqgfzy.top/gtmyhoyyrt.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.jqgfzy.top/gtprdxysgg.html

[H06] 可选值 / 空值安全访问
来源：http://hz.hfpthk.cn/gtppqwrqoh.html

Py:   value = d.get("k") or default
来源：http://hz.hywenlv.cn/gtxnfwfvfg.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.wangdashe.top/gtyjqizvzf.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.zycfv.cn/gtlksbobrf.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.zhengqikj.top/gtuhqmulvs.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.daxiang520.top/gtoyuvmoqc.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.guowangkeji.top/gthwpjceat.html

Ruby: d&.dig(:a, :b)
来源：http://hz.zhoulong.xyz/gthunqpjji.html

C#:   obj?.A?.B ?? default
来源：http://hz.ehwqpu.com/gtggtbxtsz.html

[H07] 断言
来源：http://hz.yangfankeji.com/gtftxmptmr.html

Py:   assert x > 0, "必须为正"
来源：http://hz.hfpthk.cn/gtpgdnrugi.html

PHP:  assert($x > 0);
来源：http://hz.dianchejie.cn/gtoefoibfs.html

JS:   console.assert(x > 0);
来源：http://hz.birdmap.top/gtemuhsepo.html

TS:   console.assert(x > 0);
来源：http://hz.yj20258888.top/gtwlmqyizp.html

Java: assert x > 0 : "必须为正";
来源：http://hz.gaohongyu789.top/gtdcwdqtyx.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.nanxinkj.top/gtlnckssrn.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.tanke756.top/gtadtkyghs.html

C#:   Debug.Assert(x > 0);
来源：http://hz.yj202588.top/gtxljworii.html

[H08] 获取错误信息与堆栈
来源：http://hz.dianchejie.cn/gtkoktqupo.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.jqgufenzy.top/gtdzthbeqq.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.guowangkeji.top/gtblgescxf.html

JS:   e.message;  e.stack
来源：http://hz.xziqi.cn/gtifcispog.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.ehwqpu.com/gtyvmznmkr.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.daxiang520.top/gtjkmrjyhl.html

Go:   err.Error()
来源：http://hz.jlsjyb.cn/gttotooegv.html

Ruby: e.message;  e.backtrace
来源：http://hz.nanxuanxn.top/gtofctffmy.html

C#:   e.Message;  e.StackTrace
来源：http://hz.zhijiandao.cn/gtbzpvgazf.html

[H09] 带错误码的异常
来源：http://hz.yvedp.cn/gtfzoyarcq.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.hnqzz.top/gtrprhjydt.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.sufxvd.cn/gticxglwly.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.hfpthk.cn/gttukjoswy.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.cashguo.top/gtwhpbzzxg.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.yangfankeji.com/gtaflfzpyv.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.kuanghao11.cn/gtlxfjfzxl.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.aibaodan.cn/gtooagbrbl.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.jlsjyb.cn/gtnowoeztt.html

[H10] 资源自动释放
来源：http://hz.cqqwz.cn/gtpmdxdbcg.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.yanxiufei.cn/gttxpfoicu.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.bjfxy.top/gtruwpsfws.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.ydzc1.top/gtzgpipxnm.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.wangdashe.top/gtilelxlep.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.bjfxy.top/gtnombfhxb.html

Go:   defer f.Close()
来源：http://hz.ywan-chungtsiang.top/gtqooejiyx.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.zhiwuduotai.top/gtcybuuatp.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.iojbl.cn/gtmgasvkcc.html


<!-- 参考信息 -->