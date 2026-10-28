代发 wailian999

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.zhaomingkeji.xyz/gtrnhycwnd.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.nanxuanxn.top/gtvglaysxx.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.xingfuxueyuan.xyz/gtbufqkpok.html

TS:   // 同上
来源：http://hz.ppjwa.cn/gtwxhxexup.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.vqdsnc.cn/gtrclsatda.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.chenzaomai.com/gtdbwrzngh.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.wangdashe.top/gttmcesgrp.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.jlsjyb.cn/gtejpaakvu.html

================================================================================
来源：http://hz.vqdsnc.cn/gtldusases.html

G. 面向对象
来源：http://hz.gaohongyu789.top/gtreeamasd.html

================================================================================
来源：http://hz.xziqi.cn/gtguqnofei.html

[G01] 定义类
来源：http://hz.sweek.top/gtgtfyhpau.html

Py:   class User: pass
来源：http://hz.andypj.xyz/gtynlrbkms.html

PHP:  class User {}
来源：http://hz.daxiang520.top/gtzstgmdsm.html

JS:   class User {}
来源：http://hz.chenjidiqi.icu/gtoxuxshde.html

TS:   class User { name: string = ""; }
来源：http://hz.yvedp.cn/gtdotxhltr.html

Java: class User {}
来源：http://hz.sweek.top/gtdfyqjqqw.html

Go:   type User struct { Name string }
来源：http://hz.cheryme.top/gtkpvnshdf.html

Ruby: class User; end
来源：http://hz.hongshengwenyu.top/gtrpgxqojz.html

C#:   class User {}
来源：http://hz.gaohongyu789.top/gthevfzawu.html

[G02] 构造函数
来源：http://hz.dashuyun.cn/gtfbpcmzwi.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.havefunace.top/gtstnpahqi.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.shanyushiyangkeji.top/gtfstmujvj.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.iojbl.cn/gtagnorlcm.html

TS:   constructor(public name: string) {}
来源：http://hz.yueranfly.top/gtgosycvly.html

Java: User(String name) { this.name = name; }
来源：http://hz.nanxuanxn.top/gtrcsobial.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.daxiang520.top/gtzbmhfxhi.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.svipenyu.cn/gtsxrdgmhf.html

C#:   public User(string name) { Name = name; }
来源：http://hz.shzxlz.cn/gtpdklxaoc.html

[G03] 实例属性
来源：http://hz.yueranfly.top/gtcwtuncfk.html

Py:   self.name = "x"
来源：http://hz.c1oappe.top/gtitlooyhb.html

PHP:  public string $name = "x";
来源：http://hz.kuanghao11.cn/gtfmmbcvdn.html

JS:   this.name = "x";
来源：http://hz.iojbl.cn/gtjuqbuyyh.html

TS:   name: string = "x";
来源：http://hz.hongshengwenyu.top/gtzwpbsfgh.html

Java: private String name;
来源：http://hz.hnxiangtu.top/gtvaticrwo.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.hywenlv.cn/gtlvnpsjvt.html

Ruby: @name = "x"
来源：http://hz.hysaishi.cn/gtdpsnudqu.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.yongpay.top/gtiljfjarj.html

[G04] 定义方法
来源：http://hz.svipenyu.cn/gtcpxkssns.html

Py:   def greet(self): return self.name
来源：http://hz.ydzc1.top/gtjslqtqej.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.yueranfly.top/gtxinnctyh.html

JS:   greet() { return this.name; }
来源：http://hz.quarkkingdee.top/gtkjlllhob.html

TS:   greet(): string { return this.name; }
来源：http://hz.daria6918.cn/gtgkkmrpso.html

Java: String greet() { return name; }
来源：http://hz.0kj1m.cn/gtpfwnbcyn.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.ivvv.top/gtupqwwoii.html

Ruby: def greet; @name; end
来源：http://hz.dashuyun.cn/gtdsamtiqk.html

C#:   public string Greet() => Name;
来源：http://hz.zhoulong.xyz/gtzdtlxubh.html

[G05] 继承
来源：http://hz.yanxiufei.cn/gtjcebjduv.html

Py:   class Admin(User): pass
来源：http://hz.jinyuanbaomall.cn/gtoadttkrm.html

PHP:  class Admin extends User {}
来源：http://hz.kuanghao11.cn/gtwlhfhsqg.html

JS:   class Admin extends User {}
来源：http://hz.sweek.top/gtxwdjgvgf.html

TS:   class Admin extends User {}
来源：http://hz.wangdashe.top/gteeitjmbj.html

Java: class Admin extends User {}
来源：http://hz.jinyuanbaomall.cn/gtphhxmgug.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.haohaochexian.top/gtngxjymbv.html

Ruby: class Admin < User; end
来源：http://hz.sysykeji.top/gtgajbhbhx.html

C#:   class Admin : User {}
来源：http://hz.meibo888.top/gtsqtjxaem.html

[G06] 重写方法
来源：http://hz.shzxlz.cn/gtlsoluaro.html

Py:   def greet(self): return "admin"
来源：http://hz.dashuyun.cn/gtocthavuq.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.cucudq.cn/gtkuakylpt.html

JS:   greet() { return "admin"; }
来源：http://hz.hammf.cn/gtgvrxeutp.html

TS:   greet(): string { return "admin"; }
来源：http://hz.hnqzz.top/gtnqimiswl.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.yueranfly.top/gtjomkzaia.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.aibaodan.cn/gtaekonebt.html

Ruby: def greet; "admin"; end
来源：http://hz.feifeiyinyue.top/gtweyrfdgq.html

C#:   public override string Greet() => "admin";
来源：http://hz.zhijiandao.cn/gtzlizzcqz.html

[G07] 调用父类方法
来源：http://hz.fengsongda.top/gtmxxgfhyf.html

Py:   super().greet()
来源：http://hz.gaohongyu789.top/gtnrzgqifn.html

PHP:  parent::greet();
来源：http://hz.guannengcc.top/gtiibvviwf.html

JS:   super.greet();
来源：http://hz.xuetiantiany.cn/gtlyzarzoe.html

TS:   super.greet();
来源：http://hz.vqdsnc.cn/gtgmnbqhis.html

Java: super.greet();
来源：http://hz.yangfankeji.com/gtquytekbp.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.yj20258888.top/gtssvaxrup.html

Ruby: super
来源：http://hz.guowangkeji.top/gthswcskkq.html

C#:   base.Greet();
来源：http://hz.nwbrower.top/gtqtqkxlvx.html

[G08] 静态方法与属性
来源：http://hz.yongpay.top/gtrlwnphih.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.sweek.top/gtheglibkt.html

PHP:  public static function f() {}
来源：http://hz.kuanghao11.cn/gtsqciwhuo.html

JS:   static f() {}
来源：http://hz.pycfn.com/gtsxrrbiwv.html

TS:   static f(): void {}
来源：http://hz.quarkkingdee.top/gtlrpaqllu.html

Java: static void f() {}
来源：http://hz.xuetiantiany.cn/gtibhuyliq.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.wangshuangyany.cn/gtgibaoadk.html

Ruby: def self.f; end
来源：http://hz.chenlongwang.top/gtmsjzqyhe.html

C#:   public static void F() {}
来源：http://hz.gzhubu.top/gtlnwmcrql.html

[G09] 接口 / 抽象类
来源：http://hz.jinyuanbaomall.cn/gtvveeuvdd.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.birdmap.top/gtbumsxhss.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.nanxuanxn.top/gtkfcijouy.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.mhx1999.top/gtkwmibaxc.html

TS:   interface Shape { area(): number; }
来源：http://hz.shanyushiyangtech.top/gtmudqwdqq.html

Java: interface Shape { double area(); }
来源：http://hz.jinqigfzy.top/gtepupjfgd.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.aibaodan.cn/gttdgdqpsd.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.aizwys.cn/gtwtgiutoj.html

C#:   interface IShape { double Area(); }
来源：http://hz.zdqjudy.top/gtadyokihr.html

[G10] 访问控制
来源：http://hz.andypj.xyz/gtonuobkxx.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.0kj1m.cn/gtdqwyxbbd.html

PHP:  public / protected / private
来源：http://hz.shangyingyoupin.top/gteczgmcqj.html

JS:   #private 字段；其余公开
来源：http://hz.tian-w.cn/gtjmutqrik.html

TS:   public / protected / private
来源：http://hz.hammf.cn/gtwxusqwow.html

Java: public / protected / private / 默认包级
来源：http://hz.cucudq.cn/gtcznqsgvz.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.ywan-chungtsiang.top/gtvmuzslvt.html

Ruby: public / protected / private
来源：http://hz.quarkkingdee.top/gtyywalbyl.html

C#:   public / protected / private / internal
来源：http://hz.cqqwz.cn/gtvgjteyig.html

[G11] getter / setter
来源：http://hz.chenjidiqi.icu/gtbqnmynnf.html

Py:   @property 与 @x.setter
来源：http://hz.tanke756.top/gthmianakp.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.yj202588.top/gtwtadnflw.html

JS:   get name() { return this._name; }
来源：http://hz.zhengqikj.top/gthnlytdnv.html

TS:   get name(): string { return this._name; }
来源：http://hz.hywenlv.cn/gtlsoakieo.html

Java: public String getName() { return name; }
来源：http://hz.ppjwa.cn/gtduowzdij.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.haohaochexian.top/gtqvkthcul.html

Ruby: attr_accessor :name
来源：http://hz.kuanghao11.cn/gtszglqwck.html

C#:   public string Name { get; set; }
来源：http://hz.xinyue.icu/gthytacqdc.html

[G12] 对象转字符串
来源：http://hz.xingfuxueyuan.xyz/gtwouburga.html

Py:   def __str__(self): return self.name
来源：http://hz.316326.xyz/gtflmkgavu.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.daxiang520.top/gtmrnwtdje.html

JS:   toString() { return this.name; }
来源：http://hz.xylfe.cn/gtdlpdoulg.html

TS:   toString(): string { return this.name; }
来源：http://hz.hnqzz.top/gtmyknshom.html

Java: @Override public String toString() { return name; }
来源：http://hz.ywan-chungtsiang.top/gtvkfixcdc.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.gogol.net.cn/gtdypdplvm.html

Ruby: def to_s; @name; end
来源：http://hz.shzxlz.cn/gtnpfvggec.html

C#:   public override string ToString() => Name;
来源：http://hz.gotoacloud.top/gtdmbimiwy.html

[G13] 判断对象类型
来源：http://hz.zhengqikj.top/gtpazcnnjz.html

Py:   isinstance(u, User)
来源：http://hz.vqdsnc.cn/gteqnzkykh.html

PHP:  $u instanceof User
来源：http://hz.hfpthk.cn/gtawlfpipk.html

JS:   u instanceof User
来源：http://hz.jiagoushi.top/gtfxtipnyq.html

TS:   u instanceof User
来源：http://hz.ppjwa.cn/gteclecwoy.html

Java: u instanceof User
来源：http://hz.aizwys.cn/gtbegyuema.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.gogol.net.cn/gthxjcffyy.html

Ruby: u.is_a?(User)
来源：http://hz.dashuyun.cn/gttfbelogy.html

C#:   u is User
来源：http://hz.bjfxy.top/gtmvkcpldl.html

[G14] 数据类 / record
来源：http://hz.hongshengwenyu.top/gtlxveaxon.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.yongpay.top/gtgkjgkkyb.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.redwolf501.top/gtdsfyzoyf.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.snrcjt.cn/gtbinixlld.html

TS:   type User = { name: string; age: number };
来源：http://hz.mhx1999.top/gtipmblpqa.html

Java: record User(String name, int age) {}
来源：http://hz.yj20258888.top/gtubooxjzl.html

Go:   type User struct { Name string; Age int }
来源：http://hz.sysykeji.top/gtjlrhmloh.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.hnxiangtu.top/gtkaumyyuf.html

C#:   record User(string Name, int Age);
来源：http://hz.yj202588.top/gtfebesmgm.html

[G15] 枚举
来源：http://hz.andypj.xyz/gtlwtjpgep.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.gotoacloud.top/gtllczacpf.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.svipenyu.cn/gtcetkoboc.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.guowangkeji.top/gtdtbxmwqq.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.redwolf501.top/gtyjybtgmj.html

Java: enum Color { RED, GREEN }
来源：http://hz.havefunace.top/gthnbtacuy.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.zhengqikj.top/gtriddoycb.html

Ruby: Color = %i[red green].freeze
来源：http://hz.yanxiufei.cn/gtyvfjqfxk.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.hammf.cn/gtjhxdupmk.html

[G16] 对象转数组 / 字典
来源：http://hz.yj20258888.top/gtnzwzkxyh.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.mhx1999.top/gtcntwzzng.html

PHP:  get_object_vars($obj);
来源：http://hz.pengpengdd.cyou/gtivpxhzan.html

JS:   Object.entries(obj)
来源：http://hz.sxryk.cn/gtduqlzvcg.html

TS:   Object.entries(obj)
来源：http://hz.aizwys.cn/gtasfvgntp.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.shangyingyoupin.top/gtcomwuoub.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.pengpengdd.cyou/gtxmpkidhh.html

Ruby: obj.instance_variables
来源：http://hz.dianchejie.cn/gtpkgxslhx.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.quarkkingdee.top/gtkrsyiaqq.html

================================================================================
来源：http://hz.xziqi.cn/gtgpwuxpgh.html

H. 异常与错误处理
来源：http://hz.yonumen.top/gtqrgbxdgn.html

================================================================================
来源：http://hz.tian-w.cn/gtykggdbzd.html

[H01] try / catch 基础
来源：http://hz.shanyushiyangkeji.top/gttvaacuiv.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.cqqwz.cn/gtxkmymgzn.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.chenzaomai.com/gtvgojggpp.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.sxryk.cn/gtwxbxdbvp.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.gogol.net.cn/gtfkzgafmo.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.ywan-chungtsiang.top/gtbzniswxx.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.ivvv.top/gtmkcdcsjx.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.hfpthk.cn/gtymbvsxfh.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.gaohongyu789.top/gtwyznmihq.html

[H02] finally / ensure 收尾
来源：http://hz.ehwqpu.com/gtxlsgnfkh.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.quarkkingdee.top/gtqjkwjwqn.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.fzhhl.top/gtsivsvdza.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.yuxming.cn/gtlosanncp.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.gogol.net.cn/gtcmzfiztc.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.jqgufenzy.top/gtwflcdmtp.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.guannengcc.top/gtgzjmoons.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.ybcxt.top/gtnttmnuri.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.nanxuanxn.top/gtwbrtsakl.html

[H03] 主动抛出异常
来源：http://hz.dashuyun.cn/gtxxqgrtkh.html

Py:   raise ValueError("错误信息")
来源：http://hz.ivvv.top/gtfrhutfyj.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.fzhhl.top/gtpazoozce.html

JS:   throw new Error("错误信息");
来源：http://hz.ppjwa.cn/gtbeqqwfcs.html

TS:   throw new Error("错误信息");
来源：http://hz.0kj1m.cn/gtsjepfgst.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.zhoulong.xyz/gtlrhmkklh.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.52xcode.cn/gtqzzceeln.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.tian-w.cn/gtbkiursde.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.xinyue.icu/gtbotpzezx.html

[H04] 自定义异常类型
来源：http://hz.mhx1999.top/gtercjeldm.html

Py:   class MyError(Exception): pass
来源：http://hz.nwbrower.top/gtwzvviwhl.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.xylfe.cn/gtgrqhnvds.html

JS:   class MyError extends Error {}
来源：http://hz.xuanzx.com/gtezzfelof.html

TS:   class MyError extends Error {}
来源：http://hz.yongpay.top/gtgmjfyueq.html

Java: class MyException extends RuntimeException {}
来源：http://hz.birdmap.top/gtjuriqnjv.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.c1oappe.top/gtxbkrwbld.html

Ruby: class MyError < StandardError; end
来源：http://hz.ehwqpu.com/gtvpmorqff.html

C#:   class MyException : Exception {}
来源：http://hz.yueranfly.top/gtxiivqjzq.html

[H05] 捕获特定类型
来源：http://hz.chenjidiqi.icu/gtpezlreaq.html

Py:   except ValueError as e:
来源：http://hz.jqgufenzy.top/gtclutownr.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.bjfxy.top/gtcjjogtjx.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.xuanzx.com/gtqjpqgrcf.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.hnxiangtu.top/gtvkdpaunp.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.sxryk.cn/gtaahacaor.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.zhoulong.xyz/gtiuzeqtas.html

Ruby: rescue ArgumentError => e
来源：http://hz.xingfuxueyuan.xyz/gtysankfzn.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.xziqi.cn/gtyexkqjhv.html

[H06] 可选值 / 空值安全访问
来源：http://hz.guannengcc.top/gtxpwttoyq.html

Py:   value = d.get("k") or default
来源：http://hz.ywan-chungtsiang.top/gtrahicbqc.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.andypj.xyz/gtnixvqsli.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.haohaochexian.top/gtjqtzskkz.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.haohaochexian.top/gttaiyhota.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.ppjwa.cn/gtrodmddvn.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.jqgfzy.top/gtbluicjxn.html

Ruby: d&.dig(:a, :b)
来源：http://hz.jyoumei.cn/gtkpidarsf.html

C#:   obj?.A?.B ?? default
来源：http://hz.hammf.cn/gtkjvdhqdq.html

[H07] 断言
来源：http://hz.sufxvd.cn/gtuexqehbe.html

Py:   assert x > 0, "必须为正"
来源：http://hz.jinghuilouyu.cn/gttdwjufxy.html

PHP:  assert($x > 0);
来源：http://hz.sxryk.cn/gtynmuhomh.html

JS:   console.assert(x > 0);
来源：http://hz.zhengqikj.top/gtrgyetjhe.html

TS:   console.assert(x > 0);
来源：http://hz.shzxlz.cn/gtrsrvnxbd.html

Java: assert x > 0 : "必须为正";
来源：http://hz.ivvv.top/gtczwlqyxe.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.xuanzx.com/gthbwkspao.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.xziqi.cn/gtejaqvamz.html

C#:   Debug.Assert(x > 0);
来源：http://hz.zhaomingkeji.xyz/gtqtxbonhg.html

[H08] 获取错误信息与堆栈
来源：http://hz.yj20258.top/gtxnxflycj.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.gzhubu.top/gtkljzijmw.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.zhoulong.xyz/gtbkbgvwcm.html

JS:   e.message;  e.stack
来源：http://hz.xylfe.cn/gtzcevilce.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.xziqi.cn/gtdmmonnmn.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.ywan-chungtsiang.top/gtjesyjwyz.html

Go:   err.Error()
来源：http://hz.tianlin.xyz/gtwpwvjdfc.html

Ruby: e.message;  e.backtrace
来源：http://hz.jqgfzy.top/gtzurbbwqq.html

C#:   e.Message;  e.StackTrace
来源：http://hz.yuanzhike.top/gtldzprpno.html

[H09] 带错误码的异常
来源：http://hz.yangfankeji.com/gtulexokmd.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.yj202588.top/gtsytzhnit.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.yongpay.top/gtfagvalij.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.nanxuanxn.top/gtemieecfk.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.nwbrower.top/gtpgxvvala.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.ydzc1.top/gtlnnnyika.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.xuanzx.com/gtydtoaazz.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.zhengqikj.top/gtgfpuvsuv.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.gotoacloud.top/gtuxdrvewk.html

[H10] 资源自动释放
来源：http://hz.dianchejie.cn/gtzrczmazg.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.zdqjudy.top/gtzaaxnqga.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.aibaodan.cn/gtupbsqgkk.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.jqgfzy.top/gtdlpjpmws.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.pycfn.com/gtkxcbphrz.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.hfpthk.cn/gtloiwfwae.html

Go:   defer f.Close()
来源：http://hz.hnxiangtu.top/gtrhhruwua.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.haohaochexian.top/gtrfhyofom.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.aibaodan.cn/gtfvydyoob.html

================================================================================
来源：http://hz.ivvv.top/gtauiznqgn.html

I. 正则表达式
来源：http://hz.vqdsnc.cn/gtpksathah.html

================================================================================
来源：http://hz.nanxuanxn.top/gtnmosfqes.html

[I01] 判断是否匹配
来源：http://hz.nanxinkj.top/gtpyzlkdnd.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.shuidangran.top/gtromobaxq.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.yj20258.top/gtxciapxvm.html

JS:   /\d+/.test(s)
来源：http://hz.cdnleiting.top/gtbfraiuyr.html

TS:   /\d+/.test(s)
来源：http://hz.gaohongyu789.top/gtcqtqzlvf.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.gotoacloud.top/gtowjglkgz.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.dianchejie.cn/gthigbuidi.html

Ruby: s.match?(/\d+/)
来源：http://hz.feifeiyinyue.top/gtsznjxepu.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.hnxiangtu.top/gtrkgnkruz.html

[I02] 提取所有匹配
来源：http://hz.shanyushiyangkeji.top/gtdoybkvtt.html

Py:   re.findall(r"\d+", s)
来源：http://hz.hammf.cn/gtpkujhtqv.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.iojbl.cn/gtxzprbxti.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.wangdashe.top/gtbbwbwksy.html

TS:   s.match(/\d+/g)
来源：http://hz.zhijiandao.cn/gtuakajxok.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.vqdsnc.cn/gtpezopauh.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.wangshuangyany.cn/gtjjxmfgjs.html

Ruby: s.scan(/\d+/)
来源：http://hz.tian-w.cn/gtgpmgaqip.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.xuetiantiany.cn/gtjpndsepb.html

[I03] 提取捕获分组
来源：http://hz.aibaodan.cn/gtnrztseds.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.hfpthk.cn/gtcxxxgkwa.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.yongpay.top/gtnyeccxza.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.ydzc1.top/gtftwxyawo.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.yanxiufei.cn/gtrchchyse.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.dianchejie.cn/gtfrsmrjwk.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.yj20258.top/gtsyewceiw.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.sxryk.cn/gtqzrvqwee.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.yanxiufei.cn/gtozlcvdsz.html

[I04] 正则替换
来源：http://hz.gzhubu.top/gtufqvaftt.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.cdnleiting.top/gtunjzavhz.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.yonumen.top/gtgkgqrstg.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.jiagoushi.top/gtbgoeiuyr.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.gogol.net.cn/gtmiugfcca.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.havefunace.top/gtjzkxfpvi.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.xylfe.cn/gteajljejl.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.daria6918.cn/gtztqinulf.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.tianlin.xyz/gtytubjrli.html

[I05] 按正则拆分
来源：http://hz.andypj.xyz/gtnjbvaznz.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.gaohongyu789.top/gtezecnswk.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.jinghuilouyu.cn/gtbemvuhal.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.chenjidiqi.icu/gtpfmgvxop.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.ivvv.top/gtpbxsiesc.html

Java: s.split("\\s*,\\s*")
来源：http://hz.shanyushiyangtech.top/gterwsunrs.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.jqgufenzy.top/gtfwrndnpv.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.hnqzz.top/gtclueegax.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.hammf.cn/gtqsomvoju.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.yj20258.top/gtnzxgpibv.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.iojbl.cn/gtozdsznxv.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.jinghuilouyu.cn/gtgworjszw.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.jinyuanbaomall.cn/gtrcznfhck.html


<!-- 参考信息 -->