代发 wailian999

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.xingfuxueyuan.xyz/gtrbxgyzqb.html

TS:   path.extname("a.txt")
来源：http://hz.hywenlv.cn/gtzklmndum.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.redwolf501.top/gtlipaakbc.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.gzhubu.top/gtrlnajzux.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.ppjwa.cn/gtnhajwgtv.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.shanyushiyangkeji.top/gtxrztiosd.html

[F11] 复制与移动文件
来源：http://hz.jinqigufen.top/gtskdnjdac.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.nwbrower.top/gtmvyhqqeu.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.snrcjt.cn/gtglvvhsjv.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.ybcxt.top/gtdkwninuh.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.dianchejie.cn/gtyrhyoclq.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.aibaodan.cn/gtbzpxxrdu.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.chenjidiqi.icu/gtznzmhdhz.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.hywenlv.cn/gtvuxsznve.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.redwolf501.top/gttxqtiyci.html

[F12] CSV 读写
来源：http://hz.jianghu66.top/gtjmhqjsgb.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.jinqigfzy.top/gtgrnfzpdo.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.iojbl.cn/gtebvfkekd.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.guowangkeji.top/gtphkssmgh.html

TS:   // 同上
来源：http://hz.hywenlv.cn/gtgttficuq.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.gogol.net.cn/gtvrwhmarj.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.yuxming.cn/gtmgdoqbxe.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.jinghuilouyu.cn/gtustumvnu.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.quarkkingdee.top/gtvmguunaf.html

================================================================================
来源：http://hz.ydjk.org.cn/gtwvdyiyax.html

G. 面向对象
来源：http://hz.hongshengwenyu.top/gthuardoxc.html

================================================================================
来源：http://hz.shuidangran.top/gtljihxnkj.html

[G01] 定义类
来源：http://hz.yangfankeji.com/gtdnytrrvb.html

Py:   class User: pass
来源：http://hz.mhx1999.top/gtevnudbzn.html

PHP:  class User {}
来源：http://hz.chenlongwang.top/gtybrpmhrt.html

JS:   class User {}
来源：http://hz.cqqwz.cn/gtzbluvzgv.html

TS:   class User { name: string = ""; }
来源：http://hz.yj20258.top/gtmdyuebyx.html

Java: class User {}
来源：http://hz.gzhubu.top/gtsgzcfxem.html

Go:   type User struct { Name string }
来源：http://hz.gotoacloud.top/gtkjjikwee.html

Ruby: class User; end
来源：http://hz.316326.xyz/gtaokfzjvy.html

C#:   class User {}
来源：http://hz.gzhubu.top/gtbcspzgim.html

[G02] 构造函数
来源：http://hz.kuanghao11.cn/gtyvoovquf.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.nanxuanxn.top/gtxwkhxuza.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.yvedp.cn/gtmsbgkfrl.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.aibaodan.cn/gtwtctkfdn.html

TS:   constructor(public name: string) {}
来源：http://hz.shangyingyoupin.top/gtxcjwmuxa.html

Java: User(String name) { this.name = name; }
来源：http://hz.zhoulong.xyz/gtccfegwda.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.vqdsnc.cn/gtrabhschz.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.kuanghao11.cn/gthyhuqvfa.html

C#:   public User(string name) { Name = name; }
来源：http://hz.zhongyouzk.top/gtcynmmams.html

[G03] 实例属性
来源：http://hz.snrcjt.cn/gtgepmifnw.html

Py:   self.name = "x"
来源：http://hz.zhoulong.xyz/gtnfxkyukm.html

PHP:  public string $name = "x";
来源：http://hz.jinghuilouyu.cn/gtvgilqzfo.html

JS:   this.name = "x";
来源：http://hz.jqgfzy.top/gtymsibexw.html

TS:   name: string = "x";
来源：http://hz.tianlin.xyz/gtibttmtfz.html

Java: private String name;
来源：http://hz.xuanzx.com/gtuiozjdmh.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.xingfuxueyuan.xyz/gtmekthhre.html

Ruby: @name = "x"
来源：http://hz.xziqi.cn/gtamlymxoo.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.xinyue.icu/gtxdskrqys.html

[G04] 定义方法
来源：http://hz.dianchejie.cn/gthddktaft.html

Py:   def greet(self): return self.name
来源：http://hz.zhengqikj.top/gtbocxmtkz.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.birdmap.top/gtkfmzivni.html

JS:   greet() { return this.name; }
来源：http://hz.meibo888.top/gtfqjqcuuv.html

TS:   greet(): string { return this.name; }
来源：http://hz.hfpthk.cn/gtdebqathx.html

Java: String greet() { return name; }
来源：http://hz.yvedp.cn/gtjstqsckf.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.aibaodan.cn/gttovbjxtw.html

Ruby: def greet; @name; end
来源：http://hz.cdnleiting.top/gtdouolocz.html

C#:   public string Greet() => Name;
来源：http://hz.sxryk.cn/gtbuzknqdv.html

[G05] 继承
来源：http://hz.smart0.xyz/gtfhlvypsm.html

Py:   class Admin(User): pass
来源：http://hz.cqqwz.cn/gtkilobiyj.html

PHP:  class Admin extends User {}
来源：http://hz.guannengcc.top/gtfjmmoihp.html

JS:   class Admin extends User {}
来源：http://hz.yanxiufei.cn/gtykvinmth.html

TS:   class Admin extends User {}
来源：http://hz.xinyue.icu/gtucyatgmf.html

Java: class Admin extends User {}
来源：http://hz.xuanzx.com/gtqucdfuno.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.chenjidiqi.icu/gtoligkqox.html

Ruby: class Admin < User; end
来源：http://hz.cqqwz.cn/gteriavpua.html

C#:   class Admin : User {}
来源：http://hz.xylfe.cn/gtvevbnvzl.html

[G06] 重写方法
来源：http://hz.smart0.xyz/gtmtulranz.html

Py:   def greet(self): return "admin"
来源：http://hz.jiagoushi.top/gtzzkkatxd.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.nwbrower.top/gtyazbysqe.html

JS:   greet() { return "admin"; }
来源：http://hz.yvedp.cn/gtrtsdxezo.html

TS:   greet(): string { return "admin"; }
来源：http://hz.gaohongyu789.top/gtqpviaqel.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.haohaochexian.top/gthilcnipq.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.shanyushiyangtech.top/gtedutbhzj.html

Ruby: def greet; "admin"; end
来源：http://hz.jyoumei.cn/gtldfrunfv.html

C#:   public override string Greet() => "admin";
来源：http://hz.birdmap.top/gtlhbrkley.html

[G07] 调用父类方法
来源：http://hz.tian-w.cn/gtlbkpcuxj.html

Py:   super().greet()
来源：http://hz.jinghuilouyu.cn/gtrxhqurwh.html

PHP:  parent::greet();
来源：http://hz.meibo888.top/gtvbzcrxct.html

JS:   super.greet();
来源：http://hz.haohaochexian.top/gtcwnxsnou.html

TS:   super.greet();
来源：http://hz.nanxuanxn.top/gtljsmgdbn.html

Java: super.greet();
来源：http://hz.pengpengdd.cyou/gtirlkwtvj.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.cashguo.top/gtisjhkqej.html

Ruby: super
来源：http://hz.zhoulong.xyz/gtjduyaevx.html

C#:   base.Greet();
来源：http://hz.svipenyu.cn/gtjpieqlgm.html

[G08] 静态方法与属性
来源：http://hz.nanxuanxn.top/gtkdlybnhd.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.shanyushiyangtech.top/gtsyegqegt.html

PHP:  public static function f() {}
来源：http://hz.cheryme.top/gtocmkibnh.html

JS:   static f() {}
来源：http://hz.316326.xyz/gtjuqxicpc.html

TS:   static f(): void {}
来源：http://hz.jianghu66.top/gtzkbqypsi.html

Java: static void f() {}
来源：http://hz.sysykeji.top/gtqyhhmtpc.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.chenjidiqi.icu/gtlrysoyir.html

Ruby: def self.f; end
来源：http://hz.svipenyu.cn/gttxehekpd.html

C#:   public static void F() {}
来源：http://hz.9152youxi.cn/gtrzswqckg.html

[G09] 接口 / 抽象类
来源：http://hz.yuanzhike.top/gtwtehhekm.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.hnxiangtu.top/gtwyqdohiu.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.dianchejie.cn/gtxatrueta.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.bjfxy.top/gthopdgpzz.html

TS:   interface Shape { area(): number; }
来源：http://hz.tianlin.xyz/gtmqkjgziw.html

Java: interface Shape { double area(); }
来源：http://hz.0kj1m.cn/gtalgxijdu.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.yuanzhike.top/gtcrjxzhlg.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.yj20258.top/gtfmlmsejs.html

C#:   interface IShape { double Area(); }
来源：http://hz.0kj1m.cn/gtfkjnvyyx.html

[G10] 访问控制
来源：http://hz.guowangkeji.top/gtkmoqviys.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.birdmap.top/gttjxkhtaq.html

PHP:  public / protected / private
来源：http://hz.guowangkeji.top/gtoynooxmp.html

JS:   #private 字段；其余公开
来源：http://hz.hywenlv.cn/gtsxyghzki.html

TS:   public / protected / private
来源：http://hz.jiagoushi.top/gthhiwhzca.html

Java: public / protected / private / 默认包级
来源：http://hz.nwbrower.top/gtmxipcczp.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.iojbl.cn/gtgmdgecag.html

Ruby: public / protected / private
来源：http://hz.meibo888.top/gtzfbqcujz.html

C#:   public / protected / private / internal
来源：http://hz.gotoacloud.top/gtmbozznuy.html

[G11] getter / setter
来源：http://hz.yj20258888.top/gtjrsyoofg.html

Py:   @property 与 @x.setter
来源：http://hz.zhixingplan.top/gtfpmvpgzn.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.yanxiufei.cn/gtlacroitd.html

JS:   get name() { return this._name; }
来源：http://hz.zycfv.cn/gtqdymddcv.html

TS:   get name(): string { return this._name; }
来源：http://hz.xuetiantiany.cn/gtaxchleqz.html

Java: public String getName() { return name; }
来源：http://hz.yj20258888.top/gtdqregumi.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.cheryme.top/gtvavvvame.html

Ruby: attr_accessor :name
来源：http://hz.ivvv.top/gtirykxcfo.html

C#:   public string Name { get; set; }
来源：http://hz.yonumen.top/gtwwejhvpw.html

[G12] 对象转字符串
来源：http://hz.316326.xyz/gtzbhbqwqn.html

Py:   def __str__(self): return self.name
来源：http://hz.zhoulong.xyz/gtnccdcdhe.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.pengpengdd.cyou/gttpdsdhca.html

JS:   toString() { return this.name; }
来源：http://hz.quarkkingdee.top/gtjwpbkzbm.html

TS:   toString(): string { return this.name; }
来源：http://hz.fzhhl.top/gtdtzjmobw.html

Java: @Override public String toString() { return name; }
来源：http://hz.fzhhl.top/gtozsqekbx.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.fengsongda.top/gtutvedqgp.html

Ruby: def to_s; @name; end
来源：http://hz.jqgufenzy.top/gttaemjgxj.html

C#:   public override string ToString() => Name;
来源：http://hz.xingfuxueyuan.xyz/gtryjwpure.html

[G13] 判断对象类型
来源：http://hz.c1oappe.top/gtclrtpjtq.html

Py:   isinstance(u, User)
来源：http://hz.snrcjt.cn/gtepuiddal.html

PHP:  $u instanceof User
来源：http://hz.shanyushiyangtech.top/gtfafgifwp.html

JS:   u instanceof User
来源：http://hz.zycfv.cn/gtasazsubt.html

TS:   u instanceof User
来源：http://hz.smart0.xyz/gtxafnwkhu.html

Java: u instanceof User
来源：http://hz.zhongyouzk.top/gtpuzeuryz.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.birdmap.top/gtqrikzjcw.html

Ruby: u.is_a?(User)
来源：http://hz.aizwys.cn/gtwusokqjh.html

C#:   u is User
来源：http://hz.haohaochexian.top/gtvfmlmigz.html

[G14] 数据类 / record
来源：http://hz.jinghuilouyu.cn/gtqfrfpiyd.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.gzhubu.top/gthwmbesal.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.zhijiandao.cn/gtetpsfvrb.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.meibo888.top/gtwazfikck.html

TS:   type User = { name: string; age: number };
来源：http://hz.shuidangran.top/gtwptzkefx.html

Java: record User(String name, int age) {}
来源：http://hz.haohaochexian.top/gtrhoduvga.html

Go:   type User struct { Name string; Age int }
来源：http://hz.jinqigfzy.top/gtompipotw.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.zhoulong.xyz/gtiqjztwuz.html

C#:   record User(string Name, int Age);
来源：http://hz.guannengcc.top/gtjxgjvyqf.html

[G15] 枚举
来源：http://hz.gogol.net.cn/gtpodtpcbi.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.yvedp.cn/gtdmefucsx.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.shanyushiyangkeji.top/gtdtzpbdam.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.jyoumei.cn/gticpzzwwe.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.shanyushiyangtech.top/gtsgsgweap.html

Java: enum Color { RED, GREEN }
来源：http://hz.hnqzz.top/gtrcswluqw.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.yj20258.top/gthldntxhj.html

Ruby: Color = %i[red green].freeze
来源：http://hz.wangdashe.top/gtwpxjjqmv.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.aibaodan.cn/gtvicvwhtc.html

[G16] 对象转数组 / 字典
来源：http://hz.ivvv.top/gtfppawjgj.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.bjfxy.top/gtqbqccmrg.html

PHP:  get_object_vars($obj);
来源：http://hz.sufxvd.cn/gtczksbycf.html

JS:   Object.entries(obj)
来源：http://hz.sufxvd.cn/gtwlqzvwdf.html

TS:   Object.entries(obj)
来源：http://hz.jlsjyb.cn/gtkzcaiscc.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.meibo888.top/gtbefhnvlf.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.sxryk.cn/gtwxbochvt.html

Ruby: obj.instance_variables
来源：http://hz.nwbrower.top/gtawqfhuvk.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.tian-w.cn/gtnhnzotjz.html

================================================================================
来源：http://hz.shzxlz.cn/gtxhimkmag.html

H. 异常与错误处理
来源：http://hz.shuidangran.top/gteoowsgpn.html

================================================================================
来源：http://hz.jinqigufen.top/gtbtnladhi.html

[H01] try / catch 基础
来源：http://hz.cqqwz.cn/gtexuvbbjs.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.hywenlv.cn/gtrkmmlnpk.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.ehwqpu.com/gtmbkioyon.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.fengsongda.top/gtpgwtumdp.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.hnxiangtu.top/gtbqrrifjl.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.jinyuanbaomall.cn/gtndhcaamw.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.yonumen.top/gtksczyctq.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.fzhhl.top/gtnulwhoeb.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.ehwqpu.com/gtkcjtergb.html

[H02] finally / ensure 收尾
来源：http://hz.guowangkeji.top/gthtlgwcpj.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.cheryme.top/gtnyjydech.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.pycfn.com/gtrmobthjv.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.hongshengwenyu.top/gtjwggridh.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.shzxlz.cn/gtsdigfbmy.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.xziqi.cn/gtypmxayui.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.snrcjt.cn/gtnbknyicc.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.yueranfly.top/gtchjwqrnf.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.chenzaomai.com/gthhphtfhf.html

[H03] 主动抛出异常
来源：http://hz.yj20258.top/gtihvrzaja.html

Py:   raise ValueError("错误信息")
来源：http://hz.ydjk.org.cn/gtlincigee.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.tianlin.xyz/gtsyldajsz.html

JS:   throw new Error("错误信息");
来源：http://hz.dashuyun.cn/gtqesqqcdn.html

TS:   throw new Error("错误信息");
来源：http://hz.andypj.xyz/gtrmzalevd.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.zhijiandao.cn/gtzgktzidr.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.fengsongda.top/gtpyagtkqb.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.cqqwz.cn/gtvliukvst.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.zhongyouzk.top/gtghijlrmw.html

[H04] 自定义异常类型
来源：http://hz.sweek.top/gtqfmenqvz.html

Py:   class MyError(Exception): pass
来源：http://hz.tanke756.top/gtjczoffma.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.sysykeji.top/gtpthjwgxz.html

JS:   class MyError extends Error {}
来源：http://hz.hywenlv.cn/gtnmijhaya.html

TS:   class MyError extends Error {}
来源：http://hz.redwolf501.top/gtqmwcfjco.html

Java: class MyException extends RuntimeException {}
来源：http://hz.jlsjyb.cn/gtzmajxzer.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.yueranfly.top/gtnoufapfr.html

Ruby: class MyError < StandardError; end
来源：http://hz.yuxming.cn/gtjjwofpnp.html

C#:   class MyException : Exception {}
来源：http://hz.hfpthk.cn/gtmvzdiamp.html

[H05] 捕获特定类型
来源：http://hz.xinyue.icu/gtlyeoxfzl.html

Py:   except ValueError as e:
来源：http://hz.yuxming.cn/gtezmxgvpn.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.zhiwuduotai.top/gtzhpfwnke.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.ydjk.org.cn/gtwxknenpp.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.shanyushiyangkeji.top/gtnbquijbt.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.jyoumei.cn/gtcndbciif.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.yuxming.cn/gtuxokdhuu.html

Ruby: rescue ArgumentError => e
来源：http://hz.hfpthk.cn/gtgiyuahia.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.hywenlv.cn/gtzazbotoq.html

[H06] 可选值 / 空值安全访问
来源：http://hz.dashuyun.cn/gtgvzqjzyq.html

Py:   value = d.get("k") or default
来源：http://hz.guowangkeji.top/gtwzhnfpxu.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.c1oappe.top/gtmrxmefqc.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.yuanzhike.top/gtqszcyzrc.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.havefunace.top/gthitgsght.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.pengpengdd.cyou/gtvmzfxeqg.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.pycfn.com/gtwcyozfdu.html

Ruby: d&.dig(:a, :b)
来源：http://hz.ehwqpu.com/gtkcupitag.html

C#:   obj?.A?.B ?? default
来源：http://hz.zhengqikj.top/gtdbdlefmn.html

[H07] 断言
来源：http://hz.sxryk.cn/gtftvunymp.html

Py:   assert x > 0, "必须为正"
来源：http://hz.jlsjyb.cn/gtivouhhpt.html

PHP:  assert($x > 0);
来源：http://hz.shanyushiyangtech.top/gttjlidzma.html

JS:   console.assert(x > 0);
来源：http://hz.yanxiufei.cn/gtkuouiizq.html

TS:   console.assert(x > 0);
来源：http://hz.daria6918.cn/gtquhzxsjq.html

Java: assert x > 0 : "必须为正";
来源：http://hz.xingfuxueyuan.xyz/gtdegtirco.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.xuanzx.com/gtmcmfkxpi.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.jqgfzy.top/gtfbqqqupx.html

C#:   Debug.Assert(x > 0);
来源：http://hz.xuetiantiany.cn/gtpmhkrhqa.html

[H08] 获取错误信息与堆栈
来源：http://hz.nwbrower.top/gtqzfbzxzh.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.sufxvd.cn/gtsufbqtqq.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.xuetiantiany.cn/gtqvakgltm.html

JS:   e.message;  e.stack
来源：http://hz.yuxming.cn/gtepmclybq.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.jinghuilouyu.cn/gtohtsrcse.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.jinqigfzy.top/gteojhfdas.html

Go:   err.Error()
来源：http://hz.tanke756.top/gtplpfktde.html

Ruby: e.message;  e.backtrace
来源：http://hz.sysykeji.top/gttovdhjnq.html

C#:   e.Message;  e.StackTrace
来源：http://hz.zhixingplan.top/gthrrrmbka.html

[H09] 带错误码的异常
来源：http://hz.hammf.cn/gtihskmbtc.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.cashguo.top/gtnphoxamw.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.shanyushiyangkeji.top/gtmyxwphpn.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.bjfxy.top/gtcqjlxvls.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.cqqwz.cn/gtxgbhfuzd.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.mhx1999.top/gtaiivxlao.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.xinyue.icu/gtsicghbgq.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.dashuyun.cn/gtbhuotgqo.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.sysykeji.top/gtcxpuogbc.html

[H10] 资源自动释放
来源：http://hz.zhaomingkeji.xyz/gtlrxztoij.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.ehwqpu.com/gtbqslbggk.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.tian-w.cn/gtgbpuysto.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.sxryk.cn/gtksujrogm.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.shangyingyoupin.top/gtbzgmgkhv.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.yuxming.cn/gtddhvtlts.html

Go:   defer f.Close()
来源：http://hz.chenzaomai.com/gtvdrmynov.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.hysaishi.cn/gturkynydv.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.jinghuilouyu.cn/gtbwshksfy.html

================================================================================
来源：http://hz.xylfe.cn/gtzzwdvjpf.html

I. 正则表达式
来源：http://hz.guannengcc.top/gtrcjuodzb.html

================================================================================
来源：http://hz.wangdashe.top/gtucrtznhz.html

[I01] 判断是否匹配
来源：http://hz.xuetiantiany.cn/gtvaogzfuo.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.gogol.net.cn/gtuequhlnp.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.cqqwz.cn/gtjvlsewts.html

JS:   /\d+/.test(s)
来源：http://hz.shuidangran.top/gtjcgriuex.html

TS:   /\d+/.test(s)
来源：http://hz.cucudq.cn/gtqlhjfurr.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.hywenlv.cn/gtqgippwzz.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.bjfxy.top/gtarrrfkcs.html

Ruby: s.match?(/\d+/)
来源：http://hz.jinqigufen.top/gtiaqowsop.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.daxiang520.top/gtkrptxubj.html

[I02] 提取所有匹配
来源：http://hz.yanxiufei.cn/gtczquellj.html

Py:   re.findall(r"\d+", s)
来源：http://hz.gzhubu.top/gteyanhrpx.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.tanke756.top/gtalqdsgic.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.iojbl.cn/gtuhinxenz.html

TS:   s.match(/\d+/g)
来源：http://hz.xinyue.icu/gtlyzgfeku.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.sufxvd.cn/gtuddkowxm.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.jqgufenzy.top/gtswlttjto.html

Ruby: s.scan(/\d+/)
来源：http://hz.tian-w.cn/gtgqllkajd.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.chenjidiqi.icu/gtnxfmelay.html

[I03] 提取捕获分组
来源：http://hz.zhongyouzk.top/gtqrpaazng.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.hfpthk.cn/gttkqzzmvh.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.yvedp.cn/gtgdtjqfga.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.zhijiandao.cn/gtcbzmpjrn.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.zhongyouzk.top/gtupqlzmpz.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.jinyuanbaomall.cn/gtokrhnrvy.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.yonumen.top/gtkfzbuwaa.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.gotoacloud.top/gtxypezlec.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.yuxming.cn/gtbxmckuvl.html

[I04] 正则替换
来源：http://hz.guowangkeji.top/gtsqkursgl.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.gaohongyu789.top/gtrjxfsceo.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.zhongyouzk.top/gtycacrsjr.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.bjfxy.top/gteuqcjhkh.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.andypj.xyz/gtnudirqjj.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.jinqigufen.top/gtytciukxm.html


<!-- 参考信息 -->