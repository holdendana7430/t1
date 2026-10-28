代发 wailian999

TS:   fs.statSync("a.txt").size
来源：http://hz.gaohongyu789.top/gtsciljeay.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.andypj.xyz/gtjyykvdok.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.zhijiandao.cn/gtifskljwq.html

Ruby: File.size("a.txt")
来源：http://hz.zycfv.cn/gtslanmrlx.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.hnqzz.top/gtpmrjidpa.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.vqdsnc.cn/gtvlxyplom.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.daria6918.cn/gtxuubigcr.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.316326.xyz/gtuooxavcm.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.shangyingyoupin.top/gtudinrphe.html

TS:   path.extname("a.txt")
来源：http://hz.ehwqpu.com/gtguisrofp.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.nanxuanxn.top/gtfviycdfi.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.zhixingplan.top/gtdolyjiel.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.9152youxi.cn/gttuqsxnvv.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.quarkkingdee.top/gtxyfwzxgv.html

[F11] 复制与移动文件
来源：http://hz.fzhhl.top/gtmtmcjzcf.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.tianlin.xyz/gtviqonfse.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.feifeiyinyue.top/gtbckrxmew.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.gogol.net.cn/gtjinthqiv.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.jinghuilouyu.cn/gtuqfxpvlb.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.sysykeji.top/gtiehtaook.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.daria6918.cn/gtgteepipn.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.smart0.xyz/gtqhilvjwx.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.yanxiufei.cn/gtelsxcdvw.html

[F12] CSV 读写
来源：http://hz.ybcxt.top/gtqxgocqpi.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.cqqwz.cn/gtrwtmzhyp.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.andypj.xyz/gtscwkxasf.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.yanxiufei.cn/gtfnuuhhrc.html

TS:   // 同上
来源：http://hz.chenlongwang.top/gtgozxlwvq.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.shuidangran.top/gtlfuwxbav.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.quarkkingdee.top/gtfxwelnht.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.hfpthk.cn/gtqbymvrkz.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.tianlin.xyz/gtjkfhkngs.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtplsmikil.html

G. 面向对象
来源：http://hz.wangshuangyany.cn/gtfmwoiqep.html

================================================================================
来源：http://hz.chenlongwang.top/gtkmrpxoua.html

[G01] 定义类
来源：http://hz.ydzc1.top/gtpvblsidc.html

Py:   class User: pass
来源：http://hz.hongshengwenyu.top/gtprhdtrsq.html

PHP:  class User {}
来源：http://hz.havefunace.top/gtyijsgqvg.html

JS:   class User {}
来源：http://hz.52xcode.cn/gtzwmelrjt.html

TS:   class User { name: string = ""; }
来源：http://hz.vqdsnc.cn/gtaugaxopl.html

Java: class User {}
来源：http://hz.yanxiufei.cn/gthqpgxvse.html

Go:   type User struct { Name string }
来源：http://hz.shanyushiyangtech.top/gtlbkfatgm.html

Ruby: class User; end
来源：http://hz.nanxuanxn.top/gtlsisqfwq.html

C#:   class User {}
来源：http://hz.vqdsnc.cn/gtaowohiui.html

[G02] 构造函数
来源：http://hz.xziqi.cn/gtybhyxgpq.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.cdnleiting.top/gtlktxtxxz.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.hammf.cn/gtnbekoeif.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.zhoulong.xyz/gtbolwcljt.html

TS:   constructor(public name: string) {}
来源：http://hz.yanxiufei.cn/gtqpxwxkpb.html

Java: User(String name) { this.name = name; }
来源：http://hz.jinqigfzy.top/gtbspiomff.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.zhijiandao.cn/gtijtbwvum.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.zycfv.cn/gtzmdbvyuu.html

C#:   public User(string name) { Name = name; }
来源：http://hz.yuxming.cn/gtxpdrzfrw.html

[G03] 实例属性
来源：http://hz.shzxlz.cn/gtuyvdydxn.html

Py:   self.name = "x"
来源：http://hz.daxiang520.top/gtylpxdwfp.html

PHP:  public string $name = "x";
来源：http://hz.gaohongyu789.top/gtrhwxooix.html

JS:   this.name = "x";
来源：http://hz.hywenlv.cn/gtgfksmsnj.html

TS:   name: string = "x";
来源：http://hz.ivvv.top/gtjxwkeajy.html

Java: private String name;
来源：http://hz.cdnleiting.top/gtayfcvoxv.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.hongshengwenyu.top/gttbnsdxox.html

Ruby: @name = "x"
来源：http://hz.hammf.cn/gtvfjqtzxe.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.ydjk.org.cn/gteljyaajp.html

[G04] 定义方法
来源：http://hz.hnxiangtu.top/gtrugdhyuy.html

Py:   def greet(self): return self.name
来源：http://hz.jianghu66.top/gtrilfgyej.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.vqdsnc.cn/gthlweongn.html

JS:   greet() { return this.name; }
来源：http://hz.gaohongyu789.top/gtypdiabaz.html

TS:   greet(): string { return this.name; }
来源：http://hz.nanxinkj.top/gtzogloiwe.html

Java: String greet() { return name; }
来源：http://hz.jlsjyb.cn/gtgemvzrcd.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.xylfe.cn/gtrikskfxg.html

Ruby: def greet; @name; end
来源：http://hz.xylfe.cn/gtufypvfvn.html

C#:   public string Greet() => Name;
来源：http://hz.guowangkeji.top/gtdhxnkixd.html

[G05] 继承
来源：http://hz.jianghu66.top/gtvvhihmwx.html

Py:   class Admin(User): pass
来源：http://hz.zhijiandao.cn/gtboknzlck.html

PHP:  class Admin extends User {}
来源：http://hz.nanxinkj.top/gtkxanexrb.html

JS:   class Admin extends User {}
来源：http://hz.shangyingyoupin.top/gttnoqhkco.html

TS:   class Admin extends User {}
来源：http://hz.nanxuanxn.top/gtgbooganf.html

Java: class Admin extends User {}
来源：http://hz.hfpthk.cn/gtkdgxcoxo.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.shanyushiyangkeji.top/gtiwuafofp.html

Ruby: class Admin < User; end
来源：http://hz.xingfuxueyuan.xyz/gtaimgjmco.html

C#:   class Admin : User {}
来源：http://hz.yonumen.top/gtegkphjkw.html

[G06] 重写方法
来源：http://hz.sweek.top/gtctwrqjnr.html

Py:   def greet(self): return "admin"
来源：http://hz.jinyuanbaomall.cn/gtwevqabvg.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.hnqzz.top/gtvgljhaal.html

JS:   greet() { return "admin"; }
来源：http://hz.iojbl.cn/gtmjmeucve.html

TS:   greet(): string { return "admin"; }
来源：http://hz.zhengqikj.top/gttgpaiumw.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.shanyushiyangkeji.top/gtysqzoanx.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.316326.xyz/gtpdagjavf.html

Ruby: def greet; "admin"; end
来源：http://hz.svipenyu.cn/gtgpercjku.html

C#:   public override string Greet() => "admin";
来源：http://hz.jqgufenzy.top/gtvwogzeam.html

[G07] 调用父类方法
来源：http://hz.jqgfzy.top/gttluisyti.html

Py:   super().greet()
来源：http://hz.jinyuanbaomall.cn/gtifdipdgu.html

PHP:  parent::greet();
来源：http://hz.pengpengdd.cyou/gtatchrvco.html

JS:   super.greet();
来源：http://hz.sufxvd.cn/gtxiqagxzu.html

TS:   super.greet();
来源：http://hz.cashguo.top/gtkkmmvthn.html

Java: super.greet();
来源：http://hz.zhijiandao.cn/gtngfntuff.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.hnxiangtu.top/gthybflsnr.html

Ruby: super
来源：http://hz.zycfv.cn/gtvsvoujns.html

C#:   base.Greet();
来源：http://hz.quarkkingdee.top/gtaazfjjwd.html

[G08] 静态方法与属性
来源：http://hz.xziqi.cn/gtqqurwway.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.redwolf501.top/gtganpfqvs.html

PHP:  public static function f() {}
来源：http://hz.jinyuanbaomall.cn/gtrdbqjcaf.html

JS:   static f() {}
来源：http://hz.sufxvd.cn/gtwmdmmmqh.html

TS:   static f(): void {}
来源：http://hz.dianchejie.cn/gtjczmqyxq.html

Java: static void f() {}
来源：http://hz.yanxiufei.cn/gtexvxqwyl.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.chenzaomai.com/gtvlyamuhq.html

Ruby: def self.f; end
来源：http://hz.xziqi.cn/gtroyuinbc.html

C#:   public static void F() {}
来源：http://hz.vqdsnc.cn/gtojnunihi.html

[G09] 接口 / 抽象类
来源：http://hz.zhongyouzk.top/gtnlxlqqbh.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.aizwys.cn/gtbjcqhuti.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.snrcjt.cn/gtypnmxowk.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.cdnleiting.top/gtcaoefjnk.html

TS:   interface Shape { area(): number; }
来源：http://hz.tianlin.xyz/gtooemtzgg.html

Java: interface Shape { double area(); }
来源：http://hz.shzxlz.cn/gtmtnoaykh.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.yanxiufei.cn/gtktrhxicu.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.bjfxy.top/gtohzpvgfh.html

C#:   interface IShape { double Area(); }
来源：http://hz.zdqjudy.top/gtdtmqokox.html

[G10] 访问控制
来源：http://hz.chenjidiqi.icu/gtxtmiymsr.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.xylfe.cn/gtuclsskns.html

PHP:  public / protected / private
来源：http://hz.smart0.xyz/gtrdcquofo.html

JS:   #private 字段；其余公开
来源：http://hz.aibaodan.cn/gtzgyykprg.html

TS:   public / protected / private
来源：http://hz.sweek.top/gtcmmgruqc.html

Java: public / protected / private / 默认包级
来源：http://hz.jinghuilouyu.cn/gtkmzufwmf.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.jinyuanbaomall.cn/gtvysarpcb.html

Ruby: public / protected / private
来源：http://hz.jinyuanbaomall.cn/gtpopqfbsx.html

C#:   public / protected / private / internal
来源：http://hz.guannengcc.top/gtiipmgttz.html

[G11] getter / setter
来源：http://hz.jqgufenzy.top/gthdqnsgcg.html

Py:   @property 与 @x.setter
来源：http://hz.gaohongyu789.top/gthsqezjrp.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.andypj.xyz/gtcjqktzob.html

JS:   get name() { return this._name; }
来源：http://hz.pycfn.com/gtueinjwbf.html

TS:   get name(): string { return this._name; }
来源：http://hz.zhaomingkeji.xyz/gtkgtycjaf.html

Java: public String getName() { return name; }
来源：http://hz.hfpthk.cn/gtwauszpve.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.feifeiyinyue.top/gtmsrsstdx.html

Ruby: attr_accessor :name
来源：http://hz.jinqigufen.top/gtufcednzk.html

C#:   public string Name { get; set; }
来源：http://hz.havefunace.top/gtanohewcw.html

[G12] 对象转字符串
来源：http://hz.redwolf501.top/gtitptdijv.html

Py:   def __str__(self): return self.name
来源：http://hz.aibaodan.cn/gtzyhhqeik.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.zhijiandao.cn/gtuysuaudj.html

JS:   toString() { return this.name; }
来源：http://hz.tanke756.top/gtlmiummnn.html

TS:   toString(): string { return this.name; }
来源：http://hz.gogol.net.cn/gtfqdgyoun.html

Java: @Override public String toString() { return name; }
来源：http://hz.ppjwa.cn/gtbsxdmbpe.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.hongshengwenyu.top/gtxvbvoxob.html

Ruby: def to_s; @name; end
来源：http://hz.chenjidiqi.icu/gtoknmzvza.html

C#:   public override string ToString() => Name;
来源：http://hz.pengpengdd.cyou/gtgajqrncy.html

[G13] 判断对象类型
来源：http://hz.havefunace.top/gtdwvdkxwa.html

Py:   isinstance(u, User)
来源：http://hz.52xcode.cn/gtogzjmeie.html

PHP:  $u instanceof User
来源：http://hz.guowangkeji.top/gthfixfsbe.html

JS:   u instanceof User
来源：http://hz.chenjidiqi.icu/gtqqpazvgf.html

TS:   u instanceof User
来源：http://hz.gaohongyu789.top/gtcyqawchx.html

Java: u instanceof User
来源：http://hz.316326.xyz/gtemogtyok.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.daria6918.cn/gtpwkytzor.html

Ruby: u.is_a?(User)
来源：http://hz.kuanghao11.cn/gtdxrjfeju.html

C#:   u is User
来源：http://hz.chenjidiqi.icu/gtkotrpkjb.html

[G14] 数据类 / record
来源：http://hz.pycfn.com/gtjfjcqznk.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.hfpthk.cn/gtqizijvlz.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.jlsjyb.cn/gtwehjymww.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.cqqwz.cn/gtsxkamsky.html

TS:   type User = { name: string; age: number };
来源：http://hz.sysykeji.top/gtnbryyhex.html

Java: record User(String name, int age) {}
来源：http://hz.jinqigufen.top/gtgorjtjmg.html

Go:   type User struct { Name string; Age int }
来源：http://hz.dashuyun.cn/gtxeiobgij.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.tian-w.cn/gtjztcytoc.html

C#:   record User(string Name, int Age);
来源：http://hz.yangfankeji.com/gtlcwnodho.html

[G15] 枚举
来源：http://hz.shzxlz.cn/gtwzhqpfeq.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.hysaishi.cn/gtrdbvnttp.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.snrcjt.cn/gtanittjmi.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.ydjk.org.cn/gtvxfabawt.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.tianlin.xyz/gtgepdknws.html

Java: enum Color { RED, GREEN }
来源：http://hz.jyoumei.cn/gtqqpqisyg.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.cucudq.cn/gtgtanpvka.html

Ruby: Color = %i[red green].freeze
来源：http://hz.yj20258.top/gtjmqlrdoa.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.shuidangran.top/gthuyqvsfz.html

[G16] 对象转数组 / 字典
来源：http://hz.redwolf501.top/gtihjccanu.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.yueranfly.top/gtlysjnlzp.html

PHP:  get_object_vars($obj);
来源：http://hz.0kj1m.cn/gtzvcinyxu.html

JS:   Object.entries(obj)
来源：http://hz.9152youxi.cn/gtmwhszksj.html

TS:   Object.entries(obj)
来源：http://hz.gaohongyu789.top/gtwxxyqbzo.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.jinqigfzy.top/gteupdxdrp.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.sxryk.cn/gtfkidoinb.html

Ruby: obj.instance_variables
来源：http://hz.jiagoushi.top/gtmsqzqyea.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.andypj.xyz/gtdyavnpvi.html

================================================================================
来源：http://hz.xinyue.icu/gtudppuknf.html

H. 异常与错误处理
来源：http://hz.shzxlz.cn/gtqngedkro.html

================================================================================
来源：http://hz.ybcxt.top/gtbztycfuy.html

[H01] try / catch 基础
来源：http://hz.yuanzhike.top/gtrqhoabro.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.jinqigufen.top/gtgnzhkkfd.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.snrcjt.cn/gtgdnkaimg.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.zhoulong.xyz/gtobgbxmhl.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.hammf.cn/gtuhaxmkjw.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.zhijiandao.cn/gtemevacsx.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.jiagoushi.top/gtlgjmjafe.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.yj20258888.top/gtrofxjmdz.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.ywan-chungtsiang.top/gtowykrtut.html

[H02] finally / ensure 收尾
来源：http://hz.0kj1m.cn/gtmjacetoa.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.hysaishi.cn/gtyhvwahzg.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.yongpay.top/gtcgwonesy.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.jiagoushi.top/gtqhzfyvnf.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.sufxvd.cn/gtgcuvyqfw.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.haohaochexian.top/gtzpdbppiq.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.redwolf501.top/gtooeiralg.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.meibo888.top/gtsjduflsf.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.smart0.xyz/gtjsvmnxfx.html

[H03] 主动抛出异常
来源：http://hz.ydzc1.top/gticdwdttn.html

Py:   raise ValueError("错误信息")
来源：http://hz.52xcode.cn/gtpdwrkptt.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.hywenlv.cn/gtgpbjumsj.html

JS:   throw new Error("错误信息");
来源：http://hz.zhoulong.xyz/gtqpvlantb.html

TS:   throw new Error("错误信息");
来源：http://hz.yj20258888.top/gtzhipraog.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.cashguo.top/gtmsaegwoo.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.yj202588.top/gtyttibnps.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.zdqjudy.top/gtvyqfxwet.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.ywan-chungtsiang.top/gtowyxoacy.html

[H04] 自定义异常类型
来源：http://hz.shzxlz.cn/gthkmrvvye.html

Py:   class MyError(Exception): pass
来源：http://hz.zhixingplan.top/gtdqegqybf.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.yongpay.top/gtusojdkba.html

JS:   class MyError extends Error {}
来源：http://hz.jinqigfzy.top/gtinjtkdch.html

TS:   class MyError extends Error {}
来源：http://hz.c1oappe.top/gthbyoevhv.html

Java: class MyException extends RuntimeException {}
来源：http://hz.chenzaomai.com/gtreswfsip.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.xziqi.cn/gtxpeyllbk.html

Ruby: class MyError < StandardError; end
来源：http://hz.zhiwuduotai.top/gtrljzaohq.html

C#:   class MyException : Exception {}
来源：http://hz.ydjk.org.cn/gtdqxdwgyp.html

[H05] 捕获特定类型
来源：http://hz.hywenlv.cn/gtrefvvhwu.html

Py:   except ValueError as e:
来源：http://hz.guowangkeji.top/gtbucagdlf.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.iojbl.cn/gtehvrjour.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.zhongyouzk.top/gtbnpbxxgc.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.yvedp.cn/gtuaozxwwy.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.birdmap.top/gtlxmgsodt.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.zhiwuduotai.top/gttwakenlv.html

Ruby: rescue ArgumentError => e
来源：http://hz.jinyuanbaomall.cn/gtgyylnfgf.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.52xcode.cn/gtfdxhrzzh.html

[H06] 可选值 / 空值安全访问
来源：http://hz.vqdsnc.cn/gteyvqqnsn.html

Py:   value = d.get("k") or default
来源：http://hz.yj20258.top/gtqbgghizm.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.tianlin.xyz/gtcmlapgud.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.kuanghao11.cn/gteuvgdfce.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.yuanzhike.top/gtjqgejzab.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.jyoumei.cn/gtuytzftrj.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.nanxinkj.top/gtubnvvdah.html

Ruby: d&.dig(:a, :b)
来源：http://hz.tianlin.xyz/gtuqungnsm.html

C#:   obj?.A?.B ?? default
来源：http://hz.hammf.cn/gtfeagkehu.html

[H07] 断言
来源：http://hz.sufxvd.cn/gtnrdyofqn.html

Py:   assert x > 0, "必须为正"
来源：http://hz.ivvv.top/gtsittbebs.html

PHP:  assert($x > 0);
来源：http://hz.pycfn.com/gtuxpbgbig.html

JS:   console.assert(x > 0);
来源：http://hz.shanyushiyangkeji.top/gtzocafmxm.html

TS:   console.assert(x > 0);
来源：http://hz.cqqwz.cn/gttkhmhcaz.html

Java: assert x > 0 : "必须为正";
来源：http://hz.316326.xyz/gttzkzedya.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.pycfn.com/gtdmxzueqp.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.vqdsnc.cn/gtnsmngcds.html

C#:   Debug.Assert(x > 0);
来源：http://hz.tanke756.top/gtqdjdends.html

[H08] 获取错误信息与堆栈
来源：http://hz.cheryme.top/gtqgowmtql.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.havefunace.top/gtqquqgrra.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.hnqzz.top/gttolxflng.html

JS:   e.message;  e.stack
来源：http://hz.xingfuxueyuan.xyz/gtculepzrp.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.shangyingyoupin.top/gtmrvjstzl.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.jqgufenzy.top/gtxdiwijgt.html

Go:   err.Error()
来源：http://hz.vqdsnc.cn/gtohautqrx.html

Ruby: e.message;  e.backtrace
来源：http://hz.cashguo.top/gtvaubbllo.html

C#:   e.Message;  e.StackTrace
来源：http://hz.yongpay.top/gtncjrhlkq.html

[H09] 带错误码的异常
来源：http://hz.aibaodan.cn/gtwulaakjm.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.yj202588.top/gtdwlzemrz.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.c1oappe.top/gtjltrojbm.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.yueranfly.top/gthcuqvhzc.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.tian-w.cn/gtncyjccun.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.mhx1999.top/gtyuieazwm.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.sysykeji.top/gtiuzlykti.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.jyoumei.cn/gtqvbgsmkc.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.zhaomingkeji.xyz/gtgjzqflmo.html

[H10] 资源自动释放
来源：http://hz.daria6918.cn/gtpkexjkpi.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.shanyushiyangkeji.top/gtvxssjcue.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.ydjk.org.cn/gtvghrbpwb.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.zhoulong.xyz/gtyvbbgjdw.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.jqgufenzy.top/gttnlgnoue.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.yj202588.top/gtfrrsjkxe.html

Go:   defer f.Close()
来源：http://hz.hywenlv.cn/gtihxwneff.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.jianghu66.top/gteqxmcmbu.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.zhoulong.xyz/gtoepqrwrh.html

================================================================================
来源：http://hz.gzhubu.top/gtldssqlev.html

I. 正则表达式
来源：http://hz.shanyushiyangkeji.top/gtgyumemsn.html

================================================================================
来源：http://hz.sweek.top/gtaymaupop.html

[I01] 判断是否匹配
来源：http://hz.yonumen.top/gtybecdzjp.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.mhx1999.top/gtsuzyswmt.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.jinqigfzy.top/gtppyitbgu.html

JS:   /\d+/.test(s)
来源：http://hz.aizwys.cn/gtlpnuqnhj.html

TS:   /\d+/.test(s)
来源：http://hz.daxiang520.top/gtxpnudwpp.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.yuanzhike.top/gtdzsgoamm.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.yongpay.top/gtyuogoaxf.html

Ruby: s.match?(/\d+/)
来源：http://hz.zhijiandao.cn/gtfhlmzhlk.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.cheryme.top/gtkaukawrg.html

[I02] 提取所有匹配
来源：http://hz.yonumen.top/gtvzpuqxpc.html

Py:   re.findall(r"\d+", s)
来源：http://hz.yuxming.cn/gtowljauez.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.shanyushiyangkeji.top/gtwufehzeo.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.aizwys.cn/gtzyrvzfmc.html

TS:   s.match(/\d+/g)
来源：http://hz.sweek.top/gtetexnpyi.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.cdnleiting.top/gtpyapdrdo.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.fzhhl.top/gtwujwydba.html

Ruby: s.scan(/\d+/)
来源：http://hz.jianghu66.top/gtvdpjolcr.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.jinyuanbaomall.cn/gtpxuknuwj.html

[I03] 提取捕获分组
来源：http://hz.jinqigufen.top/gttqicwmdd.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.vqdsnc.cn/gtfurfsqdy.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.meibo888.top/gtchjzwzop.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.yonumen.top/gtmbjazqhj.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.hammf.cn/gtqwytyoef.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.jqgufenzy.top/gtvcdstcdf.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.gogol.net.cn/gtyuisnmhe.html


<!-- 参考信息 -->