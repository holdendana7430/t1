代发 wailian999

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.zdqjudy.top/gtdgywfyft.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.dashuyun.cn/gtajmhjswc.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.yj20258.top/gtdzodnspx.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.sufxvd.cn/gtploksdnb.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.svipenyu.cn/gtocpkmiyl.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.dianchejie.cn/gtgcrjlgbk.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.jiagoushi.top/gthfavdbvk.html

[F12] CSV 读写
来源：http://hz.gzhubu.top/gtxpifwyzu.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.jinghuilouyu.cn/gtthiwuljj.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.zhaomingkeji.xyz/gtzezvwswk.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.tian-w.cn/gtzglnranh.html

TS:   // 同上
来源：http://hz.daria6918.cn/gtqfaubanh.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.chenzaomai.com/gtdyqppxxv.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.iojbl.cn/gtbsoxbong.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.guowangkeji.top/gtpzyckqce.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.shuidangran.top/gtgarickyf.html

================================================================================
来源：http://hz.xuanzx.com/gtysivdoxp.html

G. 面向对象
来源：http://hz.cheryme.top/gtdynvbncy.html

================================================================================
来源：http://hz.vqdsnc.cn/gtkwkwqhdu.html

[G01] 定义类
来源：http://hz.yongpay.top/gttuhtlrpy.html

Py:   class User: pass
来源：http://hz.pycfn.com/gtamsyciug.html

PHP:  class User {}
来源：http://hz.zhaomingkeji.xyz/gthwgogxmi.html

JS:   class User {}
来源：http://hz.jiagoushi.top/gtkwwtzghc.html

TS:   class User { name: string = ""; }
来源：http://hz.mhx1999.top/gtwxddzkxj.html

Java: class User {}
来源：http://hz.ybcxt.top/gtwfajemqy.html

Go:   type User struct { Name string }
来源：http://hz.feifeiyinyue.top/gthaswhqqf.html

Ruby: class User; end
来源：http://hz.hnxiangtu.top/gtvfveyeqw.html

C#:   class User {}
来源：http://hz.cdnleiting.top/gtontynxdx.html

[G02] 构造函数
来源：http://hz.xinyue.icu/gtuppxbsjv.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.mhx1999.top/gttxjnlmrp.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.andypj.xyz/gtscqomvdt.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.hysaishi.cn/gtnreyvyif.html

TS:   constructor(public name: string) {}
来源：http://hz.ywan-chungtsiang.top/gtwbfuvndq.html

Java: User(String name) { this.name = name; }
来源：http://hz.guannengcc.top/gtegagvcre.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.jqgfzy.top/gtzhfbiody.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.sysykeji.top/gtvbrrsjih.html

C#:   public User(string name) { Name = name; }
来源：http://hz.gotoacloud.top/gtjynoazfj.html

[G03] 实例属性
来源：http://hz.gaohongyu789.top/gtwdlzbknq.html

Py:   self.name = "x"
来源：http://hz.haohaochexian.top/gtkdixdoqg.html

PHP:  public string $name = "x";
来源：http://hz.fzhhl.top/gtgmnxqjcz.html

JS:   this.name = "x";
来源：http://hz.jqgfzy.top/gtcfnaurak.html

TS:   name: string = "x";
来源：http://hz.yuanzhike.top/gtpybyaeli.html

Java: private String name;
来源：http://hz.xuanzx.com/gtjsiwbzkl.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.fzhhl.top/gtjixxgjva.html

Ruby: @name = "x"
来源：http://hz.ydzc1.top/gtdrblomxe.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.chenlongwang.top/gtvdvroozc.html

[G04] 定义方法
来源：http://hz.hnxiangtu.top/gtowfxkcvb.html

Py:   def greet(self): return self.name
来源：http://hz.jiagoushi.top/gtsqazqnmx.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.jqgfzy.top/gtbruyarac.html

JS:   greet() { return this.name; }
来源：http://hz.birdmap.top/gtpugbyvtf.html

TS:   greet(): string { return this.name; }
来源：http://hz.zdqjudy.top/gtfynavqgm.html

Java: String greet() { return name; }
来源：http://hz.sufxvd.cn/gttnxiobvo.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.52xcode.cn/gtgarwymvr.html

Ruby: def greet; @name; end
来源：http://hz.guowangkeji.top/gtntbkhkfw.html

C#:   public string Greet() => Name;
来源：http://hz.zdqjudy.top/gtbbdybhby.html

[G05] 继承
来源：http://hz.zdqjudy.top/gtvetvmwgh.html

Py:   class Admin(User): pass
来源：http://hz.shanyushiyangkeji.top/gtijxdutjc.html

PHP:  class Admin extends User {}
来源：http://hz.svipenyu.cn/gtrkmgenny.html

JS:   class Admin extends User {}
来源：http://hz.redwolf501.top/gtltdofvle.html

TS:   class Admin extends User {}
来源：http://hz.shuidangran.top/gtcepnpydo.html

Java: class Admin extends User {}
来源：http://hz.xziqi.cn/gtnuphmrhw.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.yongpay.top/gteeqeevzl.html

Ruby: class Admin < User; end
来源：http://hz.zhijiandao.cn/gtprdtjxqe.html

C#:   class Admin : User {}
来源：http://hz.nanxuanxn.top/gtbqcedhkm.html

[G06] 重写方法
来源：http://hz.shangyingyoupin.top/gtngwweicp.html

Py:   def greet(self): return "admin"
来源：http://hz.nanxinkj.top/gtbprixsoq.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.ybcxt.top/gtkwmwikyi.html

JS:   greet() { return "admin"; }
来源：http://hz.meibo888.top/gtfwplizns.html

TS:   greet(): string { return "admin"; }
来源：http://hz.wangdashe.top/gtkzbjlmfd.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.ybcxt.top/gtstlboeou.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.hywenlv.cn/gtrkcquerx.html

Ruby: def greet; "admin"; end
来源：http://hz.yvedp.cn/gtzttnbhgt.html

C#:   public override string Greet() => "admin";
来源：http://hz.yuxming.cn/gtnuamwidf.html

[G07] 调用父类方法
来源：http://hz.hysaishi.cn/gtmrdmvjes.html

Py:   super().greet()
来源：http://hz.vqdsnc.cn/gtuwpkmqia.html

PHP:  parent::greet();
来源：http://hz.guannengcc.top/gtsfbygdth.html

JS:   super.greet();
来源：http://hz.9152youxi.cn/gtmwqedhke.html

TS:   super.greet();
来源：http://hz.hnxiangtu.top/gtimhqwvbg.html

Java: super.greet();
来源：http://hz.aibaodan.cn/gtbvnwcgdz.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.yonumen.top/gtyesijrds.html

Ruby: super
来源：http://hz.iojbl.cn/gtfsrznfwj.html

C#:   base.Greet();
来源：http://hz.yj20258888.top/gtxdgqqhft.html

[G08] 静态方法与属性
来源：http://hz.vqdsnc.cn/gtditqhgbx.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.yueranfly.top/gthkdmsnsi.html

PHP:  public static function f() {}
来源：http://hz.gaohongyu789.top/gtfoqoaxsk.html

JS:   static f() {}
来源：http://hz.gogol.net.cn/gtcjwrkfxc.html

TS:   static f(): void {}
来源：http://hz.shanyushiyangkeji.top/gtsnaiyqkv.html

Java: static void f() {}
来源：http://hz.daria6918.cn/gtmfaixnfn.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.fengsongda.top/gtuyxuidpi.html

Ruby: def self.f; end
来源：http://hz.yonumen.top/gtboftgykp.html

C#:   public static void F() {}
来源：http://hz.jqgufenzy.top/gtgekqnomq.html

[G09] 接口 / 抽象类
来源：http://hz.quarkkingdee.top/gtnfpbevpp.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.yonumen.top/gtqofjjccf.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.hnxiangtu.top/gtrirmocrq.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.redwolf501.top/gtwrbdswcq.html

TS:   interface Shape { area(): number; }
来源：http://hz.jiagoushi.top/gtcccjpbvf.html

Java: interface Shape { double area(); }
来源：http://hz.hfpthk.cn/gtopasevsw.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.feifeiyinyue.top/gtfprnkjhq.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.jyoumei.cn/gtxzyyyvex.html

C#:   interface IShape { double Area(); }
来源：http://hz.xinyue.icu/gtkygsbanp.html

[G10] 访问控制
来源：http://hz.aizwys.cn/gtzdeiubkh.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.havefunace.top/gtmpqmgska.html

PHP:  public / protected / private
来源：http://hz.wangdashe.top/gtqjnspfhd.html

JS:   #private 字段；其余公开
来源：http://hz.havefunace.top/gtoskrkagf.html

TS:   public / protected / private
来源：http://hz.cashguo.top/gtaazouomb.html

Java: public / protected / private / 默认包级
来源：http://hz.chenjidiqi.icu/gthsneluwi.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.cdnleiting.top/gtsyxqobbx.html

Ruby: public / protected / private
来源：http://hz.sufxvd.cn/gtugofytjn.html

C#:   public / protected / private / internal
来源：http://hz.fzhhl.top/gtisjclqvw.html

[G11] getter / setter
来源：http://hz.52xcode.cn/gtvshmfnbv.html

Py:   @property 与 @x.setter
来源：http://hz.guannengcc.top/gtmscjrcnw.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.jinqigfzy.top/gtblplgvby.html

JS:   get name() { return this._name; }
来源：http://hz.wangdashe.top/gtgfqqcdxh.html

TS:   get name(): string { return this._name; }
来源：http://hz.dashuyun.cn/gtjkhmookm.html

Java: public String getName() { return name; }
来源：http://hz.chenzaomai.com/gtbphdqxvr.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.hongshengwenyu.top/gtlibqtxwb.html

Ruby: attr_accessor :name
来源：http://hz.hysaishi.cn/gtjvbjpfyw.html

C#:   public string Name { get; set; }
来源：http://hz.guannengcc.top/gtrvvffxdu.html

[G12] 对象转字符串
来源：http://hz.xuanzx.com/gtkojztonq.html

Py:   def __str__(self): return self.name
来源：http://hz.gaohongyu789.top/gtmfcugppu.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.pengpengdd.cyou/gtbblacvch.html

JS:   toString() { return this.name; }
来源：http://hz.zhaomingkeji.xyz/gtdwsctrba.html

TS:   toString(): string { return this.name; }
来源：http://hz.ehwqpu.com/gtzifvkxen.html

Java: @Override public String toString() { return name; }
来源：http://hz.aizwys.cn/gtrdgbrodi.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.jqgfzy.top/gtipaigdld.html

Ruby: def to_s; @name; end
来源：http://hz.zhengqikj.top/gtlpgdpvji.html

C#:   public override string ToString() => Name;
来源：http://hz.jianghu66.top/gtyirhknti.html

[G13] 判断对象类型
来源：http://hz.cqqwz.cn/gtkvsssgnb.html

Py:   isinstance(u, User)
来源：http://hz.snrcjt.cn/gttxuzeyiq.html

PHP:  $u instanceof User
来源：http://hz.gzhubu.top/gteomercll.html

JS:   u instanceof User
来源：http://hz.quarkkingdee.top/gtedqzwnbm.html

TS:   u instanceof User
来源：http://hz.zhongyouzk.top/gtlishlspv.html

Java: u instanceof User
来源：http://hz.jlsjyb.cn/gtxgqaarng.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.jianghu66.top/gtfckuxtsh.html

Ruby: u.is_a?(User)
来源：http://hz.shangyingyoupin.top/gtzvwkedkp.html

C#:   u is User
来源：http://hz.jinyuanbaomall.cn/gtcrrfsxyf.html

[G14] 数据类 / record
来源：http://hz.yonumen.top/gtwvdngjrd.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.yueranfly.top/gtnarpmwmr.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.shanyushiyangkeji.top/gtmpjmcwtc.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.snrcjt.cn/gtckcshcrk.html

TS:   type User = { name: string; age: number };
来源：http://hz.zhongyouzk.top/gtwroxihzp.html

Java: record User(String name, int age) {}
来源：http://hz.xylfe.cn/gtwvdqwpif.html

Go:   type User struct { Name string; Age int }
来源：http://hz.hywenlv.cn/gtixiuavaj.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.nanxuanxn.top/gtmsxjbjrz.html

C#:   record User(string Name, int Age);
来源：http://hz.dashuyun.cn/gtxeqphstl.html

[G15] 枚举
来源：http://hz.ehwqpu.com/gtckxeivqg.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.guowangkeji.top/gtnyusijmk.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.daria6918.cn/gtsrjokrxq.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.chenjidiqi.icu/gtnwnjljrg.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.zhoulong.xyz/gtljpheekg.html

Java: enum Color { RED, GREEN }
来源：http://hz.shanyushiyangtech.top/gtkjtszeyf.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.zhixingplan.top/gtzjqwcjhk.html

Ruby: Color = %i[red green].freeze
来源：http://hz.cucudq.cn/gtbobfcmgq.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.316326.xyz/gtrqbqlytd.html

[G16] 对象转数组 / 字典
来源：http://hz.ybcxt.top/gtapeqmcil.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.fengsongda.top/gtqdpgptte.html

PHP:  get_object_vars($obj);
来源：http://hz.cucudq.cn/gtthegonne.html

JS:   Object.entries(obj)
来源：http://hz.cucudq.cn/gtvlrtwxtw.html

TS:   Object.entries(obj)
来源：http://hz.guannengcc.top/gtnqebreim.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.yj20258888.top/gtaoorievf.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.kuanghao11.cn/gtghhzwwxd.html

Ruby: obj.instance_variables
来源：http://hz.cqqwz.cn/gtxvxhbjlq.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.xuanzx.com/gtlbdmsygv.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtvlxwodkb.html

H. 异常与错误处理
来源：http://hz.jinqigufen.top/gthsjtgwrf.html

================================================================================
来源：http://hz.zhengqikj.top/gtajyassii.html

[H01] try / catch 基础
来源：http://hz.yj20258.top/gtuwnvnvff.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.pengpengdd.cyou/gtkaduglbm.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.vqdsnc.cn/gtwxaclvro.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.aibaodan.cn/gttryqkhqv.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.shangyingyoupin.top/gtekvjkgdj.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.iojbl.cn/gtqyqtldan.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.haohaochexian.top/gterroktms.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.yvedp.cn/gtkpldoiba.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.yonumen.top/gtwqwodnyb.html

[H02] finally / ensure 收尾
来源：http://hz.tianlin.xyz/gtxmooxaxc.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.gotoacloud.top/gtiusnqedf.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.yvedp.cn/gterdftskz.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.xuetiantiany.cn/gtzuhzloaz.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.gogol.net.cn/gtjvihmekx.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.jinyuanbaomall.cn/gtufjbklzi.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.yvedp.cn/gthosordso.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.cqqwz.cn/gthvbnflok.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.yj202588.top/gtojyuwnho.html

[H03] 主动抛出异常
来源：http://hz.jinyuanbaomall.cn/gtobuplzsq.html

Py:   raise ValueError("错误信息")
来源：http://hz.gotoacloud.top/gtvvdfeiai.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.feifeiyinyue.top/gtpicgpcsz.html

JS:   throw new Error("错误信息");
来源：http://hz.jianghu66.top/gtwiesweti.html

TS:   throw new Error("错误信息");
来源：http://hz.meibo888.top/gtmssgcelj.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.snrcjt.cn/gtsaztyycd.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.ivvv.top/gtpvobhras.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.sweek.top/gtiueqzvtk.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.9152youxi.cn/gtchgheugt.html

[H04] 自定义异常类型
来源：http://hz.nanxinkj.top/gtkysbpmds.html

Py:   class MyError(Exception): pass
来源：http://hz.smart0.xyz/gtgwswtydl.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.fengsongda.top/gtxefipsud.html

JS:   class MyError extends Error {}
来源：http://hz.cdnleiting.top/gtvzwbogxs.html

TS:   class MyError extends Error {}
来源：http://hz.ydzc1.top/gtrdfkrsjd.html

Java: class MyException extends RuntimeException {}
来源：http://hz.birdmap.top/gtlupjwwqk.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.52xcode.cn/gtniyujlen.html

Ruby: class MyError < StandardError; end
来源：http://hz.ppjwa.cn/gtzhtjwxyz.html

C#:   class MyException : Exception {}
来源：http://hz.hfpthk.cn/gtzqhkobor.html

[H05] 捕获特定类型
来源：http://hz.jqgfzy.top/gtlxbldcov.html

Py:   except ValueError as e:
来源：http://hz.zhengqikj.top/gtefiyuaty.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.gotoacloud.top/gtkwvlrfit.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.gzhubu.top/gtickzfcic.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.zhijiandao.cn/gtgkcilaei.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.sufxvd.cn/gtxvdwcuro.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.yonumen.top/gtzzwwefxb.html

Ruby: rescue ArgumentError => e
来源：http://hz.316326.xyz/gtmnkvzztz.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.pycfn.com/gtenydxrpj.html

[H06] 可选值 / 空值安全访问
来源：http://hz.zycfv.cn/gtptuliyny.html

Py:   value = d.get("k") or default
来源：http://hz.sweek.top/gtgjcjjtra.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.snrcjt.cn/gtduxutaai.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.jqgfzy.top/gtyrbzpnsx.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.aizwys.cn/gtwtizaifi.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.gotoacloud.top/gtzgeybzir.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.pycfn.com/gteqfhvwkb.html

Ruby: d&.dig(:a, :b)
来源：http://hz.xuetiantiany.cn/gtmqncdkpn.html

C#:   obj?.A?.B ?? default
来源：http://hz.sysykeji.top/gttxixivkh.html

[H07] 断言
来源：http://hz.daria6918.cn/gtfzzheakt.html

Py:   assert x > 0, "必须为正"
来源：http://hz.jinqigfzy.top/gtcfudvmzm.html

PHP:  assert($x > 0);
来源：http://hz.havefunace.top/gtyuvofsga.html

JS:   console.assert(x > 0);
来源：http://hz.shzxlz.cn/gtftvgcnjq.html

TS:   console.assert(x > 0);
来源：http://hz.yj20258.top/gtheusnmby.html

Java: assert x > 0 : "必须为正";
来源：http://hz.fengsongda.top/gtjwkmbutc.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.gaohongyu789.top/gtaqoxavqi.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.ppjwa.cn/gtardksljg.html

C#:   Debug.Assert(x > 0);
来源：http://hz.birdmap.top/gttpniklba.html

[H08] 获取错误信息与堆栈
来源：http://hz.meibo888.top/gttisgtqvn.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.kuanghao11.cn/gtovfopkmb.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.gaohongyu789.top/gtaoyudycp.html

JS:   e.message;  e.stack
来源：http://hz.hysaishi.cn/gtoudpsaem.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.shuidangran.top/gtofamciro.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.bjfxy.top/gtvnullowr.html

Go:   err.Error()
来源：http://hz.shuidangran.top/gtbcrxhdji.html

Ruby: e.message;  e.backtrace
来源：http://hz.jqgufenzy.top/gtkbfigzqg.html

C#:   e.Message;  e.StackTrace
来源：http://hz.9152youxi.cn/gtiaesxert.html

[H09] 带错误码的异常
来源：http://hz.gogol.net.cn/gtzlgnrqux.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.sxryk.cn/gttuusfjew.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.cqqwz.cn/gtupuoyqpl.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.yuanzhike.top/gtxumtottv.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.hywenlv.cn/gtleeffdmt.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.xinyue.icu/gtikycymxu.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.yanxiufei.cn/gtttvgogty.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.meibo888.top/gteyqtzizt.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.jyoumei.cn/gtrffhwwrs.html

[H10] 资源自动释放
来源：http://hz.birdmap.top/gtvheqpdao.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.jqgufenzy.top/gtnqpvhenc.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.zhaomingkeji.xyz/gtswcnrlby.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.fengsongda.top/gtgmxttybp.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.cashguo.top/gtqvypcwlq.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.dianchejie.cn/gtciofypts.html

Go:   defer f.Close()
来源：http://hz.shangyingyoupin.top/gtjsplcztq.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.jinqigfzy.top/gtpwfgzxls.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.wangdashe.top/gtlpaulvzm.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtmgvrpmbt.html

I. 正则表达式
来源：http://hz.shzxlz.cn/gttkfllsty.html

================================================================================
来源：http://hz.shuidangran.top/gtxullecao.html

[I01] 判断是否匹配
来源：http://hz.aizwys.cn/gtdrzxvzxi.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.svipenyu.cn/gtbwnkmmvf.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.svipenyu.cn/gtlljirfzs.html

JS:   /\d+/.test(s)
来源：http://hz.shanyushiyangkeji.top/gtczelpkht.html

TS:   /\d+/.test(s)
来源：http://hz.sysykeji.top/gtddolhgrq.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.aibaodan.cn/gtzghyfwcd.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.hongshengwenyu.top/gtjmqwfmbp.html

Ruby: s.match?(/\d+/)
来源：http://hz.cashguo.top/gtspncjkgm.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.sufxvd.cn/gtktyosbzv.html

[I02] 提取所有匹配
来源：http://hz.smart0.xyz/gtpekyxppm.html

Py:   re.findall(r"\d+", s)
来源：http://hz.ydjk.org.cn/gtxgdjsgqn.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.52xcode.cn/gtibfpgbdj.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.jinqigfzy.top/gtxrhezrwc.html

TS:   s.match(/\d+/g)
来源：http://hz.smart0.xyz/gtksngvnqr.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.daxiang520.top/gtcxkunfmi.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.316326.xyz/gttdslyars.html

Ruby: s.scan(/\d+/)
来源：http://hz.ywan-chungtsiang.top/gtmscbatft.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.ydzc1.top/gtxtayhdos.html

[I03] 提取捕获分组
来源：http://hz.0kj1m.cn/gtrgcbjafw.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.ydzc1.top/gtexveseui.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.hnxiangtu.top/gtfnhilycf.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.fzhhl.top/gttqvjvrai.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.fzhhl.top/gtxbnpdfho.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.chenlongwang.top/gtcsxqfacf.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.guannengcc.top/gtfpqlcrcb.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.xingfuxueyuan.xyz/gtcygeruss.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.jyoumei.cn/gtrqvwctoy.html

[I04] 正则替换
来源：http://hz.hammf.cn/gtaxxksyko.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.shangyingyoupin.top/gtgbfzyraq.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.feifeiyinyue.top/gtrwmgpirf.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.cheryme.top/gtazbezdbf.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.cashguo.top/gtzbcvtohz.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.xingfuxueyuan.xyz/gtqeieluuw.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.havefunace.top/gtknvoptvo.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.vqdsnc.cn/gtgkourewr.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.ydjk.org.cn/gtfqfumxto.html

[I05] 按正则拆分
来源：http://hz.jianghu66.top/gthiijyloj.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.cheryme.top/gtpfkgfgla.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.daxiang520.top/gtkhdumtpi.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.jqgufenzy.top/gtnfevucul.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.chenzaomai.com/gtiomlcimk.html


<!-- 参考信息 -->