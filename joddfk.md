代发 wailian999

C#:   new FileInfo("a.txt").Length
来源：http://hz.ydzc1.top/gtfzpgeutg.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.hywenlv.cn/gtelstedvj.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.jiagoushi.top/gtmfetisee.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.zhoulong.xyz/gtmaxwoboj.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.52xcode.cn/gtczcyztnl.html

TS:   path.extname("a.txt")
来源：http://hz.chenjidiqi.icu/gtzcnhlyro.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.pengpengdd.cyou/gtkyearhze.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.aibaodan.cn/gtgytygdig.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.chenjidiqi.icu/gtmqvwntbe.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.wangdashe.top/gtxmtfowoi.html

[F11] 复制与移动文件
来源：http://hz.haohaochexian.top/gtkowogouw.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.yangfankeji.com/gtzirldska.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.wangshuangyany.cn/gtmehmozhz.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.nanxinkj.top/gtnmdeicxe.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.yvedp.cn/gtqqycxkdw.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.zhongyouzk.top/gthddjwpop.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.yongpay.top/gtiscefkwz.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.nwbrower.top/gtblojrmzk.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.52xcode.cn/gtxxwjkwui.html

[F12] CSV 读写
来源：http://hz.wangdashe.top/gtmasamtog.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.wangdashe.top/gtbnehtzwg.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.316326.xyz/gtvmpfrjbj.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.vqdsnc.cn/gtsudmnaxs.html

TS:   // 同上
来源：http://hz.yj202588.top/gtbwvlljpn.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.xingfuxueyuan.xyz/gtmmznqjjd.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.shangyingyoupin.top/gtaxdisquh.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.xinyue.icu/gtfizeeyeu.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.shzxlz.cn/gtmxabtrll.html

================================================================================
来源：http://hz.yueranfly.top/gtputihqii.html

G. 面向对象
来源：http://hz.wangdashe.top/gtshtihvvj.html

================================================================================
来源：http://hz.tianlin.xyz/gtbvqdxbwz.html

[G01] 定义类
来源：http://hz.snrcjt.cn/gtbjuanjek.html

Py:   class User: pass
来源：http://hz.jinqigfzy.top/gtrwxtovvn.html

PHP:  class User {}
来源：http://hz.0kj1m.cn/gtfsscvqcr.html

JS:   class User {}
来源：http://hz.cqqwz.cn/gtmgmjpxhs.html

TS:   class User { name: string = ""; }
来源：http://hz.chenlongwang.top/gtlfwtdyqg.html

Java: class User {}
来源：http://hz.cqqwz.cn/gtswyuixze.html

Go:   type User struct { Name string }
来源：http://hz.fzhhl.top/gtyqjvksyj.html

Ruby: class User; end
来源：http://hz.jqgfzy.top/gtzrifbljf.html

C#:   class User {}
来源：http://hz.jinqigufen.top/gtyvczqopd.html

[G02] 构造函数
来源：http://hz.svipenyu.cn/gtmqxbtflj.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.yangfankeji.com/gtpiqdpeiy.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.ydjk.org.cn/gtvpbtpeca.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.gogol.net.cn/gtvhkmhstm.html

TS:   constructor(public name: string) {}
来源：http://hz.yonumen.top/gtgaphvwer.html

Java: User(String name) { this.name = name; }
来源：http://hz.quarkkingdee.top/gtawtdyjhz.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.meibo888.top/gtyvfhnuyx.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.c1oappe.top/gtjdijvizp.html

C#:   public User(string name) { Name = name; }
来源：http://hz.svipenyu.cn/gtpzcsgylb.html

[G03] 实例属性
来源：http://hz.gaohongyu789.top/gtwuzdamia.html

Py:   self.name = "x"
来源：http://hz.yj20258888.top/gtnpntijeh.html

PHP:  public string $name = "x";
来源：http://hz.zhixingplan.top/gttkhysgrf.html

JS:   this.name = "x";
来源：http://hz.dianchejie.cn/gtdxmaedxg.html

TS:   name: string = "x";
来源：http://hz.ydzc1.top/gtgwkjpiri.html

Java: private String name;
来源：http://hz.c1oappe.top/gttvwcwlti.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.wangdashe.top/gtegwubkda.html

Ruby: @name = "x"
来源：http://hz.xziqi.cn/gtuforqori.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.zycfv.cn/gtqzcgxyye.html

[G04] 定义方法
来源：http://hz.shuidangran.top/gtolhaxvya.html

Py:   def greet(self): return self.name
来源：http://hz.yj20258888.top/gtiaydskyi.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.cqqwz.cn/gtltriprjl.html

JS:   greet() { return this.name; }
来源：http://hz.cashguo.top/gtwvkhjkxi.html

TS:   greet(): string { return this.name; }
来源：http://hz.316326.xyz/gtfdvdkeiy.html

Java: String greet() { return name; }
来源：http://hz.iojbl.cn/gtjboyztkw.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.sysykeji.top/gtwyvghhrq.html

Ruby: def greet; @name; end
来源：http://hz.guannengcc.top/gtondphffd.html

C#:   public string Greet() => Name;
来源：http://hz.yongpay.top/gtcdpqnoqc.html

[G05] 继承
来源：http://hz.jyoumei.cn/gtxwfawmxz.html

Py:   class Admin(User): pass
来源：http://hz.jqgfzy.top/gtztwxfzou.html

PHP:  class Admin extends User {}
来源：http://hz.xuanzx.com/gtlnpliksd.html

JS:   class Admin extends User {}
来源：http://hz.yueranfly.top/gtxmgkloun.html

TS:   class Admin extends User {}
来源：http://hz.hongshengwenyu.top/gtdeeceqrh.html

Java: class Admin extends User {}
来源：http://hz.jlsjyb.cn/gtfmctakom.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.xinyue.icu/gtwyekgwph.html

Ruby: class Admin < User; end
来源：http://hz.yj202588.top/gteapztiup.html

C#:   class Admin : User {}
来源：http://hz.daria6918.cn/gtdudgozdb.html

[G06] 重写方法
来源：http://hz.yueranfly.top/gtriejlmkx.html

Py:   def greet(self): return "admin"
来源：http://hz.gzhubu.top/gtbmakzdil.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.xinyue.icu/gtnbkrzmpi.html

JS:   greet() { return "admin"; }
来源：http://hz.cucudq.cn/gtswxayxzq.html

TS:   greet(): string { return "admin"; }
来源：http://hz.gogol.net.cn/gtihscrmvz.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.zhaomingkeji.xyz/gtvqyycgkw.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.nanxinkj.top/gtrhpvkcmi.html

Ruby: def greet; "admin"; end
来源：http://hz.xuetiantiany.cn/gtpowgnoro.html

C#:   public override string Greet() => "admin";
来源：http://hz.ydjk.org.cn/gttwstqrqa.html

[G07] 调用父类方法
来源：http://hz.chenzaomai.com/gtwubpkwui.html

Py:   super().greet()
来源：http://hz.chenlongwang.top/gtzzhewhob.html

PHP:  parent::greet();
来源：http://hz.hnqzz.top/gtctqgymbq.html

JS:   super.greet();
来源：http://hz.jiagoushi.top/gtzhkhpvfm.html

TS:   super.greet();
来源：http://hz.andypj.xyz/gtphdlwvkt.html

Java: super.greet();
来源：http://hz.yongpay.top/gtllhdcorp.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.kuanghao11.cn/gtfqxvsrsk.html

Ruby: super
来源：http://hz.ehwqpu.com/gteqdihlvr.html

C#:   base.Greet();
来源：http://hz.ydjk.org.cn/gtksimotjc.html

[G08] 静态方法与属性
来源：http://hz.redwolf501.top/gtnuphyvgz.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.shuidangran.top/gticwiihgf.html

PHP:  public static function f() {}
来源：http://hz.xingfuxueyuan.xyz/gtantrdhvk.html

JS:   static f() {}
来源：http://hz.gzhubu.top/gtjvawfzpd.html

TS:   static f(): void {}
来源：http://hz.shangyingyoupin.top/gtjadrehqc.html

Java: static void f() {}
来源：http://hz.gaohongyu789.top/gtgaikptdb.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.yongpay.top/gtopxdrsvm.html

Ruby: def self.f; end
来源：http://hz.cucudq.cn/gtpbapcatu.html

C#:   public static void F() {}
来源：http://hz.ppjwa.cn/gtjrpdjxgs.html

[G09] 接口 / 抽象类
来源：http://hz.hnqzz.top/gteliwkfte.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.sufxvd.cn/gtjcsuoiwo.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.xinyue.icu/gtxdrdyqrm.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.ywan-chungtsiang.top/gtvzfewswp.html

TS:   interface Shape { area(): number; }
来源：http://hz.hnxiangtu.top/gtrbqnujhu.html

Java: interface Shape { double area(); }
来源：http://hz.hnqzz.top/gttfynjfrt.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.xuetiantiany.cn/gtcxxegibl.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.hysaishi.cn/gtkrvmdglc.html

C#:   interface IShape { double Area(); }
来源：http://hz.jyoumei.cn/gtzddrnjlz.html

[G10] 访问控制
来源：http://hz.sysykeji.top/gtlxfcncnl.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.ivvv.top/gtaeyiklfy.html

PHP:  public / protected / private
来源：http://hz.chenjidiqi.icu/gtgrmlmzag.html

JS:   #private 字段；其余公开
来源：http://hz.gaohongyu789.top/gtmwkraznu.html

TS:   public / protected / private
来源：http://hz.xinyue.icu/gthjvpotkr.html

Java: public / protected / private / 默认包级
来源：http://hz.zhaomingkeji.xyz/gtgpgekmwm.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.jyoumei.cn/gtczosubtr.html

Ruby: public / protected / private
来源：http://hz.wangshuangyany.cn/gtclymcmyf.html

C#:   public / protected / private / internal
来源：http://hz.bjfxy.top/gtcmuhkijj.html

[G11] getter / setter
来源：http://hz.ehwqpu.com/gtsajvszwu.html

Py:   @property 与 @x.setter
来源：http://hz.cheryme.top/gteryaqkdu.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.fzhhl.top/gtutdpkjyh.html

JS:   get name() { return this._name; }
来源：http://hz.nanxuanxn.top/gtqlreagle.html

TS:   get name(): string { return this._name; }
来源：http://hz.hnxiangtu.top/gtgbfaxrfq.html

Java: public String getName() { return name; }
来源：http://hz.gogol.net.cn/gtpvnflqxp.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.svipenyu.cn/gtfiirazmz.html

Ruby: attr_accessor :name
来源：http://hz.iojbl.cn/gtussuzqkh.html

C#:   public string Name { get; set; }
来源：http://hz.jinqigfzy.top/gtpqokkeyn.html

[G12] 对象转字符串
来源：http://hz.cdnleiting.top/gtaekkxylq.html

Py:   def __str__(self): return self.name
来源：http://hz.0kj1m.cn/gtijibqcxp.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.zdqjudy.top/gtkgdbbpur.html

JS:   toString() { return this.name; }
来源：http://hz.fzhhl.top/gthfsfwqqq.html

TS:   toString(): string { return this.name; }
来源：http://hz.hfpthk.cn/gtbgpllzno.html

Java: @Override public String toString() { return name; }
来源：http://hz.gzhubu.top/gtggsugojp.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.yj20258.top/gttbfwttwz.html

Ruby: def to_s; @name; end
来源：http://hz.jianghu66.top/gtqograhed.html

C#:   public override string ToString() => Name;
来源：http://hz.svipenyu.cn/gttqxeuomh.html

[G13] 判断对象类型
来源：http://hz.yangfankeji.com/gttxucblos.html

Py:   isinstance(u, User)
来源：http://hz.bjfxy.top/gttzflwuat.html

PHP:  $u instanceof User
来源：http://hz.yuxming.cn/gterabztpl.html

JS:   u instanceof User
来源：http://hz.bjfxy.top/gtrpjvzrgr.html

TS:   u instanceof User
来源：http://hz.sweek.top/gtxhzkrixi.html

Java: u instanceof User
来源：http://hz.xylfe.cn/gtahiyckbn.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.xylfe.cn/gtsxmbfxkb.html

Ruby: u.is_a?(User)
来源：http://hz.gaohongyu789.top/gtkdiozfsq.html

C#:   u is User
来源：http://hz.xylfe.cn/gttgcgjump.html

[G14] 数据类 / record
来源：http://hz.ppjwa.cn/gtrfhfxxrg.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.kuanghao11.cn/gtnqrkywtu.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.haohaochexian.top/gtvyimmbhh.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.cheryme.top/gtieufhuvm.html

TS:   type User = { name: string; age: number };
来源：http://hz.hongshengwenyu.top/gtfcfxrgso.html

Java: record User(String name, int age) {}
来源：http://hz.wangshuangyany.cn/gtqytkduzu.html

Go:   type User struct { Name string; Age int }
来源：http://hz.9152youxi.cn/gtopqisttx.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.shanyushiyangtech.top/gtqbyyfrjz.html

C#:   record User(string Name, int Age);
来源：http://hz.shanyushiyangtech.top/gtwfdulyym.html

[G15] 枚举
来源：http://hz.ppjwa.cn/gtwxnnzlin.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.bjfxy.top/gtktnsoqnw.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.gaohongyu789.top/gtbdwhhpew.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.jinqigfzy.top/gtdfjxnywt.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.yj20258.top/gtqjewivea.html

Java: enum Color { RED, GREEN }
来源：http://hz.jlsjyb.cn/gtgqlppjhw.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.sxryk.cn/gtbnedwlim.html

Ruby: Color = %i[red green].freeze
来源：http://hz.ydzc1.top/gtcxgnjfyw.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.iojbl.cn/gtdvtotxxd.html

[G16] 对象转数组 / 字典
来源：http://hz.ydjk.org.cn/gtqbylkyta.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.fzhhl.top/gtyltakhlq.html

PHP:  get_object_vars($obj);
来源：http://hz.nwbrower.top/gtevdogczl.html

JS:   Object.entries(obj)
来源：http://hz.jlsjyb.cn/gtkksurpmy.html

TS:   Object.entries(obj)
来源：http://hz.daxiang520.top/gtbqjcwqyx.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.xingfuxueyuan.xyz/gtbwrtbzzs.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.sufxvd.cn/gtpxldknks.html

Ruby: obj.instance_variables
来源：http://hz.zhaomingkeji.xyz/gtcjsxbtkg.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.meibo888.top/gtyapbnmry.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtaolygdrl.html

H. 异常与错误处理
来源：http://hz.aibaodan.cn/gtblmknbdz.html

================================================================================
来源：http://hz.jqgfzy.top/gtqjkvifiy.html

[H01] try / catch 基础
来源：http://hz.xziqi.cn/gtyncndxkk.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.yanxiufei.cn/gtchopxgph.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.xinyue.icu/gtqlnvzcab.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.havefunace.top/gtwytmvtdp.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.0kj1m.cn/gtrifzfxni.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.sysykeji.top/gtkngltcyc.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.jqgufenzy.top/gtyejcehgq.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.zdqjudy.top/gthvsmxykv.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.hongshengwenyu.top/gtzbtjaaoo.html

[H02] finally / ensure 收尾
来源：http://hz.meibo888.top/gtszqzhokx.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.hnxiangtu.top/gtqvlmiuzy.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.sxryk.cn/gtmrjwguba.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.yj20258.top/gtndnscezf.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.jinyuanbaomall.cn/gtmedmigey.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.yuanzhike.top/gtdpedhold.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.316326.xyz/gtzrhorywo.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.xuanzx.com/gtfbmntacg.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.cheryme.top/gtujgifsxo.html

[H03] 主动抛出异常
来源：http://hz.ivvv.top/gtrvsdzork.html

Py:   raise ValueError("错误信息")
来源：http://hz.shangyingyoupin.top/gtvqayakxo.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.zhongyouzk.top/gtbnxgohjw.html

JS:   throw new Error("错误信息");
来源：http://hz.ppjwa.cn/gtdphezfwm.html

TS:   throw new Error("错误信息");
来源：http://hz.zhengqikj.top/gtgyrznmaw.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.pengpengdd.cyou/gtefoeoknw.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.vqdsnc.cn/gtpkwgcdxs.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.gaohongyu789.top/gtxkknvrma.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.316326.xyz/gtfvddjvnk.html

[H04] 自定义异常类型
来源：http://hz.tanke756.top/gtstdxjzzp.html

Py:   class MyError(Exception): pass
来源：http://hz.gotoacloud.top/gtmwlffxbj.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.ywan-chungtsiang.top/gtiwnnexag.html

JS:   class MyError extends Error {}
来源：http://hz.jqgufenzy.top/gtweerwcpn.html

TS:   class MyError extends Error {}
来源：http://hz.hywenlv.cn/gtewotgass.html

Java: class MyException extends RuntimeException {}
来源：http://hz.birdmap.top/gtwnboeagi.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.chenjidiqi.icu/gtyfxattaz.html

Ruby: class MyError < StandardError; end
来源：http://hz.gogol.net.cn/gtwhjllgfi.html

C#:   class MyException : Exception {}
来源：http://hz.jinqigufen.top/gthvmrcklp.html

[H05] 捕获特定类型
来源：http://hz.sxryk.cn/gtmswzhksl.html

Py:   except ValueError as e:
来源：http://hz.jinyuanbaomall.cn/gtlesdadoz.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.aizwys.cn/gtddxezfle.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.meibo888.top/gtyftzskcz.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.jianghu66.top/gtsmtmwtnb.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.haohaochexian.top/gteldtonti.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.jianghu66.top/gtyqeaiwrv.html

Ruby: rescue ArgumentError => e
来源：http://hz.mhx1999.top/gtiyzcydyl.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.zhiwuduotai.top/gtdrexvomx.html

[H06] 可选值 / 空值安全访问
来源：http://hz.sxryk.cn/gtzsvzspfh.html

Py:   value = d.get("k") or default
来源：http://hz.shanyushiyangkeji.top/gtahhzhbxr.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.sysykeji.top/gtiaqpnnrg.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.tanke756.top/gttplarwzv.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.haohaochexian.top/gtmvktnqje.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.nanxuanxn.top/gtjgsjkuki.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.snrcjt.cn/gtnoxvuupz.html

Ruby: d&.dig(:a, :b)
来源：http://hz.meibo888.top/gtqqevflcd.html

C#:   obj?.A?.B ?? default
来源：http://hz.ydzc1.top/gtynotkpxf.html

[H07] 断言
来源：http://hz.ppjwa.cn/gtjxyzizld.html

Py:   assert x > 0, "必须为正"
来源：http://hz.guannengcc.top/gtvftolmzj.html

PHP:  assert($x > 0);
来源：http://hz.jyoumei.cn/gtfbgbgija.html

JS:   console.assert(x > 0);
来源：http://hz.daria6918.cn/gtcrkhumau.html

TS:   console.assert(x > 0);
来源：http://hz.gotoacloud.top/gtablsvlmf.html

Java: assert x > 0 : "必须为正";
来源：http://hz.hywenlv.cn/gtqncrrddz.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.aibaodan.cn/gtxvlatqhr.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.jianghu66.top/gthgjoxwor.html

C#:   Debug.Assert(x > 0);
来源：http://hz.pycfn.com/gtlacpxrvc.html

[H08] 获取错误信息与堆栈
来源：http://hz.zhiwuduotai.top/gtmiyngxpo.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.cashguo.top/gtwanuxydn.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.zhijiandao.cn/gtxwetltxf.html

JS:   e.message;  e.stack
来源：http://hz.pycfn.com/gtrmmgaplu.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.hywenlv.cn/gtvqtluxqd.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.316326.xyz/gtakuddiuy.html

Go:   err.Error()
来源：http://hz.shanyushiyangtech.top/gtawqiqoqe.html

Ruby: e.message;  e.backtrace
来源：http://hz.hnqzz.top/gtszsnxahj.html

C#:   e.Message;  e.StackTrace
来源：http://hz.hongshengwenyu.top/gtyzhmnhuf.html

[H09] 带错误码的异常
来源：http://hz.hnxiangtu.top/gtslomttxm.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.jlsjyb.cn/gtargrbmoq.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.wangdashe.top/gtwzriysaw.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.52xcode.cn/gtymuncrno.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.fengsongda.top/gtmylzwjgx.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.fzhhl.top/gtckuxraaf.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.yanxiufei.cn/gtpdotorpb.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.jlsjyb.cn/gtsmukolmo.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.hywenlv.cn/gtpamilxbn.html

[H10] 资源自动释放
来源：http://hz.gaohongyu789.top/gtgcwwfzkw.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.aibaodan.cn/gthceesold.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.guannengcc.top/gtmwomdnnm.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.jinqigufen.top/gtfrqgwowk.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.jlsjyb.cn/gttybvkoqz.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.jiagoushi.top/gtvgdvebib.html

Go:   defer f.Close()
来源：http://hz.gotoacloud.top/gtcxravxbx.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.shangyingyoupin.top/gthblzifbe.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.jinqigufen.top/gtlgmfjdhu.html

================================================================================
来源：http://hz.yueranfly.top/gtzkbywkip.html

I. 正则表达式
来源：http://hz.haohaochexian.top/gthobbmnes.html

================================================================================
来源：http://hz.sxryk.cn/gtwtcbhdge.html

[I01] 判断是否匹配
来源：http://hz.gotoacloud.top/gtkkjgtpst.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.guowangkeji.top/gtwrnhukat.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.birdmap.top/gtjlhthvky.html

JS:   /\d+/.test(s)
来源：http://hz.yueranfly.top/gtyiuqfdvd.html

TS:   /\d+/.test(s)
来源：http://hz.yj202588.top/gtfnqdwflu.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.jianghu66.top/gtfadncsbi.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.yuanzhike.top/gtathqyfkt.html

Ruby: s.match?(/\d+/)
来源：http://hz.wangshuangyany.cn/gteamqmzfa.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.vqdsnc.cn/gtdwfomldb.html

[I02] 提取所有匹配
来源：http://hz.zhengqikj.top/gtmbftcejp.html

Py:   re.findall(r"\d+", s)
来源：http://hz.tian-w.cn/gtpxrushga.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.hnxiangtu.top/gtfbncsxck.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.zhongyouzk.top/gtzjgtmuyw.html

TS:   s.match(/\d+/g)
来源：http://hz.gogol.net.cn/gtkeaepcbc.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.yuanzhike.top/gtadrjhtdi.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.zhoulong.xyz/gtnlszckmp.html

Ruby: s.scan(/\d+/)
来源：http://hz.redwolf501.top/gtdnyvntdm.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.cqqwz.cn/gtlepazpbr.html

[I03] 提取捕获分组
来源：http://hz.chenjidiqi.icu/gtxbeirprc.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.jqgfzy.top/gtskypjggu.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.mhx1999.top/gttztomvlt.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.ybcxt.top/gtwfpoqhhn.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.vqdsnc.cn/gthmwdkoqm.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.tanke756.top/gthdnotkrt.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.zhengqikj.top/gtiddbquys.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.sysykeji.top/gtwgqaxdmj.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.svipenyu.cn/gtjsdogtju.html

[I04] 正则替换
来源：http://hz.shuidangran.top/gtdbkzzvto.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.zhiwuduotai.top/gtrlybriwc.html


<!-- 参考信息 -->