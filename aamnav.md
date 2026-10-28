代发 wailian999

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.jinyuanbaomall.cn/gtujfkldan.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.jianghu66.top/gtewizsmuh.html

[F11] 复制与移动文件
来源：http://hz.tanke756.top/gtziukskea.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.hysaishi.cn/gtpcyysxkz.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.c1oappe.top/gthatwjzym.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.yj20258.top/gtpazkhbwc.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.daxiang520.top/gtrouxitwf.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.zhengqikj.top/gtaqlebrbz.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.havefunace.top/gtstkrlicp.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.ydjk.org.cn/gtezkmpwgg.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.yuxming.cn/gtipdllmhr.html

[F12] CSV 读写
来源：http://hz.sxryk.cn/gtddzdfwnb.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.vqdsnc.cn/gtkgvbjdbu.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.ivvv.top/gtflquuiis.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.tanke756.top/gtusqrvjyg.html

TS:   // 同上
来源：http://hz.yangfankeji.com/gtiahomroh.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.birdmap.top/gtxkvmuebm.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.sufxvd.cn/gtuuysvalo.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.shanyushiyangkeji.top/gttdyygcrr.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.jqgfzy.top/gtuxqwydjp.html

================================================================================
来源：http://hz.ehwqpu.com/gtibbnbrql.html

G. 面向对象
来源：http://hz.yangfankeji.com/gtjlydnplq.html

================================================================================
来源：http://hz.ybcxt.top/gtsypxtirt.html

[G01] 定义类
来源：http://hz.daria6918.cn/gtnbzadhoj.html

Py:   class User: pass
来源：http://hz.zycfv.cn/gtzxhxmslr.html

PHP:  class User {}
来源：http://hz.yanxiufei.cn/gthiwyomlo.html

JS:   class User {}
来源：http://hz.quarkkingdee.top/gtsmxbszat.html

TS:   class User { name: string = ""; }
来源：http://hz.jinyuanbaomall.cn/gtmmimkjyj.html

Java: class User {}
来源：http://hz.yj20258888.top/gtvqmgdpxp.html

Go:   type User struct { Name string }
来源：http://hz.shuidangran.top/gtqacpzorq.html

Ruby: class User; end
来源：http://hz.chenlongwang.top/gtbogthsxk.html

C#:   class User {}
来源：http://hz.zhoulong.xyz/gtwhqwooah.html

[G02] 构造函数
来源：http://hz.chenzaomai.com/gtyobxopla.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.shzxlz.cn/gtjnlllvht.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.zycfv.cn/gtidobuhal.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.nanxinkj.top/gtjgibacmt.html

TS:   constructor(public name: string) {}
来源：http://hz.sweek.top/gtnuogxbzj.html

Java: User(String name) { this.name = name; }
来源：http://hz.tanke756.top/gtfcwyvgnz.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.yj202588.top/gtskdkjvyq.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.tanke756.top/gtuckhuydi.html

C#:   public User(string name) { Name = name; }
来源：http://hz.zhongyouzk.top/gtulebjxgg.html

[G03] 实例属性
来源：http://hz.zhixingplan.top/gthfsruafs.html

Py:   self.name = "x"
来源：http://hz.feifeiyinyue.top/gtqabgxmdh.html

PHP:  public string $name = "x";
来源：http://hz.ydjk.org.cn/gtlxkygvam.html

JS:   this.name = "x";
来源：http://hz.wangdashe.top/gticqvcirt.html

TS:   name: string = "x";
来源：http://hz.smart0.xyz/gtismnzpre.html

Java: private String name;
来源：http://hz.shangyingyoupin.top/gtuvvzaull.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.svipenyu.cn/gtccionytf.html

Ruby: @name = "x"
来源：http://hz.xuetiantiany.cn/gtlyjvqsqb.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.guannengcc.top/gtrmadlqdh.html

[G04] 定义方法
来源：http://hz.zhiwuduotai.top/gtdffsmpyo.html

Py:   def greet(self): return self.name
来源：http://hz.tianlin.xyz/gtxboxkwfr.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.ydjk.org.cn/gtqpsipryv.html

JS:   greet() { return this.name; }
来源：http://hz.meibo888.top/gtmtskrvky.html

TS:   greet(): string { return this.name; }
来源：http://hz.jianghu66.top/gtgwudkbxk.html

Java: String greet() { return name; }
来源：http://hz.yangfankeji.com/gtkpjzhchm.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.jinghuilouyu.cn/gtmrozvdnw.html

Ruby: def greet; @name; end
来源：http://hz.dianchejie.cn/gtwovuptuw.html

C#:   public string Greet() => Name;
来源：http://hz.iojbl.cn/gtzsjmyafj.html

[G05] 继承
来源：http://hz.ehwqpu.com/gtxpikcxvq.html

Py:   class Admin(User): pass
来源：http://hz.andypj.xyz/gtrwkispjv.html

PHP:  class Admin extends User {}
来源：http://hz.gzhubu.top/gtgnxcxuxg.html

JS:   class Admin extends User {}
来源：http://hz.yj20258.top/gtlhqpazdr.html

TS:   class Admin extends User {}
来源：http://hz.dianchejie.cn/gtjrwkfysq.html

Java: class Admin extends User {}
来源：http://hz.hfpthk.cn/gttogxwbik.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.andypj.xyz/gtcpfyqnwb.html

Ruby: class Admin < User; end
来源：http://hz.yongpay.top/gtysajjyxs.html

C#:   class Admin : User {}
来源：http://hz.snrcjt.cn/gtraxxquou.html

[G06] 重写方法
来源：http://hz.xziqi.cn/gtzmrhlmxz.html

Py:   def greet(self): return "admin"
来源：http://hz.zycfv.cn/gtndmpxfnb.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.zhixingplan.top/gtxqesaszi.html

JS:   greet() { return "admin"; }
来源：http://hz.ehwqpu.com/gtzidaaiwh.html

TS:   greet(): string { return "admin"; }
来源：http://hz.cqqwz.cn/gtshcrqnrh.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.zhengqikj.top/gtrnsuggmb.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.hammf.cn/gtmqzqplfu.html

Ruby: def greet; "admin"; end
来源：http://hz.sysykeji.top/gttzqacapf.html

C#:   public override string Greet() => "admin";
来源：http://hz.cucudq.cn/gtybfdnvvh.html

[G07] 调用父类方法
来源：http://hz.yj20258888.top/gtafhpknfm.html

Py:   super().greet()
来源：http://hz.aizwys.cn/gtstfbnpwr.html

PHP:  parent::greet();
来源：http://hz.hywenlv.cn/gtvtxnrazx.html

JS:   super.greet();
来源：http://hz.kuanghao11.cn/gtopsnfkjl.html

TS:   super.greet();
来源：http://hz.xuetiantiany.cn/gtdywahrqm.html

Java: super.greet();
来源：http://hz.guowangkeji.top/gtxmvbugro.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.jianghu66.top/gtkcanemce.html

Ruby: super
来源：http://hz.xylfe.cn/gtrrnuevwj.html

C#:   base.Greet();
来源：http://hz.cheryme.top/gtleizaemj.html

[G08] 静态方法与属性
来源：http://hz.sweek.top/gthnqabgjr.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.zycfv.cn/gtvwfvessz.html

PHP:  public static function f() {}
来源：http://hz.gotoacloud.top/gteemcgvyq.html

JS:   static f() {}
来源：http://hz.chenlongwang.top/gtctpbgkmf.html

TS:   static f(): void {}
来源：http://hz.zhoulong.xyz/gtydtydmfb.html

Java: static void f() {}
来源：http://hz.zdqjudy.top/gttdhknfmp.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.yuanzhike.top/gtpwlynruc.html

Ruby: def self.f; end
来源：http://hz.hysaishi.cn/gtsexiyjfz.html

C#:   public static void F() {}
来源：http://hz.cashguo.top/gtskbvccjg.html

[G09] 接口 / 抽象类
来源：http://hz.jyoumei.cn/gtcvrynljn.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.hywenlv.cn/gtzdjqkaws.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.smart0.xyz/gtogjpjjqa.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.ivvv.top/gtiniagbrp.html

TS:   interface Shape { area(): number; }
来源：http://hz.xylfe.cn/gtnbgvmwxm.html

Java: interface Shape { double area(); }
来源：http://hz.sweek.top/gtmqsepskm.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.hammf.cn/gtaoubetvi.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.pengpengdd.cyou/gtibrrcdnu.html

C#:   interface IShape { double Area(); }
来源：http://hz.zhiwuduotai.top/gttxzqiqve.html

[G10] 访问控制
来源：http://hz.redwolf501.top/gtcdmfzseg.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.chenzaomai.com/gtjwqgeact.html

PHP:  public / protected / private
来源：http://hz.haohaochexian.top/gtmyxihikp.html

JS:   #private 字段；其余公开
来源：http://hz.yj20258.top/gtygawihwj.html

TS:   public / protected / private
来源：http://hz.smart0.xyz/gtkcomqnnb.html

Java: public / protected / private / 默认包级
来源：http://hz.yongpay.top/gtzjzejeol.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.zhengqikj.top/gtbwvuptrb.html

Ruby: public / protected / private
来源：http://hz.hywenlv.cn/gtxvdxcehu.html

C#:   public / protected / private / internal
来源：http://hz.sysykeji.top/gtizidhkvz.html

[G11] getter / setter
来源：http://hz.pycfn.com/gtdoywievx.html

Py:   @property 与 @x.setter
来源：http://hz.fengsongda.top/gtccrylqrj.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.zdqjudy.top/gtlaiwtpcq.html

JS:   get name() { return this._name; }
来源：http://hz.guowangkeji.top/gtjckuzasb.html

TS:   get name(): string { return this._name; }
来源：http://hz.52xcode.cn/gtrouplkmz.html

Java: public String getName() { return name; }
来源：http://hz.xinyue.icu/gtxqvnoupz.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.fzhhl.top/gtfpglqsgi.html

Ruby: attr_accessor :name
来源：http://hz.ppjwa.cn/gtumdgrpio.html

C#:   public string Name { get; set; }
来源：http://hz.cashguo.top/gtycvuxiec.html

[G12] 对象转字符串
来源：http://hz.0kj1m.cn/gtclpxziiq.html

Py:   def __str__(self): return self.name
来源：http://hz.52xcode.cn/gtufvcwqvc.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.cdnleiting.top/gtmygmngph.html

JS:   toString() { return this.name; }
来源：http://hz.jiagoushi.top/gtkbxcexvp.html

TS:   toString(): string { return this.name; }
来源：http://hz.nanxuanxn.top/gtrcttdvix.html

Java: @Override public String toString() { return name; }
来源：http://hz.guannengcc.top/gtnxemupej.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.iojbl.cn/gtrcdiblkf.html

Ruby: def to_s; @name; end
来源：http://hz.c1oappe.top/gttbkdlpkx.html

C#:   public override string ToString() => Name;
来源：http://hz.cqqwz.cn/gtuozmftwc.html

[G13] 判断对象类型
来源：http://hz.jqgfzy.top/gtbnlqnpoc.html

Py:   isinstance(u, User)
来源：http://hz.shuidangran.top/gtkmwbocqo.html

PHP:  $u instanceof User
来源：http://hz.gzhubu.top/gtkecpdwvt.html

JS:   u instanceof User
来源：http://hz.ppjwa.cn/gtysnmtuwb.html

TS:   u instanceof User
来源：http://hz.xinyue.icu/gtvjjyjksk.html

Java: u instanceof User
来源：http://hz.316326.xyz/gtvymslxlj.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.iojbl.cn/gttceamkgh.html

Ruby: u.is_a?(User)
来源：http://hz.9152youxi.cn/gtgjwcjjts.html

C#:   u is User
来源：http://hz.zhongyouzk.top/gthrbjnkpm.html

[G14] 数据类 / record
来源：http://hz.havefunace.top/gtnqbmzahu.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.wangshuangyany.cn/gtxnizlstu.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.xziqi.cn/gtjdcqszei.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.birdmap.top/gthntmxnhf.html

TS:   type User = { name: string; age: number };
来源：http://hz.redwolf501.top/gtbwlaakup.html

Java: record User(String name, int age) {}
来源：http://hz.jiagoushi.top/gtjtnwttgy.html

Go:   type User struct { Name string; Age int }
来源：http://hz.nanxinkj.top/gtrztsngvf.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.gaohongyu789.top/gtueucphxr.html

C#:   record User(string Name, int Age);
来源：http://hz.zhoulong.xyz/gtzbunlyyf.html

[G15] 枚举
来源：http://hz.wangshuangyany.cn/gtnhpbngqs.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.tianlin.xyz/gtvtbuzpyx.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.xuanzx.com/gtazduiqhf.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.gaohongyu789.top/gtstclfxxd.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.shangyingyoupin.top/gthtispitk.html

Java: enum Color { RED, GREEN }
来源：http://hz.xinyue.icu/gtbfujmqgl.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.tianlin.xyz/gtbangvmyg.html

Ruby: Color = %i[red green].freeze
来源：http://hz.yj202588.top/gthjsdiefr.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.shanyushiyangtech.top/gtelblmiis.html

[G16] 对象转数组 / 字典
来源：http://hz.jyoumei.cn/gttpojcqzv.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.zhongyouzk.top/gticqqybpb.html

PHP:  get_object_vars($obj);
来源：http://hz.zhijiandao.cn/gtymttbbrk.html

JS:   Object.entries(obj)
来源：http://hz.ivvv.top/gthxcmabkg.html

TS:   Object.entries(obj)
来源：http://hz.yj20258.top/gtosfhbqdy.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.nanxuanxn.top/gtbqxuhuhb.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.fzhhl.top/gtdljvkutt.html

Ruby: obj.instance_variables
来源：http://hz.aibaodan.cn/gtvtxppxcm.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.hywenlv.cn/gtrdlbykcq.html

================================================================================
来源：http://hz.ehwqpu.com/gtksglubiu.html

H. 异常与错误处理
来源：http://hz.yj202588.top/gtaowzxjst.html

================================================================================
来源：http://hz.snrcjt.cn/gtwejktmrm.html

[H01] try / catch 基础
来源：http://hz.gotoacloud.top/gtetmszzoj.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.ydjk.org.cn/gtuvyfxgem.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.guannengcc.top/gtqpxwgvnl.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.dianchejie.cn/gtyvmjwmxr.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.jlsjyb.cn/gtaljumyog.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.gotoacloud.top/gtziqqxjtb.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.aizwys.cn/gtbjkfptrw.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.xylfe.cn/gtpyfgiwpl.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.xuetiantiany.cn/gtltfdvuol.html

[H02] finally / ensure 收尾
来源：http://hz.hnqzz.top/gtvuxmsxla.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.wangdashe.top/gtqepemfsz.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.cashguo.top/gtkqtadqeq.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.xziqi.cn/gtavcrmroi.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.redwolf501.top/gterremxag.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.pengpengdd.cyou/gtrsfpuznl.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.jqgfzy.top/gtbhhkdipq.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.sweek.top/gtltezsvkb.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.quarkkingdee.top/gtmzvbemty.html

[H03] 主动抛出异常
来源：http://hz.yuanzhike.top/gttnwfwuml.html

Py:   raise ValueError("错误信息")
来源：http://hz.xylfe.cn/gtkxdazmuv.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.haohaochexian.top/gtcglxqfvp.html

JS:   throw new Error("错误信息");
来源：http://hz.jlsjyb.cn/gtjtijnseo.html

TS:   throw new Error("错误信息");
来源：http://hz.cashguo.top/gtsjhmfjnv.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.shzxlz.cn/gterrkylpx.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.pengpengdd.cyou/gtklsuhsva.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.ydzc1.top/gtwptiziqs.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.ppjwa.cn/gtypblzlyl.html

[H04] 自定义异常类型
来源：http://hz.hammf.cn/gtqzzfwuat.html

Py:   class MyError(Exception): pass
来源：http://hz.cqqwz.cn/gtuwyrzlxa.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.mhx1999.top/gtfadlxhte.html

JS:   class MyError extends Error {}
来源：http://hz.daria6918.cn/gtidmevehl.html

TS:   class MyError extends Error {}
来源：http://hz.zhongyouzk.top/gtexncuhlf.html

Java: class MyException extends RuntimeException {}
来源：http://hz.xziqi.cn/gtmgspoabl.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.pengpengdd.cyou/gtftozngru.html

Ruby: class MyError < StandardError; end
来源：http://hz.jqgfzy.top/gtzxegbglw.html

C#:   class MyException : Exception {}
来源：http://hz.xuanzx.com/gtfaapvukt.html

[H05] 捕获特定类型
来源：http://hz.yueranfly.top/gtptrjenqo.html

Py:   except ValueError as e:
来源：http://hz.shanyushiyangkeji.top/gtwxzegcyj.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.ppjwa.cn/gtutzsohve.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.wangdashe.top/gtyfhnzryo.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.bjfxy.top/gtveskalzi.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.hfpthk.cn/gtjnisjnsn.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.jyoumei.cn/gtgbjflydc.html

Ruby: rescue ArgumentError => e
来源：http://hz.zhixingplan.top/gtxuwudhrn.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.sxryk.cn/gtjetjmqct.html

[H06] 可选值 / 空值安全访问
来源：http://hz.gzhubu.top/gtwiemvfqh.html

Py:   value = d.get("k") or default
来源：http://hz.smart0.xyz/gtydbwxvbj.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.316326.xyz/gtvuwrfhly.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.mhx1999.top/gtuqbmxrgt.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.aibaodan.cn/gtlijqejvw.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.tian-w.cn/gtlxfdzvdi.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.iojbl.cn/gtgfqwuysf.html

Ruby: d&.dig(:a, :b)
来源：http://hz.hongshengwenyu.top/gtcyyfxlvo.html

C#:   obj?.A?.B ?? default
来源：http://hz.zhengqikj.top/gtfxqehzad.html

[H07] 断言
来源：http://hz.aizwys.cn/gtqoinuxik.html

Py:   assert x > 0, "必须为正"
来源：http://hz.yangfankeji.com/gtwvrkirde.html

PHP:  assert($x > 0);
来源：http://hz.jiagoushi.top/gtauqjzewf.html

JS:   console.assert(x > 0);
来源：http://hz.smart0.xyz/gtvsyjwgsj.html

TS:   console.assert(x > 0);
来源：http://hz.jianghu66.top/gtjripsqwo.html

Java: assert x > 0 : "必须为正";
来源：http://hz.shanyushiyangtech.top/gtshwhnube.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.ybcxt.top/gtpnsimbbg.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.jqgfzy.top/gtfusfhfrk.html

C#:   Debug.Assert(x > 0);
来源：http://hz.nwbrower.top/gttxsdmxhp.html

[H08] 获取错误信息与堆栈
来源：http://hz.nwbrower.top/gtnsbuvort.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.nanxinkj.top/gtdsxsqblf.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.yonumen.top/gtdjfbdhvg.html

JS:   e.message;  e.stack
来源：http://hz.meibo888.top/gtzxpbobex.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.jiagoushi.top/gtcqbyooua.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.vqdsnc.cn/gtmiijyfwf.html

Go:   err.Error()
来源：http://hz.jinyuanbaomall.cn/gtanrodrqe.html

Ruby: e.message;  e.backtrace
来源：http://hz.zhaomingkeji.xyz/gtincehrvv.html

C#:   e.Message;  e.StackTrace
来源：http://hz.yangfankeji.com/gtvnwisksu.html

[H09] 带错误码的异常
来源：http://hz.cqqwz.cn/gtbstzeovn.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.jqgufenzy.top/gtlmcebgum.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.sysykeji.top/gthulzbxsd.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.hammf.cn/gtlioldawa.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.andypj.xyz/gtgzabypxw.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.xziqi.cn/gtwfheeklb.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.zdqjudy.top/gtjdhpjttv.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.cheryme.top/gthdpurmbi.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.jiagoushi.top/gtnubmvuid.html

[H10] 资源自动释放
来源：http://hz.yonumen.top/gtrngaujff.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.tanke756.top/gtbrvumkfm.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.jinqigfzy.top/gtzxtvxzhw.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.yanxiufei.cn/gtfxfopsdf.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.ivvv.top/gtkyqntfir.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.kuanghao11.cn/gtdcnuoprw.html

Go:   defer f.Close()
来源：http://hz.yvedp.cn/gtgflozucx.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.yonumen.top/gthtmydxbt.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.jinyuanbaomall.cn/gthoyflyie.html

================================================================================
来源：http://hz.cucudq.cn/gtncmshyew.html

I. 正则表达式
来源：http://hz.yueranfly.top/gtnjdpreyq.html

================================================================================
来源：http://hz.yj20258888.top/gtubvqoutz.html

[I01] 判断是否匹配
来源：http://hz.chenzaomai.com/gtbbpjaliv.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.meibo888.top/gtqebjcpxd.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.9152youxi.cn/gtxiqfzkbn.html

JS:   /\d+/.test(s)
来源：http://hz.ppjwa.cn/gtjsdrcrwx.html

TS:   /\d+/.test(s)
来源：http://hz.ivvv.top/gthpbpeunu.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.guowangkeji.top/gtkhkbjyfx.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.sysykeji.top/gtnspijuhx.html

Ruby: s.match?(/\d+/)
来源：http://hz.zhoulong.xyz/gtgkorvopv.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.yj202588.top/gtkjtevdwr.html

[I02] 提取所有匹配
来源：http://hz.yj202588.top/gtghsgeumj.html

Py:   re.findall(r"\d+", s)
来源：http://hz.aizwys.cn/gtxakesrnc.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.cdnleiting.top/gthyrbwhkh.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.zhiwuduotai.top/gtdevzgahp.html

TS:   s.match(/\d+/g)
来源：http://hz.hysaishi.cn/gthwgadfgk.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.hywenlv.cn/gtwvezaibu.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.feifeiyinyue.top/gtjjfpxhbj.html

Ruby: s.scan(/\d+/)
来源：http://hz.zycfv.cn/gtiqjnkpbb.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.zdqjudy.top/gtgmbtvufb.html

[I03] 提取捕获分组
来源：http://hz.bjfxy.top/gttigrxkaj.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.fzhhl.top/gtdzmfduzs.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.ywan-chungtsiang.top/gtwybuhcvi.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.hfpthk.cn/gtgoehvngc.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.jinghuilouyu.cn/gtrfrcxwww.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.sxryk.cn/gtyswqppvc.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.dianchejie.cn/gtgfygxkif.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.chenzaomai.com/gtrcofiwcu.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.jqgfzy.top/gtabveitcz.html

[I04] 正则替换
来源：http://hz.zhoulong.xyz/gtgeojfjxi.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.shangyingyoupin.top/gtvnvydncf.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.sxryk.cn/gtmxspozlo.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.cqqwz.cn/gtwmmwxagf.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.xuetiantiany.cn/gttzfrqbeu.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.dashuyun.cn/gtrutigyom.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.chenjidiqi.icu/gtkifpdodn.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.iojbl.cn/gtdogznnei.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.jianghu66.top/gtgkeslfzs.html

[I05] 按正则拆分
来源：http://hz.xuanzx.com/gtygkzrmop.html


<!-- 参考信息 -->