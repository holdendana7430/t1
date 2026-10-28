代发 wailian999

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.guannengcc.top/gtsuwgkenz.html

TS:   path.extname("a.txt")
来源：http://hz.chenlongwang.top/gtaclqdsem.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.daria6918.cn/gtxsyypmkz.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.jinghuilouyu.cn/gtdxohbqaq.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.9152youxi.cn/gtuidculkt.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.wangshuangyany.cn/gtnobrzhpk.html

[F11] 复制与移动文件
来源：http://hz.xziqi.cn/gtltckxmgv.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.guannengcc.top/gtrlxpntjx.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.shangyingyoupin.top/gtqxiouwno.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.jinqigufen.top/gtpjjyqojw.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.shuidangran.top/gtxbnywzng.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.yuanzhike.top/gtqoyjnfpx.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.xinyue.icu/gtpekcosyk.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.zhoulong.xyz/gtkpixosgs.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.yongpay.top/gtppkslmuy.html

[F12] CSV 读写
来源：http://hz.yvedp.cn/gtantqgndk.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.jiagoushi.top/gtwgdpyvfg.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.c1oappe.top/gtroiluecg.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.zhaomingkeji.xyz/gtostsaetb.html

TS:   // 同上
来源：http://hz.haohaochexian.top/gtqxkebjqa.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.haohaochexian.top/gtnzkzpioe.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.xziqi.cn/gtrnknmcgs.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.sysykeji.top/gtmwjjwboc.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.shanyushiyangtech.top/gttzcwxyxb.html

================================================================================
来源：http://hz.shzxlz.cn/gtwhieukjm.html

G. 面向对象
来源：http://hz.zhoulong.xyz/gtlqwqyspc.html

================================================================================
来源：http://hz.cheryme.top/gtythfdatg.html

[G01] 定义类
来源：http://hz.jianghu66.top/gtsziywhlx.html

Py:   class User: pass
来源：http://hz.0kj1m.cn/gtquenqdtc.html

PHP:  class User {}
来源：http://hz.tianlin.xyz/gttatkqkql.html

JS:   class User {}
来源：http://hz.gotoacloud.top/gtfgqfovbc.html

TS:   class User { name: string = ""; }
来源：http://hz.jqgufenzy.top/gtktndjduh.html

Java: class User {}
来源：http://hz.yanxiufei.cn/gtsbcdrdxv.html

Go:   type User struct { Name string }
来源：http://hz.52xcode.cn/gtjcrzclub.html

Ruby: class User; end
来源：http://hz.ywan-chungtsiang.top/gtpneuhfwd.html

C#:   class User {}
来源：http://hz.zhoulong.xyz/gthhnwmtol.html

[G02] 构造函数
来源：http://hz.jyoumei.cn/gthbnuozsl.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.xinyue.icu/gtrbxnfgye.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.xuanzx.com/gtsptjytwi.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.dashuyun.cn/gtaoahkejk.html

TS:   constructor(public name: string) {}
来源：http://hz.daria6918.cn/gthgrxsbiv.html

Java: User(String name) { this.name = name; }
来源：http://hz.zdqjudy.top/gttbiftzvp.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.haohaochexian.top/gtsglcldrz.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.yanxiufei.cn/gtuovsbtph.html

C#:   public User(string name) { Name = name; }
来源：http://hz.snrcjt.cn/gtjuqbiccm.html

[G03] 实例属性
来源：http://hz.gaohongyu789.top/gtsuemdxxy.html

Py:   self.name = "x"
来源：http://hz.jiagoushi.top/gtszpwrrbk.html

PHP:  public string $name = "x";
来源：http://hz.nwbrower.top/gtvsykfisb.html

JS:   this.name = "x";
来源：http://hz.tanke756.top/gtmhkoxebl.html

TS:   name: string = "x";
来源：http://hz.guannengcc.top/gtxjcebrfw.html

Java: private String name;
来源：http://hz.yongpay.top/gtymkofvxw.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.snrcjt.cn/gttemupwej.html

Ruby: @name = "x"
来源：http://hz.ppjwa.cn/gtuucpdyhx.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.pycfn.com/gtnspmfycw.html

[G04] 定义方法
来源：http://hz.zhengqikj.top/gtjqlpfizl.html

Py:   def greet(self): return self.name
来源：http://hz.cucudq.cn/gtkargyttk.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.ydjk.org.cn/gtrzebzqku.html

JS:   greet() { return this.name; }
来源：http://hz.jinqigfzy.top/gtiwjkxtnz.html

TS:   greet(): string { return this.name; }
来源：http://hz.jyoumei.cn/gteiowayrx.html

Java: String greet() { return name; }
来源：http://hz.yanxiufei.cn/gtllgvgozj.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.zhixingplan.top/gteflafxwl.html

Ruby: def greet; @name; end
来源：http://hz.jqgufenzy.top/gtokjarvcb.html

C#:   public string Greet() => Name;
来源：http://hz.nwbrower.top/gtbxaciwug.html

[G05] 继承
来源：http://hz.ybcxt.top/gtglfgilas.html

Py:   class Admin(User): pass
来源：http://hz.jqgfzy.top/gtufsoowfb.html

PHP:  class Admin extends User {}
来源：http://hz.yj20258.top/gtjisgygpj.html

JS:   class Admin extends User {}
来源：http://hz.aizwys.cn/gtdcfemthu.html

TS:   class Admin extends User {}
来源：http://hz.nanxuanxn.top/gthsmanzll.html

Java: class Admin extends User {}
来源：http://hz.jinqigufen.top/gtfundkdyb.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.vqdsnc.cn/gtbcmcjcas.html

Ruby: class Admin < User; end
来源：http://hz.meibo888.top/gtoirddzce.html

C#:   class Admin : User {}
来源：http://hz.xziqi.cn/gtkyfxpaps.html

[G06] 重写方法
来源：http://hz.yongpay.top/gtxcmhxbma.html

Py:   def greet(self): return "admin"
来源：http://hz.andypj.xyz/gtjudkibxb.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.jqgfzy.top/gtgtiodqzr.html

JS:   greet() { return "admin"; }
来源：http://hz.jinghuilouyu.cn/gtlduypjih.html

TS:   greet(): string { return "admin"; }
来源：http://hz.yangfankeji.com/gtoyaimate.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.yueranfly.top/gtqwozrqis.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.mhx1999.top/gtjxvnjjie.html

Ruby: def greet; "admin"; end
来源：http://hz.shangyingyoupin.top/gtxmcbyunw.html

C#:   public override string Greet() => "admin";
来源：http://hz.shuidangran.top/gtexoelfrh.html

[G07] 调用父类方法
来源：http://hz.cdnleiting.top/gtteoiinjq.html

Py:   super().greet()
来源：http://hz.chenlongwang.top/gtprgruzch.html

PHP:  parent::greet();
来源：http://hz.snrcjt.cn/gtdfkijqal.html

JS:   super.greet();
来源：http://hz.cdnleiting.top/gtvamjvsck.html

TS:   super.greet();
来源：http://hz.hywenlv.cn/gtfspdtifx.html

Java: super.greet();
来源：http://hz.ppjwa.cn/gtdzphnogx.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.jqgfzy.top/gtqleikhgw.html

Ruby: super
来源：http://hz.yonumen.top/gtckiwbaat.html

C#:   base.Greet();
来源：http://hz.yvedp.cn/gtzxbqfnjr.html

[G08] 静态方法与属性
来源：http://hz.xinyue.icu/gtyydflltj.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.hysaishi.cn/gtkngubxxh.html

PHP:  public static function f() {}
来源：http://hz.kuanghao11.cn/gteqssxcht.html

JS:   static f() {}
来源：http://hz.yanxiufei.cn/gtdfstsrkt.html

TS:   static f(): void {}
来源：http://hz.yuxming.cn/gtamkdajgq.html

Java: static void f() {}
来源：http://hz.yj20258.top/gtulnmtamm.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.svipenyu.cn/gteyxqqwsw.html

Ruby: def self.f; end
来源：http://hz.zhiwuduotai.top/gtcnawrfnb.html

C#:   public static void F() {}
来源：http://hz.yuanzhike.top/gtjltydphn.html

[G09] 接口 / 抽象类
来源：http://hz.fengsongda.top/gtkjbeewtk.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.sysykeji.top/gtnylxtvug.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.cucudq.cn/gtojlyfjnd.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.jqgfzy.top/gtdynzycda.html

TS:   interface Shape { area(): number; }
来源：http://hz.redwolf501.top/gthdvwcsaa.html

Java: interface Shape { double area(); }
来源：http://hz.yj20258.top/gtsndiinbu.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.redwolf501.top/gtbagtczpe.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.jinqigufen.top/gtaujccjbi.html

C#:   interface IShape { double Area(); }
来源：http://hz.zdqjudy.top/gtpetpudod.html

[G10] 访问控制
来源：http://hz.ppjwa.cn/gtaprlatbl.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.feifeiyinyue.top/gtxkouehvg.html

PHP:  public / protected / private
来源：http://hz.quarkkingdee.top/gtyybfzefv.html

JS:   #private 字段；其余公开
来源：http://hz.shangyingyoupin.top/gtgctowyty.html

TS:   public / protected / private
来源：http://hz.chenlongwang.top/gtkmiumbfs.html

Java: public / protected / private / 默认包级
来源：http://hz.jinghuilouyu.cn/gtrktnxnsy.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.chenzaomai.com/gtumhgblbp.html

Ruby: public / protected / private
来源：http://hz.haohaochexian.top/gtuaspfmxw.html

C#:   public / protected / private / internal
来源：http://hz.hywenlv.cn/gtlzrwuboy.html

[G11] getter / setter
来源：http://hz.52xcode.cn/gthowfjkjm.html

Py:   @property 与 @x.setter
来源：http://hz.shzxlz.cn/gtqnfibtog.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.xuanzx.com/gtuycsywip.html

JS:   get name() { return this._name; }
来源：http://hz.yueranfly.top/gttkqzmoly.html

TS:   get name(): string { return this._name; }
来源：http://hz.xuetiantiany.cn/gtpvfdyzib.html

Java: public String getName() { return name; }
来源：http://hz.9152youxi.cn/gtpletebgw.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.shanyushiyangkeji.top/gtryeifhra.html

Ruby: attr_accessor :name
来源：http://hz.cqqwz.cn/gtoomwuucs.html

C#:   public string Name { get; set; }
来源：http://hz.daxiang520.top/gtoxtowsok.html

[G12] 对象转字符串
来源：http://hz.pycfn.com/gtdbxogjon.html

Py:   def __str__(self): return self.name
来源：http://hz.shanyushiyangkeji.top/gtcvkcovts.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.redwolf501.top/gtolbqdgch.html

JS:   toString() { return this.name; }
来源：http://hz.hfpthk.cn/gtsefvetwv.html

TS:   toString(): string { return this.name; }
来源：http://hz.shanyushiyangtech.top/gtjxlduqmz.html

Java: @Override public String toString() { return name; }
来源：http://hz.dashuyun.cn/gtfkmdbisn.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.zhixingplan.top/gthiwzvqvb.html

Ruby: def to_s; @name; end
来源：http://hz.ywan-chungtsiang.top/gtiiywaqet.html

C#:   public override string ToString() => Name;
来源：http://hz.hammf.cn/gtvtmvzofh.html

[G13] 判断对象类型
来源：http://hz.dashuyun.cn/gtdsbgdwyi.html

Py:   isinstance(u, User)
来源：http://hz.cashguo.top/gtieqehxvc.html

PHP:  $u instanceof User
来源：http://hz.fzhhl.top/gtfmpuvrqd.html

JS:   u instanceof User
来源：http://hz.cucudq.cn/gtnqfzmyqg.html

TS:   u instanceof User
来源：http://hz.guowangkeji.top/gtniwghoxx.html

Java: u instanceof User
来源：http://hz.zhijiandao.cn/gtjdwuqblr.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.zdqjudy.top/gtkuhgbhpw.html

Ruby: u.is_a?(User)
来源：http://hz.xuetiantiany.cn/gtizucclfe.html

C#:   u is User
来源：http://hz.jqgufenzy.top/gtbecidalr.html

[G14] 数据类 / record
来源：http://hz.vqdsnc.cn/gtlqajnkpy.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.yj20258888.top/gtmuifdaec.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.wangdashe.top/gtuqtdylgr.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.fzhhl.top/gtfiiwdyvl.html

TS:   type User = { name: string; age: number };
来源：http://hz.tian-w.cn/gtspsmgiiq.html

Java: record User(String name, int age) {}
来源：http://hz.mhx1999.top/gtssendobq.html

Go:   type User struct { Name string; Age int }
来源：http://hz.nwbrower.top/gtwjesxpar.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.gzhubu.top/gtgkjktgxn.html

C#:   record User(string Name, int Age);
来源：http://hz.hysaishi.cn/gtqxgiyera.html

[G15] 枚举
来源：http://hz.ybcxt.top/gtgsboojcr.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.yj20258888.top/gtmeaysbkw.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.hnqzz.top/gtcfffkvel.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.zhengqikj.top/gtghxxkdro.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.nanxuanxn.top/gtynzlqmhy.html

Java: enum Color { RED, GREEN }
来源：http://hz.shuidangran.top/gtftftqrmf.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.jinghuilouyu.cn/gtjaugcrsl.html

Ruby: Color = %i[red green].freeze
来源：http://hz.yj20258888.top/gtuzjtqphz.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.mhx1999.top/gtzcskuxfk.html

[G16] 对象转数组 / 字典
来源：http://hz.zhixingplan.top/gtlofwehee.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.wangshuangyany.cn/gtvbrfkqhf.html

PHP:  get_object_vars($obj);
来源：http://hz.zhiwuduotai.top/gthingkwxx.html

JS:   Object.entries(obj)
来源：http://hz.hywenlv.cn/gtvbyifews.html

TS:   Object.entries(obj)
来源：http://hz.dashuyun.cn/gtaxobagxz.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.hfpthk.cn/gtxjjzymmz.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.xuanzx.com/gtqvbiavfs.html

Ruby: obj.instance_variables
来源：http://hz.jianghu66.top/gtcoefunkj.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.xuetiantiany.cn/gtptmfymxv.html

================================================================================
来源：http://hz.yj20258.top/gtnpiddjwo.html

H. 异常与错误处理
来源：http://hz.daria6918.cn/gtgyczhawm.html

================================================================================
来源：http://hz.pycfn.com/gtdmsqaztr.html

[H01] try / catch 基础
来源：http://hz.hongshengwenyu.top/gtlziotkgu.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.xziqi.cn/gtazbdcgpm.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.zhaomingkeji.xyz/gteueqzjry.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.zhoulong.xyz/gtjuoffvuu.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.nwbrower.top/gtwlqyjyjm.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.xylfe.cn/gtsecyhfpb.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.gogol.net.cn/gtavfdyewc.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.yj20258888.top/gtrtitunde.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.aizwys.cn/gtzayeoifk.html

[H02] finally / ensure 收尾
来源：http://hz.yongpay.top/gtdyfnparx.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.fzhhl.top/gtdcjbfkcl.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.316326.xyz/gtzkgsvgmf.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.ydzc1.top/gtcwptkokz.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.jinyuanbaomall.cn/gtzxzrjfwi.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.cucudq.cn/gtfuewcnpe.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.guannengcc.top/gtbekbokut.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.c1oappe.top/gtcczdocvp.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.jianghu66.top/gtxerxqcgd.html

[H03] 主动抛出异常
来源：http://hz.jinghuilouyu.cn/gttndgrlsg.html

Py:   raise ValueError("错误信息")
来源：http://hz.hammf.cn/gtqmdbahbu.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.jiagoushi.top/gtqxcbguvx.html

JS:   throw new Error("错误信息");
来源：http://hz.gzhubu.top/gtrrvjubrp.html

TS:   throw new Error("错误信息");
来源：http://hz.jianghu66.top/gtofyuqngi.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.bjfxy.top/gtdcvowfai.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.0kj1m.cn/gtvyykpepe.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.gaohongyu789.top/gtuzovgswe.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.aibaodan.cn/gtdzvtcmph.html

[H04] 自定义异常类型
来源：http://hz.jinyuanbaomall.cn/gtgpcmgyxz.html

Py:   class MyError(Exception): pass
来源：http://hz.yanxiufei.cn/gtlgngasxi.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.wangdashe.top/gtmkduidpv.html

JS:   class MyError extends Error {}
来源：http://hz.jinghuilouyu.cn/gtkedyirzx.html

TS:   class MyError extends Error {}
来源：http://hz.ydzc1.top/gtcuhiiqzr.html

Java: class MyException extends RuntimeException {}
来源：http://hz.ydjk.org.cn/gtemgzkvzc.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.ppjwa.cn/gtzsgbugne.html

Ruby: class MyError < StandardError; end
来源：http://hz.yanxiufei.cn/gtlxwzxogh.html

C#:   class MyException : Exception {}
来源：http://hz.shuidangran.top/gtzfrylqae.html

[H05] 捕获特定类型
来源：http://hz.xuanzx.com/gtsdwutmwh.html

Py:   except ValueError as e:
来源：http://hz.yueranfly.top/gtxxdcaaez.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.gogol.net.cn/gtrxdisocs.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.redwolf501.top/gtoejsorby.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.shangyingyoupin.top/gtrkfarroj.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.dianchejie.cn/gtadlqowhw.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.yj20258.top/gtjbuuazrl.html

Ruby: rescue ArgumentError => e
来源：http://hz.xingfuxueyuan.xyz/gtrpyagrnb.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.cashguo.top/gttitymzdu.html

[H06] 可选值 / 空值安全访问
来源：http://hz.yonumen.top/gtssprbhjy.html

Py:   value = d.get("k") or default
来源：http://hz.hongshengwenyu.top/gtwbqwjnqn.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.sxryk.cn/gtbddqvsta.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.jqgufenzy.top/gtbmeqpoiy.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.jyoumei.cn/gtuuhdwuzr.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.yj20258.top/gtknznynwu.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.pengpengdd.cyou/gtofturcuw.html

Ruby: d&.dig(:a, :b)
来源：http://hz.fengsongda.top/gtkdgnhzkv.html

C#:   obj?.A?.B ?? default
来源：http://hz.zhiwuduotai.top/gtpqjiqnfd.html

[H07] 断言
来源：http://hz.snrcjt.cn/gttzlgjpmw.html

Py:   assert x > 0, "必须为正"
来源：http://hz.wangshuangyany.cn/gtkzweyazi.html

PHP:  assert($x > 0);
来源：http://hz.316326.xyz/gtbhxtghpo.html

JS:   console.assert(x > 0);
来源：http://hz.jqgfzy.top/gtbacswhyd.html

TS:   console.assert(x > 0);
来源：http://hz.birdmap.top/gtcpqxrstv.html

Java: assert x > 0 : "必须为正";
来源：http://hz.guowangkeji.top/gtywhcrfyt.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.hnxiangtu.top/gtevmscmfx.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.chenlongwang.top/gtmewpqtps.html

C#:   Debug.Assert(x > 0);
来源：http://hz.pengpengdd.cyou/gtcvxvoshf.html

[H08] 获取错误信息与堆栈
来源：http://hz.hnxiangtu.top/gtizgrbsmm.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.nanxuanxn.top/gtzawvofre.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.yvedp.cn/gtroddvoeo.html

JS:   e.message;  e.stack
来源：http://hz.jqgfzy.top/gtneklgtcq.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.ehwqpu.com/gtuzrbmqrt.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.gotoacloud.top/gtyjaonwpb.html

Go:   err.Error()
来源：http://hz.daria6918.cn/gthnbvxnrr.html

Ruby: e.message;  e.backtrace
来源：http://hz.yvedp.cn/gtxkpjqhrp.html

C#:   e.Message;  e.StackTrace
来源：http://hz.aizwys.cn/gtdihbnnmb.html

[H09] 带错误码的异常
来源：http://hz.ehwqpu.com/gthusvfpwj.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.tanke756.top/gtviqatpnp.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.meibo888.top/gtpvxqvpce.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.redwolf501.top/gthhcqctre.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.snrcjt.cn/gtlejkzplt.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.yvedp.cn/gtukvjpzqg.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.hongshengwenyu.top/gtnefqoyfl.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.sufxvd.cn/gttnhlxkhf.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.meibo888.top/gtvzvnycdk.html

[H10] 资源自动释放
来源：http://hz.yanxiufei.cn/gthhxztyfc.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.smart0.xyz/gtiekjwvdk.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.andypj.xyz/gtmpppqzoh.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.nanxinkj.top/gtbccxypoc.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.fengsongda.top/gtxtxileoq.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.quarkkingdee.top/gteyxjcojw.html

Go:   defer f.Close()
来源：http://hz.nanxuanxn.top/gttqjawzxp.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.yongpay.top/gtyirkcbyh.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.ivvv.top/gtroddjuyv.html

================================================================================
来源：http://hz.yanxiufei.cn/gtotofimaj.html

I. 正则表达式
来源：http://hz.wangshuangyany.cn/gtealbpvpe.html

================================================================================
来源：http://hz.dashuyun.cn/gtpbjjkfef.html

[I01] 判断是否匹配
来源：http://hz.andypj.xyz/gtfvapejhi.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.zhiwuduotai.top/gtllqhjral.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.hnxiangtu.top/gtmunfyacr.html

JS:   /\d+/.test(s)
来源：http://hz.xylfe.cn/gtzqttilmy.html

TS:   /\d+/.test(s)
来源：http://hz.sysykeji.top/gttyeixiqc.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.chenzaomai.com/gtixthtakg.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.meibo888.top/gttfcitiuv.html

Ruby: s.match?(/\d+/)
来源：http://hz.ydzc1.top/gtcbhsoxen.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.wangdashe.top/gtruprsmht.html

[I02] 提取所有匹配
来源：http://hz.birdmap.top/gtuvygwllk.html

Py:   re.findall(r"\d+", s)
来源：http://hz.vqdsnc.cn/gtaujcuism.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.ehwqpu.com/gtaxtqgxdy.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.jqgfzy.top/gtcvexrmur.html

TS:   s.match(/\d+/g)
来源：http://hz.yj20258.top/gthzshzcsd.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.zdqjudy.top/gtqsswiozg.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.guannengcc.top/gtdsnyjpuc.html

Ruby: s.scan(/\d+/)
来源：http://hz.ehwqpu.com/gthiomywcj.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.shanyushiyangtech.top/gtecplvpks.html

[I03] 提取捕获分组
来源：http://hz.ivvv.top/gtlikgmdgj.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.hfpthk.cn/gtrvdnnoip.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.zhijiandao.cn/gtkzbtkope.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.zhongyouzk.top/gturzaivek.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.yonumen.top/gtorgarvis.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.yangfankeji.com/gtmsjrbfho.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.guannengcc.top/gtsrbqiukv.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.chenzaomai.com/gtwgecvukt.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.fzhhl.top/gteuyspyyg.html

[I04] 正则替换
来源：http://hz.ehwqpu.com/gtqhxmimbr.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.wangshuangyany.cn/gtukrmvxez.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.quarkkingdee.top/gtbcxuyrcb.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.mhx1999.top/gtdhevgvmu.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.chenzaomai.com/gtafwsphqc.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.yanxiufei.cn/gtqlwsahxd.html


<!-- 参考信息 -->