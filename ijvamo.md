代发 wailian999

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.sweek.top/gtoepoaojw.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.jianghu66.top/gtxjnkztmg.html

JS:   fs.readdirSync("dir")
来源：http://hz.yuanzhike.top/gtfzrgpsid.html

TS:   fs.readdirSync("dir")
来源：http://hz.bjfxy.top/gtmtclwpby.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.birdmap.top/gtjdygpztm.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.zhaomingkeji.xyz/gthxyjsszn.html

Ruby: Dir.children("dir")
来源：http://hz.gogol.net.cn/gtgjpaxvsz.html

C#:   Directory.GetFiles("dir")
来源：http://hz.yueranfly.top/gtsxxurxvi.html

[F09] 获取文件大小
来源：http://hz.chenlongwang.top/gtxakqaeoc.html

Py:   os.path.getsize("a.txt")
来源：http://hz.tanke756.top/gtgzdmjdko.html

PHP:  filesize("a.txt");
来源：http://hz.ywan-chungtsiang.top/gtjukcyevh.html

JS:   fs.statSync("a.txt").size
来源：http://hz.mhx1999.top/gtgosaqktc.html

TS:   fs.statSync("a.txt").size
来源：http://hz.xuanzx.com/gtiiojdoiv.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.dianchejie.cn/gtqxckwlod.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.hongshengwenyu.top/gtodxdftuf.html

Ruby: File.size("a.txt")
来源：http://hz.zhiwuduotai.top/gtkywmgswz.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.tianlin.xyz/gtvdfutlfd.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.yonumen.top/gtxutaffws.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.bjfxy.top/gtzowwikoq.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.jinyuanbaomall.cn/gtcyleoztp.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.hysaishi.cn/gtlbizkxli.html

TS:   path.extname("a.txt")
来源：http://hz.pengpengdd.cyou/gtngqkuisk.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.jlsjyb.cn/gtydajfanc.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.ydzc1.top/gtorwzhbmu.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.haohaochexian.top/gtwjzdsxya.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.yuxming.cn/gtlalbjhkb.html

[F11] 复制与移动文件
来源：http://hz.ydzc1.top/gtudnbynwq.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.cdnleiting.top/gtsqjbehrk.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.hammf.cn/gtdksscowu.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.hysaishi.cn/gtgkbprwel.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.gotoacloud.top/gttjkqgtth.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.yvedp.cn/gtbbyaztgs.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.cheryme.top/gtqfeqbdbi.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.xuanzx.com/gtmdctmson.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.jlsjyb.cn/gtxlqjzxzr.html

[F12] CSV 读写
来源：http://hz.tian-w.cn/gtzxlkbkyb.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.zhaomingkeji.xyz/gttpkaufyi.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.jyoumei.cn/gtcouctwgk.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.xziqi.cn/gtmlorxmdx.html

TS:   // 同上
来源：http://hz.bjfxy.top/gtzmlxegnf.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.guannengcc.top/gtucajuyed.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.jqgufenzy.top/gtdtbtrxct.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.yvedp.cn/gtojwofutm.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.gogol.net.cn/gtzmmwhaqy.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtwapswiro.html

G. 面向对象
来源：http://hz.guannengcc.top/gtxafxbtnn.html

================================================================================
来源：http://hz.zycfv.cn/gttslyhaue.html

[G01] 定义类
来源：http://hz.aibaodan.cn/gtlabbmbbn.html

Py:   class User: pass
来源：http://hz.jqgufenzy.top/gtsdpxetyk.html

PHP:  class User {}
来源：http://hz.tanke756.top/gtiogzlimr.html

JS:   class User {}
来源：http://hz.gogol.net.cn/gteiwupytt.html

TS:   class User { name: string = ""; }
来源：http://hz.cdnleiting.top/gttzlkcgck.html

Java: class User {}
来源：http://hz.fzhhl.top/gtxjenbapb.html

Go:   type User struct { Name string }
来源：http://hz.sweek.top/gtoazzqixr.html

Ruby: class User; end
来源：http://hz.jqgufenzy.top/gtbpbyhtcw.html

C#:   class User {}
来源：http://hz.zhongyouzk.top/gtoxvpgxjz.html

[G02] 构造函数
来源：http://hz.pycfn.com/gtxotayvmp.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.jlsjyb.cn/gtviqbjkjh.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.daxiang520.top/gtbbnvxzgy.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.xziqi.cn/gthvrskjhp.html

TS:   constructor(public name: string) {}
来源：http://hz.ppjwa.cn/gtyvanfysr.html

Java: User(String name) { this.name = name; }
来源：http://hz.dianchejie.cn/gtvjbxphit.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.ydjk.org.cn/gteehvvvdb.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.hongshengwenyu.top/gthujfgzbr.html

C#:   public User(string name) { Name = name; }
来源：http://hz.yuxming.cn/gtxfczdtjh.html

[G03] 实例属性
来源：http://hz.sufxvd.cn/gtynavknqj.html

Py:   self.name = "x"
来源：http://hz.nanxinkj.top/gtnrkmmcin.html

PHP:  public string $name = "x";
来源：http://hz.sufxvd.cn/gtytckleqv.html

JS:   this.name = "x";
来源：http://hz.zhongyouzk.top/gtvxksfqmj.html

TS:   name: string = "x";
来源：http://hz.shanyushiyangtech.top/gtlqqmfpeh.html

Java: private String name;
来源：http://hz.wangdashe.top/gtjggpydgc.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.quarkkingdee.top/gtkipaxtba.html

Ruby: @name = "x"
来源：http://hz.hammf.cn/gtszyzasvz.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.hammf.cn/gtouskwwib.html

[G04] 定义方法
来源：http://hz.sxryk.cn/gtszfhvphv.html

Py:   def greet(self): return self.name
来源：http://hz.yanxiufei.cn/gtdnjhrswu.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.wangdashe.top/gttjwekfby.html

JS:   greet() { return this.name; }
来源：http://hz.aibaodan.cn/gtgeaaaczu.html

TS:   greet(): string { return this.name; }
来源：http://hz.0kj1m.cn/gttaxlsgtq.html

Java: String greet() { return name; }
来源：http://hz.yj20258888.top/gtfgqszyva.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.xuetiantiany.cn/gtngohygxe.html

Ruby: def greet; @name; end
来源：http://hz.xinyue.icu/gtjfmocuhm.html

C#:   public string Greet() => Name;
来源：http://hz.quarkkingdee.top/gtlnvihlvf.html

[G05] 继承
来源：http://hz.chenlongwang.top/gtfeizfgxv.html

Py:   class Admin(User): pass
来源：http://hz.bjfxy.top/gtkndqtmch.html

PHP:  class Admin extends User {}
来源：http://hz.shanyushiyangkeji.top/gtfefnxynq.html

JS:   class Admin extends User {}
来源：http://hz.sufxvd.cn/gtigyysfwx.html

TS:   class Admin extends User {}
来源：http://hz.52xcode.cn/gtufnzahbg.html

Java: class Admin extends User {}
来源：http://hz.wangdashe.top/gtkwokovfl.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.mhx1999.top/gtjfllfnif.html

Ruby: class Admin < User; end
来源：http://hz.yj202588.top/gtjylibbbc.html

C#:   class Admin : User {}
来源：http://hz.316326.xyz/gtfeqthmkb.html

[G06] 重写方法
来源：http://hz.sufxvd.cn/gtbgqlowuw.html

Py:   def greet(self): return "admin"
来源：http://hz.haohaochexian.top/gtesbbbcdb.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.chenzaomai.com/gtaljrnoqq.html

JS:   greet() { return "admin"; }
来源：http://hz.snrcjt.cn/gtmrdcwzus.html

TS:   greet(): string { return "admin"; }
来源：http://hz.vqdsnc.cn/gtnuostenm.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.vqdsnc.cn/gtozuehzot.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.jiagoushi.top/gtnloymtns.html

Ruby: def greet; "admin"; end
来源：http://hz.zycfv.cn/gtmojkewti.html

C#:   public override string Greet() => "admin";
来源：http://hz.9152youxi.cn/gtyxhlndga.html

[G07] 调用父类方法
来源：http://hz.shuidangran.top/gtmznyaqlw.html

Py:   super().greet()
来源：http://hz.yanxiufei.cn/gteujymxqe.html

PHP:  parent::greet();
来源：http://hz.yangfankeji.com/gticvnzkew.html

JS:   super.greet();
来源：http://hz.jinqigufen.top/gtokggionw.html

TS:   super.greet();
来源：http://hz.ywan-chungtsiang.top/gtpklgqcsw.html

Java: super.greet();
来源：http://hz.zhengqikj.top/gtrrdscdgw.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.hfpthk.cn/gtswifqqus.html

Ruby: super
来源：http://hz.ppjwa.cn/gtyamuccat.html

C#:   base.Greet();
来源：http://hz.dashuyun.cn/gtwzznsypg.html

[G08] 静态方法与属性
来源：http://hz.cdnleiting.top/gtbnrowwgu.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.tian-w.cn/gttcizpntl.html

PHP:  public static function f() {}
来源：http://hz.hywenlv.cn/gtfykziztn.html

JS:   static f() {}
来源：http://hz.xylfe.cn/gtkdctkmev.html

TS:   static f(): void {}
来源：http://hz.jinqigufen.top/gtpvurnbmh.html

Java: static void f() {}
来源：http://hz.hammf.cn/gtqagovsey.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.c1oappe.top/gtgtntuwwn.html

Ruby: def self.f; end
来源：http://hz.0kj1m.cn/gtdrhqhoru.html

C#:   public static void F() {}
来源：http://hz.tanke756.top/gtcjuevpvb.html

[G09] 接口 / 抽象类
来源：http://hz.havefunace.top/gtyvghfwky.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.shanyushiyangtech.top/gtzicjtowz.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.shuidangran.top/gtoborvoey.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.gaohongyu789.top/gtdsnqbokf.html

TS:   interface Shape { area(): number; }
来源：http://hz.jinqigufen.top/gtqwiazhrr.html

Java: interface Shape { double area(); }
来源：http://hz.ydjk.org.cn/gtelcddljh.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.jinqigufen.top/gtfnjmhjvk.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.zhijiandao.cn/gtqjzsynja.html

C#:   interface IShape { double Area(); }
来源：http://hz.jinqigfzy.top/gtlpioipwf.html

[G10] 访问控制
来源：http://hz.yanxiufei.cn/gtmjupciip.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.dashuyun.cn/gtxmeqhgwg.html

PHP:  public / protected / private
来源：http://hz.yongpay.top/gtmwhxcanj.html

JS:   #private 字段；其余公开
来源：http://hz.yvedp.cn/gttpvdxgqk.html

TS:   public / protected / private
来源：http://hz.yongpay.top/gtfsiqaldf.html

Java: public / protected / private / 默认包级
来源：http://hz.redwolf501.top/gticjdjhxl.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.cdnleiting.top/gtquzukugf.html

Ruby: public / protected / private
来源：http://hz.cheryme.top/gtiqmyyjey.html

C#:   public / protected / private / internal
来源：http://hz.zycfv.cn/gtdnfawhjp.html

[G11] getter / setter
来源：http://hz.daria6918.cn/gtgxvlgxlr.html

Py:   @property 与 @x.setter
来源：http://hz.jiagoushi.top/gtfpkqehpd.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.jinyuanbaomall.cn/gtbpxrwmge.html

JS:   get name() { return this._name; }
来源：http://hz.guowangkeji.top/gtvijecnjv.html

TS:   get name(): string { return this._name; }
来源：http://hz.zhoulong.xyz/gtawhsapvs.html

Java: public String getName() { return name; }
来源：http://hz.cheryme.top/gtxokltric.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.svipenyu.cn/gtzsmtxszu.html

Ruby: attr_accessor :name
来源：http://hz.shuidangran.top/gtjiuhemvg.html

C#:   public string Name { get; set; }
来源：http://hz.sxryk.cn/gtvmsuxcvz.html

[G12] 对象转字符串
来源：http://hz.dashuyun.cn/gtztpxhpki.html

Py:   def __str__(self): return self.name
来源：http://hz.chenzaomai.com/gtcifwcdok.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.316326.xyz/gtwdrivcbg.html

JS:   toString() { return this.name; }
来源：http://hz.cheryme.top/gthaqzcgbp.html

TS:   toString(): string { return this.name; }
来源：http://hz.jinghuilouyu.cn/gtvdxnbgif.html

Java: @Override public String toString() { return name; }
来源：http://hz.chenlongwang.top/gtswttmxwx.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.shuidangran.top/gtvvfaxwiz.html

Ruby: def to_s; @name; end
来源：http://hz.vqdsnc.cn/gttitbhnhk.html

C#:   public override string ToString() => Name;
来源：http://hz.aizwys.cn/gtpghowgmz.html

[G13] 判断对象类型
来源：http://hz.quarkkingdee.top/gtdfcojqxx.html

Py:   isinstance(u, User)
来源：http://hz.chenzaomai.com/gtitqnbrlo.html

PHP:  $u instanceof User
来源：http://hz.hfpthk.cn/gtrctxwzfs.html

JS:   u instanceof User
来源：http://hz.cucudq.cn/gtisiaqtsq.html

TS:   u instanceof User
来源：http://hz.ehwqpu.com/gtviuctmma.html

Java: u instanceof User
来源：http://hz.tian-w.cn/gtdtzlqkmd.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.sxryk.cn/gtklerxils.html

Ruby: u.is_a?(User)
来源：http://hz.daria6918.cn/gtdgiuwrmv.html

C#:   u is User
来源：http://hz.aizwys.cn/gtjkhdateo.html

[G14] 数据类 / record
来源：http://hz.aizwys.cn/gtntutoylj.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.snrcjt.cn/gtsbebuazj.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.nanxuanxn.top/gtpczkwuke.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.zhaomingkeji.xyz/gtpbhyfjdf.html

TS:   type User = { name: string; age: number };
来源：http://hz.aizwys.cn/gthcfnmvuv.html

Java: record User(String name, int age) {}
来源：http://hz.zhaomingkeji.xyz/gtbzbeetrs.html

Go:   type User struct { Name string; Age int }
来源：http://hz.sysykeji.top/gtredbosoj.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.tanke756.top/gtflospvgu.html

C#:   record User(string Name, int Age);
来源：http://hz.jinqigufen.top/gtewlndsyc.html

[G15] 枚举
来源：http://hz.gotoacloud.top/gtyuhxgzsa.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.hnxiangtu.top/gtrcldxrfl.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.havefunace.top/gtdmyuaxdb.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.xingfuxueyuan.xyz/gtrlaktttd.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.ydjk.org.cn/gtplctbmca.html

Java: enum Color { RED, GREEN }
来源：http://hz.0kj1m.cn/gtprtwlftd.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.nanxuanxn.top/gtwuhedzdj.html

Ruby: Color = %i[red green].freeze
来源：http://hz.pengpengdd.cyou/gtdvwqkzog.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.cqqwz.cn/gtnhvoupox.html

[G16] 对象转数组 / 字典
来源：http://hz.jyoumei.cn/gtsczquayi.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.zycfv.cn/gtghxmjzak.html

PHP:  get_object_vars($obj);
来源：http://hz.jianghu66.top/gtpwmkqbty.html

JS:   Object.entries(obj)
来源：http://hz.jinqigufen.top/gtlxrzbdni.html

TS:   Object.entries(obj)
来源：http://hz.ybcxt.top/gttmxhdyfq.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.zhaomingkeji.xyz/gtrfywshqp.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.cashguo.top/gtqnkxyncx.html

Ruby: obj.instance_variables
来源：http://hz.9152youxi.cn/gtjpibwpxh.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.andypj.xyz/gtrshwcosj.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtbfvpcvvo.html

H. 异常与错误处理
来源：http://hz.yvedp.cn/gtspwosqxi.html

================================================================================
来源：http://hz.jiagoushi.top/gtfhmksfit.html

[H01] try / catch 基础
来源：http://hz.zhaomingkeji.xyz/gtrcrcshqh.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.chenjidiqi.icu/gtmxfbnwqq.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.shanyushiyangkeji.top/gtkrayvcij.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.daria6918.cn/gtplowmoak.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.shzxlz.cn/gtsfxqsfgv.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.zhoulong.xyz/gtzekfasdp.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.cqqwz.cn/gtnibxjwnv.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.dianchejie.cn/gtpfptdlfm.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.nwbrower.top/gtcsxnqsol.html

[H02] finally / ensure 收尾
来源：http://hz.xuanzx.com/gtkvmxnaul.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.ybcxt.top/gtotjhwejc.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.dianchejie.cn/gtdpndegpm.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.tian-w.cn/gtdlimohfg.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.zdqjudy.top/gtjupibzlo.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.hnqzz.top/gtjcijgyjv.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.guannengcc.top/gteujabgez.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.hysaishi.cn/gtftqelfkn.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.xingfuxueyuan.xyz/gtclblyzwo.html

[H03] 主动抛出异常
来源：http://hz.ivvv.top/gtrvhgnskg.html

Py:   raise ValueError("错误信息")
来源：http://hz.zhengqikj.top/gtqvitevsy.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.tanke756.top/gtfaqaipmv.html

JS:   throw new Error("错误信息");
来源：http://hz.fzhhl.top/gtdyjkobyo.html

TS:   throw new Error("错误信息");
来源：http://hz.zhongyouzk.top/gtsulqtpyg.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.zhongyouzk.top/gtknodwsoh.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.shanyushiyangkeji.top/gtbvgrzbgd.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.hywenlv.cn/gtorffpkzc.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.quarkkingdee.top/gtcgfckpfi.html

[H04] 自定义异常类型
来源：http://hz.hammf.cn/gtntqxvboo.html

Py:   class MyError(Exception): pass
来源：http://hz.cheryme.top/gtacsipfhz.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.jinqigfzy.top/gtgdjvdesn.html

JS:   class MyError extends Error {}
来源：http://hz.nanxuanxn.top/gtmjcxuvfk.html

TS:   class MyError extends Error {}
来源：http://hz.cucudq.cn/gtldxluvck.html

Java: class MyException extends RuntimeException {}
来源：http://hz.jianghu66.top/gtmtddufoz.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.yvedp.cn/gtvxhmuvqo.html

Ruby: class MyError < StandardError; end
来源：http://hz.haohaochexian.top/gtitrwbfir.html

C#:   class MyException : Exception {}
来源：http://hz.smart0.xyz/gtiprrnliw.html

[H05] 捕获特定类型
来源：http://hz.zdqjudy.top/gtnpedlcug.html

Py:   except ValueError as e:
来源：http://hz.shuidangran.top/gtidapsive.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.yj20258.top/gtziusjcbq.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.dianchejie.cn/gtwsyaplwk.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.jqgfzy.top/gtzociiqpo.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.svipenyu.cn/gtzwtgyhac.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.xuanzx.com/gtmxlyhsxa.html

Ruby: rescue ArgumentError => e
来源：http://hz.hammf.cn/gtochayrko.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.zhongyouzk.top/gtulttsbwf.html

[H06] 可选值 / 空值安全访问
来源：http://hz.gaohongyu789.top/gtxeicsyze.html

Py:   value = d.get("k") or default
来源：http://hz.zdqjudy.top/gtpomkerve.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.c1oappe.top/gtssadkfpt.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.guannengcc.top/gtitfrxokp.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.sxryk.cn/gtkeuacyya.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.svipenyu.cn/gtcblvrcfz.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.wangdashe.top/gtgashudgs.html

Ruby: d&.dig(:a, :b)
来源：http://hz.cashguo.top/gtrxgdilzh.html

C#:   obj?.A?.B ?? default
来源：http://hz.jinyuanbaomall.cn/gtpvlfjbst.html

[H07] 断言
来源：http://hz.sweek.top/gtvvnfitjf.html

Py:   assert x > 0, "必须为正"
来源：http://hz.52xcode.cn/gtwvhdepmx.html

PHP:  assert($x > 0);
来源：http://hz.yangfankeji.com/gtlkymbetx.html

JS:   console.assert(x > 0);
来源：http://hz.ywan-chungtsiang.top/gtxhxshcnu.html

TS:   console.assert(x > 0);
来源：http://hz.sweek.top/gtulhzkldc.html

Java: assert x > 0 : "必须为正";
来源：http://hz.tian-w.cn/gtgmsngeqw.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.jinqigfzy.top/gttioujlrg.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.jinghuilouyu.cn/gtykmbmbpp.html

C#:   Debug.Assert(x > 0);
来源：http://hz.yanxiufei.cn/gtwmwqsnuu.html

[H08] 获取错误信息与堆栈
来源：http://hz.gogol.net.cn/gtypadftid.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.chenzaomai.com/gteffheuqu.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.yongpay.top/gtlcpmzsbt.html

JS:   e.message;  e.stack
来源：http://hz.jlsjyb.cn/gtuhxnfjvc.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.snrcjt.cn/gtixluqrfx.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.0kj1m.cn/gtrlypdeig.html

Go:   err.Error()
来源：http://hz.andypj.xyz/gtjradbnmx.html

Ruby: e.message;  e.backtrace
来源：http://hz.pengpengdd.cyou/gtanvmfgbk.html

C#:   e.Message;  e.StackTrace
来源：http://hz.mhx1999.top/gteufsevqm.html

[H09] 带错误码的异常
来源：http://hz.yuxming.cn/gtitywkdge.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.nanxuanxn.top/gtvkblnkxq.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.yj20258888.top/gtbuywdvpm.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.jiagoushi.top/gtohxwienv.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.zycfv.cn/gtkrbuxfrz.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.zdqjudy.top/gtdnudovfu.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.guannengcc.top/gtsfaveiba.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.jinqigfzy.top/gtgxlqstak.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.hnxiangtu.top/gtzyhngnku.html

[H10] 资源自动释放
来源：http://hz.ydjk.org.cn/gtkhtfdezi.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.yuanzhike.top/gtotueljfz.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.bjfxy.top/gtyidnfxwa.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.cucudq.cn/gtdphwvmsq.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.redwolf501.top/gtfiittwxb.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.52xcode.cn/gtnrlimhbh.html

Go:   defer f.Close()
来源：http://hz.aizwys.cn/gtquywxble.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.shzxlz.cn/gtupxinbxm.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.shangyingyoupin.top/gtqcpnytim.html

================================================================================
来源：http://hz.haohaochexian.top/gtvkwbetwe.html

I. 正则表达式
来源：http://hz.ybcxt.top/gtrzqclave.html

================================================================================
来源：http://hz.haohaochexian.top/gtwtnxfpiq.html

[I01] 判断是否匹配
来源：http://hz.cdnleiting.top/gtyabpkmbx.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.jianghu66.top/gtrqabtstk.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.jianghu66.top/gtzvmmwjty.html

JS:   /\d+/.test(s)
来源：http://hz.cqqwz.cn/gthlwaexzi.html

TS:   /\d+/.test(s)
来源：http://hz.hnqzz.top/gtvejqodkl.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.ehwqpu.com/gttbzubmgm.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.c1oappe.top/gtuvkcwyav.html

Ruby: s.match?(/\d+/)
来源：http://hz.ppjwa.cn/gtdumjrvlx.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.zhengqikj.top/gtbwkfmzdb.html

[I02] 提取所有匹配
来源：http://hz.mhx1999.top/gtkeeurfnr.html

Py:   re.findall(r"\d+", s)
来源：http://hz.jinghuilouyu.cn/gtwgfzpire.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.pengpengdd.cyou/gtknzgznbz.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.jqgufenzy.top/gtkmfyaabp.html


<!-- 参考信息 -->