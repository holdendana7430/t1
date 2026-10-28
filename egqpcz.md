代发 wailian999

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.cheryme.top/gtuhuhxghs.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.aizwys.cn/gtrlkdpmim.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.zhongyouzk.top/gtnqpxuodv.html

[F08] 遍历目录
来源：http://hz.9152youxi.cn/gtrklyllwd.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.xingfuxueyuan.xyz/gtjyteqxlo.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.haohaochexian.top/gtvtsnfzju.html

JS:   fs.readdirSync("dir")
来源：http://hz.haohaochexian.top/gtftvpbbgk.html

TS:   fs.readdirSync("dir")
来源：http://hz.shangyingyoupin.top/gtggxfzyua.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.yongpay.top/gtuqghxebz.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.yangfankeji.com/gtcsdwhwnt.html

Ruby: Dir.children("dir")
来源：http://hz.hfpthk.cn/gtrabyrxvt.html

C#:   Directory.GetFiles("dir")
来源：http://hz.jinqigfzy.top/gtbyvvuzzg.html

[F09] 获取文件大小
来源：http://hz.yueranfly.top/gttqqvcolu.html

Py:   os.path.getsize("a.txt")
来源：http://hz.hfpthk.cn/gtveziruwk.html

PHP:  filesize("a.txt");
来源：http://hz.zhixingplan.top/gthmkxpnch.html

JS:   fs.statSync("a.txt").size
来源：http://hz.9152youxi.cn/gtejdnejwr.html

TS:   fs.statSync("a.txt").size
来源：http://hz.xuetiantiany.cn/gtmldiuflp.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.jinqigfzy.top/gtkzkgtudd.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.fengsongda.top/gtahsdclqk.html

Ruby: File.size("a.txt")
来源：http://hz.gaohongyu789.top/gtkghzzawc.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.smart0.xyz/gtnqkxvfcs.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.yj202588.top/gtcfskumef.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.jyoumei.cn/gtormsjitz.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.shuidangran.top/gtvnkfekwy.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.chenjidiqi.icu/gtugwmtbtp.html

TS:   path.extname("a.txt")
来源：http://hz.fengsongda.top/gtgjztglgw.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.nanxinkj.top/gttzrhtozq.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.wangdashe.top/gtwdowldwb.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.gaohongyu789.top/gtpggkuabl.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.hnxiangtu.top/gtomdhzfqb.html

[F11] 复制与移动文件
来源：http://hz.yuxming.cn/gtfzrelzer.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.bjfxy.top/gtjzejwfnj.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.yj20258.top/gteyxwugjl.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.hammf.cn/gtttgrbsje.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.shangyingyoupin.top/gtqxyzdygj.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.gzhubu.top/gtfpbcukqe.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.dashuyun.cn/gtnvaenjkg.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.dashuyun.cn/gthogvadqh.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.aizwys.cn/gtxpmmrwop.html

[F12] CSV 读写
来源：http://hz.dianchejie.cn/gtpqtmtbgb.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.sxryk.cn/gtshlqczhb.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.hnqzz.top/gtismrzwwq.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.yj20258888.top/gtzptzmlam.html

TS:   // 同上
来源：http://hz.gotoacloud.top/gtckvjqtvx.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.feifeiyinyue.top/gtcapamgxw.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.zycfv.cn/gtptwlotsh.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.chenjidiqi.icu/gtejjlxmma.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.quarkkingdee.top/gtufmpmymb.html

================================================================================
来源：http://hz.gzhubu.top/gteokytdmx.html

G. 面向对象
来源：http://hz.zhongyouzk.top/gtzpgfsbye.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtxxmezmkw.html

[G01] 定义类
来源：http://hz.daxiang520.top/gthlqtxndn.html

Py:   class User: pass
来源：http://hz.jianghu66.top/gtjaiiogta.html

PHP:  class User {}
来源：http://hz.jyoumei.cn/gtqxmyqvem.html

JS:   class User {}
来源：http://hz.hywenlv.cn/gtajyztzjk.html

TS:   class User { name: string = ""; }
来源：http://hz.shangyingyoupin.top/gtrbwxcwsx.html

Java: class User {}
来源：http://hz.yueranfly.top/gtdlbyhpei.html

Go:   type User struct { Name string }
来源：http://hz.xylfe.cn/gtynmiogkz.html

Ruby: class User; end
来源：http://hz.xziqi.cn/gtzhcjfmqw.html

C#:   class User {}
来源：http://hz.zhengqikj.top/gtxfnnmfud.html

[G02] 构造函数
来源：http://hz.cheryme.top/gtwinjlnpp.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.52xcode.cn/gtbbbmdtjl.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.hfpthk.cn/gtwfqbakvx.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.redwolf501.top/gtmhvpdfrc.html

TS:   constructor(public name: string) {}
来源：http://hz.hywenlv.cn/gttcpevobz.html

Java: User(String name) { this.name = name; }
来源：http://hz.wangshuangyany.cn/gtqmmpwchz.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.jinghuilouyu.cn/gtnxohpmtf.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.316326.xyz/gtnlisrccj.html

C#:   public User(string name) { Name = name; }
来源：http://hz.cheryme.top/gtoewvgmac.html

[G03] 实例属性
来源：http://hz.mhx1999.top/gtepgofdch.html

Py:   self.name = "x"
来源：http://hz.yuanzhike.top/gttqyjxxtq.html

PHP:  public string $name = "x";
来源：http://hz.c1oappe.top/gtncoyobib.html

JS:   this.name = "x";
来源：http://hz.yangfankeji.com/gtitjjkhud.html

TS:   name: string = "x";
来源：http://hz.daria6918.cn/gtcgwktvbm.html

Java: private String name;
来源：http://hz.zhiwuduotai.top/gtjfbytncl.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.9152youxi.cn/gtqkmpbylt.html

Ruby: @name = "x"
来源：http://hz.xuanzx.com/gtzwhymzje.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.tanke756.top/gtshgvhetz.html

[G04] 定义方法
来源：http://hz.fengsongda.top/gtvkrnescn.html

Py:   def greet(self): return self.name
来源：http://hz.yonumen.top/gtvhwyglrq.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.jinghuilouyu.cn/gtlctvopjv.html

JS:   greet() { return this.name; }
来源：http://hz.hywenlv.cn/gtrtrrrvyu.html

TS:   greet(): string { return this.name; }
来源：http://hz.kuanghao11.cn/gtpolmwndp.html

Java: String greet() { return name; }
来源：http://hz.nwbrower.top/gtpxgpohbm.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.nanxinkj.top/gtdalvmfnq.html

Ruby: def greet; @name; end
来源：http://hz.ehwqpu.com/gtsqlqzxgs.html

C#:   public string Greet() => Name;
来源：http://hz.yueranfly.top/gtetnjdkvj.html

[G05] 继承
来源：http://hz.jqgfzy.top/gtzuqpozlh.html

Py:   class Admin(User): pass
来源：http://hz.pengpengdd.cyou/gtxmqdxavn.html

PHP:  class Admin extends User {}
来源：http://hz.jqgufenzy.top/gthhrykden.html

JS:   class Admin extends User {}
来源：http://hz.0kj1m.cn/gtiwzamujp.html

TS:   class Admin extends User {}
来源：http://hz.kuanghao11.cn/gtyfgmswox.html

Java: class Admin extends User {}
来源：http://hz.cucudq.cn/gtvqjajozd.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.jlsjyb.cn/gtsnnksrwb.html

Ruby: class Admin < User; end
来源：http://hz.gaohongyu789.top/gtprepbffe.html

C#:   class Admin : User {}
来源：http://hz.nanxuanxn.top/gtmeuquvub.html

[G06] 重写方法
来源：http://hz.zhengqikj.top/gtykktsgmz.html

Py:   def greet(self): return "admin"
来源：http://hz.jiagoushi.top/gtpvtcekgg.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.yj20258.top/gthmenedtw.html

JS:   greet() { return "admin"; }
来源：http://hz.yonumen.top/gtylaxoxvx.html

TS:   greet(): string { return "admin"; }
来源：http://hz.jinghuilouyu.cn/gthntvepne.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.dashuyun.cn/gtpicvxxep.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.bjfxy.top/gtoumrbvxy.html

Ruby: def greet; "admin"; end
来源：http://hz.pengpengdd.cyou/gtfwpyuepb.html

C#:   public override string Greet() => "admin";
来源：http://hz.gotoacloud.top/gtmonqhrfv.html

[G07] 调用父类方法
来源：http://hz.aibaodan.cn/gtwxjqeqia.html

Py:   super().greet()
来源：http://hz.guowangkeji.top/gtjkgegzma.html

PHP:  parent::greet();
来源：http://hz.hysaishi.cn/gtoirnrnai.html

JS:   super.greet();
来源：http://hz.xuetiantiany.cn/gttwacvcip.html

TS:   super.greet();
来源：http://hz.zhoulong.xyz/gtzkvfgctd.html

Java: super.greet();
来源：http://hz.9152youxi.cn/gthzvzzzpw.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.tanke756.top/gtwmigbxuj.html

Ruby: super
来源：http://hz.chenzaomai.com/gtrqduntgt.html

C#:   base.Greet();
来源：http://hz.meibo888.top/gtfezipams.html

[G08] 静态方法与属性
来源：http://hz.cdnleiting.top/gtfieyhgoa.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.dashuyun.cn/gtkphvvczc.html

PHP:  public static function f() {}
来源：http://hz.xziqi.cn/gtwmfahcmp.html

JS:   static f() {}
来源：http://hz.zhongyouzk.top/gtoxzdylui.html

TS:   static f(): void {}
来源：http://hz.xuetiantiany.cn/gtbdmpajxr.html

Java: static void f() {}
来源：http://hz.52xcode.cn/gtqzudiwpv.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.chenlongwang.top/gtpmydgkdh.html

Ruby: def self.f; end
来源：http://hz.tian-w.cn/gtmcytcpsl.html

C#:   public static void F() {}
来源：http://hz.tianlin.xyz/gthtswdhxy.html

[G09] 接口 / 抽象类
来源：http://hz.nwbrower.top/gtyiypxfxq.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.xuetiantiany.cn/gtsgaxbeda.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.9152youxi.cn/gttqnrpbxt.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.xuanzx.com/gtfyxdfodz.html

TS:   interface Shape { area(): number; }
来源：http://hz.ybcxt.top/gtcjrftxel.html

Java: interface Shape { double area(); }
来源：http://hz.sweek.top/gtfyarzzan.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.jqgfzy.top/gtackmlhdx.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.nanxinkj.top/gtbmetropq.html

C#:   interface IShape { double Area(); }
来源：http://hz.smart0.xyz/gtedwmtadb.html

[G10] 访问控制
来源：http://hz.yanxiufei.cn/gtrgormlzy.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.ivvv.top/gtzwpgddxh.html

PHP:  public / protected / private
来源：http://hz.shangyingyoupin.top/gtyyusiecz.html

JS:   #private 字段；其余公开
来源：http://hz.sweek.top/gtwtonujgg.html

TS:   public / protected / private
来源：http://hz.dianchejie.cn/gtjmqwiaxl.html

Java: public / protected / private / 默认包级
来源：http://hz.zycfv.cn/gtsnzxddwa.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.guannengcc.top/gtrloylyeg.html

Ruby: public / protected / private
来源：http://hz.fzhhl.top/gtwqeafeyq.html

C#:   public / protected / private / internal
来源：http://hz.cheryme.top/gtrawoffkx.html

[G11] getter / setter
来源：http://hz.hammf.cn/gtilkgjhze.html

Py:   @property 与 @x.setter
来源：http://hz.zycfv.cn/gtxfckalmn.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.andypj.xyz/gtjoykkgjz.html

JS:   get name() { return this._name; }
来源：http://hz.0kj1m.cn/gthofhxqto.html

TS:   get name(): string { return this._name; }
来源：http://hz.shanyushiyangtech.top/gtvrslmmtt.html

Java: public String getName() { return name; }
来源：http://hz.zhengqikj.top/gtcugmusse.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.nanxinkj.top/gteixuchso.html

Ruby: attr_accessor :name
来源：http://hz.jinyuanbaomall.cn/gthnncxuow.html

C#:   public string Name { get; set; }
来源：http://hz.feifeiyinyue.top/gtryxtxask.html

[G12] 对象转字符串
来源：http://hz.ydzc1.top/gtgiedgjoc.html

Py:   def __str__(self): return self.name
来源：http://hz.guowangkeji.top/gterfxmyzq.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.aizwys.cn/gttyxduiwh.html

JS:   toString() { return this.name; }
来源：http://hz.xuanzx.com/gtdapfcxma.html

TS:   toString(): string { return this.name; }
来源：http://hz.mhx1999.top/gtqedboelh.html

Java: @Override public String toString() { return name; }
来源：http://hz.shuidangran.top/gtoxgzoioc.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.iojbl.cn/gtbplpkkhf.html

Ruby: def to_s; @name; end
来源：http://hz.xylfe.cn/gtokykzzql.html

C#:   public override string ToString() => Name;
来源：http://hz.sysykeji.top/gtatqzpigy.html

[G13] 判断对象类型
来源：http://hz.jqgfzy.top/gtbwggrejf.html

Py:   isinstance(u, User)
来源：http://hz.hongshengwenyu.top/gtmcvmcuay.html

PHP:  $u instanceof User
来源：http://hz.pengpengdd.cyou/gtwzetkrlj.html

JS:   u instanceof User
来源：http://hz.kuanghao11.cn/gtxfsrulkb.html

TS:   u instanceof User
来源：http://hz.nwbrower.top/gtabpqhmmm.html

Java: u instanceof User
来源：http://hz.xylfe.cn/gtjznoaxjv.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.hnqzz.top/gtqtfedxqy.html

Ruby: u.is_a?(User)
来源：http://hz.jyoumei.cn/gtnshobxii.html

C#:   u is User
来源：http://hz.havefunace.top/gtyfnmdoen.html

[G14] 数据类 / record
来源：http://hz.jqgfzy.top/gtcdvhqehg.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.xuanzx.com/gtugcryghj.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.hongshengwenyu.top/gtvnvwpyey.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.shanyushiyangtech.top/gtvojosxmd.html

TS:   type User = { name: string; age: number };
来源：http://hz.shuidangran.top/gtrteswbjn.html

Java: record User(String name, int age) {}
来源：http://hz.wangdashe.top/gtxnignhgj.html

Go:   type User struct { Name string; Age int }
来源：http://hz.zhongyouzk.top/gtjnsepdyc.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.zhongyouzk.top/gtpgjgfmdb.html

C#:   record User(string Name, int Age);
来源：http://hz.nanxuanxn.top/gtlvumdtdg.html

[G15] 枚举
来源：http://hz.jiagoushi.top/gtssndatfo.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.nwbrower.top/gtmeqjqhnh.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.havefunace.top/gtyhrgulhj.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.shzxlz.cn/gtyqnbtzgp.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.ehwqpu.com/gtvcwyfsft.html

Java: enum Color { RED, GREEN }
来源：http://hz.bjfxy.top/gtkpyywfpr.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.jiagoushi.top/gtsdvvhgok.html

Ruby: Color = %i[red green].freeze
来源：http://hz.nanxinkj.top/gtzukkcwfw.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.0kj1m.cn/gtkkgzosfs.html

[G16] 对象转数组 / 字典
来源：http://hz.cheryme.top/gtfcfynhkh.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.xuetiantiany.cn/gtxdkiixtw.html

PHP:  get_object_vars($obj);
来源：http://hz.zhijiandao.cn/gtqywjdbdm.html

JS:   Object.entries(obj)
来源：http://hz.shanyushiyangkeji.top/gtfpaehrez.html

TS:   Object.entries(obj)
来源：http://hz.yonumen.top/gtijzhoobf.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.haohaochexian.top/gtdosejtuy.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.tianlin.xyz/gtnpuxtxcx.html

Ruby: obj.instance_variables
来源：http://hz.tianlin.xyz/gttfwownsz.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.yuxming.cn/gtvejwsfrj.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtxcyswbhb.html

H. 异常与错误处理
来源：http://hz.sufxvd.cn/gtlfgymzbg.html

================================================================================
来源：http://hz.yueranfly.top/gtbdgafzoe.html

[H01] try / catch 基础
来源：http://hz.nanxuanxn.top/gtuetahzbj.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.nanxinkj.top/gtkazephej.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.yuxming.cn/gtcqmhnkxo.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.ehwqpu.com/gtsivastzv.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.yj20258.top/gtgqhguvvt.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.dashuyun.cn/gtwmouobhd.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.yuanzhike.top/gtfzfhseai.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.yangfankeji.com/gthlewypxy.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.jinqigfzy.top/gtbhojetnq.html

[H02] finally / ensure 收尾
来源：http://hz.zycfv.cn/gtloanxkuw.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.gotoacloud.top/gtukgbqmbk.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.sufxvd.cn/gthxcexxzi.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.xylfe.cn/gtjujdxxdw.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.yuxming.cn/gtiaxkegaj.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.ydzc1.top/gtxziapdxc.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.sxryk.cn/gtyybteojh.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.ydzc1.top/gtgevnzcay.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.pengpengdd.cyou/gtbckrdzyj.html

[H03] 主动抛出异常
来源：http://hz.smart0.xyz/gtyaakvrgj.html

Py:   raise ValueError("错误信息")
来源：http://hz.sufxvd.cn/gtcgujsnoc.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.zhiwuduotai.top/gtqdwwtorm.html

JS:   throw new Error("错误信息");
来源：http://hz.sweek.top/gtiqfohxox.html

TS:   throw new Error("错误信息");
来源：http://hz.cucudq.cn/gtzklmrgaz.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.jinqigfzy.top/gtsbbexpvb.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.vqdsnc.cn/gtlhpvpczn.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.guannengcc.top/gtmcmrmlxu.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.nwbrower.top/gtdxkgaonn.html

[H04] 自定义异常类型
来源：http://hz.sysykeji.top/gtlqtkbkcc.html

Py:   class MyError(Exception): pass
来源：http://hz.hnqzz.top/gtrpykdrkx.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.mhx1999.top/gtmzzcidfm.html

JS:   class MyError extends Error {}
来源：http://hz.sxryk.cn/gtbujxpibk.html

TS:   class MyError extends Error {}
来源：http://hz.shangyingyoupin.top/gtowqnbvqf.html

Java: class MyException extends RuntimeException {}
来源：http://hz.birdmap.top/gtyjwiwets.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.redwolf501.top/gtkiygpvwx.html

Ruby: class MyError < StandardError; end
来源：http://hz.jqgufenzy.top/gtuekcfzsj.html

C#:   class MyException : Exception {}
来源：http://hz.yj202588.top/gtucrmguvo.html

[H05] 捕获特定类型
来源：http://hz.yj20258888.top/gtxjmvliok.html

Py:   except ValueError as e:
来源：http://hz.redwolf501.top/gtcsqkvdwi.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.zhixingplan.top/gtvpnijoti.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.jyoumei.cn/gtcmuknqzu.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.sufxvd.cn/gtuqxqaixb.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.cucudq.cn/gtpyttbrwu.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.svipenyu.cn/gtqwanziol.html

Ruby: rescue ArgumentError => e
来源：http://hz.sxryk.cn/gtwxcnnqic.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.xylfe.cn/gtoptuvyhx.html

[H06] 可选值 / 空值安全访问
来源：http://hz.yvedp.cn/gtmvlxetge.html

Py:   value = d.get("k") or default
来源：http://hz.jyoumei.cn/gtwicjkbpf.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.tian-w.cn/gtfimjsoxi.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.pycfn.com/gtvropbrmz.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.yanxiufei.cn/gtvhcxuozs.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.pengpengdd.cyou/gtjtfpaihu.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.hysaishi.cn/gtnvdgaaly.html

Ruby: d&.dig(:a, :b)
来源：http://hz.chenlongwang.top/gtrnwnmjzo.html

C#:   obj?.A?.B ?? default
来源：http://hz.nanxuanxn.top/gtoqxahqau.html

[H07] 断言
来源：http://hz.vqdsnc.cn/gtrmjghyfa.html

Py:   assert x > 0, "必须为正"
来源：http://hz.0kj1m.cn/gtawsycdah.html

PHP:  assert($x > 0);
来源：http://hz.cdnleiting.top/gtqtezbsdl.html

JS:   console.assert(x > 0);
来源：http://hz.cashguo.top/gtabjikbno.html

TS:   console.assert(x > 0);
来源：http://hz.birdmap.top/gtakmsxitq.html

Java: assert x > 0 : "必须为正";
来源：http://hz.sweek.top/gthsawqygo.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.yj20258888.top/gtahiqwiha.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.jinqigufen.top/gtghchfeup.html

C#:   Debug.Assert(x > 0);
来源：http://hz.iojbl.cn/gtozuitmqw.html

[H08] 获取错误信息与堆栈
来源：http://hz.shuidangran.top/gtpdgegxkv.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.jyoumei.cn/gtwttlnzhm.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.xinyue.icu/gtnmcdndrv.html

JS:   e.message;  e.stack
来源：http://hz.yueranfly.top/gtjrhzpbjk.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.pengpengdd.cyou/gtcveefevh.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.mhx1999.top/gtfbohaihc.html

Go:   err.Error()
来源：http://hz.jinyuanbaomall.cn/gtkxawjwpj.html

Ruby: e.message;  e.backtrace
来源：http://hz.jqgufenzy.top/gtviummqgd.html

C#:   e.Message;  e.StackTrace
来源：http://hz.yanxiufei.cn/gtyfppdzju.html

[H09] 带错误码的异常
来源：http://hz.shzxlz.cn/gttbkeorwg.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.chenlongwang.top/gtxhpqmtuu.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.tanke756.top/gtpagknnne.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.xinyue.icu/gtgqockxfg.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.jinqigufen.top/gtkjiwxmjs.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.hywenlv.cn/gtifvfgaur.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.sysykeji.top/gtpvpeqcgs.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.tian-w.cn/gtfnyijdws.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.jinqigfzy.top/gtjlpxvnff.html

[H10] 资源自动释放
来源：http://hz.ehwqpu.com/gtymvgtrho.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.ydjk.org.cn/gtxevetaxm.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.tian-w.cn/gtknhvfbrl.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.hnqzz.top/gtwkxhlnfo.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.yuxming.cn/gtyqxniowr.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.meibo888.top/gtogwphdvz.html

Go:   defer f.Close()
来源：http://hz.nanxuanxn.top/gtgvlnwtec.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.sweek.top/gtpjgwcrtf.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.52xcode.cn/gtcjvnznsb.html

================================================================================
来源：http://hz.pycfn.com/gtdvpopsww.html

I. 正则表达式
来源：http://hz.yonumen.top/gtlgnsxzzh.html

================================================================================
来源：http://hz.fzhhl.top/gthhrbgxos.html

[I01] 判断是否匹配
来源：http://hz.haohaochexian.top/gtmjzfxnwt.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.xziqi.cn/gtgivvhnsa.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.yj20258888.top/gtpbpxdicc.html

JS:   /\d+/.test(s)
来源：http://hz.haohaochexian.top/gttgxouvre.html

TS:   /\d+/.test(s)
来源：http://hz.ywan-chungtsiang.top/gtleykicfx.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.hnxiangtu.top/gtbdjlhqiv.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.jinghuilouyu.cn/gtxnpisvra.html

Ruby: s.match?(/\d+/)
来源：http://hz.yanxiufei.cn/gtygpmpouc.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.tianlin.xyz/gtpqlemman.html


<!-- 参考信息 -->