代发 wailian999

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.meibo888.top/gtelvohulv.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.snrcjt.cn/gtqherekuh.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.jyoumei.cn/gtxjlgijnt.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.tanke756.top/gtrpqosaqr.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.gotoacloud.top/gtjbiljfxi.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.0kj1m.cn/gthlhfvdjh.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.sysykeji.top/gtyzmabhab.html

[F12] CSV 读写
来源：http://hz.wangdashe.top/gtqtmqaiei.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.c1oappe.top/gtkaqexqwa.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.havefunace.top/gtowrjhmyx.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.zdqjudy.top/gtuzznyeqj.html

TS:   // 同上
来源：http://hz.quarkkingdee.top/gtytrrijeq.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.guannengcc.top/gtfmjnzikp.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.nwbrower.top/gtrkeolafq.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.xuetiantiany.cn/gtfundufwv.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.hfpthk.cn/gtqwuvruft.html

================================================================================
来源：http://hz.zdqjudy.top/gtfxguhxmi.html

G. 面向对象
来源：http://hz.ybcxt.top/gtctwxnmin.html

================================================================================
来源：http://hz.yj202588.top/gtesdpvlhx.html

[G01] 定义类
来源：http://hz.haohaochexian.top/gtykqyosbh.html

Py:   class User: pass
来源：http://hz.gzhubu.top/gtmczfpfju.html

PHP:  class User {}
来源：http://hz.ehwqpu.com/gtilrnwdna.html

JS:   class User {}
来源：http://hz.kuanghao11.cn/gtipabftnh.html

TS:   class User { name: string = ""; }
来源：http://hz.yueranfly.top/gtdivvdgph.html

Java: class User {}
来源：http://hz.zhengqikj.top/gtkeoixoxl.html

Go:   type User struct { Name string }
来源：http://hz.shanyushiyangtech.top/gtjugmwufs.html

Ruby: class User; end
来源：http://hz.zhiwuduotai.top/gtpvfpzfhk.html

C#:   class User {}
来源：http://hz.zhaomingkeji.xyz/gtiindqdfc.html

[G02] 构造函数
来源：http://hz.fengsongda.top/gtbqhjejal.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.zhijiandao.cn/gtnlzuovtt.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.xuetiantiany.cn/gtmmowfpek.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.kuanghao11.cn/gtzbdjqaoj.html

TS:   constructor(public name: string) {}
来源：http://hz.yuxming.cn/gtecadnfff.html

Java: User(String name) { this.name = name; }
来源：http://hz.daria6918.cn/gtoiqjaftf.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.hammf.cn/gtiusjzsgz.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.chenzaomai.com/gtdrxuglor.html

C#:   public User(string name) { Name = name; }
来源：http://hz.pengpengdd.cyou/gtnvtjndkg.html

[G03] 实例属性
来源：http://hz.9152youxi.cn/gtyrfrhxxk.html

Py:   self.name = "x"
来源：http://hz.sysykeji.top/gtodpibguf.html

PHP:  public string $name = "x";
来源：http://hz.yueranfly.top/gtiznegbhy.html

JS:   this.name = "x";
来源：http://hz.yonumen.top/gthrdlpkhz.html

TS:   name: string = "x";
来源：http://hz.ehwqpu.com/gtusziwdzs.html

Java: private String name;
来源：http://hz.chenlongwang.top/gtnxgbwsim.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.andypj.xyz/gtofqlfgjs.html

Ruby: @name = "x"
来源：http://hz.yj20258888.top/gtwdgnopoi.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.0kj1m.cn/gtqyeqopef.html

[G04] 定义方法
来源：http://hz.yj20258.top/gtitlddekb.html

Py:   def greet(self): return self.name
来源：http://hz.zhiwuduotai.top/gtqiqniary.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.jinyuanbaomall.cn/gtpwyebpws.html

JS:   greet() { return this.name; }
来源：http://hz.smart0.xyz/gtfswjnmbt.html

TS:   greet(): string { return this.name; }
来源：http://hz.yj202588.top/gtfmvhfwau.html

Java: String greet() { return name; }
来源：http://hz.zhixingplan.top/gtwmjwrypo.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.chenjidiqi.icu/gtubfriwsz.html

Ruby: def greet; @name; end
来源：http://hz.nwbrower.top/gtwxqwoemq.html

C#:   public string Greet() => Name;
来源：http://hz.hongshengwenyu.top/gtmvtmrxps.html

[G05] 继承
来源：http://hz.daria6918.cn/gtrslaxeqx.html

Py:   class Admin(User): pass
来源：http://hz.gotoacloud.top/gttfmtipwh.html

PHP:  class Admin extends User {}
来源：http://hz.sweek.top/gtuzlvfzfx.html

JS:   class Admin extends User {}
来源：http://hz.fengsongda.top/gtfcjydnwi.html

TS:   class Admin extends User {}
来源：http://hz.yongpay.top/gtidetqfpr.html

Java: class Admin extends User {}
来源：http://hz.aizwys.cn/gtaqgscuop.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.zhixingplan.top/gtwystxbow.html

Ruby: class Admin < User; end
来源：http://hz.gotoacloud.top/gtzgqpnqhp.html

C#:   class Admin : User {}
来源：http://hz.smart0.xyz/gttnukvpzd.html

[G06] 重写方法
来源：http://hz.hongshengwenyu.top/gtgptgyvgp.html

Py:   def greet(self): return "admin"
来源：http://hz.zhongyouzk.top/gtjpjnyzwj.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.0kj1m.cn/gtntpsrqka.html

JS:   greet() { return "admin"; }
来源：http://hz.zdqjudy.top/gtfiglfooo.html

TS:   greet(): string { return "admin"; }
来源：http://hz.daria6918.cn/gtbirgsicr.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.hysaishi.cn/gtegwugitu.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.xingfuxueyuan.xyz/gtnoyeahqs.html

Ruby: def greet; "admin"; end
来源：http://hz.xuanzx.com/gtiqmjeuvh.html

C#:   public override string Greet() => "admin";
来源：http://hz.yangfankeji.com/gtxrbiieub.html

[G07] 调用父类方法
来源：http://hz.jiagoushi.top/gtuashegwe.html

Py:   super().greet()
来源：http://hz.quarkkingdee.top/gtakdasekc.html

PHP:  parent::greet();
来源：http://hz.yongpay.top/gtiffeutfg.html

JS:   super.greet();
来源：http://hz.cheryme.top/gttflnjore.html

TS:   super.greet();
来源：http://hz.meibo888.top/gtkeipueqc.html

Java: super.greet();
来源：http://hz.zhengqikj.top/gtnfhxijeq.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.gzhubu.top/gtihpgragk.html

Ruby: super
来源：http://hz.hongshengwenyu.top/gtotvccogn.html

C#:   base.Greet();
来源：http://hz.jyoumei.cn/gtoqtyooso.html

[G08] 静态方法与属性
来源：http://hz.hfpthk.cn/gtlalkqmcw.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.9152youxi.cn/gtljlfsfsw.html

PHP:  public static function f() {}
来源：http://hz.wangshuangyany.cn/gtfsxmdbuk.html

JS:   static f() {}
来源：http://hz.ppjwa.cn/gtpvfisish.html

TS:   static f(): void {}
来源：http://hz.aibaodan.cn/gtchebziro.html

Java: static void f() {}
来源：http://hz.zhaomingkeji.xyz/gtrpguactq.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.zhixingplan.top/gtwnugwjzq.html

Ruby: def self.f; end
来源：http://hz.jinqigufen.top/gtpnuvjtdy.html

C#:   public static void F() {}
来源：http://hz.dashuyun.cn/gtpzdphhjh.html

[G09] 接口 / 抽象类
来源：http://hz.ybcxt.top/gtpjdkhbnv.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.cqqwz.cn/gtzrwfjobt.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.wangshuangyany.cn/gtwubatbor.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.jinyuanbaomall.cn/gtmxpjihja.html

TS:   interface Shape { area(): number; }
来源：http://hz.vqdsnc.cn/gtnuveifzu.html

Java: interface Shape { double area(); }
来源：http://hz.daxiang520.top/gtvptuyhqm.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.iojbl.cn/gtcspgdysr.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.sysykeji.top/gtodwwmrun.html

C#:   interface IShape { double Area(); }
来源：http://hz.tanke756.top/gtjibqcmhy.html

[G10] 访问控制
来源：http://hz.jinqigfzy.top/gtquqksymw.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.iojbl.cn/gtnofsxrip.html

PHP:  public / protected / private
来源：http://hz.guannengcc.top/gtgbvquzcj.html

JS:   #private 字段；其余公开
来源：http://hz.daria6918.cn/gtbrwnxbdf.html

TS:   public / protected / private
来源：http://hz.hnxiangtu.top/gtmqntcahv.html

Java: public / protected / private / 默认包级
来源：http://hz.jqgfzy.top/gtempnefwt.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.jiagoushi.top/gtvlitfngf.html

Ruby: public / protected / private
来源：http://hz.cqqwz.cn/gtnsniwjpj.html

C#:   public / protected / private / internal
来源：http://hz.yongpay.top/gtzieqbayr.html

[G11] getter / setter
来源：http://hz.fzhhl.top/gtlhwfhufr.html

Py:   @property 与 @x.setter
来源：http://hz.hnqzz.top/gtrtzmkwio.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.svipenyu.cn/gtfpvckhie.html

JS:   get name() { return this._name; }
来源：http://hz.cheryme.top/gtkysuzdyw.html

TS:   get name(): string { return this._name; }
来源：http://hz.fengsongda.top/gteqlzcbnx.html

Java: public String getName() { return name; }
来源：http://hz.nanxinkj.top/gtsqwkszfg.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.jiagoushi.top/gtnnhyooxh.html

Ruby: attr_accessor :name
来源：http://hz.iojbl.cn/gtjwqrgguc.html

C#:   public string Name { get; set; }
来源：http://hz.zhaomingkeji.xyz/gttdznlqct.html

[G12] 对象转字符串
来源：http://hz.jinqigfzy.top/gttdkpmlyo.html

Py:   def __str__(self): return self.name
来源：http://hz.shuidangran.top/gtxylcocgk.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.hywenlv.cn/gttnnjeyab.html

JS:   toString() { return this.name; }
来源：http://hz.yvedp.cn/gtxnljlpmj.html

TS:   toString(): string { return this.name; }
来源：http://hz.jqgfzy.top/gtmsmfkpuc.html

Java: @Override public String toString() { return name; }
来源：http://hz.jinqigfzy.top/gtwojrcpdm.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.aibaodan.cn/gtxgsixwdg.html

Ruby: def to_s; @name; end
来源：http://hz.tian-w.cn/gtvgeypujz.html

C#:   public override string ToString() => Name;
来源：http://hz.tianlin.xyz/gtelzueoyp.html

[G13] 判断对象类型
来源：http://hz.yueranfly.top/gtiyfruhsu.html

Py:   isinstance(u, User)
来源：http://hz.hnxiangtu.top/gtimqvmien.html

PHP:  $u instanceof User
来源：http://hz.sweek.top/gtaykplyug.html

JS:   u instanceof User
来源：http://hz.andypj.xyz/gtzwqkrcqu.html

TS:   u instanceof User
来源：http://hz.ywan-chungtsiang.top/gtsglexyzw.html

Java: u instanceof User
来源：http://hz.redwolf501.top/gtareezkkc.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.yangfankeji.com/gtxevyxpzq.html

Ruby: u.is_a?(User)
来源：http://hz.havefunace.top/gtpikkdfms.html

C#:   u is User
来源：http://hz.fzhhl.top/gtpjgybead.html

[G14] 数据类 / record
来源：http://hz.jyoumei.cn/gtsrivtavw.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.yj202588.top/gtplsqihim.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.aibaodan.cn/gttpivhauz.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.nanxuanxn.top/gtgeotueid.html

TS:   type User = { name: string; age: number };
来源：http://hz.gaohongyu789.top/gteowctphx.html

Java: record User(String name, int age) {}
来源：http://hz.yuanzhike.top/gtnyzuiflo.html

Go:   type User struct { Name string; Age int }
来源：http://hz.hfpthk.cn/gtwzmahnwx.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.xylfe.cn/gthtepiczc.html

C#:   record User(string Name, int Age);
来源：http://hz.gaohongyu789.top/gtxwpetiuk.html

[G15] 枚举
来源：http://hz.pengpengdd.cyou/gtlynfosxf.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.nanxinkj.top/gtfyzbumqx.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.yuxming.cn/gteuukoymr.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.zhoulong.xyz/gtfwlgdsxo.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.zhengqikj.top/gtqvvujegu.html

Java: enum Color { RED, GREEN }
来源：http://hz.zhaomingkeji.xyz/gtvchbvete.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.chenlongwang.top/gtartjlynb.html

Ruby: Color = %i[red green].freeze
来源：http://hz.yongpay.top/gtkfxczpiz.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.tianlin.xyz/gtjwceomuk.html

[G16] 对象转数组 / 字典
来源：http://hz.guannengcc.top/gtsepkxzyp.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.mhx1999.top/gtgbnmlimk.html

PHP:  get_object_vars($obj);
来源：http://hz.c1oappe.top/gtytsfbspc.html

JS:   Object.entries(obj)
来源：http://hz.dianchejie.cn/gtadbnadqv.html

TS:   Object.entries(obj)
来源：http://hz.havefunace.top/gtowifpewr.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.chenzaomai.com/gtzidmlryz.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.cucudq.cn/gtmcrgylyc.html

Ruby: obj.instance_variables
来源：http://hz.cdnleiting.top/gtnsswqpra.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.fzhhl.top/gttitrkvpy.html

================================================================================
来源：http://hz.cashguo.top/gtufkhjkry.html

H. 异常与错误处理
来源：http://hz.guowangkeji.top/gtfzhzcuvy.html

================================================================================
来源：http://hz.smart0.xyz/gtnyaveewl.html

[H01] try / catch 基础
来源：http://hz.aibaodan.cn/gtsdhdtbrm.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.nwbrower.top/gtagmvjior.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.nanxinkj.top/gtpmbqpwmz.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.wangdashe.top/gtojahccxe.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.guannengcc.top/gttfnkihti.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.xylfe.cn/gtytawppfe.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.kuanghao11.cn/gtdzjwlzhf.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.daria6918.cn/gtrosukals.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.tianlin.xyz/gtbxhvkzyq.html

[H02] finally / ensure 收尾
来源：http://hz.quarkkingdee.top/gtvxfalwnz.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.gogol.net.cn/gtzdoaiszf.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.yonumen.top/gtuednvwih.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.jqgfzy.top/gtsibajjgo.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.dashuyun.cn/gtkurfkrrj.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.jlsjyb.cn/gtimyiqhir.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.feifeiyinyue.top/gtjplpyozd.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.yangfankeji.com/gtkgmbcdzi.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.zhaomingkeji.xyz/gtagggjayq.html

[H03] 主动抛出异常
来源：http://hz.sxryk.cn/gtmordxdwi.html

Py:   raise ValueError("错误信息")
来源：http://hz.ywan-chungtsiang.top/gtjcnuafwv.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.hfpthk.cn/gtjeshaqye.html

JS:   throw new Error("错误信息");
来源：http://hz.aibaodan.cn/gtaqmccekg.html

TS:   throw new Error("错误信息");
来源：http://hz.feifeiyinyue.top/gtuovuhtki.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.ybcxt.top/gtzsezeshm.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.meibo888.top/gthklbctgy.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.hnqzz.top/gtgjshhiiy.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.52xcode.cn/gtwzojcdjw.html

[H04] 自定义异常类型
来源：http://hz.xylfe.cn/gtfldevvox.html

Py:   class MyError(Exception): pass
来源：http://hz.nanxuanxn.top/gtnkjwhmjs.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.redwolf501.top/gtedsnxdax.html

JS:   class MyError extends Error {}
来源：http://hz.hysaishi.cn/gtzzkosnks.html

TS:   class MyError extends Error {}
来源：http://hz.yonumen.top/gtfrerpmnu.html

Java: class MyException extends RuntimeException {}
来源：http://hz.redwolf501.top/gtbxsmxrau.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.chenzaomai.com/gtuvpliobi.html

Ruby: class MyError < StandardError; end
来源：http://hz.shuidangran.top/gttceorfvy.html

C#:   class MyException : Exception {}
来源：http://hz.chenzaomai.com/gtlrvaaalg.html

[H05] 捕获特定类型
来源：http://hz.iojbl.cn/gtgboiowzk.html

Py:   except ValueError as e:
来源：http://hz.tanke756.top/gtfddviipb.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.yueranfly.top/gtpglyrock.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.hammf.cn/gtipwjgufc.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.jqgufenzy.top/gtggxoorxg.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.xuetiantiany.cn/gtagfszonr.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.jianghu66.top/gtdwspsdeo.html

Ruby: rescue ArgumentError => e
来源：http://hz.birdmap.top/gtfirzimfr.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.zhiwuduotai.top/gttspanxch.html

[H06] 可选值 / 空值安全访问
来源：http://hz.52xcode.cn/gtrebnceoz.html

Py:   value = d.get("k") or default
来源：http://hz.zhiwuduotai.top/gtatjwlfxa.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.hongshengwenyu.top/gtxrchbguw.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.xylfe.cn/gtxefifabg.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.nanxuanxn.top/gtzdzzxckt.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.tianlin.xyz/gtrohqkjqb.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.chenzaomai.com/gtjsgegkag.html

Ruby: d&.dig(:a, :b)
来源：http://hz.jyoumei.cn/gthhsmjzbc.html

C#:   obj?.A?.B ?? default
来源：http://hz.xuetiantiany.cn/gtqfrbvfyp.html

[H07] 断言
来源：http://hz.jqgfzy.top/gtobqsgdfl.html

Py:   assert x > 0, "必须为正"
来源：http://hz.pycfn.com/gtxgrrdaws.html

PHP:  assert($x > 0);
来源：http://hz.sweek.top/gtrdmsojjw.html

JS:   console.assert(x > 0);
来源：http://hz.ivvv.top/gtgyeqzwrj.html

TS:   console.assert(x > 0);
来源：http://hz.fengsongda.top/gtgvmqmpqh.html

Java: assert x > 0 : "必须为正";
来源：http://hz.cqqwz.cn/gthssbrgya.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.mhx1999.top/gtiabhqgjz.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.havefunace.top/gtgmsqgaum.html

C#:   Debug.Assert(x > 0);
来源：http://hz.jinghuilouyu.cn/gteisxahmx.html

[H08] 获取错误信息与堆栈
来源：http://hz.gaohongyu789.top/gtonuntgej.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.zhoulong.xyz/gtqbjwiede.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.ywan-chungtsiang.top/gtgslgceox.html

JS:   e.message;  e.stack
来源：http://hz.dashuyun.cn/gtxqpwrndd.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.hnqzz.top/gtnrjyimjo.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.ydzc1.top/gtidkuibpr.html

Go:   err.Error()
来源：http://hz.gaohongyu789.top/gtrgsuzrmy.html

Ruby: e.message;  e.backtrace
来源：http://hz.hfpthk.cn/gtlintqcke.html

C#:   e.Message;  e.StackTrace
来源：http://hz.sufxvd.cn/gtmjzivqnj.html

[H09] 带错误码的异常
来源：http://hz.snrcjt.cn/gtiktdcpkq.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.zhiwuduotai.top/gtcbyiwykw.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.jinqigfzy.top/gtehcuvzol.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.xuanzx.com/gtekeaeorz.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.sufxvd.cn/gtbdiketth.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.ivvv.top/gtxfwiejzm.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.52xcode.cn/gtogfqhrda.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.snrcjt.cn/gtoiasxpvm.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.zhiwuduotai.top/gtgujfdsif.html

[H10] 资源自动释放
来源：http://hz.jyoumei.cn/gttrwtrcso.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.shanyushiyangkeji.top/gtgruxuwld.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.jinqigfzy.top/gtoihwqubt.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.yueranfly.top/gtbtnusakq.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.xziqi.cn/gtslmkxalq.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.chenzaomai.com/gtrxsfvvet.html

Go:   defer f.Close()
来源：http://hz.guowangkeji.top/gtvpehmisr.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.zhaomingkeji.xyz/gtsbbxgyoc.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.xinyue.icu/gtjxzcpucx.html

================================================================================
来源：http://hz.bjfxy.top/gtdczqfeta.html

I. 正则表达式
来源：http://hz.kuanghao11.cn/gtalmwxmns.html

================================================================================
来源：http://hz.xylfe.cn/gtbafaonsk.html

[I01] 判断是否匹配
来源：http://hz.hywenlv.cn/gtcitodnkd.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.hfpthk.cn/gtlbgeulpo.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.9152youxi.cn/gtmxtbvfpg.html

JS:   /\d+/.test(s)
来源：http://hz.wangdashe.top/gtmcogsiao.html

TS:   /\d+/.test(s)
来源：http://hz.ydjk.org.cn/gtkvvgvzcz.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.fzhhl.top/gtsehzizgy.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.hnqzz.top/gtlvcfyceu.html

Ruby: s.match?(/\d+/)
来源：http://hz.yuxming.cn/gtvebgbflg.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.pycfn.com/gtildaffsl.html

[I02] 提取所有匹配
来源：http://hz.yongpay.top/gtzjcgxgvv.html

Py:   re.findall(r"\d+", s)
来源：http://hz.tian-w.cn/gtsqptyiam.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.quarkkingdee.top/gtwxddtiec.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.wangshuangyany.cn/gtjggmdptj.html

TS:   s.match(/\d+/g)
来源：http://hz.jlsjyb.cn/gtmdqesktm.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.yonumen.top/gtlukxgetr.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.shzxlz.cn/gtacdkybcp.html

Ruby: s.scan(/\d+/)
来源：http://hz.gogol.net.cn/gtnqjikbku.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.0kj1m.cn/gtgvwysdqk.html

[I03] 提取捕获分组
来源：http://hz.feifeiyinyue.top/gtrbxskxss.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.shanyushiyangtech.top/gtozjjwgdp.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.gaohongyu789.top/gtbgnacoap.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.zhiwuduotai.top/gtfhjlloqk.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.kuanghao11.cn/gtgaegjufb.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.jyoumei.cn/gtojilqsvk.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.zhiwuduotai.top/gtaldsywwt.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.hfpthk.cn/gtmgfoylwf.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.cashguo.top/gtlqqoomqy.html

[I04] 正则替换
来源：http://hz.zhongyouzk.top/gtlsmizdtj.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.jlsjyb.cn/gtimkzrqkf.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.zdqjudy.top/gtakrdzukf.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.zhengqikj.top/gthepryzdi.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.pengpengdd.cyou/gtirxrnddv.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.jyoumei.cn/gthippjfpm.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.haohaochexian.top/gtwqhohctv.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.xziqi.cn/gtwkgfhwir.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.cqqwz.cn/gtdorzhpyq.html

[I05] 按正则拆分
来源：http://hz.jinqigfzy.top/gteednuogp.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.fengsongda.top/gtugooqfgg.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.wangdashe.top/gtbhnvzlro.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.yj202588.top/gtkgtqzfjl.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.shanyushiyangkeji.top/gtibxvzbto.html


<!-- 参考信息 -->