代发 wailian999

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.chenjidiqi.icu/gtxsftumks.html

TS:   path.extname("a.txt")
来源：http://hz.xziqi.cn/gtpkvikabk.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.iojbl.cn/gtekvgakdq.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.hnxiangtu.top/gtghmpbawd.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.hywenlv.cn/gtbrndprob.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.feifeiyinyue.top/gtmuqlcytd.html

[F11] 复制与移动文件
来源：http://hz.hnqzz.top/gtamzpncbl.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.yanxiufei.cn/gttwswdoix.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.yvedp.cn/gtomtzxoer.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.316326.xyz/gtkagwtbzt.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.yongpay.top/gtzsnfnrov.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.yonumen.top/gtazmmxsky.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.xuanzx.com/gtxgkmezod.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.gzhubu.top/gtfjwduiad.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.zhixingplan.top/gtodknxmfl.html

[F12] CSV 读写
来源：http://hz.yj20258888.top/gtjnqepocb.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.andypj.xyz/gtfhgukicx.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.wangdashe.top/gtonbwultx.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.ywan-chungtsiang.top/gteijapuqe.html

TS:   // 同上
来源：http://hz.zycfv.cn/gtpdirqsgc.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.nanxinkj.top/gtqsrpjhyn.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.jinqigufen.top/gtnunvkpzc.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.daria6918.cn/gthhixedwh.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.svipenyu.cn/gtquexjmmp.html

================================================================================
来源：http://hz.gzhubu.top/gtiykyazlj.html

G. 面向对象
来源：http://hz.zhiwuduotai.top/gtcjvhvafp.html

================================================================================
来源：http://hz.dianchejie.cn/gtmodmfmjz.html

[G01] 定义类
来源：http://hz.yangfankeji.com/gtlgkcjiax.html

Py:   class User: pass
来源：http://hz.yanxiufei.cn/gtzyqrtrrv.html

PHP:  class User {}
来源：http://hz.yongpay.top/gtksyydcqc.html

JS:   class User {}
来源：http://hz.hysaishi.cn/gtowmnytjl.html

TS:   class User { name: string = ""; }
来源：http://hz.gotoacloud.top/gtycrmkplc.html

Java: class User {}
来源：http://hz.xuetiantiany.cn/gtiwqcistx.html

Go:   type User struct { Name string }
来源：http://hz.hammf.cn/gtehzkhylk.html

Ruby: class User; end
来源：http://hz.cqqwz.cn/gtpumtajem.html

C#:   class User {}
来源：http://hz.snrcjt.cn/gtufrnexhn.html

[G02] 构造函数
来源：http://hz.hysaishi.cn/gteoilkqnp.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.smart0.xyz/gtvuxqncqy.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.yuxming.cn/gtfwbsednh.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.feifeiyinyue.top/gtxfmieehn.html

TS:   constructor(public name: string) {}
来源：http://hz.guowangkeji.top/gttpphdklc.html

Java: User(String name) { this.name = name; }
来源：http://hz.guowangkeji.top/gtdtqqcwhd.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.cheryme.top/gthqyvdjyd.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.52xcode.cn/gtuvvzzgve.html

C#:   public User(string name) { Name = name; }
来源：http://hz.mhx1999.top/gtxsvywldu.html

[G03] 实例属性
来源：http://hz.ivvv.top/gtzhchmyql.html

Py:   self.name = "x"
来源：http://hz.xuanzx.com/gtqdofgvzd.html

PHP:  public string $name = "x";
来源：http://hz.xinyue.icu/gtspmehzkn.html

JS:   this.name = "x";
来源：http://hz.feifeiyinyue.top/gtsxscdzhw.html

TS:   name: string = "x";
来源：http://hz.zhixingplan.top/gtwtdkcjib.html

Java: private String name;
来源：http://hz.shanyushiyangkeji.top/gtrvmcxhie.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.hywenlv.cn/gthzlrojmg.html

Ruby: @name = "x"
来源：http://hz.xuetiantiany.cn/gtdepaawtx.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.nwbrower.top/gtxrjwztfe.html

[G04] 定义方法
来源：http://hz.hongshengwenyu.top/gtptzirghd.html

Py:   def greet(self): return self.name
来源：http://hz.shuidangran.top/gtssuypmun.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.andypj.xyz/gtdyqgcekj.html

JS:   greet() { return this.name; }
来源：http://hz.shanyushiyangkeji.top/gtvzgwmdxk.html

TS:   greet(): string { return this.name; }
来源：http://hz.cucudq.cn/gtnnhlfnot.html

Java: String greet() { return name; }
来源：http://hz.bjfxy.top/gtbgqexhel.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.xuetiantiany.cn/gtcjkftsgr.html

Ruby: def greet; @name; end
来源：http://hz.jqgufenzy.top/gtvypbgndf.html

C#:   public string Greet() => Name;
来源：http://hz.ywan-chungtsiang.top/gtbxvxzbrv.html

[G05] 继承
来源：http://hz.redwolf501.top/gtilsdctoj.html

Py:   class Admin(User): pass
来源：http://hz.birdmap.top/gthrbbnvhq.html

PHP:  class Admin extends User {}
来源：http://hz.nanxuanxn.top/gtchqhjtcu.html

JS:   class Admin extends User {}
来源：http://hz.hammf.cn/gtosfgaaeo.html

TS:   class Admin extends User {}
来源：http://hz.hnxiangtu.top/gtqfarqdtt.html

Java: class Admin extends User {}
来源：http://hz.jinqigufen.top/gtzqjafzxr.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.wangshuangyany.cn/gtqcshalbd.html

Ruby: class Admin < User; end
来源：http://hz.ppjwa.cn/gtiueysyxk.html

C#:   class Admin : User {}
来源：http://hz.iojbl.cn/gtzcxkfbua.html

[G06] 重写方法
来源：http://hz.xziqi.cn/gttuasgyst.html

Py:   def greet(self): return "admin"
来源：http://hz.nanxuanxn.top/gthmwoksxt.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.shanyushiyangkeji.top/gtzbqvansy.html

JS:   greet() { return "admin"; }
来源：http://hz.vqdsnc.cn/gttyttlbqs.html

TS:   greet(): string { return "admin"; }
来源：http://hz.snrcjt.cn/gtqxnuvinp.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.jqgfzy.top/gtkhprecpj.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.yangfankeji.com/gtoqnipkbu.html

Ruby: def greet; "admin"; end
来源：http://hz.sweek.top/gtxzkexgps.html

C#:   public override string Greet() => "admin";
来源：http://hz.hammf.cn/gtbtyetumo.html

[G07] 调用父类方法
来源：http://hz.havefunace.top/gtuaylfeyq.html

Py:   super().greet()
来源：http://hz.nanxuanxn.top/gtulnxobci.html

PHP:  parent::greet();
来源：http://hz.yongpay.top/gtreoutifa.html

JS:   super.greet();
来源：http://hz.316326.xyz/gtingualah.html

TS:   super.greet();
来源：http://hz.yvedp.cn/gtkahrlujt.html

Java: super.greet();
来源：http://hz.cheryme.top/gtsucwfecn.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.yanxiufei.cn/gtomyghweq.html

Ruby: super
来源：http://hz.yuanzhike.top/gtedzszdnt.html

C#:   base.Greet();
来源：http://hz.daxiang520.top/gtbroejoqa.html

[G08] 静态方法与属性
来源：http://hz.jqgfzy.top/gtrhcfesip.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.nwbrower.top/gtusrkttwy.html

PHP:  public static function f() {}
来源：http://hz.cdnleiting.top/gtoesenjvp.html

JS:   static f() {}
来源：http://hz.haohaochexian.top/gtzftthnlx.html

TS:   static f(): void {}
来源：http://hz.hysaishi.cn/gtczbcnxds.html

Java: static void f() {}
来源：http://hz.chenjidiqi.icu/gtlgslxqdp.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.gotoacloud.top/gteivkcqag.html

Ruby: def self.f; end
来源：http://hz.havefunace.top/gtmikholqn.html

C#:   public static void F() {}
来源：http://hz.zhongyouzk.top/gtevhnfvef.html

[G09] 接口 / 抽象类
来源：http://hz.pengpengdd.cyou/gtnoixfagj.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.yvedp.cn/gtqacxmqhb.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.cqqwz.cn/gtrzbvjqnz.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.0kj1m.cn/gtaxlaildm.html

TS:   interface Shape { area(): number; }
来源：http://hz.zhixingplan.top/gtemwalalz.html

Java: interface Shape { double area(); }
来源：http://hz.c1oappe.top/gtsvaaqvpe.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.hywenlv.cn/gtvfttokhm.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.xuetiantiany.cn/gtutczorcu.html

C#:   interface IShape { double Area(); }
来源：http://hz.pycfn.com/gtztjgtwss.html

[G10] 访问控制
来源：http://hz.zhijiandao.cn/gtegidozrg.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.cashguo.top/gtuukfiusr.html

PHP:  public / protected / private
来源：http://hz.yueranfly.top/gtlmepirdi.html

JS:   #private 字段；其余公开
来源：http://hz.zhaomingkeji.xyz/gtbtwuvsni.html

TS:   public / protected / private
来源：http://hz.zhaomingkeji.xyz/gtdhahmuzb.html

Java: public / protected / private / 默认包级
来源：http://hz.zhengqikj.top/gteqxqbfzr.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.ivvv.top/gtvnjvxggm.html

Ruby: public / protected / private
来源：http://hz.xylfe.cn/gttfmlixqo.html

C#:   public / protected / private / internal
来源：http://hz.jiagoushi.top/gtgogdvudr.html

[G11] getter / setter
来源：http://hz.hammf.cn/gtvxlcqfsi.html

Py:   @property 与 @x.setter
来源：http://hz.c1oappe.top/gtfcllrvbb.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.zhaomingkeji.xyz/gtqrivoeix.html

JS:   get name() { return this._name; }
来源：http://hz.cashguo.top/gtpvdyqvqs.html

TS:   get name(): string { return this._name; }
来源：http://hz.sweek.top/gtxamdoyjy.html

Java: public String getName() { return name; }
来源：http://hz.gotoacloud.top/gtncroltxy.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.pengpengdd.cyou/gthjwetoru.html

Ruby: attr_accessor :name
来源：http://hz.chenjidiqi.icu/gtcvwrdtbp.html

C#:   public string Name { get; set; }
来源：http://hz.feifeiyinyue.top/gtysppgrnd.html

[G12] 对象转字符串
来源：http://hz.hfpthk.cn/gtzwnqwqje.html

Py:   def __str__(self): return self.name
来源：http://hz.cqqwz.cn/gtconvgodk.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.nwbrower.top/gtjnqveudv.html

JS:   toString() { return this.name; }
来源：http://hz.316326.xyz/gtmtwchjmy.html

TS:   toString(): string { return this.name; }
来源：http://hz.redwolf501.top/gtputdbqvs.html

Java: @Override public String toString() { return name; }
来源：http://hz.yangfankeji.com/gtddmxetbp.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.yj20258.top/gtndkowcac.html

Ruby: def to_s; @name; end
来源：http://hz.nwbrower.top/gtizpmxfbw.html

C#:   public override string ToString() => Name;
来源：http://hz.fzhhl.top/gthnhpkyiy.html

[G13] 判断对象类型
来源：http://hz.shzxlz.cn/gtpuhdcubt.html

Py:   isinstance(u, User)
来源：http://hz.jqgufenzy.top/gtkntcqxth.html

PHP:  $u instanceof User
来源：http://hz.ybcxt.top/gtkfyjpnso.html

JS:   u instanceof User
来源：http://hz.xylfe.cn/gtshebwheh.html

TS:   u instanceof User
来源：http://hz.tian-w.cn/gtmguhdhmc.html

Java: u instanceof User
来源：http://hz.chenjidiqi.icu/gtozagashz.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.jinyuanbaomall.cn/gtzbablgun.html

Ruby: u.is_a?(User)
来源：http://hz.jyoumei.cn/gtuerbshvv.html

C#:   u is User
来源：http://hz.dianchejie.cn/gtszvefiry.html

[G14] 数据类 / record
来源：http://hz.chenjidiqi.icu/gtbyyymmul.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.cheryme.top/gtskshwyfj.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.fzhhl.top/gtcmqaoond.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.zhoulong.xyz/gtlyfesktp.html

TS:   type User = { name: string; age: number };
来源：http://hz.tianlin.xyz/gttgvirlei.html

Java: record User(String name, int age) {}
来源：http://hz.jqgfzy.top/gtjsnicsjn.html

Go:   type User struct { Name string; Age int }
来源：http://hz.meibo888.top/gtbbadlipv.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.gotoacloud.top/gtktdwglal.html

C#:   record User(string Name, int Age);
来源：http://hz.sxryk.cn/gtawdwuwdk.html

[G15] 枚举
来源：http://hz.ydzc1.top/gtzoxrylip.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.nanxinkj.top/gtdcixdhop.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.chenzaomai.com/gtvtdcqrsd.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.yanxiufei.cn/gtgwlsujny.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.9152youxi.cn/gtbbplchme.html

Java: enum Color { RED, GREEN }
来源：http://hz.nanxinkj.top/gtepvfqoqo.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.chenzaomai.com/gtagqqizax.html

Ruby: Color = %i[red green].freeze
来源：http://hz.hnxiangtu.top/gtacywnnkz.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.gzhubu.top/gtiptyekfz.html

[G16] 对象转数组 / 字典
来源：http://hz.zhixingplan.top/gtmumzszni.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.tianlin.xyz/gtagqvxuqd.html

PHP:  get_object_vars($obj);
来源：http://hz.xylfe.cn/gtjllypldj.html

JS:   Object.entries(obj)
来源：http://hz.fengsongda.top/gtdjnxuuia.html

TS:   Object.entries(obj)
来源：http://hz.chenzaomai.com/gtoqztrsih.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.yangfankeji.com/gtbbnzdeic.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.daria6918.cn/gttwzkzuvv.html

Ruby: obj.instance_variables
来源：http://hz.xingfuxueyuan.xyz/gteoqzhcus.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.yuanzhike.top/gtelppjgck.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtfaranrui.html

H. 异常与错误处理
来源：http://hz.smart0.xyz/gtntxcuuil.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtkqesrtvw.html

[H01] try / catch 基础
来源：http://hz.haohaochexian.top/gtqvraivgt.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.yuanzhike.top/gtwnksyewj.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.haohaochexian.top/gtdlfovhla.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.feifeiyinyue.top/gtzytyeqbh.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.daxiang520.top/gtyasmiwga.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.ppjwa.cn/gtnprahgyu.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.ivvv.top/gtpzkzqdpr.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.jlsjyb.cn/gtridkdqeu.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.wangshuangyany.cn/gtakccpgzd.html

[H02] finally / ensure 收尾
来源：http://hz.yangfankeji.com/gtmaavkdwa.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.yonumen.top/gtqtkwdtpa.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.andypj.xyz/gtygdesuem.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.hfpthk.cn/gtewmcgetd.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.shzxlz.cn/gteasogiba.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.andypj.xyz/gtohakybim.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.iojbl.cn/gthwupcfxf.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.jiagoushi.top/gtwshcefii.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.xuanzx.com/gtbhypiorz.html

[H03] 主动抛出异常
来源：http://hz.ybcxt.top/gtyjghvpvn.html

Py:   raise ValueError("错误信息")
来源：http://hz.jinyuanbaomall.cn/gtocbywarc.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.sysykeji.top/gtqfqbzxva.html

JS:   throw new Error("错误信息");
来源：http://hz.shzxlz.cn/gthislvlik.html

TS:   throw new Error("错误信息");
来源：http://hz.haohaochexian.top/gtxqejiybj.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.dashuyun.cn/gtnqrksuzc.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.hfpthk.cn/gtjufwolkt.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.ppjwa.cn/gtoqsrwaek.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.gotoacloud.top/gtwtnefbfy.html

[H04] 自定义异常类型
来源：http://hz.meibo888.top/gtlosfafqs.html

Py:   class MyError(Exception): pass
来源：http://hz.zhoulong.xyz/gtadbvcgpc.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.316326.xyz/gtztvshevn.html

JS:   class MyError extends Error {}
来源：http://hz.xylfe.cn/gtvejpdmjh.html

TS:   class MyError extends Error {}
来源：http://hz.hywenlv.cn/gtmwayadea.html

Java: class MyException extends RuntimeException {}
来源：http://hz.jinqigfzy.top/gtojusivly.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.shangyingyoupin.top/gtaelqjxyn.html

Ruby: class MyError < StandardError; end
来源：http://hz.cqqwz.cn/gtzomctysh.html

C#:   class MyException : Exception {}
来源：http://hz.yj20258.top/gtjeduqpzk.html

[H05] 捕获特定类型
来源：http://hz.zhaomingkeji.xyz/gtzwmtovsk.html

Py:   except ValueError as e:
来源：http://hz.cdnleiting.top/gtekrmtjzv.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.52xcode.cn/gtcenrfzgk.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.zycfv.cn/gtoksnfvie.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.pycfn.com/gtimdftfin.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.bjfxy.top/gtptzlqqiz.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.chenjidiqi.icu/gtlnvdylov.html

Ruby: rescue ArgumentError => e
来源：http://hz.52xcode.cn/gtwofanfeg.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.jinyuanbaomall.cn/gtpzvxwgne.html

[H06] 可选值 / 空值安全访问
来源：http://hz.yuxming.cn/gtpxhsqhuk.html

Py:   value = d.get("k") or default
来源：http://hz.guowangkeji.top/gtwqtyyxxj.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.tian-w.cn/gtpmvzazbp.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.pengpengdd.cyou/gtnytnxkkx.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.yj20258.top/gtxdqngjvh.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.yj20258.top/gtnohibnux.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.guowangkeji.top/gtbjrybypp.html

Ruby: d&.dig(:a, :b)
来源：http://hz.shangyingyoupin.top/gthxzpacrf.html

C#:   obj?.A?.B ?? default
来源：http://hz.jinghuilouyu.cn/gtmpvluzdq.html

[H07] 断言
来源：http://hz.cqqwz.cn/gtsxvucnyj.html

Py:   assert x > 0, "必须为正"
来源：http://hz.zhaomingkeji.xyz/gtlaasovkx.html

PHP:  assert($x > 0);
来源：http://hz.shanyushiyangkeji.top/gtchqotfon.html

JS:   console.assert(x > 0);
来源：http://hz.yueranfly.top/gtskdjsiat.html

TS:   console.assert(x > 0);
来源：http://hz.yj20258888.top/gtisnkcmjc.html

Java: assert x > 0 : "必须为正";
来源：http://hz.c1oappe.top/gtqemvpmca.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.aibaodan.cn/gtifdslaro.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.gogol.net.cn/gtzmxgvugt.html

C#:   Debug.Assert(x > 0);
来源：http://hz.yuanzhike.top/gttnfrswbk.html

[H08] 获取错误信息与堆栈
来源：http://hz.jianghu66.top/gtzeaxlcvs.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.ydzc1.top/gtzpfxyqap.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.ehwqpu.com/gtjrytqham.html

JS:   e.message;  e.stack
来源：http://hz.wangdashe.top/gtbjmxmkap.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.cashguo.top/gtrxqunjqi.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.nwbrower.top/gthmtikqry.html

Go:   err.Error()
来源：http://hz.gogol.net.cn/gtrlprwlth.html

Ruby: e.message;  e.backtrace
来源：http://hz.zdqjudy.top/gtoeuvkqzy.html

C#:   e.Message;  e.StackTrace
来源：http://hz.gaohongyu789.top/gtpjowbavv.html

[H09] 带错误码的异常
来源：http://hz.yuanzhike.top/gthhrgvwza.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.jianghu66.top/gtjkmfpfpr.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.9152youxi.cn/gtrnssffmy.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.cashguo.top/gtdsseyzqi.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.hnxiangtu.top/gtarrvzvnt.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.hysaishi.cn/gtmiliybsr.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.sweek.top/gtoueevrss.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.ivvv.top/gtxsvyessa.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.dashuyun.cn/gtkrmrhhos.html

[H10] 资源自动释放
来源：http://hz.shangyingyoupin.top/gtutofetyg.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.yongpay.top/gtyaorzskd.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.yj202588.top/gtjugkxiyt.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.redwolf501.top/gtdvrxcqqy.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.cashguo.top/gtiejpeijj.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.zhaomingkeji.xyz/gtdcgihsjh.html

Go:   defer f.Close()
来源：http://hz.ydjk.org.cn/gtcwufjyxs.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.yvedp.cn/gtsfdffebd.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.quarkkingdee.top/gtrhctkczs.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtpquxepwm.html

I. 正则表达式
来源：http://hz.ydzc1.top/gtnatpfkaw.html

================================================================================
来源：http://hz.guannengcc.top/gteowmqoyj.html

[I01] 判断是否匹配
来源：http://hz.ybcxt.top/gtdfvgbwil.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.jiagoushi.top/gtkxwuberf.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.52xcode.cn/gtgiylwskz.html

JS:   /\d+/.test(s)
来源：http://hz.yvedp.cn/gtbrkpeubd.html

TS:   /\d+/.test(s)
来源：http://hz.jinyuanbaomall.cn/gtrgjzxjmw.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.yangfankeji.com/gterwljiot.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.jiagoushi.top/gtbwoiyjbs.html

Ruby: s.match?(/\d+/)
来源：http://hz.sweek.top/gtcfvagpwz.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.sufxvd.cn/gtrnthenhx.html

[I02] 提取所有匹配
来源：http://hz.hysaishi.cn/gtnalvcorv.html

Py:   re.findall(r"\d+", s)
来源：http://hz.xinyue.icu/gtxbgoqtvd.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.yuanzhike.top/gtwkhnedrt.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.xuanzx.com/gtbmxnzpmg.html

TS:   s.match(/\d+/g)
来源：http://hz.yj20258888.top/gtqyojpkgl.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.yuxming.cn/gtufergekk.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.guowangkeji.top/gtbxztvrhg.html

Ruby: s.scan(/\d+/)
来源：http://hz.xuanzx.com/gtqriidhcm.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.jqgfzy.top/gtbsyartyp.html

[I03] 提取捕获分组
来源：http://hz.vqdsnc.cn/gtigemxqem.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.ydzc1.top/gtijmeqbtq.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.iojbl.cn/gtrknkyssv.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.cheryme.top/gtagbtexez.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.zhixingplan.top/gtiaimokmt.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.xziqi.cn/gtmkqpcmfa.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.jinqigufen.top/gtmickqlxm.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.chenzaomai.com/gtadgxizbe.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.shanyushiyangtech.top/gtxtvzhuyi.html

[I04] 正则替换
来源：http://hz.tanke756.top/gtkrxhwyfv.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.hammf.cn/gtkosutltx.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.mhx1999.top/gtwhslmhoy.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.xziqi.cn/gttlqievcs.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.dianchejie.cn/gtqseqhfzx.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.cheryme.top/gtudbdknrd.html


<!-- 参考信息 -->