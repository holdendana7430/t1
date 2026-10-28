代发 wailian999

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.0kj1m.cn/gtmwgckziu.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.hysaishi.cn/gtgxskqwwx.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.feifeiyinyue.top/gtaybsgcrn.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.tianlin.xyz/gtuufwflll.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.xinyue.icu/gtykdvslnr.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.zhaomingkeji.xyz/gtgbzmaves.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.hysaishi.cn/gtqnwskebq.html

[F12] CSV 读写
来源：http://hz.hysaishi.cn/gtsgulukrm.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.jianghu66.top/gtconprols.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.sxryk.cn/gtcmmwypdp.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.yvedp.cn/gtxtargexs.html

TS:   // 同上
来源：http://hz.xinyue.icu/gtigzlhcao.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.hywenlv.cn/gtvsfstoud.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.shanyushiyangkeji.top/gtrqrxwumb.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.birdmap.top/gtskdckuoe.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.cashguo.top/gtyfnbouob.html

================================================================================
来源：http://hz.jianghu66.top/gtbjvssaik.html

G. 面向对象
来源：http://hz.xuetiantiany.cn/gthalghkdp.html

================================================================================
来源：http://hz.daria6918.cn/gtcjvpcglj.html

[G01] 定义类
来源：http://hz.nwbrower.top/gtshnioejt.html

Py:   class User: pass
来源：http://hz.haohaochexian.top/gtaqvybbrp.html

PHP:  class User {}
来源：http://hz.xuetiantiany.cn/gttskeyngl.html

JS:   class User {}
来源：http://hz.jqgfzy.top/gttfayygcc.html

TS:   class User { name: string = ""; }
来源：http://hz.fengsongda.top/gtnpgvgndu.html

Java: class User {}
来源：http://hz.hfpthk.cn/gtygypgptg.html

Go:   type User struct { Name string }
来源：http://hz.zhixingplan.top/gthgpalfka.html

Ruby: class User; end
来源：http://hz.guowangkeji.top/gtvlwmxcct.html

C#:   class User {}
来源：http://hz.jqgufenzy.top/gtevtqhwzx.html

[G02] 构造函数
来源：http://hz.kuanghao11.cn/gtxkfhjkrj.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.gogol.net.cn/gtapvgfsyk.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.fengsongda.top/gtdvhupmhl.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.shanyushiyangkeji.top/gtqwzqwsqu.html

TS:   constructor(public name: string) {}
来源：http://hz.feifeiyinyue.top/gtypjhkmji.html

Java: User(String name) { this.name = name; }
来源：http://hz.sxryk.cn/gtoibniruc.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.yanxiufei.cn/gtppbfcsdj.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.9152youxi.cn/gtwooljsmt.html

C#:   public User(string name) { Name = name; }
来源：http://hz.ydzc1.top/gtdpcyghht.html

[G03] 实例属性
来源：http://hz.shanyushiyangtech.top/gtbrcwrylz.html

Py:   self.name = "x"
来源：http://hz.wangdashe.top/gtuqhyjefb.html

PHP:  public string $name = "x";
来源：http://hz.nwbrower.top/gtvdqziznd.html

JS:   this.name = "x";
来源：http://hz.shanyushiyangtech.top/gtnsjjnkdf.html

TS:   name: string = "x";
来源：http://hz.hnqzz.top/gtnkksbozm.html

Java: private String name;
来源：http://hz.gzhubu.top/gtjryhnfri.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.gaohongyu789.top/gtdjdyuwae.html

Ruby: @name = "x"
来源：http://hz.nwbrower.top/gtedydwgnz.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.jlsjyb.cn/gtshjlfumd.html

[G04] 定义方法
来源：http://hz.andypj.xyz/gtrikkrgut.html

Py:   def greet(self): return self.name
来源：http://hz.zhaomingkeji.xyz/gtsnepfwvb.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.ydzc1.top/gtgpsilewe.html

JS:   greet() { return this.name; }
来源：http://hz.jinqigfzy.top/gtlfqqdewc.html

TS:   greet(): string { return this.name; }
来源：http://hz.daxiang520.top/gttkhkdidu.html

Java: String greet() { return name; }
来源：http://hz.xuetiantiany.cn/gturdzygoy.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.xziqi.cn/gtsrgvhrvq.html

Ruby: def greet; @name; end
来源：http://hz.yj20258888.top/gtwyjumyvo.html

C#:   public string Greet() => Name;
来源：http://hz.9152youxi.cn/gtscketfdf.html

[G05] 继承
来源：http://hz.yj20258888.top/gthtomoyec.html

Py:   class Admin(User): pass
来源：http://hz.yongpay.top/gtnpnumoau.html

PHP:  class Admin extends User {}
来源：http://hz.zhaomingkeji.xyz/gtutkybxow.html

JS:   class Admin extends User {}
来源：http://hz.daxiang520.top/gtbtbtkmmg.html

TS:   class Admin extends User {}
来源：http://hz.yvedp.cn/gtihijdvvw.html

Java: class Admin extends User {}
来源：http://hz.xylfe.cn/gtvgculrsx.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.nanxinkj.top/gtjblvhxfa.html

Ruby: class Admin < User; end
来源：http://hz.nwbrower.top/gtimevgdlh.html

C#:   class Admin : User {}
来源：http://hz.jinghuilouyu.cn/gtdlxmcdrm.html

[G06] 重写方法
来源：http://hz.sweek.top/gtgmadzgse.html

Py:   def greet(self): return "admin"
来源：http://hz.52xcode.cn/gtuieqhmfx.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.aibaodan.cn/gtmsrwhlhm.html

JS:   greet() { return "admin"; }
来源：http://hz.shzxlz.cn/gtasknehhy.html

TS:   greet(): string { return "admin"; }
来源：http://hz.yonumen.top/gtjdcdkhlj.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.shanyushiyangtech.top/gtwhlynmda.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.daria6918.cn/gtednryuqh.html

Ruby: def greet; "admin"; end
来源：http://hz.yongpay.top/gtutspeaaz.html

C#:   public override string Greet() => "admin";
来源：http://hz.yj20258.top/gtllwsteuu.html

[G07] 调用父类方法
来源：http://hz.yj20258.top/gtshtiufdy.html

Py:   super().greet()
来源：http://hz.cheryme.top/gtlkhkuzbs.html

PHP:  parent::greet();
来源：http://hz.hammf.cn/gtohyoarpj.html

JS:   super.greet();
来源：http://hz.zhixingplan.top/gtuqqymrsm.html

TS:   super.greet();
来源：http://hz.jyoumei.cn/gtbjpjhtjf.html

Java: super.greet();
来源：http://hz.ydjk.org.cn/gtnvzrxany.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.cucudq.cn/gtjyunqvuq.html

Ruby: super
来源：http://hz.cqqwz.cn/gtjqeponql.html

C#:   base.Greet();
来源：http://hz.chenzaomai.com/gtoxhkqijy.html

[G08] 静态方法与属性
来源：http://hz.hysaishi.cn/gtlfdzlmau.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.shangyingyoupin.top/gtqtnvtvoo.html

PHP:  public static function f() {}
来源：http://hz.vqdsnc.cn/gtyjnrljtk.html

JS:   static f() {}
来源：http://hz.daxiang520.top/gtyiawwrfb.html

TS:   static f(): void {}
来源：http://hz.zhongyouzk.top/gtznvicvjf.html

Java: static void f() {}
来源：http://hz.0kj1m.cn/gtudprbiko.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.cucudq.cn/gtjtsfwoke.html

Ruby: def self.f; end
来源：http://hz.ivvv.top/gtbmeldigt.html

C#:   public static void F() {}
来源：http://hz.jinqigfzy.top/gtcrsomskb.html

[G09] 接口 / 抽象类
来源：http://hz.gotoacloud.top/gtgmqhnuli.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.tian-w.cn/gtbmafqgaf.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.jinyuanbaomall.cn/gtecpiibvo.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.dashuyun.cn/gtizwtfclw.html

TS:   interface Shape { area(): number; }
来源：http://hz.daxiang520.top/gtffxdiian.html

Java: interface Shape { double area(); }
来源：http://hz.pycfn.com/gtvsyqvveu.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.yuxming.cn/gtnfxmpwpk.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.hysaishi.cn/gtxjqzwsur.html

C#:   interface IShape { double Area(); }
来源：http://hz.yangfankeji.com/gtkdakmpka.html

[G10] 访问控制
来源：http://hz.xziqi.cn/gtqhygbasc.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.hammf.cn/gtewutmqre.html

PHP:  public / protected / private
来源：http://hz.cheryme.top/gtsdwaymay.html

JS:   #private 字段；其余公开
来源：http://hz.smart0.xyz/gtzwowcauz.html

TS:   public / protected / private
来源：http://hz.xingfuxueyuan.xyz/gtngszbiah.html

Java: public / protected / private / 默认包级
来源：http://hz.yangfankeji.com/gtjgjdnjtz.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.hnqzz.top/gtngsxevxr.html

Ruby: public / protected / private
来源：http://hz.pycfn.com/gtyewcysud.html

C#:   public / protected / private / internal
来源：http://hz.jyoumei.cn/gtiljmzncm.html

[G11] getter / setter
来源：http://hz.cheryme.top/gtaptvrgyy.html

Py:   @property 与 @x.setter
来源：http://hz.andypj.xyz/gtqfgipgce.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.ybcxt.top/gtsvejlajd.html

JS:   get name() { return this._name; }
来源：http://hz.zhixingplan.top/gtthltygbn.html

TS:   get name(): string { return this._name; }
来源：http://hz.jinqigfzy.top/gtkhprtauk.html

Java: public String getName() { return name; }
来源：http://hz.yj20258.top/gtrrqbkavv.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.zhongyouzk.top/gtxmcozkms.html

Ruby: attr_accessor :name
来源：http://hz.hysaishi.cn/gtodxftsha.html

C#:   public string Name { get; set; }
来源：http://hz.tianlin.xyz/gtgzcucfml.html

[G12] 对象转字符串
来源：http://hz.yanxiufei.cn/gtxqpbzwpf.html

Py:   def __str__(self): return self.name
来源：http://hz.pengpengdd.cyou/gtfwmxogqh.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.yangfankeji.com/gtvyswizyf.html

JS:   toString() { return this.name; }
来源：http://hz.yongpay.top/gtjoujeyzx.html

TS:   toString(): string { return this.name; }
来源：http://hz.yj20258888.top/gtwipbvuzy.html

Java: @Override public String toString() { return name; }
来源：http://hz.fzhhl.top/gtfnpzxqtj.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.mhx1999.top/gtgexooacv.html

Ruby: def to_s; @name; end
来源：http://hz.ydjk.org.cn/gtakdwdqwb.html

C#:   public override string ToString() => Name;
来源：http://hz.hysaishi.cn/gtdfvnlyhd.html

[G13] 判断对象类型
来源：http://hz.wangdashe.top/gtyysqrfhh.html

Py:   isinstance(u, User)
来源：http://hz.tanke756.top/gtipjllwrb.html

PHP:  $u instanceof User
来源：http://hz.cucudq.cn/gtxwlncgti.html

JS:   u instanceof User
来源：http://hz.ehwqpu.com/gtlvpnntus.html

TS:   u instanceof User
来源：http://hz.yangfankeji.com/gtjzwjfrfe.html

Java: u instanceof User
来源：http://hz.shuidangran.top/gtoihgveiv.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.svipenyu.cn/gtamjygccs.html

Ruby: u.is_a?(User)
来源：http://hz.sweek.top/gtinqjvhkv.html

C#:   u is User
来源：http://hz.sysykeji.top/gtcvvjozjx.html

[G14] 数据类 / record
来源：http://hz.sxryk.cn/gthkoqmndx.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.52xcode.cn/gtrxkqppru.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.zhaomingkeji.xyz/gtjigywfnz.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.jqgufenzy.top/gtkgkownmc.html

TS:   type User = { name: string; age: number };
来源：http://hz.9152youxi.cn/gtkiaqbvwy.html

Java: record User(String name, int age) {}
来源：http://hz.hongshengwenyu.top/gtnuwglqmt.html

Go:   type User struct { Name string; Age int }
来源：http://hz.sxryk.cn/gtnrwwvmor.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.0kj1m.cn/gtknlexval.html

C#:   record User(string Name, int Age);
来源：http://hz.jyoumei.cn/gtycgqqazv.html

[G15] 枚举
来源：http://hz.ppjwa.cn/gtsssxjvqt.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.sufxvd.cn/gtjwkxcsgh.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.yongpay.top/gtsznybpou.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.zhixingplan.top/gtnrntmoxx.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.jiagoushi.top/gtzsxhyiwr.html

Java: enum Color { RED, GREEN }
来源：http://hz.sysykeji.top/gtoxvmnyjp.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.chenlongwang.top/gtavxojppl.html

Ruby: Color = %i[red green].freeze
来源：http://hz.0kj1m.cn/gtytvscsvr.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.316326.xyz/gtbxfakgcu.html

[G16] 对象转数组 / 字典
来源：http://hz.guannengcc.top/gtawnbrxjq.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.cqqwz.cn/gtoagivfox.html

PHP:  get_object_vars($obj);
来源：http://hz.feifeiyinyue.top/gtizbjorbk.html

JS:   Object.entries(obj)
来源：http://hz.snrcjt.cn/gtiiobzabp.html

TS:   Object.entries(obj)
来源：http://hz.zhengqikj.top/gtowmxpoax.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.ivvv.top/gthfsfktkv.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.yj202588.top/gtxwitoeqp.html

Ruby: obj.instance_variables
来源：http://hz.ivvv.top/gtuumrpfqc.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.smart0.xyz/gtsywarlvc.html

================================================================================
来源：http://hz.yanxiufei.cn/gtrjurenfz.html

H. 异常与错误处理
来源：http://hz.zhoulong.xyz/gtlftwtdhq.html

================================================================================
来源：http://hz.jinqigufen.top/gtbkqokgko.html

[H01] try / catch 基础
来源：http://hz.9152youxi.cn/gtswajqhfi.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.yuanzhike.top/gtblqhxtmm.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.havefunace.top/gtiqaqpvaw.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.ydjk.org.cn/gtwlnvephf.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.shanyushiyangtech.top/gtpuugtsvg.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.cheryme.top/gtpuobtxfs.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.cashguo.top/gtenzzvrua.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.vqdsnc.cn/gtoylowmcc.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.52xcode.cn/gtgvqynffl.html

[H02] finally / ensure 收尾
来源：http://hz.zhaomingkeji.xyz/gttpmolzye.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.xziqi.cn/gtgntvovdl.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.gzhubu.top/gtlgiwtkzy.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.jqgufenzy.top/gtntbxcztm.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.jlsjyb.cn/gtwhqrulkh.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.jinghuilouyu.cn/gtlgrhqvyc.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.yonumen.top/gtffohslnk.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.jinghuilouyu.cn/gtxqqapbbt.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.pengpengdd.cyou/gtfcawnxdg.html

[H03] 主动抛出异常
来源：http://hz.yangfankeji.com/gtirptjbac.html

Py:   raise ValueError("错误信息")
来源：http://hz.nanxinkj.top/gteqgyojxm.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.aibaodan.cn/gtagefqcvx.html

JS:   throw new Error("错误信息");
来源：http://hz.cdnleiting.top/gttisfnrcj.html

TS:   throw new Error("错误信息");
来源：http://hz.pengpengdd.cyou/gtcqsypltc.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.gotoacloud.top/gtmpahyibk.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.c1oappe.top/gtemlrpddh.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.kuanghao11.cn/gtmqvkegnw.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.aizwys.cn/gtaelcjgwv.html

[H04] 自定义异常类型
来源：http://hz.cucudq.cn/gtxfbanyag.html

Py:   class MyError(Exception): pass
来源：http://hz.shanyushiyangtech.top/gtyysrosch.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.hysaishi.cn/gtuxqixxgg.html

JS:   class MyError extends Error {}
来源：http://hz.aizwys.cn/gtltbuowom.html

TS:   class MyError extends Error {}
来源：http://hz.shanyushiyangkeji.top/gtmqxoqgbw.html

Java: class MyException extends RuntimeException {}
来源：http://hz.daria6918.cn/gtuczczkmo.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.sxryk.cn/gtbifqyrns.html

Ruby: class MyError < StandardError; end
来源：http://hz.yuanzhike.top/gtmqbcjfcr.html

C#:   class MyException : Exception {}
来源：http://hz.shzxlz.cn/gtwnokyekc.html

[H05] 捕获特定类型
来源：http://hz.snrcjt.cn/gtsvfjpctw.html

Py:   except ValueError as e:
来源：http://hz.shuidangran.top/gtxxrparru.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.jlsjyb.cn/gtxrerbhpf.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.pycfn.com/gtxktbfnnl.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.fengsongda.top/gtnikisssy.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.vqdsnc.cn/gtsdnfylgh.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.birdmap.top/gtuxugfhwj.html

Ruby: rescue ArgumentError => e
来源：http://hz.jinyuanbaomall.cn/gtereirtnh.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.xuetiantiany.cn/gtohqubsfa.html

[H06] 可选值 / 空值安全访问
来源：http://hz.jinqigufen.top/gtvntedmzz.html

Py:   value = d.get("k") or default
来源：http://hz.hysaishi.cn/gtoltufhtz.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.cdnleiting.top/gtnqjvkszb.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.yj20258.top/gtkvbyphju.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.snrcjt.cn/gtavqalgyr.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.52xcode.cn/gtxhuqmwui.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.xuetiantiany.cn/gtzybxvnri.html

Ruby: d&.dig(:a, :b)
来源：http://hz.jinyuanbaomall.cn/gtxlxgkazo.html

C#:   obj?.A?.B ?? default
来源：http://hz.chenjidiqi.icu/gtazytksxi.html

[H07] 断言
来源：http://hz.dianchejie.cn/gtsgtxsbzl.html

Py:   assert x > 0, "必须为正"
来源：http://hz.yvedp.cn/gtwjpjegxw.html

PHP:  assert($x > 0);
来源：http://hz.316326.xyz/gtxficmfcm.html

JS:   console.assert(x > 0);
来源：http://hz.guowangkeji.top/gtnxgthdlp.html

TS:   console.assert(x > 0);
来源：http://hz.jinqigufen.top/gtglxhlawx.html

Java: assert x > 0 : "必须为正";
来源：http://hz.sysykeji.top/gtwfgizxfz.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.jinqigufen.top/gtrpcaqztv.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.quarkkingdee.top/gtraxwlnrg.html

C#:   Debug.Assert(x > 0);
来源：http://hz.yj202588.top/gtqwkohfqn.html

[H08] 获取错误信息与堆栈
来源：http://hz.9152youxi.cn/gtojusfdig.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.gogol.net.cn/gtlyjjhnoz.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.daria6918.cn/gtidvxofpu.html

JS:   e.message;  e.stack
来源：http://hz.guannengcc.top/gthsjnlkcx.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.jqgfzy.top/gtmskydxtp.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.c1oappe.top/gtzzzihamy.html

Go:   err.Error()
来源：http://hz.ivvv.top/gtkfszkrte.html

Ruby: e.message;  e.backtrace
来源：http://hz.zycfv.cn/gtkdmwhsvj.html

C#:   e.Message;  e.StackTrace
来源：http://hz.guowangkeji.top/gtqxlrcjee.html

[H09] 带错误码的异常
来源：http://hz.zhiwuduotai.top/gtjqzwbbve.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.jinyuanbaomall.cn/gtxizovutq.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.havefunace.top/gtzhrubqjx.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.hnxiangtu.top/gtwdlmdxnx.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.wangdashe.top/gtikhcpzza.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.tianlin.xyz/gtejmwenta.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.cucudq.cn/gtepjwtpql.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.ydzc1.top/gtbwljhdij.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.aizwys.cn/gtxficzais.html

[H10] 资源自动释放
来源：http://hz.fzhhl.top/gtxouwneak.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.shanyushiyangtech.top/gtelsfxbuo.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.fzhhl.top/gtilaeijze.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.aibaodan.cn/gtnfhprpwi.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.xingfuxueyuan.xyz/gtsltvqbel.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.hnxiangtu.top/gtfekxfkpx.html

Go:   defer f.Close()
来源：http://hz.shuidangran.top/gtavyybekq.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.tian-w.cn/gtkbxscyxd.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.jinqigufen.top/gttxliamsi.html

================================================================================
来源：http://hz.xuanzx.com/gtbajfmdxo.html

I. 正则表达式
来源：http://hz.nwbrower.top/gtuezhflim.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtctjerfmn.html

[I01] 判断是否匹配
来源：http://hz.bjfxy.top/gtfsvzgpnk.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.hnqzz.top/gtgeloiruc.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.aibaodan.cn/gtjxgxgspb.html

JS:   /\d+/.test(s)
来源：http://hz.9152youxi.cn/gtmuwbmsju.html

TS:   /\d+/.test(s)
来源：http://hz.chenzaomai.com/gtkshinpjh.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.svipenyu.cn/gtxingwrxo.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.tianlin.xyz/gtuzyqfogk.html

Ruby: s.match?(/\d+/)
来源：http://hz.tianlin.xyz/gtsxjcgxsz.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.sufxvd.cn/gtjxkxuqcn.html

[I02] 提取所有匹配
来源：http://hz.dashuyun.cn/gtvdrxbhfk.html

Py:   re.findall(r"\d+", s)
来源：http://hz.yvedp.cn/gtrmlqoiqq.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.sysykeji.top/gtribymxbd.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.316326.xyz/gtvbarhruh.html

TS:   s.match(/\d+/g)
来源：http://hz.gaohongyu789.top/gtdjsnjono.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.nanxinkj.top/gtqbsfloqf.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.xuanzx.com/gtbtdoqema.html

Ruby: s.scan(/\d+/)
来源：http://hz.yuxming.cn/gtnchtfwvk.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.jlsjyb.cn/gtopmarlaw.html

[I03] 提取捕获分组
来源：http://hz.ydzc1.top/gtdueexobo.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.hywenlv.cn/gtevamgppp.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.ywan-chungtsiang.top/gtrnoqgoni.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.daxiang520.top/gtamqbgbzg.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.redwolf501.top/gtklvqrijl.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.kuanghao11.cn/gthloplxfq.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.guowangkeji.top/gtyopkgzsb.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.pengpengdd.cyou/gtxwjreyij.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.hnqzz.top/gtkbmduusq.html

[I04] 正则替换
来源：http://hz.sysykeji.top/gtuyvonylk.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.svipenyu.cn/gtikunzgiv.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.jinqigfzy.top/gtzwkugirx.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.gotoacloud.top/gtmhccffai.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.hfpthk.cn/gtcvigoknx.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.gogol.net.cn/gtgdyxnrds.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.hfpthk.cn/gtklvdpjib.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.jqgfzy.top/gtvjhexddi.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.xingfuxueyuan.xyz/gtezviuzin.html

[I05] 按正则拆分
来源：http://hz.redwolf501.top/gtgpztyyxv.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.gotoacloud.top/gtajuszwpl.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.jinqigfzy.top/gtrtrhlcqf.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.svipenyu.cn/gtempijuoq.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.yangfankeji.com/gtdgewizca.html


<!-- 参考信息 -->