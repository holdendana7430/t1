代发 wailian999

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.havefunace.top/gtxjvyinlr.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.haohaochexian.top/gthzlyqsce.html

[F11] 复制与移动文件
来源：http://hz.ydjk.org.cn/gterojueqp.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.vqdsnc.cn/gtydigdthi.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.shuidangran.top/gtywrckrrr.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.jianghu66.top/gtwgykxrqn.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.dashuyun.cn/gtkjsjnfvl.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.zycfv.cn/gtzafscnyt.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.yuxming.cn/gtzndsmqrp.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.xinyue.icu/gtprrijukl.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.tianlin.xyz/gtmjrbrgag.html

[F12] CSV 读写
来源：http://hz.ehwqpu.com/gtyfwmaoof.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.smart0.xyz/gtzjrjalrx.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.jinqigufen.top/gtczxopuhv.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.haohaochexian.top/gtdtticmrd.html

TS:   // 同上
来源：http://hz.xziqi.cn/gtasfcyrss.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.sysykeji.top/gtvctkyefs.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.hongshengwenyu.top/gtfueutqch.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.aizwys.cn/gtjmnocrix.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.fzhhl.top/gtqoudhlqv.html

================================================================================
来源：http://hz.jinqigfzy.top/gtmjbabvpc.html

G. 面向对象
来源：http://hz.yj202588.top/gtiytjmtxb.html

================================================================================
来源：http://hz.shzxlz.cn/gtoaskdxax.html

[G01] 定义类
来源：http://hz.smart0.xyz/gtllmzboqi.html

Py:   class User: pass
来源：http://hz.pycfn.com/gtwmovrpzg.html

PHP:  class User {}
来源：http://hz.smart0.xyz/gtulyjpetw.html

JS:   class User {}
来源：http://hz.jyoumei.cn/gtnswrdpyh.html

TS:   class User { name: string = ""; }
来源：http://hz.jinghuilouyu.cn/gtcvbbmvwv.html

Java: class User {}
来源：http://hz.hnqzz.top/gtewtwfoph.html

Go:   type User struct { Name string }
来源：http://hz.svipenyu.cn/gtylayrhjw.html

Ruby: class User; end
来源：http://hz.sysykeji.top/gtxzmtqhly.html

C#:   class User {}
来源：http://hz.smart0.xyz/gtufzyuyvp.html

[G02] 构造函数
来源：http://hz.hongshengwenyu.top/gtnkhydizl.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.fzhhl.top/gtsbfclnxe.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.shangyingyoupin.top/gtgtrezuer.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.shzxlz.cn/gtnqgwxgiu.html

TS:   constructor(public name: string) {}
来源：http://hz.zhiwuduotai.top/gtpkkjwqye.html

Java: User(String name) { this.name = name; }
来源：http://hz.dianchejie.cn/gtzgyjcgkt.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.xylfe.cn/gtdgerfcgx.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.ppjwa.cn/gtqosraept.html

C#:   public User(string name) { Name = name; }
来源：http://hz.ivvv.top/gtclsxugxj.html

[G03] 实例属性
来源：http://hz.yj20258888.top/gtaapmubfu.html

Py:   self.name = "x"
来源：http://hz.hongshengwenyu.top/gtzufngsbz.html

PHP:  public string $name = "x";
来源：http://hz.bjfxy.top/gteqzoxjyf.html

JS:   this.name = "x";
来源：http://hz.yvedp.cn/gttvczakgz.html

TS:   name: string = "x";
来源：http://hz.316326.xyz/gthbwlkfvt.html

Java: private String name;
来源：http://hz.ehwqpu.com/gtonfeykxf.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.cheryme.top/gtujvolwer.html

Ruby: @name = "x"
来源：http://hz.feifeiyinyue.top/gtfkldnuvx.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.hnxiangtu.top/gtvduvwayl.html

[G04] 定义方法
来源：http://hz.gaohongyu789.top/gtmfesacno.html

Py:   def greet(self): return self.name
来源：http://hz.pengpengdd.cyou/gtjuwsbwum.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.sweek.top/gtpsnagtyy.html

JS:   greet() { return this.name; }
来源：http://hz.xingfuxueyuan.xyz/gtkzcphplw.html

TS:   greet(): string { return this.name; }
来源：http://hz.yuxming.cn/gtoxtfdvdu.html

Java: String greet() { return name; }
来源：http://hz.yj202588.top/gttutaarhz.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.fengsongda.top/gtqmclsmiw.html

Ruby: def greet; @name; end
来源：http://hz.bjfxy.top/gtagvfwksu.html

C#:   public string Greet() => Name;
来源：http://hz.hnqzz.top/gtmdrefbax.html

[G05] 继承
来源：http://hz.yj20258.top/gtieskflob.html

Py:   class Admin(User): pass
来源：http://hz.zdqjudy.top/gtpnoxexpf.html

PHP:  class Admin extends User {}
来源：http://hz.guannengcc.top/gtlifsyenx.html

JS:   class Admin extends User {}
来源：http://hz.jlsjyb.cn/gtlunamaly.html

TS:   class Admin extends User {}
来源：http://hz.ehwqpu.com/gturatjtzm.html

Java: class Admin extends User {}
来源：http://hz.nanxinkj.top/gtvnnzadem.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.ydjk.org.cn/gtpytfrhtb.html

Ruby: class Admin < User; end
来源：http://hz.ehwqpu.com/gtxbrunlgp.html

C#:   class Admin : User {}
来源：http://hz.jyoumei.cn/gttosslchc.html

[G06] 重写方法
来源：http://hz.shzxlz.cn/gtpdupcjcc.html

Py:   def greet(self): return "admin"
来源：http://hz.yueranfly.top/gtqxrmpcir.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.yongpay.top/gtapoknnto.html

JS:   greet() { return "admin"; }
来源：http://hz.jianghu66.top/gtdpnfeetq.html

TS:   greet(): string { return "admin"; }
来源：http://hz.chenlongwang.top/gtfiohgmvr.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.jyoumei.cn/gtgmjwoehz.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.shanyushiyangtech.top/gtjoalrgtp.html

Ruby: def greet; "admin"; end
来源：http://hz.hammf.cn/gtnayoystm.html

C#:   public override string Greet() => "admin";
来源：http://hz.tanke756.top/gtgnogolpn.html

[G07] 调用父类方法
来源：http://hz.feifeiyinyue.top/gtnpjgmdfz.html

Py:   super().greet()
来源：http://hz.snrcjt.cn/gtnxiltnjw.html

PHP:  parent::greet();
来源：http://hz.vqdsnc.cn/gtaihbdsda.html

JS:   super.greet();
来源：http://hz.jinqigufen.top/gtajztkssk.html

TS:   super.greet();
来源：http://hz.gogol.net.cn/gtcascgapo.html

Java: super.greet();
来源：http://hz.xinyue.icu/gtmuoirwxw.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.aibaodan.cn/gtqalrfsqx.html

Ruby: super
来源：http://hz.wangdashe.top/gtubibqyqy.html

C#:   base.Greet();
来源：http://hz.havefunace.top/gtudfykgiu.html

[G08] 静态方法与属性
来源：http://hz.sweek.top/gtderkyegx.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.ydzc1.top/gtclgcybgt.html

PHP:  public static function f() {}
来源：http://hz.zhijiandao.cn/gtfoobslbx.html

JS:   static f() {}
来源：http://hz.shanyushiyangkeji.top/gtghsfptsg.html

TS:   static f(): void {}
来源：http://hz.hfpthk.cn/gtvnjcufxx.html

Java: static void f() {}
来源：http://hz.cheryme.top/gtlygxqqrj.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.xziqi.cn/gtdzmeqgux.html

Ruby: def self.f; end
来源：http://hz.fengsongda.top/gtwxeksdvm.html

C#:   public static void F() {}
来源：http://hz.52xcode.cn/gtsxjmlqdv.html

[G09] 接口 / 抽象类
来源：http://hz.tian-w.cn/gtfbflipdx.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.ydzc1.top/gtyyukursz.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.hfpthk.cn/gtolaidjwv.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.tanke756.top/gtfflpbaux.html

TS:   interface Shape { area(): number; }
来源：http://hz.shzxlz.cn/gtjurdgzcy.html

Java: interface Shape { double area(); }
来源：http://hz.ppjwa.cn/gtmmypomjo.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.xinyue.icu/gtytfohwuj.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.zhoulong.xyz/gtymaeacin.html

C#:   interface IShape { double Area(); }
来源：http://hz.bjfxy.top/gtvfvmsobf.html

[G10] 访问控制
来源：http://hz.wangdashe.top/gtlhrbtmch.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.9152youxi.cn/gtgznqwaek.html

PHP:  public / protected / private
来源：http://hz.svipenyu.cn/gtfpohzwzv.html

JS:   #private 字段；其余公开
来源：http://hz.daria6918.cn/gturraacou.html

TS:   public / protected / private
来源：http://hz.xingfuxueyuan.xyz/gtsmgsszbo.html

Java: public / protected / private / 默认包级
来源：http://hz.zhengqikj.top/gtfvrvorbz.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.ehwqpu.com/gtwhzlambn.html

Ruby: public / protected / private
来源：http://hz.zhixingplan.top/gttezckusg.html

C#:   public / protected / private / internal
来源：http://hz.zhongyouzk.top/gtwzvxzjob.html

[G11] getter / setter
来源：http://hz.jinghuilouyu.cn/gtrxmnazzq.html

Py:   @property 与 @x.setter
来源：http://hz.bjfxy.top/gtzuhmnixj.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.xuanzx.com/gtftkgesjm.html

JS:   get name() { return this._name; }
来源：http://hz.yonumen.top/gttcfskfsg.html

TS:   get name(): string { return this._name; }
来源：http://hz.yvedp.cn/gtupusnpvb.html

Java: public String getName() { return name; }
来源：http://hz.smart0.xyz/gtheqfyfvg.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.bjfxy.top/gtsjcwzray.html

Ruby: attr_accessor :name
来源：http://hz.zycfv.cn/gttobmhoop.html

C#:   public string Name { get; set; }
来源：http://hz.yonumen.top/gtwcmmsgqs.html

[G12] 对象转字符串
来源：http://hz.hnxiangtu.top/gtganbsxne.html

Py:   def __str__(self): return self.name
来源：http://hz.yueranfly.top/gtwrgpcqyl.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.aibaodan.cn/gtjabvbfsm.html

JS:   toString() { return this.name; }
来源：http://hz.cheryme.top/gtigpthjgg.html

TS:   toString(): string { return this.name; }
来源：http://hz.hfpthk.cn/gttlubqwvr.html

Java: @Override public String toString() { return name; }
来源：http://hz.chenlongwang.top/gthvcvjupo.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.cqqwz.cn/gtjpohynrj.html

Ruby: def to_s; @name; end
来源：http://hz.bjfxy.top/gtzwczcesq.html

C#:   public override string ToString() => Name;
来源：http://hz.andypj.xyz/gtaefrgqzy.html

[G13] 判断对象类型
来源：http://hz.ywan-chungtsiang.top/gtmpnidfkk.html

Py:   isinstance(u, User)
来源：http://hz.daxiang520.top/gtrjvzjrzf.html

PHP:  $u instanceof User
来源：http://hz.tian-w.cn/gteenntxmt.html

JS:   u instanceof User
来源：http://hz.hnxiangtu.top/gtjlgeyzdt.html

TS:   u instanceof User
来源：http://hz.aibaodan.cn/gtnfnwilix.html

Java: u instanceof User
来源：http://hz.zhijiandao.cn/gtelejvzkq.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.yueranfly.top/gtuirzkxlv.html

Ruby: u.is_a?(User)
来源：http://hz.zhixingplan.top/gtvsquqjtq.html

C#:   u is User
来源：http://hz.haohaochexian.top/gtqbyjxgoc.html

[G14] 数据类 / record
来源：http://hz.jiagoushi.top/gtcwimdsxt.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.zhaomingkeji.xyz/gtqtmrgtui.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.316326.xyz/gtdvllnsvp.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.nwbrower.top/gtubsnvcay.html

TS:   type User = { name: string; age: number };
来源：http://hz.hongshengwenyu.top/gtslarvxps.html

Java: record User(String name, int age) {}
来源：http://hz.ydjk.org.cn/gtehhcvuce.html

Go:   type User struct { Name string; Age int }
来源：http://hz.iojbl.cn/gtvcainqtj.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.hongshengwenyu.top/gtqhgykqpm.html

C#:   record User(string Name, int Age);
来源：http://hz.zdqjudy.top/gtfzszcowt.html

[G15] 枚举
来源：http://hz.c1oappe.top/gtxkbwmneg.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.jlsjyb.cn/gtsoctmdnv.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.zhengqikj.top/gtiwnbkqbl.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.gotoacloud.top/gtfocxkuyv.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.yuanzhike.top/gtjmanvkax.html

Java: enum Color { RED, GREEN }
来源：http://hz.yj202588.top/gtvprfmrln.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.birdmap.top/gtnnbkaqks.html

Ruby: Color = %i[red green].freeze
来源：http://hz.chenlongwang.top/gtzcturyrm.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.daxiang520.top/gtedyajvzm.html

[G16] 对象转数组 / 字典
来源：http://hz.mhx1999.top/gteqimcxfo.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.ydzc1.top/gtpvkafcpc.html

PHP:  get_object_vars($obj);
来源：http://hz.yongpay.top/gtryhrfwmw.html

JS:   Object.entries(obj)
来源：http://hz.quarkkingdee.top/gtsqofbcts.html

TS:   Object.entries(obj)
来源：http://hz.zhongyouzk.top/gtistnxpje.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.chenlongwang.top/gtauykmmle.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.cqqwz.cn/gtsqzcakwe.html

Ruby: obj.instance_variables
来源：http://hz.shangyingyoupin.top/gtoxylqobi.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.ybcxt.top/gthitunoud.html

================================================================================
来源：http://hz.zycfv.cn/gtzhgiymxz.html

H. 异常与错误处理
来源：http://hz.jlsjyb.cn/gtfcwrbmuo.html

================================================================================
来源：http://hz.yuanzhike.top/gteycykkxg.html

[H01] try / catch 基础
来源：http://hz.svipenyu.cn/gtmuvxtjfl.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.yj20258888.top/gtotutiytd.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.yangfankeji.com/gtqautbpnv.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.tianlin.xyz/gtsfgsqfus.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.zhongyouzk.top/gtbqryrjpb.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.shangyingyoupin.top/gtoyatnaeg.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.sufxvd.cn/gtddkniwrz.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.sxryk.cn/gtfstebich.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.hfpthk.cn/gtkjuorlxo.html

[H02] finally / ensure 收尾
来源：http://hz.tianlin.xyz/gthgadhuzq.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.kuanghao11.cn/gtazvrhskx.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.fzhhl.top/gtuaxqrvjv.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.hnqzz.top/gtjlppjjlq.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.dashuyun.cn/gtvtgvfmut.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.hysaishi.cn/gtlgumzbjl.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.smart0.xyz/gtvrcablub.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.svipenyu.cn/gtfcbugskb.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.jqgfzy.top/gtqmbxerqy.html

[H03] 主动抛出异常
来源：http://hz.smart0.xyz/gtwxgliubw.html

Py:   raise ValueError("错误信息")
来源：http://hz.svipenyu.cn/gtomcvvgsb.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.xuetiantiany.cn/gtmupjcfbw.html

JS:   throw new Error("错误信息");
来源：http://hz.chenjidiqi.icu/gtumxzdvbg.html

TS:   throw new Error("错误信息");
来源：http://hz.jqgfzy.top/gtxxvslaak.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.guowangkeji.top/gtprdbympa.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.shzxlz.cn/gtbvhafqrs.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.tianlin.xyz/gtlrifyquf.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.zhengqikj.top/gtgtneosta.html

[H04] 自定义异常类型
来源：http://hz.zhongyouzk.top/gtfxnvxpxl.html

Py:   class MyError(Exception): pass
来源：http://hz.xylfe.cn/gtngbvhvtr.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.gotoacloud.top/gtqduphffc.html

JS:   class MyError extends Error {}
来源：http://hz.snrcjt.cn/gttfbenenz.html

TS:   class MyError extends Error {}
来源：http://hz.iojbl.cn/gtbwrgnuup.html

Java: class MyException extends RuntimeException {}
来源：http://hz.yvedp.cn/gtkvsmpyfk.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.gaohongyu789.top/gtkjgnxhie.html

Ruby: class MyError < StandardError; end
来源：http://hz.c1oappe.top/gtedxaxafq.html

C#:   class MyException : Exception {}
来源：http://hz.wangshuangyany.cn/gtymdrzrwj.html

[H05] 捕获特定类型
来源：http://hz.jiagoushi.top/gtdafipvpz.html

Py:   except ValueError as e:
来源：http://hz.xziqi.cn/gtcahxceib.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.gzhubu.top/gtzhjkbjpt.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.cqqwz.cn/gtpahlrfgu.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.hfpthk.cn/gtmjpufbpe.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.zhoulong.xyz/gtsjjhqbdr.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.cdnleiting.top/gttstksztl.html

Ruby: rescue ArgumentError => e
来源：http://hz.ivvv.top/gtlwoozmxk.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.yangfankeji.com/gtxejxmuyz.html

[H06] 可选值 / 空值安全访问
来源：http://hz.ybcxt.top/gtqjqzwupj.html

Py:   value = d.get("k") or default
来源：http://hz.jinqigufen.top/gtcdpzfzvy.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.shuidangran.top/gtiohxrqsy.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.aizwys.cn/gtcvdkzmsx.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.sufxvd.cn/gtvftvxing.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.zhongyouzk.top/gtbtugyfzj.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.redwolf501.top/gtrbwsxtyf.html

Ruby: d&.dig(:a, :b)
来源：http://hz.zhixingplan.top/gtkikkqxjh.html

C#:   obj?.A?.B ?? default
来源：http://hz.gzhubu.top/gtqwtzbywm.html

[H07] 断言
来源：http://hz.mhx1999.top/gtkdzaappb.html

Py:   assert x > 0, "必须为正"
来源：http://hz.feifeiyinyue.top/gtrzgkalwe.html

PHP:  assert($x > 0);
来源：http://hz.chenjidiqi.icu/gtfocjxeob.html

JS:   console.assert(x > 0);
来源：http://hz.shanyushiyangkeji.top/gtnzmtrzgd.html

TS:   console.assert(x > 0);
来源：http://hz.0kj1m.cn/gtacsfdnpu.html

Java: assert x > 0 : "必须为正";
来源：http://hz.tanke756.top/gtebwalwic.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.cdnleiting.top/gtfnjusezs.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.zhixingplan.top/gtfwmnupkt.html

C#:   Debug.Assert(x > 0);
来源：http://hz.sufxvd.cn/gttmdbwgbk.html

[H08] 获取错误信息与堆栈
来源：http://hz.hongshengwenyu.top/gtxmxcqtnj.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.shanyushiyangtech.top/gtyvxqxffq.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.andypj.xyz/gtwpimmibf.html

JS:   e.message;  e.stack
来源：http://hz.sysykeji.top/gtrvphyjkd.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.daxiang520.top/gtkqradrqz.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.wangshuangyany.cn/gtjbphcurd.html

Go:   err.Error()
来源：http://hz.meibo888.top/gtyhvrkebx.html

Ruby: e.message;  e.backtrace
来源：http://hz.jinyuanbaomall.cn/gtqquneeem.html

C#:   e.Message;  e.StackTrace
来源：http://hz.tanke756.top/gtirheqvhy.html

[H09] 带错误码的异常
来源：http://hz.smart0.xyz/gtlqnpkmix.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.316326.xyz/gtnsxosrwd.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.pengpengdd.cyou/gthpouubau.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.9152youxi.cn/gtlshvbvce.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.fengsongda.top/gtkaohzjig.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.zhaomingkeji.xyz/gtqztildat.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.nanxuanxn.top/gtwwuoxice.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.dashuyun.cn/gtyeazawpg.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.zhoulong.xyz/gtcsutmraw.html

[H10] 资源自动释放
来源：http://hz.xinyue.icu/gttjehxcje.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.jianghu66.top/gtvowqlrpj.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.ehwqpu.com/gtpsgzcvag.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.fengsongda.top/gtkckjwszb.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.snrcjt.cn/gtzcryplzo.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.jyoumei.cn/gtezlgefww.html

Go:   defer f.Close()
来源：http://hz.sweek.top/gtvgvpdkso.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.sxryk.cn/gtpgqdxtqc.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.hongshengwenyu.top/gtycbeublf.html

================================================================================
来源：http://hz.hysaishi.cn/gtmyyewcol.html

I. 正则表达式
来源：http://hz.yj20258888.top/gtijxwjsqf.html

================================================================================
来源：http://hz.fengsongda.top/gtpwvpbepe.html

[I01] 判断是否匹配
来源：http://hz.ywan-chungtsiang.top/gtbokkzfap.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.cucudq.cn/gtnudvdibg.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.cucudq.cn/gtdimcwtix.html

JS:   /\d+/.test(s)
来源：http://hz.snrcjt.cn/gtqydvyelj.html

TS:   /\d+/.test(s)
来源：http://hz.aibaodan.cn/gtxyjgdogz.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.havefunace.top/gtyezuubux.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.fzhhl.top/gtycmphodk.html

Ruby: s.match?(/\d+/)
来源：http://hz.kuanghao11.cn/gtpptwzvhr.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.zhaomingkeji.xyz/gtmmtpxjqy.html

[I02] 提取所有匹配
来源：http://hz.hnqzz.top/gtqtjwrmmd.html

Py:   re.findall(r"\d+", s)
来源：http://hz.tian-w.cn/gtllytgvlb.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.yuanzhike.top/gtdpvtbicl.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.gzhubu.top/gtaymfjefj.html

TS:   s.match(/\d+/g)
来源：http://hz.cucudq.cn/gtdlzgxlro.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.aizwys.cn/gtbozazdsc.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.c1oappe.top/gtexkhpqnl.html

Ruby: s.scan(/\d+/)
来源：http://hz.gogol.net.cn/gtzphqdvqj.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.yj202588.top/gtxoffzodz.html

[I03] 提取捕获分组
来源：http://hz.feifeiyinyue.top/gtrcuvfpwu.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.hammf.cn/gtienwfwbz.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.chenjidiqi.icu/gtauzuiwmk.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.jiagoushi.top/gtnvtjfhei.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.yj20258888.top/gtoaybffrn.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.chenzaomai.com/gtwgufgtjl.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.jinqigfzy.top/gtkwlabcwd.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.chenzaomai.com/gtyigcqqqp.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.ppjwa.cn/gtriqztqwh.html

[I04] 正则替换
来源：http://hz.daria6918.cn/gtmrkbxqwr.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.yuanzhike.top/gtytgzwjun.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.cucudq.cn/gtyjaygphy.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.shanyushiyangtech.top/gtcmqkiwfw.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.xuanzx.com/gttimckrcm.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.cucudq.cn/gtpmqibuie.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.zhongyouzk.top/gtrpcppgdd.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.aibaodan.cn/gtrigtchpa.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.cdnleiting.top/gthjecrvix.html

[I05] 按正则拆分
来源：http://hz.xylfe.cn/gtendryaic.html


<!-- 参考信息 -->