代发 wailian999

[F09] 获取文件大小
来源：http://hz.havefunace.top/gtfnvnvgcl.html

Py:   os.path.getsize("a.txt")
来源：http://hz.yuanzhike.top/gtctqnrymx.html

PHP:  filesize("a.txt");
来源：http://hz.fengsongda.top/gtjxrqksiv.html

JS:   fs.statSync("a.txt").size
来源：http://hz.redwolf501.top/gtybgnlzma.html

TS:   fs.statSync("a.txt").size
来源：http://hz.birdmap.top/gtxygrswct.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.yueranfly.top/gtmezgxvyh.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.zhixingplan.top/gtjzfbsnta.html

Ruby: File.size("a.txt")
来源：http://hz.52xcode.cn/gtathtupda.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.yangfankeji.com/gtlpxmlymy.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.cucudq.cn/gtroqwphak.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.0kj1m.cn/gtftcnrmuv.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.guowangkeji.top/gtxfgjsfmn.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.dashuyun.cn/gtttuwxzzh.html

TS:   path.extname("a.txt")
来源：http://hz.zhixingplan.top/gtipilcwzn.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.hywenlv.cn/gtgadqvoaw.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.hfpthk.cn/gtvjrdzbai.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.xuanzx.com/gtxrxbttnr.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.sysykeji.top/gtcjxiefaf.html

[F11] 复制与移动文件
来源：http://hz.316326.xyz/gttebuxysy.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.dashuyun.cn/gtilqzanyg.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.xuetiantiany.cn/gtwfabmjtd.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.fzhhl.top/gtpyrohycn.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.sweek.top/gtlgmfpftr.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.shangyingyoupin.top/gthphxchhy.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.haohaochexian.top/gtjkoiadhk.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.haohaochexian.top/gtgpgosksf.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.yangfankeji.com/gtposcjoja.html

[F12] CSV 读写
来源：http://hz.hongshengwenyu.top/gtcbnnblek.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.vqdsnc.cn/gtuzqoseou.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.sweek.top/gtpiebxbnm.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.ywan-chungtsiang.top/gtlftfcclo.html

TS:   // 同上
来源：http://hz.xingfuxueyuan.xyz/gtkskhpwjr.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.smart0.xyz/gtvxszntic.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.yj202588.top/gtgzwuzfma.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.ybcxt.top/gtzhpmbqwd.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.jinghuilouyu.cn/gtupjkikpn.html

================================================================================
来源：http://hz.zhoulong.xyz/gtgobidaws.html

G. 面向对象
来源：http://hz.tian-w.cn/gtnfngprwl.html

================================================================================
来源：http://hz.9152youxi.cn/gtroczbjuh.html

[G01] 定义类
来源：http://hz.zhaomingkeji.xyz/gtegcurnur.html

Py:   class User: pass
来源：http://hz.c1oappe.top/gtlgnydeig.html

PHP:  class User {}
来源：http://hz.9152youxi.cn/gtokohtbgf.html

JS:   class User {}
来源：http://hz.ybcxt.top/gtweorgjrg.html

TS:   class User { name: string = ""; }
来源：http://hz.tanke756.top/gtetduyloe.html

Java: class User {}
来源：http://hz.xingfuxueyuan.xyz/gtfppyhzmf.html

Go:   type User struct { Name string }
来源：http://hz.hammf.cn/gtjgncnqql.html

Ruby: class User; end
来源：http://hz.jianghu66.top/gtjtzlmnqg.html

C#:   class User {}
来源：http://hz.jinyuanbaomall.cn/gtbhsyitkz.html

[G02] 构造函数
来源：http://hz.gaohongyu789.top/gtfdzyquzq.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.yvedp.cn/gtyzegvppg.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.yangfankeji.com/gtaetwlfis.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.xylfe.cn/gtpaqbbyeu.html

TS:   constructor(public name: string) {}
来源：http://hz.shzxlz.cn/gthhlxlcbh.html

Java: User(String name) { this.name = name; }
来源：http://hz.yongpay.top/gtyrxwamvj.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.bjfxy.top/gtrzfwmkpm.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.ivvv.top/gtyhusumsp.html

C#:   public User(string name) { Name = name; }
来源：http://hz.316326.xyz/gtgdyibenb.html

[G03] 实例属性
来源：http://hz.yvedp.cn/gtflthazlz.html

Py:   self.name = "x"
来源：http://hz.jinghuilouyu.cn/gtxylbkfmk.html

PHP:  public string $name = "x";
来源：http://hz.hfpthk.cn/gtqwbcjnae.html

JS:   this.name = "x";
来源：http://hz.nwbrower.top/gtvzhiuyvo.html

TS:   name: string = "x";
来源：http://hz.snrcjt.cn/gtxcgwdeqd.html

Java: private String name;
来源：http://hz.jinqigfzy.top/gtnktajhjb.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.fzhhl.top/gtayngbmon.html

Ruby: @name = "x"
来源：http://hz.zhiwuduotai.top/gtvjrepluz.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.jqgufenzy.top/gtcfogbsce.html

[G04] 定义方法
来源：http://hz.jiagoushi.top/gtyqxjplwv.html

Py:   def greet(self): return self.name
来源：http://hz.zhaomingkeji.xyz/gtjjzqwmsr.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.xuetiantiany.cn/gtxguqwcti.html

JS:   greet() { return this.name; }
来源：http://hz.fengsongda.top/gttawmcdad.html

TS:   greet(): string { return this.name; }
来源：http://hz.cheryme.top/gtwymeemqn.html

Java: String greet() { return name; }
来源：http://hz.daria6918.cn/gtarjgiltz.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.zhiwuduotai.top/gthloetogi.html

Ruby: def greet; @name; end
来源：http://hz.daxiang520.top/gtylfukmol.html

C#:   public string Greet() => Name;
来源：http://hz.hongshengwenyu.top/gthoipmvzw.html

[G05] 继承
来源：http://hz.meibo888.top/gttxiyxbfh.html

Py:   class Admin(User): pass
来源：http://hz.jyoumei.cn/gtqfoetvsn.html

PHP:  class Admin extends User {}
来源：http://hz.sweek.top/gtonebhcxp.html

JS:   class Admin extends User {}
来源：http://hz.sysykeji.top/gtbtraemir.html

TS:   class Admin extends User {}
来源：http://hz.xuanzx.com/gtwoyjceis.html

Java: class Admin extends User {}
来源：http://hz.gaohongyu789.top/gttcrhwuav.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.shzxlz.cn/gtffzqwcls.html

Ruby: class Admin < User; end
来源：http://hz.havefunace.top/gtsvdakgnm.html

C#:   class Admin : User {}
来源：http://hz.0kj1m.cn/gtfqcuxwcf.html

[G06] 重写方法
来源：http://hz.jqgufenzy.top/gthvwpxdxb.html

Py:   def greet(self): return "admin"
来源：http://hz.haohaochexian.top/gtfehjkask.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.zhijiandao.cn/gtknlyfjjz.html

JS:   greet() { return "admin"; }
来源：http://hz.hysaishi.cn/gtqzcspoap.html

TS:   greet(): string { return "admin"; }
来源：http://hz.birdmap.top/gtndufgmdc.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.jinqigfzy.top/gtqlyrwovy.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.yanxiufei.cn/gtjfmeknnn.html

Ruby: def greet; "admin"; end
来源：http://hz.mhx1999.top/gtboqsukuv.html

C#:   public override string Greet() => "admin";
来源：http://hz.gzhubu.top/gtyrcysmmz.html

[G07] 调用父类方法
来源：http://hz.tanke756.top/gthwnnrqxj.html

Py:   super().greet()
来源：http://hz.sweek.top/gtlmjxdftx.html

PHP:  parent::greet();
来源：http://hz.daria6918.cn/gtedevdcoo.html

JS:   super.greet();
来源：http://hz.zhijiandao.cn/gtnanwymbo.html

TS:   super.greet();
来源：http://hz.jqgfzy.top/gtryviwsqu.html

Java: super.greet();
来源：http://hz.zhixingplan.top/gtpcwjzqeg.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.sxryk.cn/gtlwfyoehz.html

Ruby: super
来源：http://hz.redwolf501.top/gtobntqclc.html

C#:   base.Greet();
来源：http://hz.fzhhl.top/gtzuefutql.html

[G08] 静态方法与属性
来源：http://hz.fengsongda.top/gtfyzqbudz.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.hammf.cn/gtatlzqjpm.html

PHP:  public static function f() {}
来源：http://hz.yj20258.top/gtfospeomt.html

JS:   static f() {}
来源：http://hz.jiagoushi.top/gtjggzgjuq.html

TS:   static f(): void {}
来源：http://hz.jqgfzy.top/gtnfltbovl.html

Java: static void f() {}
来源：http://hz.tian-w.cn/gtwysresen.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.cheryme.top/gtcfrstveh.html

Ruby: def self.f; end
来源：http://hz.gzhubu.top/gtvkbbhnkr.html

C#:   public static void F() {}
来源：http://hz.fzhhl.top/gtbvfwlpkq.html

[G09] 接口 / 抽象类
来源：http://hz.hammf.cn/gtshuiravr.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.vqdsnc.cn/gtgjpfhdxg.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.tian-w.cn/gtdqjpljpn.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.zhongyouzk.top/gtrywizpsm.html

TS:   interface Shape { area(): number; }
来源：http://hz.cheryme.top/gtbauznpyt.html

Java: interface Shape { double area(); }
来源：http://hz.fengsongda.top/gtsftzefhk.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.9152youxi.cn/gtlzgdypqv.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.jyoumei.cn/gtqwgcvjol.html

C#:   interface IShape { double Area(); }
来源：http://hz.wangshuangyany.cn/gtwikrpdge.html

[G10] 访问控制
来源：http://hz.zhijiandao.cn/gtwcacpeyp.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.shangyingyoupin.top/gthikrxdxt.html

PHP:  public / protected / private
来源：http://hz.zycfv.cn/gtymyzwdkt.html

JS:   #private 字段；其余公开
来源：http://hz.ppjwa.cn/gtumsmvmvr.html

TS:   public / protected / private
来源：http://hz.sxryk.cn/gtzpymdysn.html

Java: public / protected / private / 默认包级
来源：http://hz.xinyue.icu/gtpqnoprig.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.316326.xyz/gtwytjcyra.html

Ruby: public / protected / private
来源：http://hz.yangfankeji.com/gtyisarzne.html

C#:   public / protected / private / internal
来源：http://hz.hfpthk.cn/gtmqezltsw.html

[G11] getter / setter
来源：http://hz.nanxinkj.top/gtxwvpqywd.html

Py:   @property 与 @x.setter
来源：http://hz.yj20258.top/gtganwxvey.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.tian-w.cn/gtzbnjqcwi.html

JS:   get name() { return this._name; }
来源：http://hz.aibaodan.cn/gtviueszuq.html

TS:   get name(): string { return this._name; }
来源：http://hz.0kj1m.cn/gtszxotoud.html

Java: public String getName() { return name; }
来源：http://hz.jqgfzy.top/gtanqcwbmg.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.zycfv.cn/gtbgxapknu.html

Ruby: attr_accessor :name
来源：http://hz.haohaochexian.top/gtjpwxewub.html

C#:   public string Name { get; set; }
来源：http://hz.dashuyun.cn/gtsqdmrzcz.html

[G12] 对象转字符串
来源：http://hz.jianghu66.top/gteysvxfea.html

Py:   def __str__(self): return self.name
来源：http://hz.chenjidiqi.icu/gtgdmxcrsc.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.guannengcc.top/gtzhfdujrf.html

JS:   toString() { return this.name; }
来源：http://hz.daria6918.cn/gtykapbbwm.html

TS:   toString(): string { return this.name; }
来源：http://hz.jqgufenzy.top/gtibmzzpap.html

Java: @Override public String toString() { return name; }
来源：http://hz.mhx1999.top/gtzldshfss.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.nanxinkj.top/gtmevqpsol.html

Ruby: def to_s; @name; end
来源：http://hz.smart0.xyz/gtqdjuwyqs.html

C#:   public override string ToString() => Name;
来源：http://hz.feifeiyinyue.top/gtrzbdeayc.html

[G13] 判断对象类型
来源：http://hz.hysaishi.cn/gtkltavnno.html

Py:   isinstance(u, User)
来源：http://hz.yvedp.cn/gtmzndlylv.html

PHP:  $u instanceof User
来源：http://hz.yuxming.cn/gtnmzdnkxj.html

JS:   u instanceof User
来源：http://hz.jinghuilouyu.cn/gtpecbvujz.html

TS:   u instanceof User
来源：http://hz.aibaodan.cn/gtvhkoomcj.html

Java: u instanceof User
来源：http://hz.chenzaomai.com/gtqkvbakre.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.snrcjt.cn/gttwncuaqu.html

Ruby: u.is_a?(User)
来源：http://hz.dashuyun.cn/gtcaoxbquo.html

C#:   u is User
来源：http://hz.daxiang520.top/gtsmtjamnc.html

[G14] 数据类 / record
来源：http://hz.shanyushiyangtech.top/gtlxkmcwox.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.cheryme.top/gtiojxbilj.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.daxiang520.top/gtqmeoggpy.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.jinqigfzy.top/gtraabdafx.html

TS:   type User = { name: string; age: number };
来源：http://hz.zhengqikj.top/gtjwwcrhlk.html

Java: record User(String name, int age) {}
来源：http://hz.vqdsnc.cn/gtocahqwlp.html

Go:   type User struct { Name string; Age int }
来源：http://hz.yanxiufei.cn/gtpxqynmre.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.meibo888.top/gtzmccwvuh.html

C#:   record User(string Name, int Age);
来源：http://hz.hfpthk.cn/gtzcezubca.html

[G15] 枚举
来源：http://hz.yanxiufei.cn/gtihombhjc.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.dashuyun.cn/gtdmnufkbk.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.guowangkeji.top/gtuybdwbst.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.mhx1999.top/gtafyrcuqh.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.daria6918.cn/gtvmubczrp.html

Java: enum Color { RED, GREEN }
来源：http://hz.hywenlv.cn/gtwwboowjn.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.c1oappe.top/gtoxqszmso.html

Ruby: Color = %i[red green].freeze
来源：http://hz.yangfankeji.com/gtyyfjattx.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.xylfe.cn/gticbqzifl.html

[G16] 对象转数组 / 字典
来源：http://hz.jqgufenzy.top/gthiyhbazi.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.sxryk.cn/gtdshgcali.html

PHP:  get_object_vars($obj);
来源：http://hz.wangshuangyany.cn/gtrpfqdwit.html

JS:   Object.entries(obj)
来源：http://hz.gaohongyu789.top/gtslyizjml.html

TS:   Object.entries(obj)
来源：http://hz.zhoulong.xyz/gtjwqpxaii.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.jqgufenzy.top/gtijfzmeyr.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.52xcode.cn/gtznzlnqpj.html

Ruby: obj.instance_variables
来源：http://hz.tian-w.cn/gtevkolzrh.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.xuanzx.com/gtqqzfyvzk.html

================================================================================
来源：http://hz.fzhhl.top/gtsyroatnz.html

H. 异常与错误处理
来源：http://hz.jinqigfzy.top/gtnofcttqi.html

================================================================================
来源：http://hz.pycfn.com/gtlcyzwlua.html

[H01] try / catch 基础
来源：http://hz.ydjk.org.cn/gtcsbtrfys.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.hysaishi.cn/gtplefitce.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.yj20258.top/gtlrgdczrh.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.yanxiufei.cn/gtoeiminwp.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.aizwys.cn/gtolropkqd.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.xuetiantiany.cn/gtmgfndcdq.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.ydzc1.top/gtbzlylbbe.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.yonumen.top/gtkequcttk.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.cqqwz.cn/gtugqrvohr.html

[H02] finally / ensure 收尾
来源：http://hz.ppjwa.cn/gtjqrhhbol.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.zhixingplan.top/gtwqedilun.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.tian-w.cn/gtzlowycep.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.redwolf501.top/gtvloutgkd.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.xinyue.icu/gtvpvrdriy.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.wangshuangyany.cn/gtdsntfaop.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.hongshengwenyu.top/gtjxoljkav.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.cheryme.top/gtayydypbq.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.zhiwuduotai.top/gtnsihabyc.html

[H03] 主动抛出异常
来源：http://hz.zhiwuduotai.top/gtdxddxnhn.html

Py:   raise ValueError("错误信息")
来源：http://hz.yonumen.top/gtvzghnhud.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.zhijiandao.cn/gtpbvvpeoq.html

JS:   throw new Error("错误信息");
来源：http://hz.aizwys.cn/gtdctoiqlh.html

TS:   throw new Error("错误信息");
来源：http://hz.iojbl.cn/gtzwcbjzyr.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.guannengcc.top/gtmaoyaadu.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.hywenlv.cn/gtszugeoty.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.tanke756.top/gtsgqivvmq.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.jinqigufen.top/gtiwngkxkm.html

[H04] 自定义异常类型
来源：http://hz.fzhhl.top/gtcvyfpiwg.html

Py:   class MyError(Exception): pass
来源：http://hz.zhijiandao.cn/gtquevgwiz.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.jqgfzy.top/gtbiyilmkx.html

JS:   class MyError extends Error {}
来源：http://hz.cashguo.top/gtvzdztlyr.html

TS:   class MyError extends Error {}
来源：http://hz.smart0.xyz/gttnbzkbnx.html

Java: class MyException extends RuntimeException {}
来源：http://hz.yueranfly.top/gtjmvkfdnc.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.hfpthk.cn/gtgfqfqdvj.html

Ruby: class MyError < StandardError; end
来源：http://hz.sufxvd.cn/gtugugvjnx.html

C#:   class MyException : Exception {}
来源：http://hz.ybcxt.top/gtrpjbonoh.html

[H05] 捕获特定类型
来源：http://hz.hfpthk.cn/gtrzvufghr.html

Py:   except ValueError as e:
来源：http://hz.gotoacloud.top/gtwxnqodol.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.zhixingplan.top/gtiwrjqeyl.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.0kj1m.cn/gtpmunasai.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.fengsongda.top/gtmqckzlsi.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.xziqi.cn/gtfjdefnwg.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.daria6918.cn/gtihkbucnt.html

Ruby: rescue ArgumentError => e
来源：http://hz.jinyuanbaomall.cn/gtyrpoqzzl.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.sxryk.cn/gtctrylldb.html

[H06] 可选值 / 空值安全访问
来源：http://hz.shuidangran.top/gtlvufvbch.html

Py:   value = d.get("k") or default
来源：http://hz.yueranfly.top/gtstzffqmw.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.shzxlz.cn/gtpacfiuma.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.xylfe.cn/gtbwsrvcfk.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.yj20258.top/gtyudopghl.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.ppjwa.cn/gtuzrzifha.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.hnxiangtu.top/gtjblaslhb.html

Ruby: d&.dig(:a, :b)
来源：http://hz.chenzaomai.com/gtijgdvhxs.html

C#:   obj?.A?.B ?? default
来源：http://hz.guowangkeji.top/gtykgfsknm.html

[H07] 断言
来源：http://hz.ydzc1.top/gtvpfxtdnr.html

Py:   assert x > 0, "必须为正"
来源：http://hz.gotoacloud.top/gtbxaqcvmp.html

PHP:  assert($x > 0);
来源：http://hz.ydjk.org.cn/gtflzupemz.html

JS:   console.assert(x > 0);
来源：http://hz.jqgufenzy.top/gtzxunkjmm.html

TS:   console.assert(x > 0);
来源：http://hz.guannengcc.top/gtlljgrfeu.html

Java: assert x > 0 : "必须为正";
来源：http://hz.zycfv.cn/gtixkehtpy.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.havefunace.top/gttecndvkl.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.redwolf501.top/gtkingifvx.html

C#:   Debug.Assert(x > 0);
来源：http://hz.haohaochexian.top/gtbbxaqalj.html

[H08] 获取错误信息与堆栈
来源：http://hz.daxiang520.top/gtswohagnl.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.ppjwa.cn/gthgqtktgl.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.sxryk.cn/gtpvcgpkkl.html

JS:   e.message;  e.stack
来源：http://hz.xinyue.icu/gtfodczprh.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.iojbl.cn/gtdrjwindk.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.guannengcc.top/gtsjhqtwfc.html

Go:   err.Error()
来源：http://hz.hammf.cn/gtgttogttt.html

Ruby: e.message;  e.backtrace
来源：http://hz.xziqi.cn/gtjjaimdqk.html

C#:   e.Message;  e.StackTrace
来源：http://hz.pycfn.com/gtzxgdhqat.html

[H09] 带错误码的异常
来源：http://hz.bjfxy.top/gtxtgrevye.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.ydzc1.top/gtgcmvauix.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.sysykeji.top/gtwyqwsnty.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.jqgufenzy.top/gtgodggthp.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.yuxming.cn/gtstmigsju.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.snrcjt.cn/gtozprpswq.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.316326.xyz/gticecupmg.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.redwolf501.top/gtomgyjxik.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.jinyuanbaomall.cn/gttiftnurf.html

[H10] 资源自动释放
来源：http://hz.jianghu66.top/gtcngxdlka.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.feifeiyinyue.top/gttoldofmc.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.dashuyun.cn/gtocoieazi.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.jinqigufen.top/gtasjcjima.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.xuetiantiany.cn/gtovswjfii.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.yvedp.cn/gtdgmffhqb.html

Go:   defer f.Close()
来源：http://hz.gzhubu.top/gtpelemayq.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.aizwys.cn/gtianfnpai.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.zhoulong.xyz/gtmbxdufkg.html

================================================================================
来源：http://hz.daria6918.cn/gtitbawvag.html

I. 正则表达式
来源：http://hz.9152youxi.cn/gtebhedwph.html

================================================================================
来源：http://hz.ivvv.top/gthcbymhug.html

[I01] 判断是否匹配
来源：http://hz.ydjk.org.cn/gtfauqrsgn.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.hnxiangtu.top/gtervtucgm.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.cdnleiting.top/gtdnqrybxp.html

JS:   /\d+/.test(s)
来源：http://hz.jiagoushi.top/gtqlxsipmj.html

TS:   /\d+/.test(s)
来源：http://hz.hywenlv.cn/gtacddgyzm.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.ydjk.org.cn/gtimekznjj.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.yangfankeji.com/gtaomtdguf.html

Ruby: s.match?(/\d+/)
来源：http://hz.daxiang520.top/gtvvqnkybq.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.ehwqpu.com/gtgsmjpolr.html

[I02] 提取所有匹配
来源：http://hz.pycfn.com/gteyieavlr.html

Py:   re.findall(r"\d+", s)
来源：http://hz.aibaodan.cn/gtssmbjlho.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.ehwqpu.com/gtmjrdcdlo.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.yj202588.top/gtrgqkomiy.html

TS:   s.match(/\d+/g)
来源：http://hz.tian-w.cn/gtyizvznea.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.jinyuanbaomall.cn/gtqlbufqvj.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.xingfuxueyuan.xyz/gtmxbjnpsi.html

Ruby: s.scan(/\d+/)
来源：http://hz.0kj1m.cn/gtqtigqsnx.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.pengpengdd.cyou/gtmshqwnru.html

[I03] 提取捕获分组
来源：http://hz.guowangkeji.top/gtfmugxixn.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.shuidangran.top/gtefwkufar.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.ppjwa.cn/gtvkyanvcn.html


<!-- 参考信息 -->