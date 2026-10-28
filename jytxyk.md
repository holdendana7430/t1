代发 wailian999

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.fzhhl.top/gtmatiezfs.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.cashguo.top/gtqatigmpu.html

JS:   fs.readdirSync("dir")
来源：http://hz.nwbrower.top/gtylwasrcf.html

TS:   fs.readdirSync("dir")
来源：http://hz.pengpengdd.cyou/gtaqxxaavr.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.zhijiandao.cn/gtuyyfuwol.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.gaohongyu789.top/gtrtbmfdzk.html

Ruby: Dir.children("dir")
来源：http://hz.yuanzhike.top/gtbyawovqk.html

C#:   Directory.GetFiles("dir")
来源：http://hz.zycfv.cn/gtbsomwgpg.html

[F09] 获取文件大小
来源：http://hz.dashuyun.cn/gtzhilhexn.html

Py:   os.path.getsize("a.txt")
来源：http://hz.jianghu66.top/gtgypfkdtj.html

PHP:  filesize("a.txt");
来源：http://hz.zhixingplan.top/gtividcyxi.html

JS:   fs.statSync("a.txt").size
来源：http://hz.jqgufenzy.top/gtemvkmasm.html

TS:   fs.statSync("a.txt").size
来源：http://hz.nanxinkj.top/gtutcjzqjc.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.wangshuangyany.cn/gtviqesvcp.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.guowangkeji.top/gtbbjjxoiw.html

Ruby: File.size("a.txt")
来源：http://hz.cheryme.top/gtbshnvnqy.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.hammf.cn/gtufugvxbv.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.guowangkeji.top/gttyqdzkxt.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.zhaomingkeji.xyz/gtmjnuiprw.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.jqgfzy.top/gtmpjunmjo.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.jiagoushi.top/gtthcpilon.html

TS:   path.extname("a.txt")
来源：http://hz.tianlin.xyz/gtldkgjevm.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.zhijiandao.cn/gtojoxizze.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.hywenlv.cn/gtupymvdpb.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.jinyuanbaomall.cn/gtcjelgfwj.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.jinyuanbaomall.cn/gtoyisgsmi.html

[F11] 复制与移动文件
来源：http://hz.cucudq.cn/gtqigftrkg.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.yanxiufei.cn/gtbghiayzh.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.nanxuanxn.top/gtgkdydxgb.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.tianlin.xyz/gtmkvctwrp.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.shangyingyoupin.top/gtttxtteke.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.iojbl.cn/gttheuxbxd.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.redwolf501.top/gthtdvjggf.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.jinqigfzy.top/gtvquktnrm.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.yj20258.top/gtxarvpumy.html

[F12] CSV 读写
来源：http://hz.gaohongyu789.top/gtnclcqzsk.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.meibo888.top/gtnsjyeifw.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.guowangkeji.top/gtsssywjjw.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.tian-w.cn/gtnepgvybm.html

TS:   // 同上
来源：http://hz.zdqjudy.top/gthfkesshf.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.ehwqpu.com/gtvuxecayh.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.hongshengwenyu.top/gtjkzfgwfk.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.316326.xyz/gthdzqljfu.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.shuidangran.top/gtdceqgxfr.html

================================================================================
来源：http://hz.svipenyu.cn/gtgksilspw.html

G. 面向对象
来源：http://hz.yongpay.top/gteznmyytx.html

================================================================================
来源：http://hz.jinqigfzy.top/gtewbrfzbj.html

[G01] 定义类
来源：http://hz.zhijiandao.cn/gthqcpjczm.html

Py:   class User: pass
来源：http://hz.hywenlv.cn/gtwlvujjzs.html

PHP:  class User {}
来源：http://hz.yongpay.top/gtbmfdchbw.html

JS:   class User {}
来源：http://hz.hfpthk.cn/gtwikzhrkz.html

TS:   class User { name: string = ""; }
来源：http://hz.smart0.xyz/gtcbzwvvga.html

Java: class User {}
来源：http://hz.zhaomingkeji.xyz/gtixavhtip.html

Go:   type User struct { Name string }
来源：http://hz.cdnleiting.top/gtwgicoxzr.html

Ruby: class User; end
来源：http://hz.smart0.xyz/gthrjgxopd.html

C#:   class User {}
来源：http://hz.0kj1m.cn/gtiivsemyc.html

[G02] 构造函数
来源：http://hz.nanxuanxn.top/gtvvggulzy.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.sufxvd.cn/gtgxvdvxnd.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.zhengqikj.top/gtnzqydqys.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.xuetiantiany.cn/gtlvwtedld.html

TS:   constructor(public name: string) {}
来源：http://hz.cashguo.top/gtvqadscfv.html

Java: User(String name) { this.name = name; }
来源：http://hz.hysaishi.cn/gtqjfgcirh.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.ydzc1.top/gtzptyzsme.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.316326.xyz/gtgrieebkw.html

C#:   public User(string name) { Name = name; }
来源：http://hz.dashuyun.cn/gtyehgulyl.html

[G03] 实例属性
来源：http://hz.meibo888.top/gtljhirmtz.html

Py:   self.name = "x"
来源：http://hz.yj20258.top/gtyzofgiqv.html

PHP:  public string $name = "x";
来源：http://hz.pengpengdd.cyou/gtbzhccpow.html

JS:   this.name = "x";
来源：http://hz.zhengqikj.top/gtynhuuqqq.html

TS:   name: string = "x";
来源：http://hz.bjfxy.top/gteerjespg.html

Java: private String name;
来源：http://hz.andypj.xyz/gtngisumkz.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.zhaomingkeji.xyz/gtfaoveckk.html

Ruby: @name = "x"
来源：http://hz.zycfv.cn/gtwonlbfgm.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.shangyingyoupin.top/gtpzplwosw.html

[G04] 定义方法
来源：http://hz.xuanzx.com/gtenlukfkb.html

Py:   def greet(self): return self.name
来源：http://hz.jinyuanbaomall.cn/gthpmpqyis.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.gaohongyu789.top/gtddmknhtu.html

JS:   greet() { return this.name; }
来源：http://hz.jinyuanbaomall.cn/gtwddjsikh.html

TS:   greet(): string { return this.name; }
来源：http://hz.andypj.xyz/gttnwvqyfu.html

Java: String greet() { return name; }
来源：http://hz.chenlongwang.top/gttmiobsju.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.nanxinkj.top/gtaheifxvg.html

Ruby: def greet; @name; end
来源：http://hz.fengsongda.top/gteuemvuwc.html

C#:   public string Greet() => Name;
来源：http://hz.pengpengdd.cyou/gttektzvbg.html

[G05] 继承
来源：http://hz.sufxvd.cn/gtqkhsqlhv.html

Py:   class Admin(User): pass
来源：http://hz.nanxinkj.top/gthxrutjxt.html

PHP:  class Admin extends User {}
来源：http://hz.nanxuanxn.top/gtdzobbzsl.html

JS:   class Admin extends User {}
来源：http://hz.nwbrower.top/gtcayoaxgh.html

TS:   class Admin extends User {}
来源：http://hz.zhaomingkeji.xyz/gtdzzgalwx.html

Java: class Admin extends User {}
来源：http://hz.ivvv.top/gtgijuqxsd.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.ivvv.top/gtxsemjqhx.html

Ruby: class Admin < User; end
来源：http://hz.hysaishi.cn/gtgofhkrps.html

C#:   class Admin : User {}
来源：http://hz.birdmap.top/gttefdpplc.html

[G06] 重写方法
来源：http://hz.hongshengwenyu.top/gtuqvzpqej.html

Py:   def greet(self): return "admin"
来源：http://hz.andypj.xyz/gtjdecgovv.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.gotoacloud.top/gtcqqskfll.html

JS:   greet() { return "admin"; }
来源：http://hz.xuanzx.com/gtogbwegve.html

TS:   greet(): string { return "admin"; }
来源：http://hz.quarkkingdee.top/gttovbfwwb.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.shanyushiyangkeji.top/gtavkxuive.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.kuanghao11.cn/gtbnqmpoyz.html

Ruby: def greet; "admin"; end
来源：http://hz.yangfankeji.com/gtfozkxobe.html

C#:   public override string Greet() => "admin";
来源：http://hz.xinyue.icu/gtuuwkvbwd.html

[G07] 调用父类方法
来源：http://hz.zycfv.cn/gtayhlpudi.html

Py:   super().greet()
来源：http://hz.jinqigfzy.top/gtwehixokd.html

PHP:  parent::greet();
来源：http://hz.sysykeji.top/gtchtrlnpx.html

JS:   super.greet();
来源：http://hz.zycfv.cn/gthnyhmfjd.html

TS:   super.greet();
来源：http://hz.shuidangran.top/gtibivjckg.html

Java: super.greet();
来源：http://hz.jiagoushi.top/gtxobbrblj.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.guowangkeji.top/gthunygfjr.html

Ruby: super
来源：http://hz.c1oappe.top/gtrnvoufng.html

C#:   base.Greet();
来源：http://hz.zycfv.cn/gtdsxfyrjz.html

[G08] 静态方法与属性
来源：http://hz.ehwqpu.com/gtzdglngst.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.xingfuxueyuan.xyz/gtqvlswnep.html

PHP:  public static function f() {}
来源：http://hz.zhixingplan.top/gtyskfqeio.html

JS:   static f() {}
来源：http://hz.zhengqikj.top/gtamnahorp.html

TS:   static f(): void {}
来源：http://hz.andypj.xyz/gtjqltrsku.html

Java: static void f() {}
来源：http://hz.dianchejie.cn/gtpphbzwrj.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.cheryme.top/gtpurgkpct.html

Ruby: def self.f; end
来源：http://hz.gotoacloud.top/gtsbxiivmx.html

C#:   public static void F() {}
来源：http://hz.52xcode.cn/gtmuzdxnhg.html

[G09] 接口 / 抽象类
来源：http://hz.chenzaomai.com/gtgukpflck.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.c1oappe.top/gtudesawyn.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.smart0.xyz/gtzrqgqasw.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.jinghuilouyu.cn/gtqrngqdfq.html

TS:   interface Shape { area(): number; }
来源：http://hz.gotoacloud.top/gtdsrkkqps.html

Java: interface Shape { double area(); }
来源：http://hz.yonumen.top/gtidusxkkc.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.chenlongwang.top/gtenvcyodn.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.kuanghao11.cn/gtbuxwdxxw.html

C#:   interface IShape { double Area(); }
来源：http://hz.andypj.xyz/gtethrlpuv.html

[G10] 访问控制
来源：http://hz.yuanzhike.top/gtswuzeuoy.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.nanxuanxn.top/gtgpikpdqz.html

PHP:  public / protected / private
来源：http://hz.pycfn.com/gtvyaoxujl.html

JS:   #private 字段；其余公开
来源：http://hz.xuanzx.com/gtlumugrlf.html

TS:   public / protected / private
来源：http://hz.ehwqpu.com/gtjaqjgcdx.html

Java: public / protected / private / 默认包级
来源：http://hz.havefunace.top/gtmktzqnck.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.kuanghao11.cn/gtcwnsubyq.html

Ruby: public / protected / private
来源：http://hz.yj20258.top/gtxgrlomjw.html

C#:   public / protected / private / internal
来源：http://hz.xingfuxueyuan.xyz/gtorhfcbap.html

[G11] getter / setter
来源：http://hz.daxiang520.top/gtvdkhroef.html

Py:   @property 与 @x.setter
来源：http://hz.havefunace.top/gtquusyvdo.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.meibo888.top/gtnfiaqfly.html

JS:   get name() { return this._name; }
来源：http://hz.sxryk.cn/gtbrdptnys.html

TS:   get name(): string { return this._name; }
来源：http://hz.ybcxt.top/gtqpjvohqj.html

Java: public String getName() { return name; }
来源：http://hz.ppjwa.cn/gtqgevdpfl.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.andypj.xyz/gtwqesyogi.html

Ruby: attr_accessor :name
来源：http://hz.yonumen.top/gtqkbwhuww.html

C#:   public string Name { get; set; }
来源：http://hz.yanxiufei.cn/gtfxcdlcvd.html

[G12] 对象转字符串
来源：http://hz.jyoumei.cn/gtywjlrznp.html

Py:   def __str__(self): return self.name
来源：http://hz.52xcode.cn/gtfohfyyxx.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.nanxinkj.top/gtpulvtxmo.html

JS:   toString() { return this.name; }
来源：http://hz.daxiang520.top/gtanwuvvac.html

TS:   toString(): string { return this.name; }
来源：http://hz.shzxlz.cn/gtnghuklsp.html

Java: @Override public String toString() { return name; }
来源：http://hz.sufxvd.cn/gtjcnqhxdf.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.chenlongwang.top/gtbwdfpckq.html

Ruby: def to_s; @name; end
来源：http://hz.cashguo.top/gtwygwozwh.html

C#:   public override string ToString() => Name;
来源：http://hz.xinyue.icu/gtdqihrxlf.html

[G13] 判断对象类型
来源：http://hz.daxiang520.top/gtulmgybsu.html

Py:   isinstance(u, User)
来源：http://hz.nanxinkj.top/gtswlxgizd.html

PHP:  $u instanceof User
来源：http://hz.aizwys.cn/gtpndfxmod.html

JS:   u instanceof User
来源：http://hz.jinghuilouyu.cn/gtjudabopt.html

TS:   u instanceof User
来源：http://hz.tian-w.cn/gtbdfxvzmd.html

Java: u instanceof User
来源：http://hz.guannengcc.top/gtmltaizmi.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.0kj1m.cn/gtltxocsfk.html

Ruby: u.is_a?(User)
来源：http://hz.nwbrower.top/gthjmmpsoc.html

C#:   u is User
来源：http://hz.yongpay.top/gtbipvuujb.html

[G14] 数据类 / record
来源：http://hz.tianlin.xyz/gtzochsoka.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.yanxiufei.cn/gtcjcckckt.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.zhaomingkeji.xyz/gtvuophosw.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.jinqigfzy.top/gtidekxink.html

TS:   type User = { name: string; age: number };
来源：http://hz.jinqigufen.top/gtmavnvbjt.html

Java: record User(String name, int age) {}
来源：http://hz.fzhhl.top/gtvseydfdb.html

Go:   type User struct { Name string; Age int }
来源：http://hz.cdnleiting.top/gtfftpseie.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.jqgfzy.top/gtxursykor.html

C#:   record User(string Name, int Age);
来源：http://hz.iojbl.cn/gtcqvgkuzj.html

[G15] 枚举
来源：http://hz.cashguo.top/gtwmklejgp.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.hnxiangtu.top/gtbosjmsie.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.sufxvd.cn/gtyhbpjqds.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.shuidangran.top/gtabxvstsa.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.gaohongyu789.top/gtbxtvblbx.html

Java: enum Color { RED, GREEN }
来源：http://hz.zhaomingkeji.xyz/gtecwjwpgz.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.jinyuanbaomall.cn/gtchbubldd.html

Ruby: Color = %i[red green].freeze
来源：http://hz.haohaochexian.top/gtdrabcblu.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.ydjk.org.cn/gtpkrfzhmo.html

[G16] 对象转数组 / 字典
来源：http://hz.yvedp.cn/gthrsfnunk.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.fzhhl.top/gthbdmgpyp.html

PHP:  get_object_vars($obj);
来源：http://hz.daxiang520.top/gtpmbvgtcf.html

JS:   Object.entries(obj)
来源：http://hz.jinqigfzy.top/gtypfbitah.html

TS:   Object.entries(obj)
来源：http://hz.jianghu66.top/gtbpswgrvr.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.kuanghao11.cn/gtlswuwdfo.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.jqgufenzy.top/gttxlzxdvq.html

Ruby: obj.instance_variables
来源：http://hz.cashguo.top/gtqznhqqzx.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.xuetiantiany.cn/gtpxuepgrp.html

================================================================================
来源：http://hz.jqgfzy.top/gtszsoptsj.html

H. 异常与错误处理
来源：http://hz.daxiang520.top/gtfcrsppdh.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtysflxzcg.html

[H01] try / catch 基础
来源：http://hz.52xcode.cn/gthibljzlh.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.daria6918.cn/gtygzfeyfh.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.shuidangran.top/gtuusdapsl.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.yj202588.top/gtwmtfwecp.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.guannengcc.top/gtxxgbyvpb.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.tianlin.xyz/gtvqmujchm.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.yongpay.top/gttasbptbm.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.wangdashe.top/gtctpvqpfy.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.0kj1m.cn/gtqpwtyjhu.html

[H02] finally / ensure 收尾
来源：http://hz.xuetiantiany.cn/gtriwhrpoj.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.yangfankeji.com/gtzmorpajh.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.jyoumei.cn/gtmbkzfsbp.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.gogol.net.cn/gtxevcfqch.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.zhoulong.xyz/gtkbuhaxrc.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.gaohongyu789.top/gthazvexeh.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.fzhhl.top/gtlcfuxlqg.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.yuxming.cn/gtdwzwdlow.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.yueranfly.top/gtdlczyibl.html

[H03] 主动抛出异常
来源：http://hz.mhx1999.top/gtjsznbapp.html

Py:   raise ValueError("错误信息")
来源：http://hz.sxryk.cn/gtflguqhun.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.svipenyu.cn/gtfyazgebd.html

JS:   throw new Error("错误信息");
来源：http://hz.xingfuxueyuan.xyz/gtpdutldfl.html

TS:   throw new Error("错误信息");
来源：http://hz.hammf.cn/gtwtwhoumf.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.aizwys.cn/gtqplujykx.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.gogol.net.cn/gtqlqcgtga.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.tian-w.cn/gthhpumcfs.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.xinyue.icu/gttmiitmyv.html

[H04] 自定义异常类型
来源：http://hz.jyoumei.cn/gtmcvuudea.html

Py:   class MyError(Exception): pass
来源：http://hz.jinqigfzy.top/gtskrhxndh.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.tian-w.cn/gtykjpyzyj.html

JS:   class MyError extends Error {}
来源：http://hz.cucudq.cn/gtejeglwcr.html

TS:   class MyError extends Error {}
来源：http://hz.dianchejie.cn/gtsxwdlawk.html

Java: class MyException extends RuntimeException {}
来源：http://hz.hnxiangtu.top/gtonrkaddy.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.haohaochexian.top/gtfegvoyig.html

Ruby: class MyError < StandardError; end
来源：http://hz.shanyushiyangtech.top/gtnncsisqf.html

C#:   class MyException : Exception {}
来源：http://hz.zhiwuduotai.top/gtssiiiscb.html

[H05] 捕获特定类型
来源：http://hz.zhoulong.xyz/gtojnyxlyq.html

Py:   except ValueError as e:
来源：http://hz.andypj.xyz/gtiuiqkyuy.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.hnxiangtu.top/gtrdzrgzhq.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.jinyuanbaomall.cn/gtgrhngqdj.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.hfpthk.cn/gtlhtywgyc.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.sweek.top/gtcvpcffmi.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.xuanzx.com/gtvieixvkc.html

Ruby: rescue ArgumentError => e
来源：http://hz.cucudq.cn/gtwdpassol.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.hnxiangtu.top/gttjjdncxv.html

[H06] 可选值 / 空值安全访问
来源：http://hz.cheryme.top/gtcsewahks.html

Py:   value = d.get("k") or default
来源：http://hz.daria6918.cn/gtkvepvncx.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.nwbrower.top/gtmafwcwmi.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.tian-w.cn/gtyvwydnmw.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.cdnleiting.top/gtrqromoez.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.c1oappe.top/gtnwrnvkjb.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.xziqi.cn/gtfkflrdoh.html

Ruby: d&.dig(:a, :b)
来源：http://hz.gzhubu.top/gtzxqzbpjl.html

C#:   obj?.A?.B ?? default
来源：http://hz.yongpay.top/gtricbllot.html

[H07] 断言
来源：http://hz.xziqi.cn/gtvtgdpggt.html

Py:   assert x > 0, "必须为正"
来源：http://hz.dashuyun.cn/gtgafqgeks.html

PHP:  assert($x > 0);
来源：http://hz.dashuyun.cn/gtchjnheya.html

JS:   console.assert(x > 0);
来源：http://hz.yuanzhike.top/gtfdmrqysd.html

TS:   console.assert(x > 0);
来源：http://hz.xylfe.cn/gtebylfepj.html

Java: assert x > 0 : "必须为正";
来源：http://hz.zhijiandao.cn/gtrahnbozo.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.ywan-chungtsiang.top/gtitkmvqng.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.zhaomingkeji.xyz/gtxxhgzyuq.html

C#:   Debug.Assert(x > 0);
来源：http://hz.nanxuanxn.top/gtzzzgcjew.html

[H08] 获取错误信息与堆栈
来源：http://hz.pengpengdd.cyou/gtgwhheggn.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.ywan-chungtsiang.top/gtkipzfkaq.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.aibaodan.cn/gtqkevowdn.html

JS:   e.message;  e.stack
来源：http://hz.yj202588.top/gtgzmyubak.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.jqgufenzy.top/gtfjjoliow.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.yvedp.cn/gtgiqanqzg.html

Go:   err.Error()
来源：http://hz.jinghuilouyu.cn/gtgzgvbbfj.html

Ruby: e.message;  e.backtrace
来源：http://hz.sysykeji.top/gtprfexvzv.html

C#:   e.Message;  e.StackTrace
来源：http://hz.nanxuanxn.top/gtucaiusyq.html

[H09] 带错误码的异常
来源：http://hz.xingfuxueyuan.xyz/gtuyawiabp.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.jinqigufen.top/gtvyzvpuua.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.pengpengdd.cyou/gtzwdonjca.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.cheryme.top/gtigntovzn.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.cheryme.top/gtdvuwyuim.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.hnqzz.top/gtbeupukxh.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.redwolf501.top/gtkzzsgtmr.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.zycfv.cn/gtebwkbrxk.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.kuanghao11.cn/gtyihmhrdc.html

[H10] 资源自动释放
来源：http://hz.bjfxy.top/gtuxfdrqig.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.svipenyu.cn/gthmplkvzh.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.svipenyu.cn/gtddzqvuht.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.zhaomingkeji.xyz/gtxwhjwfze.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.cdnleiting.top/gtsgdocslh.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.xingfuxueyuan.xyz/gtqlgsjrxr.html

Go:   defer f.Close()
来源：http://hz.guowangkeji.top/gtxityvoni.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.jinghuilouyu.cn/gtzbtzimxb.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.dashuyun.cn/gtclulhzqk.html

================================================================================
来源：http://hz.zhengqikj.top/gticzakcjm.html

I. 正则表达式
来源：http://hz.pycfn.com/gtaalvjnjf.html

================================================================================
来源：http://hz.jqgufenzy.top/gtvopyzeff.html

[I01] 判断是否匹配
来源：http://hz.chenlongwang.top/gtgcfqjsjq.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.chenlongwang.top/gtbnbpuyux.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.zhongyouzk.top/gtzxsxnggu.html

JS:   /\d+/.test(s)
来源：http://hz.svipenyu.cn/gtnnomifdv.html

TS:   /\d+/.test(s)
来源：http://hz.jinqigfzy.top/gtewiosrbe.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.andypj.xyz/gtwcknpihq.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.cheryme.top/gtavsatzkb.html

Ruby: s.match?(/\d+/)
来源：http://hz.sxryk.cn/gtqucjnudu.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.jqgfzy.top/gtqcllflgh.html

[I02] 提取所有匹配
来源：http://hz.pycfn.com/gtbpmnhydp.html

Py:   re.findall(r"\d+", s)
来源：http://hz.tianlin.xyz/gtuyclunji.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.mhx1999.top/gtstaekcjs.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.hnxiangtu.top/gtfvfaqbrl.html


<!-- 参考信息 -->