代发 wailian999

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.jinyuanbaomall.cn/gtaqomcphz.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.yvedp.cn/gthdanjkns.html

Ruby: Dir.children("dir")
来源：http://hz.wangdashe.top/gthcmeugfw.html

C#:   Directory.GetFiles("dir")
来源：http://hz.nanxuanxn.top/gtdcluvxnp.html

[F09] 获取文件大小
来源：http://hz.xuanzx.com/gtexadrxnj.html

Py:   os.path.getsize("a.txt")
来源：http://hz.ivvv.top/gtcivewgyi.html

PHP:  filesize("a.txt");
来源：http://hz.xingfuxueyuan.xyz/gtvpcdwdgc.html

JS:   fs.statSync("a.txt").size
来源：http://hz.yanxiufei.cn/gtysdwvory.html

TS:   fs.statSync("a.txt").size
来源：http://hz.zycfv.cn/gtupfzelqk.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.meibo888.top/gtffswgfwx.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.tian-w.cn/gtdzhqcaby.html

Ruby: File.size("a.txt")
来源：http://hz.haohaochexian.top/gtrxekquxc.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.cqqwz.cn/gtfsrpxppl.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.hongshengwenyu.top/gtlroqzcqg.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.yueranfly.top/gttdgdload.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.dashuyun.cn/gtcoqjtksr.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.andypj.xyz/gtmnncrvhs.html

TS:   path.extname("a.txt")
来源：http://hz.zdqjudy.top/gtbctrnyqi.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.bjfxy.top/gturwbyvnk.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.shangyingyoupin.top/gtzxwqmnod.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.zhiwuduotai.top/gthrcqquzr.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.havefunace.top/gtxrzkzwso.html

[F11] 复制与移动文件
来源：http://hz.yonumen.top/gtsmxpxwgr.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.gzhubu.top/gtboixghtv.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.sufxvd.cn/gtkjdfcngv.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.zhengqikj.top/gtwgjknlrr.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.zhiwuduotai.top/gtmdcdpacj.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.jqgfzy.top/gtaladhbak.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.dashuyun.cn/gtxievljwg.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.hywenlv.cn/gthiuditsg.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.ppjwa.cn/gtxnuffnyu.html

[F12] CSV 读写
来源：http://hz.xuetiantiany.cn/gtunzwmhxj.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.yuanzhike.top/gtiyjqkfhi.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.aibaodan.cn/gtfuarbxmt.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.tianlin.xyz/gtgoiukwhb.html

TS:   // 同上
来源：http://hz.kuanghao11.cn/gtiasfjwpy.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.ydzc1.top/gtlotejhrp.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.jianghu66.top/gtiurdxxdq.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.gogol.net.cn/gttvouvivm.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.yvedp.cn/gtaescxrlj.html

================================================================================
来源：http://hz.xinyue.icu/gthuqwqvtw.html

G. 面向对象
来源：http://hz.sxryk.cn/gtbggthdgm.html

================================================================================
来源：http://hz.52xcode.cn/gtogyeflat.html

[G01] 定义类
来源：http://hz.yuanzhike.top/gtkptbsznx.html

Py:   class User: pass
来源：http://hz.hongshengwenyu.top/gtnsubncwv.html

PHP:  class User {}
来源：http://hz.xziqi.cn/gtrmvvsdkb.html

JS:   class User {}
来源：http://hz.smart0.xyz/gtwvsnuisu.html

TS:   class User { name: string = ""; }
来源：http://hz.snrcjt.cn/gtvkwxwiaj.html

Java: class User {}
来源：http://hz.ppjwa.cn/gtjgqadiwk.html

Go:   type User struct { Name string }
来源：http://hz.c1oappe.top/gtqxyxscax.html

Ruby: class User; end
来源：http://hz.tanke756.top/gtsrwkvlhr.html

C#:   class User {}
来源：http://hz.daxiang520.top/gtigwkafqy.html

[G02] 构造函数
来源：http://hz.52xcode.cn/gtekgxttmw.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.zhengqikj.top/gtzvpycoyq.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.guowangkeji.top/gtdtxdrczk.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.sweek.top/gtnkszhgbp.html

TS:   constructor(public name: string) {}
来源：http://hz.nanxinkj.top/gtnuvjfjwp.html

Java: User(String name) { this.name = name; }
来源：http://hz.dianchejie.cn/gthfgpdjec.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.tianlin.xyz/gtnahulaog.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.shzxlz.cn/gtkqrzrvji.html

C#:   public User(string name) { Name = name; }
来源：http://hz.zhaomingkeji.xyz/gtslghidlx.html

[G03] 实例属性
来源：http://hz.tianlin.xyz/gttdqqakoq.html

Py:   self.name = "x"
来源：http://hz.gzhubu.top/gtygrbhfyw.html

PHP:  public string $name = "x";
来源：http://hz.meibo888.top/gtifjmggbg.html

JS:   this.name = "x";
来源：http://hz.gaohongyu789.top/gtlfgtdumk.html

TS:   name: string = "x";
来源：http://hz.xuanzx.com/gtwxmcmdbw.html

Java: private String name;
来源：http://hz.gotoacloud.top/gtbwfbxfdi.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.sysykeji.top/gtmxelikar.html

Ruby: @name = "x"
来源：http://hz.gaohongyu789.top/gtrwnuszwb.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.cheryme.top/gtabhqtipf.html

[G04] 定义方法
来源：http://hz.cheryme.top/gtfjgozmpf.html

Py:   def greet(self): return self.name
来源：http://hz.shangyingyoupin.top/gtpkiffppt.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.jinghuilouyu.cn/gtrgeupqps.html

JS:   greet() { return this.name; }
来源：http://hz.chenjidiqi.icu/gtcybuvkcd.html

TS:   greet(): string { return this.name; }
来源：http://hz.cheryme.top/gtdrtzuugl.html

Java: String greet() { return name; }
来源：http://hz.yj202588.top/gtkoewqglt.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.tian-w.cn/gtauhskoik.html

Ruby: def greet; @name; end
来源：http://hz.pengpengdd.cyou/gtoxoncpat.html

C#:   public string Greet() => Name;
来源：http://hz.xziqi.cn/gtcbrekvot.html

[G05] 继承
来源：http://hz.daria6918.cn/gtwmbyphzr.html

Py:   class Admin(User): pass
来源：http://hz.guowangkeji.top/gtpoqqkdia.html

PHP:  class Admin extends User {}
来源：http://hz.aibaodan.cn/gtlamvyiuc.html

JS:   class Admin extends User {}
来源：http://hz.jinyuanbaomall.cn/gtzzgrnzos.html

TS:   class Admin extends User {}
来源：http://hz.hongshengwenyu.top/gttjgbwoba.html

Java: class Admin extends User {}
来源：http://hz.shanyushiyangtech.top/gtzuylcuyx.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.nanxinkj.top/gtrfgadrzg.html

Ruby: class Admin < User; end
来源：http://hz.sweek.top/gtphrylvxp.html

C#:   class Admin : User {}
来源：http://hz.fzhhl.top/gtagktjono.html

[G06] 重写方法
来源：http://hz.ydjk.org.cn/gtqhisgpsc.html

Py:   def greet(self): return "admin"
来源：http://hz.52xcode.cn/gtixfcszlq.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.yj202588.top/gtwvnvacol.html

JS:   greet() { return "admin"; }
来源：http://hz.shuidangran.top/gtnybjacra.html

TS:   greet(): string { return "admin"; }
来源：http://hz.jinghuilouyu.cn/gtcwagxvpq.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.ydzc1.top/gtqfvcnupw.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.guannengcc.top/gtszjhirnu.html

Ruby: def greet; "admin"; end
来源：http://hz.zhixingplan.top/gtcdmlxjjr.html

C#:   public override string Greet() => "admin";
来源：http://hz.zhiwuduotai.top/gtzqkvpzwi.html

[G07] 调用父类方法
来源：http://hz.sxryk.cn/gtwiqymvea.html

Py:   super().greet()
来源：http://hz.aizwys.cn/gtumdoojzo.html

PHP:  parent::greet();
来源：http://hz.dianchejie.cn/gtwwceznss.html

JS:   super.greet();
来源：http://hz.jlsjyb.cn/gtggjnicka.html

TS:   super.greet();
来源：http://hz.xuetiantiany.cn/gttxiixmue.html

Java: super.greet();
来源：http://hz.tianlin.xyz/gtbnfgnjjh.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.ivvv.top/gtnemrmzaf.html

Ruby: super
来源：http://hz.hammf.cn/gtiqoxpecy.html

C#:   base.Greet();
来源：http://hz.ydjk.org.cn/gtemqveben.html

[G08] 静态方法与属性
来源：http://hz.sysykeji.top/gtyhpmftuh.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.sxryk.cn/gtbyzbmgzw.html

PHP:  public static function f() {}
来源：http://hz.jinghuilouyu.cn/gtncofuisg.html

JS:   static f() {}
来源：http://hz.9152youxi.cn/gtuubjzfug.html

TS:   static f(): void {}
来源：http://hz.yj202588.top/gtfqhowyfw.html

Java: static void f() {}
来源：http://hz.gotoacloud.top/gtlteiwxwa.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.yvedp.cn/gthwfrehbd.html

Ruby: def self.f; end
来源：http://hz.dashuyun.cn/gtskumzosc.html

C#:   public static void F() {}
来源：http://hz.yongpay.top/gtiasjaabq.html

[G09] 接口 / 抽象类
来源：http://hz.zhongyouzk.top/gtenzjapib.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.zdqjudy.top/gtgtwyhiil.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.0kj1m.cn/gtvoukpjgs.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.hfpthk.cn/gtrueqnkkq.html

TS:   interface Shape { area(): number; }
来源：http://hz.jyoumei.cn/gtntcdqoev.html

Java: interface Shape { double area(); }
来源：http://hz.shanyushiyangtech.top/gtezipsblm.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.feifeiyinyue.top/gtpldyqsxj.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.jinqigfzy.top/gttkhitxse.html

C#:   interface IShape { double Area(); }
来源：http://hz.cucudq.cn/gtpkptolad.html

[G10] 访问控制
来源：http://hz.svipenyu.cn/gtowoaknnm.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.0kj1m.cn/gtjhghdbyt.html

PHP:  public / protected / private
来源：http://hz.zhaomingkeji.xyz/gtxcioylzz.html

JS:   #private 字段；其余公开
来源：http://hz.nanxinkj.top/gtjjarmase.html

TS:   public / protected / private
来源：http://hz.fengsongda.top/gtukfmcnxc.html

Java: public / protected / private / 默认包级
来源：http://hz.jinyuanbaomall.cn/gtecjbdkek.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.quarkkingdee.top/gtwjvbxcmg.html

Ruby: public / protected / private
来源：http://hz.aizwys.cn/gttpoblzat.html

C#:   public / protected / private / internal
来源：http://hz.chenjidiqi.icu/gtyzfpgpoa.html

[G11] getter / setter
来源：http://hz.9152youxi.cn/gtwldupfji.html

Py:   @property 与 @x.setter
来源：http://hz.ywan-chungtsiang.top/gtxohbglfs.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.yj202588.top/gtspzjmaxw.html

JS:   get name() { return this._name; }
来源：http://hz.kuanghao11.cn/gtrarhitxt.html

TS:   get name(): string { return this._name; }
来源：http://hz.cashguo.top/gtfjuvtlxq.html

Java: public String getName() { return name; }
来源：http://hz.zhoulong.xyz/gtoevnaspr.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.cheryme.top/gtxvpshdvy.html

Ruby: attr_accessor :name
来源：http://hz.gzhubu.top/gtvzsztutk.html

C#:   public string Name { get; set; }
来源：http://hz.shangyingyoupin.top/gteotkmplq.html

[G12] 对象转字符串
来源：http://hz.9152youxi.cn/gtqovbpzyo.html

Py:   def __str__(self): return self.name
来源：http://hz.cdnleiting.top/gtkmkgybyo.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.bjfxy.top/gteliasmal.html

JS:   toString() { return this.name; }
来源：http://hz.dianchejie.cn/gtejpdwuhq.html

TS:   toString(): string { return this.name; }
来源：http://hz.yanxiufei.cn/gtrxwlpmvc.html

Java: @Override public String toString() { return name; }
来源：http://hz.shangyingyoupin.top/gthizbymab.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.yuanzhike.top/gtobckfgbc.html

Ruby: def to_s; @name; end
来源：http://hz.cucudq.cn/gtebvawknh.html

C#:   public override string ToString() => Name;
来源：http://hz.zhijiandao.cn/gtpjfoouen.html

[G13] 判断对象类型
来源：http://hz.tian-w.cn/gtgvyopmdn.html

Py:   isinstance(u, User)
来源：http://hz.xylfe.cn/gtqhtcfvie.html

PHP:  $u instanceof User
来源：http://hz.0kj1m.cn/gtrarkzfxn.html

JS:   u instanceof User
来源：http://hz.nanxinkj.top/gtfbzkeqpc.html

TS:   u instanceof User
来源：http://hz.shzxlz.cn/gtxescoigu.html

Java: u instanceof User
来源：http://hz.tanke756.top/gtlshxklyg.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.xylfe.cn/gtzwzwhyhy.html

Ruby: u.is_a?(User)
来源：http://hz.birdmap.top/gteszwzpjw.html

C#:   u is User
来源：http://hz.ywan-chungtsiang.top/gtvzyixwbg.html

[G14] 数据类 / record
来源：http://hz.zhijiandao.cn/gtzylyamij.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.yuanzhike.top/gtegeukwre.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.chenjidiqi.icu/gtijyeqcqe.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.xuetiantiany.cn/gtpnwzcjas.html

TS:   type User = { name: string; age: number };
来源：http://hz.tanke756.top/gtnojbiuwy.html

Java: record User(String name, int age) {}
来源：http://hz.ybcxt.top/gtjslxbwfj.html

Go:   type User struct { Name string; Age int }
来源：http://hz.yj202588.top/gttsclhofb.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.jinqigfzy.top/gtrfhtjzls.html

C#:   record User(string Name, int Age);
来源：http://hz.jqgfzy.top/gtabedzouc.html

[G15] 枚举
来源：http://hz.guannengcc.top/gtmakurfzx.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.zycfv.cn/gttbrkglcp.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.jianghu66.top/gtahnjubid.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.havefunace.top/gtlkdngrvl.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.ydzc1.top/gtjtnuoyhn.html

Java: enum Color { RED, GREEN }
来源：http://hz.kuanghao11.cn/gtmmvuusep.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.jianghu66.top/gtgkjawjcg.html

Ruby: Color = %i[red green].freeze
来源：http://hz.nanxinkj.top/gtajkowbbb.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.kuanghao11.cn/gtvtxcnexr.html

[G16] 对象转数组 / 字典
来源：http://hz.shzxlz.cn/gtzmqjvsxs.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.zhaomingkeji.xyz/gtssjemkvu.html

PHP:  get_object_vars($obj);
来源：http://hz.xuetiantiany.cn/gtrpqbkjrk.html

JS:   Object.entries(obj)
来源：http://hz.jqgufenzy.top/gtuuprmhir.html

TS:   Object.entries(obj)
来源：http://hz.hammf.cn/gtajqcxhky.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.ehwqpu.com/gtrviwruxb.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.sysykeji.top/gtjwaycplc.html

Ruby: obj.instance_variables
来源：http://hz.shzxlz.cn/gtqqfnlnxi.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.ywan-chungtsiang.top/gtwvtxkrkg.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtapwprjmf.html

H. 异常与错误处理
来源：http://hz.9152youxi.cn/gtitygodlr.html

================================================================================
来源：http://hz.gotoacloud.top/gtpxahtytu.html

[H01] try / catch 基础
来源：http://hz.shanyushiyangkeji.top/gtmexyoywo.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.svipenyu.cn/gtkhrqefmc.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.xziqi.cn/gtxewhmzbj.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.ydjk.org.cn/gtqqfwchfd.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.guowangkeji.top/gtquetueea.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.shuidangran.top/gtsxdgvxkd.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.nanxinkj.top/gttzopvjag.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.ppjwa.cn/gtedwsqrsw.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.cashguo.top/gtzhkhmlvs.html

[H02] finally / ensure 收尾
来源：http://hz.yueranfly.top/gtqxrwoygp.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.dashuyun.cn/gttbklpkfp.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.hongshengwenyu.top/gtcdfoegin.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.xingfuxueyuan.xyz/gtzwgmuiel.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.jqgufenzy.top/gtfidhwool.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.havefunace.top/gtdfylunhl.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.hysaishi.cn/gteomrobns.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.zycfv.cn/gtrkqtfttf.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.hywenlv.cn/gtjvjdjndf.html

[H03] 主动抛出异常
来源：http://hz.cheryme.top/gtjowrgsxq.html

Py:   raise ValueError("错误信息")
来源：http://hz.chenlongwang.top/gtwncbbyuf.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.aizwys.cn/gtaijpneiz.html

JS:   throw new Error("错误信息");
来源：http://hz.xylfe.cn/gtbqncienb.html

TS:   throw new Error("错误信息");
来源：http://hz.wangdashe.top/gtupxmzfgo.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.zdqjudy.top/gtwvtzfiyv.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.aibaodan.cn/gtmoqetktc.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.havefunace.top/gtytpjzqod.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.yj20258888.top/gtahzplqrh.html

[H04] 自定义异常类型
来源：http://hz.52xcode.cn/gtyebdvvmq.html

Py:   class MyError(Exception): pass
来源：http://hz.zhijiandao.cn/gtealdvzrt.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.yuxming.cn/gtrccqwnle.html

JS:   class MyError extends Error {}
来源：http://hz.zhiwuduotai.top/gtrjsjhgiv.html

TS:   class MyError extends Error {}
来源：http://hz.yonumen.top/gtilsbrhwh.html

Java: class MyException extends RuntimeException {}
来源：http://hz.quarkkingdee.top/gttlfeiuhu.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.cqqwz.cn/gtmpdspiso.html

Ruby: class MyError < StandardError; end
来源：http://hz.pengpengdd.cyou/gthsvzgktk.html

C#:   class MyException : Exception {}
来源：http://hz.ydzc1.top/gtcinnkjqv.html

[H05] 捕获特定类型
来源：http://hz.jlsjyb.cn/gtzntlwmbx.html

Py:   except ValueError as e:
来源：http://hz.birdmap.top/gtbpnxttoq.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.zhiwuduotai.top/gtqkzkcqqt.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.pengpengdd.cyou/gtwlektxpy.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.hongshengwenyu.top/gtqjcbzlxa.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.cucudq.cn/gtmzcmupkr.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.aibaodan.cn/gtgwddcxjk.html

Ruby: rescue ArgumentError => e
来源：http://hz.guannengcc.top/gtwyqgkdzh.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.tanke756.top/gtydmxqdzd.html

[H06] 可选值 / 空值安全访问
来源：http://hz.xylfe.cn/gtsfnjcfiz.html

Py:   value = d.get("k") or default
来源：http://hz.wangdashe.top/gtpoukyade.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.xingfuxueyuan.xyz/gtvcnfojls.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.xuanzx.com/gtrcaatupi.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.sufxvd.cn/gtxuusopqf.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.kuanghao11.cn/gthpxjlhkf.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.jyoumei.cn/gtnsxksxmb.html

Ruby: d&.dig(:a, :b)
来源：http://hz.52xcode.cn/gtgdnrcguf.html

C#:   obj?.A?.B ?? default
来源：http://hz.ivvv.top/gtccdxzxya.html

[H07] 断言
来源：http://hz.shangyingyoupin.top/gtvzulkkgn.html

Py:   assert x > 0, "必须为正"
来源：http://hz.jyoumei.cn/gtlupaeeea.html

PHP:  assert($x > 0);
来源：http://hz.zhijiandao.cn/gtkpblrpls.html

JS:   console.assert(x > 0);
来源：http://hz.chenjidiqi.icu/gtjvrnzdwx.html

TS:   console.assert(x > 0);
来源：http://hz.zdqjudy.top/gtkbkjnijn.html

Java: assert x > 0 : "必须为正";
来源：http://hz.yongpay.top/gtzauhtdll.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.mhx1999.top/gtunnsbuyi.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.smart0.xyz/gtzvgqsqmo.html

C#:   Debug.Assert(x > 0);
来源：http://hz.xylfe.cn/gtebrokvcz.html

[H08] 获取错误信息与堆栈
来源：http://hz.cqqwz.cn/gtgtgvzdmt.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.pengpengdd.cyou/gtfbxahqdh.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.tanke756.top/gtmuhhoyre.html

JS:   e.message;  e.stack
来源：http://hz.fengsongda.top/gtomnfuwkh.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.sweek.top/gtyfoyxyqd.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.jinqigufen.top/gtxwnfsnml.html

Go:   err.Error()
来源：http://hz.xuanzx.com/gtxmbfpabf.html

Ruby: e.message;  e.backtrace
来源：http://hz.ywan-chungtsiang.top/gtfaefpvhm.html

C#:   e.Message;  e.StackTrace
来源：http://hz.c1oappe.top/gtwsnkbbql.html

[H09] 带错误码的异常
来源：http://hz.shanyushiyangkeji.top/gtiwrbzkgj.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.wangdashe.top/gtygunktpb.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.xinyue.icu/gtphscxpcq.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.xingfuxueyuan.xyz/gtvsbencnt.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.fzhhl.top/gtxgbzgulb.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.zhongyouzk.top/gtdnbivpiq.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.ybcxt.top/gtcrjozuhw.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.tanke756.top/gtosxwxits.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.ybcxt.top/gtugqjgcko.html

[H10] 资源自动释放
来源：http://hz.ehwqpu.com/gtyxzpxiuo.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.tian-w.cn/gtcsjxbvcn.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.zhiwuduotai.top/gtqsyjgznx.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.jinqigfzy.top/gtqaeaqoml.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.jinyuanbaomall.cn/gtebqejohq.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.yangfankeji.com/gtisnxgwkm.html

Go:   defer f.Close()
来源：http://hz.shanyushiyangtech.top/gtxcmwxtxu.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.hfpthk.cn/gtuxhyautw.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.zhijiandao.cn/gtikdgaqwx.html

================================================================================
来源：http://hz.yj20258.top/gtmxxyvrko.html

I. 正则表达式
来源：http://hz.ybcxt.top/gtxccnjbrd.html

================================================================================
来源：http://hz.ppjwa.cn/gtucoopzxk.html

[I01] 判断是否匹配
来源：http://hz.hammf.cn/gtgbsllium.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.xziqi.cn/gtrqsgtply.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.xingfuxueyuan.xyz/gtvlszhosv.html

JS:   /\d+/.test(s)
来源：http://hz.wangshuangyany.cn/gtmlwqfrbo.html

TS:   /\d+/.test(s)
来源：http://hz.9152youxi.cn/gtuvfmtjni.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.zhongyouzk.top/gtppdbsbkr.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.yangfankeji.com/gtumgqbhgj.html

Ruby: s.match?(/\d+/)
来源：http://hz.sufxvd.cn/gtpcnggzpe.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.aizwys.cn/gtdgrlgepg.html

[I02] 提取所有匹配
来源：http://hz.nanxinkj.top/gteqhqnqid.html

Py:   re.findall(r"\d+", s)
来源：http://hz.fengsongda.top/gtyhgqlfjb.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.ppjwa.cn/gttlravadw.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.yongpay.top/gtaggriqwk.html

TS:   s.match(/\d+/g)
来源：http://hz.zhengqikj.top/gtzowcdgqd.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.jinyuanbaomall.cn/gtghfxqrxm.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.chenlongwang.top/gtuhdlyqnw.html

Ruby: s.scan(/\d+/)
来源：http://hz.jyoumei.cn/gtbydcxgxn.html


<!-- 参考信息 -->