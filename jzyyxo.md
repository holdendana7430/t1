代发 wailian999

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.chenzaomai.com/gtzjvhoipb.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.cheryme.top/gtpopxqiuy.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.shzxlz.cn/gtyczhhlbo.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.9152youxi.cn/gtcwfyifrd.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.xinyue.icu/gtjcvfawzf.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.yonumen.top/gtobotzyyo.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.feifeiyinyue.top/gtvbzcbusy.html

[F12] CSV 读写
来源：http://hz.zycfv.cn/gtjuudkjhr.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.nanxinkj.top/gtneinosbk.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.tanke756.top/gtisinbhqx.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.sufxvd.cn/gtsfcfqqni.html

TS:   // 同上
来源：http://hz.guannengcc.top/gtpkujncuz.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.cqqwz.cn/gtzycycyus.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.jinyuanbaomall.cn/gtxbzmlink.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.daxiang520.top/gthorgtrvf.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.yj202588.top/gtidpthkjo.html

================================================================================
来源：http://hz.shzxlz.cn/gtmisiynvo.html

G. 面向对象
来源：http://hz.zhiwuduotai.top/gtyojrveni.html

================================================================================
来源：http://hz.9152youxi.cn/gtynkzsqga.html

[G01] 定义类
来源：http://hz.ydjk.org.cn/gtidcqfsis.html

Py:   class User: pass
来源：http://hz.ivvv.top/gtyfpyalft.html

PHP:  class User {}
来源：http://hz.guannengcc.top/gtpekfzgni.html

JS:   class User {}
来源：http://hz.hywenlv.cn/gtgzrjtgqx.html

TS:   class User { name: string = ""; }
来源：http://hz.bjfxy.top/gthxvlwylj.html

Java: class User {}
来源：http://hz.jiagoushi.top/gttcfzyfnh.html

Go:   type User struct { Name string }
来源：http://hz.52xcode.cn/gtvgivdqgb.html

Ruby: class User; end
来源：http://hz.zhaomingkeji.xyz/gtuastpznj.html

C#:   class User {}
来源：http://hz.birdmap.top/gtikxbodov.html

[G02] 构造函数
来源：http://hz.iojbl.cn/gtkfrpmjed.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.jqgfzy.top/gtfnixnfpb.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.sweek.top/gtlrdpdpch.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.cheryme.top/gtoneajeap.html

TS:   constructor(public name: string) {}
来源：http://hz.yonumen.top/gtzelklhnh.html

Java: User(String name) { this.name = name; }
来源：http://hz.guannengcc.top/gtbpxtyvao.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.yj202588.top/gtqocvdofk.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.sxryk.cn/gtvlrbfoff.html

C#:   public User(string name) { Name = name; }
来源：http://hz.haohaochexian.top/gtsjwaieki.html

[G03] 实例属性
来源：http://hz.birdmap.top/gtbqnzuaxu.html

Py:   self.name = "x"
来源：http://hz.chenzaomai.com/gtflgxqnnq.html

PHP:  public string $name = "x";
来源：http://hz.zhaomingkeji.xyz/gtutuuapwi.html

JS:   this.name = "x";
来源：http://hz.fengsongda.top/gtojuacmvh.html

TS:   name: string = "x";
来源：http://hz.ivvv.top/gtxaphwppw.html

Java: private String name;
来源：http://hz.dianchejie.cn/gtjbaupofw.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.fengsongda.top/gtkqnpbrpc.html

Ruby: @name = "x"
来源：http://hz.zdqjudy.top/gtnazxuosm.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.hywenlv.cn/gtjxkbcfda.html

[G04] 定义方法
来源：http://hz.jiagoushi.top/gtewsveerd.html

Py:   def greet(self): return self.name
来源：http://hz.zhixingplan.top/gtkngkbzgs.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.hfpthk.cn/gtsykyvowv.html

JS:   greet() { return this.name; }
来源：http://hz.wangdashe.top/gtmpmtkvaq.html

TS:   greet(): string { return this.name; }
来源：http://hz.tanke756.top/gtkszacfxr.html

Java: String greet() { return name; }
来源：http://hz.tanke756.top/gtrdejpifg.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.nwbrower.top/gtfgwawfcv.html

Ruby: def greet; @name; end
来源：http://hz.guannengcc.top/gtmlzjuuom.html

C#:   public string Greet() => Name;
来源：http://hz.kuanghao11.cn/gtnqhejolh.html

[G05] 继承
来源：http://hz.chenzaomai.com/gtljiliuvg.html

Py:   class Admin(User): pass
来源：http://hz.chenzaomai.com/gtipzobmdj.html

PHP:  class Admin extends User {}
来源：http://hz.havefunace.top/gtksenrejc.html

JS:   class Admin extends User {}
来源：http://hz.sweek.top/gtvvozuxiq.html

TS:   class Admin extends User {}
来源：http://hz.hnxiangtu.top/gtmvzvdkhh.html

Java: class Admin extends User {}
来源：http://hz.yuxming.cn/gtkqxxkfrv.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.hongshengwenyu.top/gtclkrssfk.html

Ruby: class Admin < User; end
来源：http://hz.ydjk.org.cn/gtwrogsewc.html

C#:   class Admin : User {}
来源：http://hz.zhengqikj.top/gtxxmitras.html

[G06] 重写方法
来源：http://hz.c1oappe.top/gtxlekmodm.html

Py:   def greet(self): return "admin"
来源：http://hz.meibo888.top/gtzvbvmpvk.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.yj20258888.top/gtmfytgkkn.html

JS:   greet() { return "admin"; }
来源：http://hz.yj202588.top/gtryrkmhss.html

TS:   greet(): string { return "admin"; }
来源：http://hz.wangdashe.top/gtrmconpww.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.wangshuangyany.cn/gttmaajvjt.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.zhaomingkeji.xyz/gtgekknbyv.html

Ruby: def greet; "admin"; end
来源：http://hz.yj20258888.top/gtnjqygppf.html

C#:   public override string Greet() => "admin";
来源：http://hz.jqgfzy.top/gtjhgxhtac.html

[G07] 调用父类方法
来源：http://hz.daxiang520.top/gtxjmbamys.html

Py:   super().greet()
来源：http://hz.zhaomingkeji.xyz/gtzmozqzbw.html

PHP:  parent::greet();
来源：http://hz.zhiwuduotai.top/gtccczgmmf.html

JS:   super.greet();
来源：http://hz.guannengcc.top/gtsbbidggr.html

TS:   super.greet();
来源：http://hz.yueranfly.top/gtgqnefdtm.html

Java: super.greet();
来源：http://hz.hysaishi.cn/gtrpivvoka.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.cashguo.top/gthafmmooe.html

Ruby: super
来源：http://hz.hnxiangtu.top/gthlxgtjkv.html

C#:   base.Greet();
来源：http://hz.tian-w.cn/gtuezmahjs.html

[G08] 静态方法与属性
来源：http://hz.wangshuangyany.cn/gtxwgudpwl.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.cqqwz.cn/gtgaavqovk.html

PHP:  public static function f() {}
来源：http://hz.hysaishi.cn/gtnpzmhite.html

JS:   static f() {}
来源：http://hz.dashuyun.cn/gtxpfphtpe.html

TS:   static f(): void {}
来源：http://hz.zhijiandao.cn/gtgoedmepl.html

Java: static void f() {}
来源：http://hz.chenzaomai.com/gtctxoomme.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.snrcjt.cn/gtswwxiita.html

Ruby: def self.f; end
来源：http://hz.vqdsnc.cn/gtcpocmzqz.html

C#:   public static void F() {}
来源：http://hz.tianlin.xyz/gtvwzjlnrp.html

[G09] 接口 / 抽象类
来源：http://hz.guannengcc.top/gtbmjnsipd.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.svipenyu.cn/gtafmiwjcq.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.zdqjudy.top/gtmnkahyes.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.iojbl.cn/gtbzcwfgra.html

TS:   interface Shape { area(): number; }
来源：http://hz.xylfe.cn/gtghmjiekl.html

Java: interface Shape { double area(); }
来源：http://hz.gaohongyu789.top/gtydjdgqdc.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.hammf.cn/gtcgygjdfa.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.dashuyun.cn/gtjrjzparh.html

C#:   interface IShape { double Area(); }
来源：http://hz.xinyue.icu/gttlphgmor.html

[G10] 访问控制
来源：http://hz.zhongyouzk.top/gtktggcxrt.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.sweek.top/gtlejtoyrn.html

PHP:  public / protected / private
来源：http://hz.daxiang520.top/gtklfdczlq.html

JS:   #private 字段；其余公开
来源：http://hz.jianghu66.top/gteffcjket.html

TS:   public / protected / private
来源：http://hz.cdnleiting.top/gtkicjxeqy.html

Java: public / protected / private / 默认包级
来源：http://hz.dianchejie.cn/gtzwhuvxvc.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.guowangkeji.top/gtsppqwxzd.html

Ruby: public / protected / private
来源：http://hz.bjfxy.top/gtjalksmpv.html

C#:   public / protected / private / internal
来源：http://hz.ivvv.top/gtidrwitbk.html

[G11] getter / setter
来源：http://hz.cdnleiting.top/gtyynxjymr.html

Py:   @property 与 @x.setter
来源：http://hz.svipenyu.cn/gtpildydps.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.wangshuangyany.cn/gtehdfvlfu.html

JS:   get name() { return this._name; }
来源：http://hz.cashguo.top/gtekjyaddf.html

TS:   get name(): string { return this._name; }
来源：http://hz.guannengcc.top/gtljpjnvpx.html

Java: public String getName() { return name; }
来源：http://hz.hammf.cn/gtzoktxhfk.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.dashuyun.cn/gtyjtylcsw.html

Ruby: attr_accessor :name
来源：http://hz.jqgfzy.top/gtviuqqaun.html

C#:   public string Name { get; set; }
来源：http://hz.snrcjt.cn/gtgpjipqhq.html

[G12] 对象转字符串
来源：http://hz.jinqigufen.top/gtnxlpfulc.html

Py:   def __str__(self): return self.name
来源：http://hz.gzhubu.top/gtlhvkukif.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.ivvv.top/gtainvgujo.html

JS:   toString() { return this.name; }
来源：http://hz.daria6918.cn/gtybqkbzce.html

TS:   toString(): string { return this.name; }
来源：http://hz.yj202588.top/gtvrarxdki.html

Java: @Override public String toString() { return name; }
来源：http://hz.sufxvd.cn/gtvfgqngfs.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.jianghu66.top/gtxtkluexy.html

Ruby: def to_s; @name; end
来源：http://hz.mhx1999.top/gteibjvbrv.html

C#:   public override string ToString() => Name;
来源：http://hz.aibaodan.cn/gtrrumdnhd.html

[G13] 判断对象类型
来源：http://hz.zycfv.cn/gtmmxudskc.html

Py:   isinstance(u, User)
来源：http://hz.aibaodan.cn/gtzwxjmzqy.html

PHP:  $u instanceof User
来源：http://hz.ivvv.top/gtkugtorcm.html

JS:   u instanceof User
来源：http://hz.sufxvd.cn/gtabayeyxj.html

TS:   u instanceof User
来源：http://hz.xuetiantiany.cn/gtenuzuhot.html

Java: u instanceof User
来源：http://hz.daxiang520.top/gtsrrpygtt.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.wangshuangyany.cn/gtjwgymcqp.html

Ruby: u.is_a?(User)
来源：http://hz.hongshengwenyu.top/gtrzurdnse.html

C#:   u is User
来源：http://hz.jqgfzy.top/gtsiaofryk.html

[G14] 数据类 / record
来源：http://hz.hnqzz.top/gtuukqymsp.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.hfpthk.cn/gtfrelqnmn.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.shzxlz.cn/gtuntrcmwq.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.daria6918.cn/gtmlkcsqvl.html

TS:   type User = { name: string; age: number };
来源：http://hz.ppjwa.cn/gtshqvhoiz.html

Java: record User(String name, int age) {}
来源：http://hz.cheryme.top/gtfgfsmcks.html

Go:   type User struct { Name string; Age int }
来源：http://hz.sxryk.cn/gtdvaxalsm.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.zhoulong.xyz/gtjybjnwfa.html

C#:   record User(string Name, int Age);
来源：http://hz.316326.xyz/gtngaqthib.html

[G15] 枚举
来源：http://hz.c1oappe.top/gtxloukyyv.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.jianghu66.top/gtljtifskb.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.xylfe.cn/gtckmjbszi.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.zycfv.cn/gtzkuzhrvl.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.hysaishi.cn/gtcmywqxhi.html

Java: enum Color { RED, GREEN }
来源：http://hz.hfpthk.cn/gtizfehplc.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.guannengcc.top/gtqrqoacqo.html

Ruby: Color = %i[red green].freeze
来源：http://hz.cashguo.top/gtkbtedkcm.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.dashuyun.cn/gtkgxbylos.html

[G16] 对象转数组 / 字典
来源：http://hz.guowangkeji.top/gthpltmcqf.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.hfpthk.cn/gtgjlkofmf.html

PHP:  get_object_vars($obj);
来源：http://hz.jianghu66.top/gtbjnmkqje.html

JS:   Object.entries(obj)
来源：http://hz.smart0.xyz/gtqahnpnyd.html

TS:   Object.entries(obj)
来源：http://hz.zhixingplan.top/gthnmnqbpe.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.sysykeji.top/gtbyxsrrpi.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.sufxvd.cn/gtmggkpghg.html

Ruby: obj.instance_variables
来源：http://hz.kuanghao11.cn/gtyzjfhqtg.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.gotoacloud.top/gtwqhyrgod.html

================================================================================
来源：http://hz.meibo888.top/gtoszrflvh.html

H. 异常与错误处理
来源：http://hz.zhongyouzk.top/gtztqmwaks.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtcfilanvm.html

[H01] try / catch 基础
来源：http://hz.hnxiangtu.top/gtciefifwr.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.316326.xyz/gtrqajougc.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.fengsongda.top/gtlneodsqd.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.sweek.top/gtbmbtbqee.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.snrcjt.cn/gtkgoilsle.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.smart0.xyz/gtrbpaaggd.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.wangdashe.top/gtdadfjslp.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.xuetiantiany.cn/gtflvwziev.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.jqgufenzy.top/gtjbzxhrom.html

[H02] finally / ensure 收尾
来源：http://hz.xuanzx.com/gtkvgbcrzd.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.ppjwa.cn/gtpktosmpq.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.chenjidiqi.icu/gtnxqlbwux.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.sxryk.cn/gtzspduydx.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.shuidangran.top/gtuhfwuzwz.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.sxryk.cn/gtvuhyvxgb.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.nanxinkj.top/gtzyuivpoq.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.ehwqpu.com/gtkfjyhbqm.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.aibaodan.cn/gtgffvxkzc.html

[H03] 主动抛出异常
来源：http://hz.shangyingyoupin.top/gtyciftkzw.html

Py:   raise ValueError("错误信息")
来源：http://hz.shuidangran.top/gtvwsniixm.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.yanxiufei.cn/gtxiwzdegc.html

JS:   throw new Error("错误信息");
来源：http://hz.daxiang520.top/gtnchwssbn.html

TS:   throw new Error("错误信息");
来源：http://hz.ppjwa.cn/gtugowotek.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.jiagoushi.top/gtrisoeznm.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.hnxiangtu.top/gtemnzrkfl.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.ybcxt.top/gtcxxznwbu.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.sxryk.cn/gtcjartjaw.html

[H04] 自定义异常类型
来源：http://hz.aibaodan.cn/gtelakjqho.html

Py:   class MyError(Exception): pass
来源：http://hz.nanxuanxn.top/gtcusodkpc.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.zhongyouzk.top/gtrxwfjmej.html

JS:   class MyError extends Error {}
来源：http://hz.zhiwuduotai.top/gtzssfllnd.html

TS:   class MyError extends Error {}
来源：http://hz.zdqjudy.top/gtsjjipvtq.html

Java: class MyException extends RuntimeException {}
来源：http://hz.hammf.cn/gtujpbjjec.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.xinyue.icu/gtdleygrzp.html

Ruby: class MyError < StandardError; end
来源：http://hz.chenlongwang.top/gtfwzivflt.html

C#:   class MyException : Exception {}
来源：http://hz.snrcjt.cn/gtvvrebukz.html

[H05] 捕获特定类型
来源：http://hz.tian-w.cn/gtukxrwrjm.html

Py:   except ValueError as e:
来源：http://hz.pengpengdd.cyou/gtbbxapaqv.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.daxiang520.top/gtylcuvqfo.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.ydjk.org.cn/gtmovxaywn.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.gzhubu.top/gtxysnicnc.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.c1oappe.top/gtwfbvlkck.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.yongpay.top/gtxhzxshgw.html

Ruby: rescue ArgumentError => e
来源：http://hz.yueranfly.top/gtdviudsoi.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.9152youxi.cn/gtejejwwot.html

[H06] 可选值 / 空值安全访问
来源：http://hz.svipenyu.cn/gtpncvrlwo.html

Py:   value = d.get("k") or default
来源：http://hz.yueranfly.top/gtovruzdnx.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.jinghuilouyu.cn/gtmpufcdsi.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.kuanghao11.cn/gtqvmcmrms.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.yueranfly.top/gtrgncryor.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.zhongyouzk.top/gthrkfvsuf.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.jlsjyb.cn/gtskvlhksi.html

Ruby: d&.dig(:a, :b)
来源：http://hz.zhiwuduotai.top/gtqwofmtor.html

C#:   obj?.A?.B ?? default
来源：http://hz.yongpay.top/gtfnuwgmgo.html

[H07] 断言
来源：http://hz.gogol.net.cn/gtnvjswiri.html

Py:   assert x > 0, "必须为正"
来源：http://hz.jinyuanbaomall.cn/gtpgyzvlwo.html

PHP:  assert($x > 0);
来源：http://hz.zdqjudy.top/gthjpgjlyl.html

JS:   console.assert(x > 0);
来源：http://hz.9152youxi.cn/gtkvpjxooz.html

TS:   console.assert(x > 0);
来源：http://hz.nanxuanxn.top/gtbkfiznjo.html

Java: assert x > 0 : "必须为正";
来源：http://hz.cucudq.cn/gtcyomfspr.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.jqgufenzy.top/gtpvaeebwd.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.svipenyu.cn/gtywjebfdo.html

C#:   Debug.Assert(x > 0);
来源：http://hz.quarkkingdee.top/gtgntrnkoc.html

[H08] 获取错误信息与堆栈
来源：http://hz.ydjk.org.cn/gtjzaszmcf.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.yangfankeji.com/gtskqyeuhc.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.hammf.cn/gtztntrpoo.html

JS:   e.message;  e.stack
来源：http://hz.jqgfzy.top/gtbyzfafcq.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.chenjidiqi.icu/gtvvtbtdsy.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.nanxuanxn.top/gtwdntzeye.html

Go:   err.Error()
来源：http://hz.feifeiyinyue.top/gtruguttvi.html

Ruby: e.message;  e.backtrace
来源：http://hz.jinqigufen.top/gtadcvbljf.html

C#:   e.Message;  e.StackTrace
来源：http://hz.zhengqikj.top/gtngufkelg.html

[H09] 带错误码的异常
来源：http://hz.xuetiantiany.cn/gtcwpojsws.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.shangyingyoupin.top/gtxcwvjzmz.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.zhengqikj.top/gtutznqskw.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.nanxuanxn.top/gtrroekfmt.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.ywan-chungtsiang.top/gtqmurxjgr.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.jqgfzy.top/gtliffftas.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.xinyue.icu/gtytyrofha.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.yj202588.top/gtslspqwyn.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.zhoulong.xyz/gtrzvxzvxm.html

[H10] 资源自动释放
来源：http://hz.yuanzhike.top/gtvrwyhfog.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.jinghuilouyu.cn/gtbvnqzixb.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.kuanghao11.cn/gtuptyodqr.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.dianchejie.cn/gtmfzpcgvg.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.jinqigfzy.top/gtwgmflyab.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.shangyingyoupin.top/gtcposxihy.html

Go:   defer f.Close()
来源：http://hz.cqqwz.cn/gtsrxttzra.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.yj20258888.top/gtxmpjkojj.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.tian-w.cn/gtsxrmkwmb.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtniqoqjqq.html

I. 正则表达式
来源：http://hz.havefunace.top/gtkhwqfzjd.html

================================================================================
来源：http://hz.fengsongda.top/gtrqlmxvix.html

[I01] 判断是否匹配
来源：http://hz.dashuyun.cn/gteidbtqth.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.ydjk.org.cn/gtzcczncsh.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.yj20258.top/gtfnqrkbqv.html

JS:   /\d+/.test(s)
来源：http://hz.xziqi.cn/gtecpcbhiz.html

TS:   /\d+/.test(s)
来源：http://hz.zhijiandao.cn/gtrthoatdn.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.yueranfly.top/gtjkypfqig.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.zdqjudy.top/gtjkwcbszz.html

Ruby: s.match?(/\d+/)
来源：http://hz.ydjk.org.cn/gtzhscpkfa.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.smart0.xyz/gtxnhhqxvj.html

[I02] 提取所有匹配
来源：http://hz.zhixingplan.top/gthhwrdior.html

Py:   re.findall(r"\d+", s)
来源：http://hz.nanxinkj.top/gtywosfziv.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.zhoulong.xyz/gtyuctycvp.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.ydjk.org.cn/gtvbdymzbf.html

TS:   s.match(/\d+/g)
来源：http://hz.dashuyun.cn/gtyyjkxyri.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.yvedp.cn/gtclmpwrrz.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.xuanzx.com/gtrtgedqyt.html

Ruby: s.scan(/\d+/)
来源：http://hz.yueranfly.top/gtblrjpjin.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.chenlongwang.top/gtvuooyqot.html

[I03] 提取捕获分组
来源：http://hz.chenlongwang.top/gtxvhjkmqw.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.fzhhl.top/gtijmswttz.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.cucudq.cn/gtxrzguiex.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.zhixingplan.top/gtgdmtrfvw.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.wangdashe.top/gtljiffedy.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.9152youxi.cn/gtdtfmjnwg.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.feifeiyinyue.top/gtnnzwscnm.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.zhaomingkeji.xyz/gtdbfinbdz.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.daria6918.cn/gtfyhbtsud.html

[I04] 正则替换
来源：http://hz.dashuyun.cn/gtcbguktwu.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.yongpay.top/gtijqgmgvk.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.gzhubu.top/gtsbiepgkl.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.jinqigfzy.top/gtrbbxigzz.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.meibo888.top/gtziicgwcv.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.hywenlv.cn/gtnzmrhuvx.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.9152youxi.cn/gtxeqdkxmz.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.birdmap.top/gtqvzgmwxm.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.yanxiufei.cn/gtdbufiyqu.html

[I05] 按正则拆分
来源：http://hz.andypj.xyz/gtocdzxknm.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.guowangkeji.top/gtmgyirerf.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.chenjidiqi.icu/gtbroarwzp.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.bjfxy.top/gtjlotyiwc.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.ywan-chungtsiang.top/gtiwgiqmun.html


<!-- 参考信息 -->