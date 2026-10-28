代发 wailian999

JS:   fs.unlinkSync("a.txt")
来源：http://hz.aizwys.cn/gttdlaxlbd.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.jianghu66.top/gtabywevhy.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.yvedp.cn/gttdnopqae.html

Go:   os.Remove("a.txt")
来源：http://hz.jinqigfzy.top/gtaeaxhgyu.html

Ruby: File.delete("a.txt")
来源：http://hz.cashguo.top/gtlfljuawx.html

C#:   File.Delete("a.txt");
来源：http://hz.hnqzz.top/gtlffojcxq.html

[F07] 创建目录（含多级）
来源：http://hz.yongpay.top/gtkntkuegz.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.gzhubu.top/gtdscrlfrk.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.52xcode.cn/gthsrxsslx.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.aibaodan.cn/gtriusslno.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.sweek.top/gtohhkyxnx.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.yanxiufei.cn/gtvsqnwrlx.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.jianghu66.top/gtgnsbcqgv.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.meibo888.top/gturgtwdhv.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.316326.xyz/gtkycwuiwe.html

[F08] 遍历目录
来源：http://hz.birdmap.top/gtzcvukwlz.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.zhiwuduotai.top/gtyalegjtg.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.cqqwz.cn/gtrmifdavj.html

JS:   fs.readdirSync("dir")
来源：http://hz.svipenyu.cn/gtayheivxh.html

TS:   fs.readdirSync("dir")
来源：http://hz.aibaodan.cn/gtlssgjpvn.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.dianchejie.cn/gtigrfltsx.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.jqgufenzy.top/gtbmpprhga.html

Ruby: Dir.children("dir")
来源：http://hz.ydjk.org.cn/gtlmbqwkzt.html

C#:   Directory.GetFiles("dir")
来源：http://hz.yuanzhike.top/gtrwbnggxj.html

[F09] 获取文件大小
来源：http://hz.ybcxt.top/gtjmlhrcnu.html

Py:   os.path.getsize("a.txt")
来源：http://hz.aizwys.cn/gtcqiozhlu.html

PHP:  filesize("a.txt");
来源：http://hz.shanyushiyangtech.top/gtmflhynux.html

JS:   fs.statSync("a.txt").size
来源：http://hz.0kj1m.cn/gtwtutlefn.html

TS:   fs.statSync("a.txt").size
来源：http://hz.yonumen.top/gtfzkxdasg.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.cdnleiting.top/gtifsikkhw.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.52xcode.cn/gtpqklpbjj.html

Ruby: File.size("a.txt")
来源：http://hz.zdqjudy.top/gtinvforyi.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.nanxuanxn.top/gtpaxujuuq.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.ydjk.org.cn/gtsytvzrei.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.shangyingyoupin.top/gttrjumdwr.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.sweek.top/gtjftybyyr.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.jqgfzy.top/gtklyxtoka.html

TS:   path.extname("a.txt")
来源：http://hz.hammf.cn/gthzwksvfp.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.yuanzhike.top/gtuktmnuim.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.shanyushiyangtech.top/gtkocoofmc.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.kuanghao11.cn/gtlnvxoamj.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.chenlongwang.top/gtxtbgbekm.html

[F11] 复制与移动文件
来源：http://hz.aizwys.cn/gtbfcrpygy.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.ppjwa.cn/gtxluflria.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.shzxlz.cn/gtnlzoxiga.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.nwbrower.top/gtgmnxhbwl.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.aizwys.cn/gtyepftvgd.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.redwolf501.top/gtevfcsqad.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.sxryk.cn/gtqtwwbgxu.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.jiagoushi.top/gtupbdxsof.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.andypj.xyz/gtbidlymsm.html

[F12] CSV 读写
来源：http://hz.hysaishi.cn/gtfblvjnpy.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.ivvv.top/gtgpdeyoot.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.hysaishi.cn/gtgmpoxkia.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.0kj1m.cn/gtofijhhnt.html

TS:   // 同上
来源：http://hz.yuxming.cn/gtsxmkbpwd.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.bjfxy.top/gtmalhlltr.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.hammf.cn/gtswklcttg.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.zycfv.cn/gthcxhufoi.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.cucudq.cn/gtfrudbpje.html

================================================================================
来源：http://hz.chenlongwang.top/gtpmnrdywp.html

G. 面向对象
来源：http://hz.nanxuanxn.top/gtundimrlz.html

================================================================================
来源：http://hz.gotoacloud.top/gtrmkcrsbm.html

[G01] 定义类
来源：http://hz.vqdsnc.cn/gtxiepmvkl.html

Py:   class User: pass
来源：http://hz.jinghuilouyu.cn/gtewdyeygn.html

PHP:  class User {}
来源：http://hz.xziqi.cn/gtgjqnthdb.html

JS:   class User {}
来源：http://hz.9152youxi.cn/gtnbwfnycr.html

TS:   class User { name: string = ""; }
来源：http://hz.xuetiantiany.cn/gtzjdnpzyu.html

Java: class User {}
来源：http://hz.zdqjudy.top/gthjpencmw.html

Go:   type User struct { Name string }
来源：http://hz.daria6918.cn/gthaztjada.html

Ruby: class User; end
来源：http://hz.tianlin.xyz/gtfzbxapgl.html

C#:   class User {}
来源：http://hz.guowangkeji.top/gtqwgzceuk.html

[G02] 构造函数
来源：http://hz.gaohongyu789.top/gtkrmrndga.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.xinyue.icu/gtxdltlkwx.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.ppjwa.cn/gtyzswjwxz.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.wangdashe.top/gtixkauhnn.html

TS:   constructor(public name: string) {}
来源：http://hz.jinghuilouyu.cn/gttuswgtqm.html

Java: User(String name) { this.name = name; }
来源：http://hz.ivvv.top/gtgpgyiyzo.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.mhx1999.top/gtpainsfia.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.nanxuanxn.top/gthozjwyjr.html

C#:   public User(string name) { Name = name; }
来源：http://hz.jinghuilouyu.cn/gtjhspuhwf.html

[G03] 实例属性
来源：http://hz.cucudq.cn/gtvdcbagah.html

Py:   self.name = "x"
来源：http://hz.hfpthk.cn/gtpsrosqhc.html

PHP:  public string $name = "x";
来源：http://hz.zhoulong.xyz/gtyqukufuc.html

JS:   this.name = "x";
来源：http://hz.xuanzx.com/gtkjbuurmu.html

TS:   name: string = "x";
来源：http://hz.nanxinkj.top/gtnafycozc.html

Java: private String name;
来源：http://hz.gzhubu.top/gtjogovywg.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.nwbrower.top/gthdchqzew.html

Ruby: @name = "x"
来源：http://hz.jianghu66.top/gtizzgwsev.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.andypj.xyz/gtwdvniuac.html

[G04] 定义方法
来源：http://hz.kuanghao11.cn/gtivsuxikc.html

Py:   def greet(self): return self.name
来源：http://hz.ivvv.top/gtbqopciel.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.nanxinkj.top/gtbvsbymln.html

JS:   greet() { return this.name; }
来源：http://hz.316326.xyz/gtgfujzjrq.html

TS:   greet(): string { return this.name; }
来源：http://hz.zycfv.cn/gttgmcujac.html

Java: String greet() { return name; }
来源：http://hz.feifeiyinyue.top/gthbfyiufo.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.shangyingyoupin.top/gtlgvtjcbu.html

Ruby: def greet; @name; end
来源：http://hz.fzhhl.top/gtjnauabth.html

C#:   public string Greet() => Name;
来源：http://hz.hammf.cn/gttbpkkgyc.html

[G05] 继承
来源：http://hz.redwolf501.top/gtyyautiov.html

Py:   class Admin(User): pass
来源：http://hz.jinqigfzy.top/gtuyvhrftn.html

PHP:  class Admin extends User {}
来源：http://hz.yongpay.top/gtzdmihoto.html

JS:   class Admin extends User {}
来源：http://hz.iojbl.cn/gtqrdmbixk.html

TS:   class Admin extends User {}
来源：http://hz.nanxinkj.top/gtbrsqhnil.html

Java: class Admin extends User {}
来源：http://hz.snrcjt.cn/gtamhdzoyy.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.9152youxi.cn/gtolbpnnwe.html

Ruby: class Admin < User; end
来源：http://hz.pengpengdd.cyou/gtcnbifloy.html

C#:   class Admin : User {}
来源：http://hz.yuanzhike.top/gtxzsbfjko.html

[G06] 重写方法
来源：http://hz.guowangkeji.top/gtvhtqggce.html

Py:   def greet(self): return "admin"
来源：http://hz.aizwys.cn/gtitzoqtqk.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.andypj.xyz/gtpwkmxsxc.html

JS:   greet() { return "admin"; }
来源：http://hz.guowangkeji.top/gtvjmdbgzy.html

TS:   greet(): string { return "admin"; }
来源：http://hz.316326.xyz/gtugpgevhi.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.nanxuanxn.top/gtjmaspftp.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.yuxming.cn/gtgksghhyh.html

Ruby: def greet; "admin"; end
来源：http://hz.ivvv.top/gtqhjzydya.html

C#:   public override string Greet() => "admin";
来源：http://hz.andypj.xyz/gtotpmzqsm.html

[G07] 调用父类方法
来源：http://hz.birdmap.top/gtqgkqxvnp.html

Py:   super().greet()
来源：http://hz.ywan-chungtsiang.top/gtlovzjiml.html

PHP:  parent::greet();
来源：http://hz.aizwys.cn/gtjhvrckrd.html

JS:   super.greet();
来源：http://hz.ehwqpu.com/gthpttcjdp.html

TS:   super.greet();
来源：http://hz.fzhhl.top/gtpsnviyzs.html

Java: super.greet();
来源：http://hz.yj202588.top/gttptiajzy.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.chenjidiqi.icu/gtjtbwtrfc.html

Ruby: super
来源：http://hz.316326.xyz/gtroadteam.html

C#:   base.Greet();
来源：http://hz.jinqigfzy.top/gtyxqliqjy.html

[G08] 静态方法与属性
来源：http://hz.zhengqikj.top/gtonmvcrvb.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.fzhhl.top/gttsvdrlgv.html

PHP:  public static function f() {}
来源：http://hz.hnxiangtu.top/gtmupcmjxw.html

JS:   static f() {}
来源：http://hz.hongshengwenyu.top/gtkqypgjml.html

TS:   static f(): void {}
来源：http://hz.andypj.xyz/gtzegwsyeq.html

Java: static void f() {}
来源：http://hz.jinqigfzy.top/gtgolpssyb.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.hfpthk.cn/gthcskfeip.html

Ruby: def self.f; end
来源：http://hz.hongshengwenyu.top/gtbvzmyyex.html

C#:   public static void F() {}
来源：http://hz.yuanzhike.top/gtvhzcptpz.html

[G09] 接口 / 抽象类
来源：http://hz.sxryk.cn/gtalsqsjoa.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.yuxming.cn/gtzmqtufcd.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.guannengcc.top/gtkfhjxqxh.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.xziqi.cn/gtyryfwcvf.html

TS:   interface Shape { area(): number; }
来源：http://hz.redwolf501.top/gtmjtxdaoz.html

Java: interface Shape { double area(); }
来源：http://hz.zhixingplan.top/gtzefpdnds.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.guannengcc.top/gtuhxcdryj.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.hywenlv.cn/gtsxhgmlhk.html

C#:   interface IShape { double Area(); }
来源：http://hz.yanxiufei.cn/gtuhjfplmu.html

[G10] 访问控制
来源：http://hz.zdqjudy.top/gtszncxqjy.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.wangshuangyany.cn/gtenosbbka.html

PHP:  public / protected / private
来源：http://hz.nwbrower.top/gtbfesgalz.html

JS:   #private 字段；其余公开
来源：http://hz.yuanzhike.top/gtkwgbblgn.html

TS:   public / protected / private
来源：http://hz.meibo888.top/gtcwgcuqud.html

Java: public / protected / private / 默认包级
来源：http://hz.xuanzx.com/gtilynjljy.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.tanke756.top/gtcileobws.html

Ruby: public / protected / private
来源：http://hz.tanke756.top/gtagnmdlud.html

C#:   public / protected / private / internal
来源：http://hz.wangshuangyany.cn/gtpmesbyct.html

[G11] getter / setter
来源：http://hz.birdmap.top/gtnclxqyrt.html

Py:   @property 与 @x.setter
来源：http://hz.0kj1m.cn/gtzagbixmt.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.tianlin.xyz/gtiiqusrqe.html

JS:   get name() { return this._name; }
来源：http://hz.xinyue.icu/gtplgbyrna.html

TS:   get name(): string { return this._name; }
来源：http://hz.aizwys.cn/gtjnkevdeh.html

Java: public String getName() { return name; }
来源：http://hz.meibo888.top/gtlhrvcyur.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.sysykeji.top/gtyfvowyhq.html

Ruby: attr_accessor :name
来源：http://hz.yanxiufei.cn/gtittwnmpi.html

C#:   public string Name { get; set; }
来源：http://hz.c1oappe.top/gtclsubzcl.html

[G12] 对象转字符串
来源：http://hz.chenzaomai.com/gttbcgrtxy.html

Py:   def __str__(self): return self.name
来源：http://hz.ydjk.org.cn/gtqfkutjkg.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.cqqwz.cn/gtgpjuldkb.html

JS:   toString() { return this.name; }
来源：http://hz.hysaishi.cn/gtnlgecrea.html

TS:   toString(): string { return this.name; }
来源：http://hz.jqgfzy.top/gteecqlraz.html

Java: @Override public String toString() { return name; }
来源：http://hz.hywenlv.cn/gtctfjktvt.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.zhoulong.xyz/gtzpyumdey.html

Ruby: def to_s; @name; end
来源：http://hz.shanyushiyangtech.top/gtfmzbijqr.html

C#:   public override string ToString() => Name;
来源：http://hz.sysykeji.top/gtnsaddyhs.html

[G13] 判断对象类型
来源：http://hz.wangdashe.top/gtlriwnhkk.html

Py:   isinstance(u, User)
来源：http://hz.zycfv.cn/gtyjikfpzu.html

PHP:  $u instanceof User
来源：http://hz.wangdashe.top/gtnhaesglb.html

JS:   u instanceof User
来源：http://hz.gzhubu.top/gthkwxxbuy.html

TS:   u instanceof User
来源：http://hz.xingfuxueyuan.xyz/gtvbctuebg.html

Java: u instanceof User
来源：http://hz.yj20258.top/gtuabwtung.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.zhijiandao.cn/gtmoxiqhov.html

Ruby: u.is_a?(User)
来源：http://hz.jinyuanbaomall.cn/gtlnzddion.html

C#:   u is User
来源：http://hz.jqgfzy.top/gtwsfyxemz.html

[G14] 数据类 / record
来源：http://hz.sysykeji.top/gtyrojqmgi.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.nwbrower.top/gtwzbnjwdr.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.sufxvd.cn/gtbgmpbrsc.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.jyoumei.cn/gtarbdboiu.html

TS:   type User = { name: string; age: number };
来源：http://hz.hfpthk.cn/gtddvktccb.html

Java: record User(String name, int age) {}
来源：http://hz.sufxvd.cn/gtupkrvxif.html

Go:   type User struct { Name string; Age int }
来源：http://hz.hfpthk.cn/gtbpcxwrjo.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.yj202588.top/gtpmzsvwcq.html

C#:   record User(string Name, int Age);
来源：http://hz.aibaodan.cn/gtawgitgdp.html

[G15] 枚举
来源：http://hz.yj20258888.top/gtsaeigves.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.yuxming.cn/gtuxqfjlmh.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.xuetiantiany.cn/gtkxkklbuz.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.nwbrower.top/gtzbtkvqta.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.yuxming.cn/gtseonjwsv.html

Java: enum Color { RED, GREEN }
来源：http://hz.jyoumei.cn/gtahbevjki.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.hfpthk.cn/gtgdnznagx.html

Ruby: Color = %i[red green].freeze
来源：http://hz.pengpengdd.cyou/gtfsqrbmxb.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.hfpthk.cn/gtcikuralb.html

[G16] 对象转数组 / 字典
来源：http://hz.zhengqikj.top/gtqtgsyxik.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.xinyue.icu/gtixshgchk.html

PHP:  get_object_vars($obj);
来源：http://hz.guowangkeji.top/gtqljgnxem.html

JS:   Object.entries(obj)
来源：http://hz.hongshengwenyu.top/gtujugerus.html

TS:   Object.entries(obj)
来源：http://hz.svipenyu.cn/gthrggvdhn.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.gaohongyu789.top/gtdkhciomm.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.dianchejie.cn/gtanzngnhu.html

Ruby: obj.instance_variables
来源：http://hz.tianlin.xyz/gtbonvkcxa.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.sufxvd.cn/gthrfuetpt.html

================================================================================
来源：http://hz.xziqi.cn/gtjmnsdvuk.html

H. 异常与错误处理
来源：http://hz.hongshengwenyu.top/gthsnyjyye.html

================================================================================
来源：http://hz.tian-w.cn/gtuhfnllez.html

[H01] try / catch 基础
来源：http://hz.shanyushiyangtech.top/gtvusyxoby.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.havefunace.top/gtdzcvytso.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.bjfxy.top/gtjpgosozx.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.gaohongyu789.top/gtuxtdyqft.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.chenlongwang.top/gtlqtwowxs.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.pycfn.com/gtpynyragd.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.nanxinkj.top/gtactgkhhh.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.zhongyouzk.top/gtprtdvdse.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.fzhhl.top/gtzjfklffr.html

[H02] finally / ensure 收尾
来源：http://hz.snrcjt.cn/gtnzehribu.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.aibaodan.cn/gtvsqzuiiy.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.jinqigfzy.top/gtliugnnhk.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.shuidangran.top/gtbmgtiacs.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.yuxming.cn/gtfpoujrpi.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.xziqi.cn/gtazgbnrob.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.cqqwz.cn/gtioxgngdy.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.redwolf501.top/gtrjtejtgz.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.shuidangran.top/gtedfhxalp.html

[H03] 主动抛出异常
来源：http://hz.cqqwz.cn/gtgscbdvfw.html

Py:   raise ValueError("错误信息")
来源：http://hz.jinqigufen.top/gtodxywetp.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.ydzc1.top/gtwfprfngu.html

JS:   throw new Error("错误信息");
来源：http://hz.mhx1999.top/gtvtstmzyn.html

TS:   throw new Error("错误信息");
来源：http://hz.sufxvd.cn/gtthvuyacw.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.cashguo.top/gtjdqxette.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.zhoulong.xyz/gtnjxlhqhn.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.yonumen.top/gtgeldmvkw.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.shzxlz.cn/gtilqnatme.html

[H04] 自定义异常类型
来源：http://hz.ywan-chungtsiang.top/gttimvrhbn.html

Py:   class MyError(Exception): pass
来源：http://hz.nanxuanxn.top/gtyorcqtxd.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.dianchejie.cn/gtdiaucayv.html

JS:   class MyError extends Error {}
来源：http://hz.hongshengwenyu.top/gtyhbchtuc.html

TS:   class MyError extends Error {}
来源：http://hz.shuidangran.top/gtwidekcxv.html

Java: class MyException extends RuntimeException {}
来源：http://hz.gotoacloud.top/gtetchzkky.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.ywan-chungtsiang.top/gtovwkstus.html

Ruby: class MyError < StandardError; end
来源：http://hz.meibo888.top/gtgtktouez.html

C#:   class MyException : Exception {}
来源：http://hz.yvedp.cn/gtcthwuwie.html

[H05] 捕获特定类型
来源：http://hz.gotoacloud.top/gtxdrmcvkd.html

Py:   except ValueError as e:
来源：http://hz.cqqwz.cn/gtswypvtjj.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.haohaochexian.top/gtzwplkigo.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.hongshengwenyu.top/gtewzieczd.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.cdnleiting.top/gtfgupihmc.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.ydzc1.top/gthqeicrns.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.meibo888.top/gtacppgecu.html

Ruby: rescue ArgumentError => e
来源：http://hz.zdqjudy.top/gtcikeoctp.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.dashuyun.cn/gtcrtxcygv.html

[H06] 可选值 / 空值安全访问
来源：http://hz.zhengqikj.top/gtuvulbbwh.html

Py:   value = d.get("k") or default
来源：http://hz.iojbl.cn/gtvjtrdqln.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.svipenyu.cn/gturhsaglk.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.jqgfzy.top/gtcauzfaqp.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.fengsongda.top/gtzphmhcfg.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.chenzaomai.com/gttbjrgngt.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.nanxinkj.top/gtqqedgokg.html

Ruby: d&.dig(:a, :b)
来源：http://hz.xingfuxueyuan.xyz/gtmzmliiuf.html

C#:   obj?.A?.B ?? default
来源：http://hz.wangshuangyany.cn/gtapblpezt.html

[H07] 断言
来源：http://hz.jinghuilouyu.cn/gtlsqneazy.html

Py:   assert x > 0, "必须为正"
来源：http://hz.iojbl.cn/gtsrviectk.html

PHP:  assert($x > 0);
来源：http://hz.birdmap.top/gtfojmqdxt.html

JS:   console.assert(x > 0);
来源：http://hz.fzhhl.top/gtgdytawtt.html

TS:   console.assert(x > 0);
来源：http://hz.yj20258888.top/gtifirziwa.html

Java: assert x > 0 : "必须为正";
来源：http://hz.tianlin.xyz/gtydeqsahq.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.daxiang520.top/gtkjstnoxm.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.nanxinkj.top/gtetcjaiib.html

C#:   Debug.Assert(x > 0);
来源：http://hz.jqgfzy.top/gtcqoxyiav.html

[H08] 获取错误信息与堆栈
来源：http://hz.jyoumei.cn/gtaqbtjwik.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.zhongyouzk.top/gtpshrivuh.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.ywan-chungtsiang.top/gtdrmawbis.html

JS:   e.message;  e.stack
来源：http://hz.jianghu66.top/gtcuobhzol.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.ywan-chungtsiang.top/gtrjziajti.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.fengsongda.top/gtttnzaiff.html

Go:   err.Error()
来源：http://hz.zhaomingkeji.xyz/gtzzgjvycf.html

Ruby: e.message;  e.backtrace
来源：http://hz.ywan-chungtsiang.top/gtreqrbbie.html

C#:   e.Message;  e.StackTrace
来源：http://hz.zhongyouzk.top/gtfziormbx.html

[H09] 带错误码的异常
来源：http://hz.zhijiandao.cn/gthpfuznif.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.yueranfly.top/gtvnqurshv.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.jinqigfzy.top/gtifofseot.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.birdmap.top/gtcegiegjp.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.shanyushiyangtech.top/gteqsjpbov.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.xuetiantiany.cn/gtrekhmbvr.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.sufxvd.cn/gtempucxij.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.dianchejie.cn/gtqiynsife.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.yonumen.top/gtxsltayst.html

[H10] 资源自动释放
来源：http://hz.yvedp.cn/gtrmshjrmz.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.kuanghao11.cn/gtfiowqzjp.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.chenlongwang.top/gtwckwcxzr.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.guowangkeji.top/gtinlqncms.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.zycfv.cn/gtcezmghto.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.cdnleiting.top/gtvygkappt.html

Go:   defer f.Close()
来源：http://hz.zdqjudy.top/gtffykplsx.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.andypj.xyz/gtumqqokuy.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.cdnleiting.top/gtvfazezym.html


<!-- 参考信息 -->