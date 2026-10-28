代发 wailian999

C#:   new FileInfo("a.txt").Length
来源：http://hz.jinyuanbaomall.cn/gtndqbfdue.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.dianchejie.cn/gtdgjbcmkn.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.daria6918.cn/gtbpwybabi.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.52xcode.cn/gtnbqgsyuv.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.cheryme.top/gtozqfmpvm.html

TS:   path.extname("a.txt")
来源：http://hz.jinghuilouyu.cn/gtlxhrnfwh.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.jinqigfzy.top/gtbtlzuhqk.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.zycfv.cn/gtkhxssilc.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.daria6918.cn/gtwnsfctqc.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.cheryme.top/gtwbjwmubj.html

[F11] 复制与移动文件
来源：http://hz.gotoacloud.top/gtmrmdpwos.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.hammf.cn/gtxkgnwauk.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.bjfxy.top/gtaxvmwsyj.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.zycfv.cn/gtzdamgfdv.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.yongpay.top/gtevpvsmxi.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.hfpthk.cn/gtntthaaww.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.yuxming.cn/gtpjpkjhmv.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.316326.xyz/gtmzpaypkg.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.yuxming.cn/gttldgnabp.html

[F12] CSV 读写
来源：http://hz.pycfn.com/gtrzyopdhw.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.shanyushiyangkeji.top/gtvbhvikob.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.fzhhl.top/gtwyjwhglx.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.chenlongwang.top/gticrlojco.html

TS:   // 同上
来源：http://hz.jqgufenzy.top/gtduccgnpq.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.sweek.top/gtmpfanutu.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.hnqzz.top/gtcwmmqjqg.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.zhijiandao.cn/gtouelhhya.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.ybcxt.top/gtccqueagb.html

================================================================================
来源：http://hz.zhongyouzk.top/gtcmlwvmgu.html

G. 面向对象
来源：http://hz.gaohongyu789.top/gtsxcujjjv.html

================================================================================
来源：http://hz.gaohongyu789.top/gtmktgmcrb.html

[G01] 定义类
来源：http://hz.hammf.cn/gtprffppqe.html

Py:   class User: pass
来源：http://hz.ivvv.top/gtmqtpcwjx.html

PHP:  class User {}
来源：http://hz.sxryk.cn/gtfcuzstvf.html

JS:   class User {}
来源：http://hz.daria6918.cn/gtvbwwriio.html

TS:   class User { name: string = ""; }
来源：http://hz.bjfxy.top/gtmnqbywev.html

Java: class User {}
来源：http://hz.pengpengdd.cyou/gtwumcxuuo.html

Go:   type User struct { Name string }
来源：http://hz.316326.xyz/gtjjyfvgmu.html

Ruby: class User; end
来源：http://hz.guannengcc.top/gtldeuoomp.html

C#:   class User {}
来源：http://hz.daria6918.cn/gtgboxihan.html

[G02] 构造函数
来源：http://hz.nanxinkj.top/gttwkqyouk.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.fzhhl.top/gtigwsomzp.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.shanyushiyangtech.top/gtsllihkrn.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.hfpthk.cn/gteguvsjkb.html

TS:   constructor(public name: string) {}
来源：http://hz.zhoulong.xyz/gtlehqndqz.html

Java: User(String name) { this.name = name; }
来源：http://hz.meibo888.top/gthebfbpug.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.mhx1999.top/gtzlkqjqeb.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.yonumen.top/gtzzfobtcg.html

C#:   public User(string name) { Name = name; }
来源：http://hz.gogol.net.cn/gtkeocezth.html

[G03] 实例属性
来源：http://hz.52xcode.cn/gthukyersy.html

Py:   self.name = "x"
来源：http://hz.zhixingplan.top/gtyohfxxda.html

PHP:  public string $name = "x";
来源：http://hz.jinqigfzy.top/gtjhnmzpgt.html

JS:   this.name = "x";
来源：http://hz.sweek.top/gtbisvdbfe.html

TS:   name: string = "x";
来源：http://hz.zhijiandao.cn/gtsllpfrgn.html

Java: private String name;
来源：http://hz.c1oappe.top/gtlhbkibno.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.yangfankeji.com/gtxqrtgvfz.html

Ruby: @name = "x"
来源：http://hz.yj20258.top/gtxyixwouz.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.pengpengdd.cyou/gtobcmesjg.html

[G04] 定义方法
来源：http://hz.jiagoushi.top/gtxxolwwel.html

Py:   def greet(self): return self.name
来源：http://hz.tianlin.xyz/gthjoicutp.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.shanyushiyangkeji.top/gttdfkynfv.html

JS:   greet() { return this.name; }
来源：http://hz.ehwqpu.com/gtzkdrobcc.html

TS:   greet(): string { return this.name; }
来源：http://hz.pycfn.com/gtmcwihnrx.html

Java: String greet() { return name; }
来源：http://hz.pycfn.com/gtuvhypkay.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.ehwqpu.com/gtzovathoe.html

Ruby: def greet; @name; end
来源：http://hz.yanxiufei.cn/gtvgycsshf.html

C#:   public string Greet() => Name;
来源：http://hz.wangshuangyany.cn/gthwfczjll.html

[G05] 继承
来源：http://hz.guowangkeji.top/gteycggcrj.html

Py:   class Admin(User): pass
来源：http://hz.cashguo.top/gttxwjywos.html

PHP:  class Admin extends User {}
来源：http://hz.shangyingyoupin.top/gtzgviliil.html

JS:   class Admin extends User {}
来源：http://hz.zhijiandao.cn/gtqtkjsykj.html

TS:   class Admin extends User {}
来源：http://hz.zhongyouzk.top/gtjjwqktbi.html

Java: class Admin extends User {}
来源：http://hz.zhijiandao.cn/gtmbquutrh.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.bjfxy.top/gttuoyscab.html

Ruby: class Admin < User; end
来源：http://hz.daxiang520.top/gtebaperfx.html

C#:   class Admin : User {}
来源：http://hz.sysykeji.top/gtvsxlfsxj.html

[G06] 重写方法
来源：http://hz.redwolf501.top/gtgyykpksy.html

Py:   def greet(self): return "admin"
来源：http://hz.wangshuangyany.cn/gtmcjqgmcc.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.snrcjt.cn/gtlxxvjjtt.html

JS:   greet() { return "admin"; }
来源：http://hz.yonumen.top/gtbikyxdac.html

TS:   greet(): string { return "admin"; }
来源：http://hz.xuetiantiany.cn/gtnadpbohj.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.quarkkingdee.top/gtuxllgxkc.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.gaohongyu789.top/gtfimijaps.html

Ruby: def greet; "admin"; end
来源：http://hz.yongpay.top/gthwcwckgr.html

C#:   public override string Greet() => "admin";
来源：http://hz.ppjwa.cn/gtllyhrekm.html

[G07] 调用父类方法
来源：http://hz.shuidangran.top/gtvkagksri.html

Py:   super().greet()
来源：http://hz.c1oappe.top/gtlzullrup.html

PHP:  parent::greet();
来源：http://hz.jinghuilouyu.cn/gtoauqdhpc.html

JS:   super.greet();
来源：http://hz.jianghu66.top/gtzbnhltct.html

TS:   super.greet();
来源：http://hz.chenlongwang.top/gtxzbygdin.html

Java: super.greet();
来源：http://hz.cashguo.top/gtgwoscubc.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.zhoulong.xyz/gtakyobmrm.html

Ruby: super
来源：http://hz.hfpthk.cn/gtngpthzej.html

C#:   base.Greet();
来源：http://hz.sweek.top/gtqqnwlaue.html

[G08] 静态方法与属性
来源：http://hz.chenlongwang.top/gtvtzxjxwj.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.xziqi.cn/gtnsncfrqb.html

PHP:  public static function f() {}
来源：http://hz.xuetiantiany.cn/gtpnketbhk.html

JS:   static f() {}
来源：http://hz.hysaishi.cn/gtmagmqwqh.html

TS:   static f(): void {}
来源：http://hz.sufxvd.cn/gtlnmuwvua.html

Java: static void f() {}
来源：http://hz.bjfxy.top/gtjsbuyags.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.quarkkingdee.top/gtymociqwr.html

Ruby: def self.f; end
来源：http://hz.jlsjyb.cn/gtteuydggs.html

C#:   public static void F() {}
来源：http://hz.birdmap.top/gtdqrmnqhd.html

[G09] 接口 / 抽象类
来源：http://hz.hfpthk.cn/gtbdfnhlka.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.yuanzhike.top/gtxwgfxsps.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.pycfn.com/gtotapeggy.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.mhx1999.top/gtnvawpnki.html

TS:   interface Shape { area(): number; }
来源：http://hz.gogol.net.cn/gtietxloyx.html

Java: interface Shape { double area(); }
来源：http://hz.wangshuangyany.cn/gtljyzlxnc.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.birdmap.top/gtgpshjllx.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.quarkkingdee.top/gtyzbwwvzd.html

C#:   interface IShape { double Area(); }
来源：http://hz.hywenlv.cn/gtwvtzoute.html

[G10] 访问控制
来源：http://hz.shzxlz.cn/gtuzbhvzea.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.birdmap.top/gtetzrsqas.html

PHP:  public / protected / private
来源：http://hz.xziqi.cn/gtdfqgrmob.html

JS:   #private 字段；其余公开
来源：http://hz.pycfn.com/gtamyekwdk.html

TS:   public / protected / private
来源：http://hz.zhengqikj.top/gtdurpztzd.html

Java: public / protected / private / 默认包级
来源：http://hz.pycfn.com/gtbgxcekvu.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.pycfn.com/gtrhbniltc.html

Ruby: public / protected / private
来源：http://hz.ivvv.top/gtxqsgcswy.html

C#:   public / protected / private / internal
来源：http://hz.gogol.net.cn/gttarcagob.html

[G11] getter / setter
来源：http://hz.yanxiufei.cn/gtrdttnajo.html

Py:   @property 与 @x.setter
来源：http://hz.pycfn.com/gtuyxurbty.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.zhijiandao.cn/gtblcafxph.html

JS:   get name() { return this._name; }
来源：http://hz.xuetiantiany.cn/gtejszxhzs.html

TS:   get name(): string { return this._name; }
来源：http://hz.yanxiufei.cn/gtyqixtbqx.html

Java: public String getName() { return name; }
来源：http://hz.ehwqpu.com/gtmdnhxkcc.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.jinqigfzy.top/gtrrrjsatv.html

Ruby: attr_accessor :name
来源：http://hz.zhongyouzk.top/gtceiublsg.html

C#:   public string Name { get; set; }
来源：http://hz.tian-w.cn/gtmeyhebuh.html

[G12] 对象转字符串
来源：http://hz.hysaishi.cn/gtfpxdrrrt.html

Py:   def __str__(self): return self.name
来源：http://hz.ydzc1.top/gtynzryyve.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.xziqi.cn/gtdinmftce.html

JS:   toString() { return this.name; }
来源：http://hz.ehwqpu.com/gtjmxwwxxq.html

TS:   toString(): string { return this.name; }
来源：http://hz.hammf.cn/gtedyfqnnk.html

Java: @Override public String toString() { return name; }
来源：http://hz.aibaodan.cn/gtzwzcpmvb.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.jqgufenzy.top/gttfendayu.html

Ruby: def to_s; @name; end
来源：http://hz.yueranfly.top/gtgvfsygqh.html

C#:   public override string ToString() => Name;
来源：http://hz.feifeiyinyue.top/gtztihcqea.html

[G13] 判断对象类型
来源：http://hz.xuanzx.com/gtxjbvgdpf.html

Py:   isinstance(u, User)
来源：http://hz.316326.xyz/gtgdpeards.html

PHP:  $u instanceof User
来源：http://hz.316326.xyz/gtqcqfbilq.html

JS:   u instanceof User
来源：http://hz.gotoacloud.top/gtnfqxsgka.html

TS:   u instanceof User
来源：http://hz.vqdsnc.cn/gtmrokubyw.html

Java: u instanceof User
来源：http://hz.yangfankeji.com/gtqertyihf.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.daria6918.cn/gtvlqjcizk.html

Ruby: u.is_a?(User)
来源：http://hz.jinyuanbaomall.cn/gtnnqvzupf.html

C#:   u is User
来源：http://hz.haohaochexian.top/gtzlghbutj.html

[G14] 数据类 / record
来源：http://hz.andypj.xyz/gtddmbxqxv.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.wangdashe.top/gtmjqndzpd.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.hnqzz.top/gtpoctdrma.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.havefunace.top/gthiaqalle.html

TS:   type User = { name: string; age: number };
来源：http://hz.redwolf501.top/gtachcfafg.html

Java: record User(String name, int age) {}
来源：http://hz.cdnleiting.top/gtkhbahcet.html

Go:   type User struct { Name string; Age int }
来源：http://hz.yangfankeji.com/gtjxkepnlh.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.zdqjudy.top/gttjqcnyhj.html

C#:   record User(string Name, int Age);
来源：http://hz.jianghu66.top/gtbbljynvd.html

[G15] 枚举
来源：http://hz.zhoulong.xyz/gtifunhgeb.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.guannengcc.top/gtkmyylztt.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.andypj.xyz/gtfuqiydkl.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.aizwys.cn/gtahittfqd.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.chenzaomai.com/gtekrqtudj.html

Java: enum Color { RED, GREEN }
来源：http://hz.yanxiufei.cn/gtiwybleyh.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.zhoulong.xyz/gtzpaejyxz.html

Ruby: Color = %i[red green].freeze
来源：http://hz.ywan-chungtsiang.top/gtnidxfqoz.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.vqdsnc.cn/gtjtxldbvc.html

[G16] 对象转数组 / 字典
来源：http://hz.gzhubu.top/gtqygmdhka.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.gaohongyu789.top/gtymxcship.html

PHP:  get_object_vars($obj);
来源：http://hz.sufxvd.cn/gtcdkflrrq.html

JS:   Object.entries(obj)
来源：http://hz.cucudq.cn/gtslqqykjy.html

TS:   Object.entries(obj)
来源：http://hz.xuetiantiany.cn/gtrwlzryfw.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.yj20258888.top/gtloaapaxu.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.cheryme.top/gtzzqyvtai.html

Ruby: obj.instance_variables
来源：http://hz.jianghu66.top/gtbqmzzdew.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.nwbrower.top/gtxpcxheky.html

================================================================================
来源：http://hz.cashguo.top/gtrxmiqddr.html

H. 异常与错误处理
来源：http://hz.wangdashe.top/gtzqahvwet.html

================================================================================
来源：http://hz.sysykeji.top/gtyqtitvqd.html

[H01] try / catch 基础
来源：http://hz.yuanzhike.top/gtrvvqqpzr.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.yonumen.top/gtwrtbrfxa.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.hnxiangtu.top/gtkdacvrxj.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.xuetiantiany.cn/gtyataerhw.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.daxiang520.top/gtgokjnusf.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.hywenlv.cn/gtthcstczr.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.dashuyun.cn/gtwblbtzrk.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.zhaomingkeji.xyz/gtmvrdaqtt.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.bjfxy.top/gtqqnoxmdu.html

[H02] finally / ensure 收尾
来源：http://hz.316326.xyz/gtmpkwmvgl.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.yonumen.top/gthlvcskvt.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.dianchejie.cn/gthszjkkol.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.zycfv.cn/gttqkzuhvz.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.mhx1999.top/gtpahkvkgt.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.jlsjyb.cn/gtfmcipqwr.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.sxryk.cn/gtjayzbbos.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.yuanzhike.top/gtcptyiwni.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.hongshengwenyu.top/gtcwjlktyh.html

[H03] 主动抛出异常
来源：http://hz.yanxiufei.cn/gtewjvckbe.html

Py:   raise ValueError("错误信息")
来源：http://hz.wangshuangyany.cn/gttgretwkf.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.pycfn.com/gtlwiaopmp.html

JS:   throw new Error("错误信息");
来源：http://hz.c1oappe.top/gtvnpwmtzm.html

TS:   throw new Error("错误信息");
来源：http://hz.sweek.top/gtaubjsesu.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.vqdsnc.cn/gtxkootsae.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.shanyushiyangtech.top/gtxoamafln.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.cdnleiting.top/gtttxdwcnq.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.jinyuanbaomall.cn/gtpylbxtlz.html

[H04] 自定义异常类型
来源：http://hz.jinqigfzy.top/gtpphoadgc.html

Py:   class MyError(Exception): pass
来源：http://hz.yangfankeji.com/gtiqwosqqk.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.haohaochexian.top/gtkdszpezn.html

JS:   class MyError extends Error {}
来源：http://hz.chenzaomai.com/gtcbjcgxdz.html

TS:   class MyError extends Error {}
来源：http://hz.jinghuilouyu.cn/gtcvrestpe.html

Java: class MyException extends RuntimeException {}
来源：http://hz.redwolf501.top/gtokryodwp.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.jinyuanbaomall.cn/gtinwsedgv.html

Ruby: class MyError < StandardError; end
来源：http://hz.cucudq.cn/gtroileoeq.html

C#:   class MyException : Exception {}
来源：http://hz.pengpengdd.cyou/gtntmcqcdi.html

[H05] 捕获特定类型
来源：http://hz.zhijiandao.cn/gtixniqmsr.html

Py:   except ValueError as e:
来源：http://hz.yongpay.top/gtzrprozge.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.quarkkingdee.top/gthzqsrxos.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.xinyue.icu/gtxdhsnynp.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.zhengqikj.top/gtlldefoia.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.zhiwuduotai.top/gtgupnzzqa.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.jlsjyb.cn/gtbeaewxji.html

Ruby: rescue ArgumentError => e
来源：http://hz.smart0.xyz/gthcapmwwd.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.dianchejie.cn/gtmcobjtjy.html

[H06] 可选值 / 空值安全访问
来源：http://hz.sweek.top/gtjoepudfr.html

Py:   value = d.get("k") or default
来源：http://hz.meibo888.top/gtvogyummz.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.zhoulong.xyz/gtffmttytr.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.shuidangran.top/gtprrzhvam.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.smart0.xyz/gtvpvbqujb.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.redwolf501.top/gtjvygxhul.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.shzxlz.cn/gtlnevbdux.html

Ruby: d&.dig(:a, :b)
来源：http://hz.chenzaomai.com/gtbtdmruyb.html

C#:   obj?.A?.B ?? default
来源：http://hz.xingfuxueyuan.xyz/gtfpfntrpm.html

[H07] 断言
来源：http://hz.shanyushiyangtech.top/gtzgnxipvz.html

Py:   assert x > 0, "必须为正"
来源：http://hz.hnqzz.top/gtmtwukmlx.html

PHP:  assert($x > 0);
来源：http://hz.cdnleiting.top/gtuiliecto.html

JS:   console.assert(x > 0);
来源：http://hz.zdqjudy.top/gtfxpaihfc.html

TS:   console.assert(x > 0);
来源：http://hz.gzhubu.top/gtjlddarqg.html

Java: assert x > 0 : "必须为正";
来源：http://hz.ehwqpu.com/gttadgzmcp.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.nanxinkj.top/gtngklpngs.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.aizwys.cn/gtlocpjtgl.html

C#:   Debug.Assert(x > 0);
来源：http://hz.shangyingyoupin.top/gttlqiqrud.html

[H08] 获取错误信息与堆栈
来源：http://hz.ydzc1.top/gtnrjpnwlo.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.xziqi.cn/gtmnyjxjdy.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.chenjidiqi.icu/gtmbetdsrn.html

JS:   e.message;  e.stack
来源：http://hz.sxryk.cn/gtczedhjlr.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.cdnleiting.top/gtdvwdfhba.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.yuanzhike.top/gtueidfopn.html

Go:   err.Error()
来源：http://hz.yj20258888.top/gtzealsifl.html

Ruby: e.message;  e.backtrace
来源：http://hz.hysaishi.cn/gtudmwytls.html

C#:   e.Message;  e.StackTrace
来源：http://hz.ywan-chungtsiang.top/gtqpxvegoh.html

[H09] 带错误码的异常
来源：http://hz.cashguo.top/gtwweokidm.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.ehwqpu.com/gtuvplcpsq.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.zhixingplan.top/gtdxkujsfk.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.jinghuilouyu.cn/gtnlqwioqu.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.fzhhl.top/gtpudoxwfh.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.sweek.top/gtaibegnwx.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.nwbrower.top/gtysvlugrt.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.ybcxt.top/gtqpkkldjc.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.cucudq.cn/gtquwywzht.html

[H10] 资源自动释放
来源：http://hz.xinyue.icu/gtabidtcdi.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.yueranfly.top/gtqyjwjnuj.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.tanke756.top/gtbucuhkof.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.wangdashe.top/gtmvnkadkz.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.hnxiangtu.top/gttnxfkqvb.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.feifeiyinyue.top/gtimhakyvm.html

Go:   defer f.Close()
来源：http://hz.nanxuanxn.top/gtxvctbogf.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.zhongyouzk.top/gtgynjgnvc.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.gogol.net.cn/gtqskwlcka.html

================================================================================
来源：http://hz.sufxvd.cn/gtptxwtkes.html

I. 正则表达式
来源：http://hz.quarkkingdee.top/gtcangfoko.html

================================================================================
来源：http://hz.chenlongwang.top/gttswardfg.html

[I01] 判断是否匹配
来源：http://hz.zhoulong.xyz/gtzlusuhsk.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.sxryk.cn/gtcwsgvffa.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.jinyuanbaomall.cn/gtezuoyqfb.html

JS:   /\d+/.test(s)
来源：http://hz.hongshengwenyu.top/gtpxzjxcpy.html

TS:   /\d+/.test(s)
来源：http://hz.hongshengwenyu.top/gtzyimrcgl.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.gogol.net.cn/gtajtckdsd.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.vqdsnc.cn/gtfghxkjzf.html

Ruby: s.match?(/\d+/)
来源：http://hz.yj202588.top/gtxxdvwhyt.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.yj202588.top/gtlgvwncga.html

[I02] 提取所有匹配
来源：http://hz.cdnleiting.top/gtkemuummu.html

Py:   re.findall(r"\d+", s)
来源：http://hz.yuanzhike.top/gtadkjrbom.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.daxiang520.top/gthowkmykb.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.yanxiufei.cn/gtoevszggo.html

TS:   s.match(/\d+/g)
来源：http://hz.tanke756.top/gtbkxiiswn.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.yj202588.top/gtvukyipjm.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.andypj.xyz/gthdwktnes.html

Ruby: s.scan(/\d+/)
来源：http://hz.quarkkingdee.top/gtolwgxjiz.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.hfpthk.cn/gtccgetvdc.html

[I03] 提取捕获分组
来源：http://hz.nanxuanxn.top/gtmjlsmzrr.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.zhengqikj.top/gtdjbxxfed.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.tian-w.cn/gtrvxsqqgt.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.tian-w.cn/gtceqnxmil.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.wangdashe.top/gtyqwpxpgr.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.hongshengwenyu.top/gtzavkqqyl.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.daxiang520.top/gtdbgprfnn.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.yueranfly.top/gtwdqjbztj.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.yj20258.top/gtshayxuni.html

[I04] 正则替换
来源：http://hz.gotoacloud.top/gtncffkynb.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.yuxming.cn/gtullrrryh.html


<!-- 参考信息 -->