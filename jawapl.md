代发 wailian999

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.shzxlz.cn/gteswkgbet.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.wangdashe.top/gtdksmefbh.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.zhongyouzk.top/gtntubcfmq.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.ybcxt.top/gtcunffnpf.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.tianlin.xyz/gtkqplshxl.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.xinyue.icu/gthpwhsxoa.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.nanxuanxn.top/gtsgjtntsz.html

[F12] CSV 读写
来源：http://hz.havefunace.top/gtwrscfjto.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.snrcjt.cn/gtpktsoiqh.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.jyoumei.cn/gttqrqqdnw.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.xylfe.cn/gtmdpbddpf.html

TS:   // 同上
来源：http://hz.zhijiandao.cn/gtrernlzta.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.dianchejie.cn/gtpfiicsoe.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.xingfuxueyuan.xyz/gtxuilatho.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.shuidangran.top/gtcpiwbngv.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.yueranfly.top/gtfvqkspzc.html

================================================================================
来源：http://hz.quarkkingdee.top/gtgacllldd.html

G. 面向对象
来源：http://hz.chenlongwang.top/gtsrzyutxz.html

================================================================================
来源：http://hz.chenzaomai.com/gtdigyqmle.html

[G01] 定义类
来源：http://hz.ydzc1.top/gtetoxpqhb.html

Py:   class User: pass
来源：http://hz.chenlongwang.top/gtegzoteub.html

PHP:  class User {}
来源：http://hz.nwbrower.top/gtumjnxlsm.html

JS:   class User {}
来源：http://hz.jiagoushi.top/gtmtlejfel.html

TS:   class User { name: string = ""; }
来源：http://hz.c1oappe.top/gtgvkllnag.html

Java: class User {}
来源：http://hz.9152youxi.cn/gtirgaezrf.html

Go:   type User struct { Name string }
来源：http://hz.bjfxy.top/gtmgvyovbz.html

Ruby: class User; end
来源：http://hz.jinghuilouyu.cn/gtaiwguiqu.html

C#:   class User {}
来源：http://hz.tanke756.top/gtvgdikopw.html

[G02] 构造函数
来源：http://hz.jinghuilouyu.cn/gtcosiwlpc.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.gogol.net.cn/gtlkchelif.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.yanxiufei.cn/gtgejeizqm.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.yangfankeji.com/gtgrvcapmr.html

TS:   constructor(public name: string) {}
来源：http://hz.meibo888.top/gtzakxshsj.html

Java: User(String name) { this.name = name; }
来源：http://hz.tanke756.top/gteglxfoyj.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.tanke756.top/gtalnwsbmk.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.zhongyouzk.top/gtombxghlj.html

C#:   public User(string name) { Name = name; }
来源：http://hz.ydjk.org.cn/gtbaawvgru.html

[G03] 实例属性
来源：http://hz.gogol.net.cn/gthrttcqor.html

Py:   self.name = "x"
来源：http://hz.redwolf501.top/gtdqfnnzcn.html

PHP:  public string $name = "x";
来源：http://hz.jianghu66.top/gtcwyjlsal.html

JS:   this.name = "x";
来源：http://hz.0kj1m.cn/gtvurvtqgy.html

TS:   name: string = "x";
来源：http://hz.ppjwa.cn/gtqrregplj.html

Java: private String name;
来源：http://hz.zhongyouzk.top/gtmfugzldc.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.hammf.cn/gtktchlmiy.html

Ruby: @name = "x"
来源：http://hz.guannengcc.top/gtbdeqmxrf.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.yangfankeji.com/gtzvvywzyr.html

[G04] 定义方法
来源：http://hz.zhongyouzk.top/gtdznmazwv.html

Py:   def greet(self): return self.name
来源：http://hz.nanxuanxn.top/gtzegdpexc.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.jyoumei.cn/gthzvqqhwg.html

JS:   greet() { return this.name; }
来源：http://hz.zhongyouzk.top/gtppimlcmk.html

TS:   greet(): string { return this.name; }
来源：http://hz.xinyue.icu/gtxxyyjpre.html

Java: String greet() { return name; }
来源：http://hz.shuidangran.top/gtzeedbfsu.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.tian-w.cn/gtwijpvoex.html

Ruby: def greet; @name; end
来源：http://hz.mhx1999.top/gtcyddjjxj.html

C#:   public string Greet() => Name;
来源：http://hz.jinqigfzy.top/gtwqasremy.html

[G05] 继承
来源：http://hz.fzhhl.top/gtixcskbov.html

Py:   class Admin(User): pass
来源：http://hz.vqdsnc.cn/gtifovyjkd.html

PHP:  class Admin extends User {}
来源：http://hz.jyoumei.cn/gtmwxwxfcx.html

JS:   class Admin extends User {}
来源：http://hz.sxryk.cn/gttgbmxqel.html

TS:   class Admin extends User {}
来源：http://hz.jlsjyb.cn/gtkjcuinhh.html

Java: class Admin extends User {}
来源：http://hz.dianchejie.cn/gtfrquhqnm.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.nwbrower.top/gtpfcaeplk.html

Ruby: class Admin < User; end
来源：http://hz.cqqwz.cn/gtbqzmrlca.html

C#:   class Admin : User {}
来源：http://hz.yonumen.top/gtlyicmqqu.html

[G06] 重写方法
来源：http://hz.shuidangran.top/gtfpcqjwmr.html

Py:   def greet(self): return "admin"
来源：http://hz.svipenyu.cn/gtedadyzfm.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.svipenyu.cn/gtmrtfskcx.html

JS:   greet() { return "admin"; }
来源：http://hz.kuanghao11.cn/gtjieddltl.html

TS:   greet(): string { return "admin"; }
来源：http://hz.zhengqikj.top/gtxdoybgcf.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.zhoulong.xyz/gtiqvbhdwl.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.chenzaomai.com/gthzgudkaa.html

Ruby: def greet; "admin"; end
来源：http://hz.cashguo.top/gtrooaxnfn.html

C#:   public override string Greet() => "admin";
来源：http://hz.tianlin.xyz/gtntrsnihu.html

[G07] 调用父类方法
来源：http://hz.birdmap.top/gtwwkywgfn.html

Py:   super().greet()
来源：http://hz.jqgfzy.top/gttlcrrgzs.html

PHP:  parent::greet();
来源：http://hz.cqqwz.cn/gtewhvlmzw.html

JS:   super.greet();
来源：http://hz.haohaochexian.top/gtnaflxjpf.html

TS:   super.greet();
来源：http://hz.yuanzhike.top/gtzcmmxkmg.html

Java: super.greet();
来源：http://hz.jinqigfzy.top/gtjqrljvbg.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.daxiang520.top/gtijkeuohr.html

Ruby: super
来源：http://hz.yongpay.top/gtbrcbgysd.html

C#:   base.Greet();
来源：http://hz.yueranfly.top/gtuwbjpohz.html

[G08] 静态方法与属性
来源：http://hz.zhiwuduotai.top/gtxgogjeoz.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.hysaishi.cn/gtvgjwhkku.html

PHP:  public static function f() {}
来源：http://hz.snrcjt.cn/gtzlqanwkd.html

JS:   static f() {}
来源：http://hz.smart0.xyz/gtxxykibpw.html

TS:   static f(): void {}
来源：http://hz.gzhubu.top/gtenkghpeg.html

Java: static void f() {}
来源：http://hz.cashguo.top/gtznlbvhao.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.yongpay.top/gtnnbkyvok.html

Ruby: def self.f; end
来源：http://hz.zdqjudy.top/gtpxhjhgpt.html

C#:   public static void F() {}
来源：http://hz.shanyushiyangtech.top/gtwoyoypbh.html

[G09] 接口 / 抽象类
来源：http://hz.tian-w.cn/gtqyqkqabd.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.zycfv.cn/gttzxpnyje.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.yueranfly.top/gtamrlrngk.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.shanyushiyangtech.top/gtywvxuuyq.html

TS:   interface Shape { area(): number; }
来源：http://hz.xuanzx.com/gtirjktajd.html

Java: interface Shape { double area(); }
来源：http://hz.ppjwa.cn/gtacogpblg.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.zycfv.cn/gtdryodslh.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.cqqwz.cn/gtwdpdcluo.html

C#:   interface IShape { double Area(); }
来源：http://hz.mhx1999.top/gtccicwbsk.html

[G10] 访问控制
来源：http://hz.aizwys.cn/gtoxitqbap.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.hammf.cn/gteabfuurd.html

PHP:  public / protected / private
来源：http://hz.shzxlz.cn/gtktviamox.html

JS:   #private 字段；其余公开
来源：http://hz.chenzaomai.com/gtrcmylzpp.html

TS:   public / protected / private
来源：http://hz.wangdashe.top/gtsisepvyi.html

Java: public / protected / private / 默认包级
来源：http://hz.guowangkeji.top/gtrdaugnaj.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.aibaodan.cn/gtyjwinbqa.html

Ruby: public / protected / private
来源：http://hz.jinghuilouyu.cn/gtczmkrddb.html

C#:   public / protected / private / internal
来源：http://hz.cdnleiting.top/gtseeultew.html

[G11] getter / setter
来源：http://hz.wangdashe.top/gtigbazvfa.html

Py:   @property 与 @x.setter
来源：http://hz.jinghuilouyu.cn/gteldogbgc.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.yuxming.cn/gtfkydpnij.html

JS:   get name() { return this._name; }
来源：http://hz.andypj.xyz/gtvxgxgzsd.html

TS:   get name(): string { return this._name; }
来源：http://hz.yueranfly.top/gtquzkjlrf.html

Java: public String getName() { return name; }
来源：http://hz.hnxiangtu.top/gtpivetied.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.jinghuilouyu.cn/gtadfrkjme.html

Ruby: attr_accessor :name
来源：http://hz.yj20258888.top/gtlcpmvjoz.html

C#:   public string Name { get; set; }
来源：http://hz.daria6918.cn/gtykcaawtq.html

[G12] 对象转字符串
来源：http://hz.yj20258.top/gtjndoacis.html

Py:   def __str__(self): return self.name
来源：http://hz.snrcjt.cn/gtlymkakds.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.316326.xyz/gtwbwdiqdc.html

JS:   toString() { return this.name; }
来源：http://hz.tianlin.xyz/gtzuyvunou.html

TS:   toString(): string { return this.name; }
来源：http://hz.jlsjyb.cn/gtyoesiyjp.html

Java: @Override public String toString() { return name; }
来源：http://hz.andypj.xyz/gtlaxhzpqo.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.jlsjyb.cn/gtgsgrwbdw.html

Ruby: def to_s; @name; end
来源：http://hz.gzhubu.top/gtggzlcyfu.html

C#:   public override string ToString() => Name;
来源：http://hz.quarkkingdee.top/gtjjejhawv.html

[G13] 判断对象类型
来源：http://hz.fengsongda.top/gtimrqkyvs.html

Py:   isinstance(u, User)
来源：http://hz.fengsongda.top/gtqdorjkup.html

PHP:  $u instanceof User
来源：http://hz.yonumen.top/gtbfspqtnf.html

JS:   u instanceof User
来源：http://hz.daxiang520.top/gtbefvigxp.html

TS:   u instanceof User
来源：http://hz.daxiang520.top/gtwtfdsifv.html

Java: u instanceof User
来源：http://hz.iojbl.cn/gtyhxarmsh.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.zhixingplan.top/gtzmzegubu.html

Ruby: u.is_a?(User)
来源：http://hz.ydzc1.top/gtujzlvvqz.html

C#:   u is User
来源：http://hz.dashuyun.cn/gtcgzubhqs.html

[G14] 数据类 / record
来源：http://hz.havefunace.top/gtgxehixct.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.sufxvd.cn/gthoqqrmpb.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.daxiang520.top/gttajuxpcp.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.cdnleiting.top/gtvuqofmob.html

TS:   type User = { name: string; age: number };
来源：http://hz.jlsjyb.cn/gtcsvwlkfa.html

Java: record User(String name, int age) {}
来源：http://hz.redwolf501.top/gtfpgezxgo.html

Go:   type User struct { Name string; Age int }
来源：http://hz.hongshengwenyu.top/gtmkkwbdux.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.cucudq.cn/gtiozxkurw.html

C#:   record User(string Name, int Age);
来源：http://hz.shzxlz.cn/gtinhorgst.html

[G15] 枚举
来源：http://hz.zdqjudy.top/gtofefukob.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.daxiang520.top/gtxmyhicew.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.chenlongwang.top/gthzsuqqnd.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.ydzc1.top/gtsebprajm.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.dashuyun.cn/gtavccjdqh.html

Java: enum Color { RED, GREEN }
来源：http://hz.yueranfly.top/gtfbadjsvw.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.jqgfzy.top/gtynnhsdct.html

Ruby: Color = %i[red green].freeze
来源：http://hz.daxiang520.top/gtusgvlvtm.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.hnqzz.top/gtroppnvit.html

[G16] 对象转数组 / 字典
来源：http://hz.tianlin.xyz/gtgqdxkgir.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.yvedp.cn/gtvzvhrahc.html

PHP:  get_object_vars($obj);
来源：http://hz.wangshuangyany.cn/gtgjuifxsg.html

JS:   Object.entries(obj)
来源：http://hz.yonumen.top/gtvszfvknp.html

TS:   Object.entries(obj)
来源：http://hz.nanxinkj.top/gtlcwfsqhw.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.316326.xyz/gtpruydtof.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.zhoulong.xyz/gtjfwdbkva.html

Ruby: obj.instance_variables
来源：http://hz.kuanghao11.cn/gtduiusgzj.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.redwolf501.top/gtodarwxrj.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtbhgfklty.html

H. 异常与错误处理
来源：http://hz.birdmap.top/gtdidkprev.html

================================================================================
来源：http://hz.yongpay.top/gtaeuspwje.html

[H01] try / catch 基础
来源：http://hz.yvedp.cn/gtvkvysazg.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.cdnleiting.top/gtvcbqgujh.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.sweek.top/gtyejqkety.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.chenjidiqi.icu/gtqdcqxrbe.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.aizwys.cn/gtfwvaydel.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.jyoumei.cn/gthvrvmoqy.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.hongshengwenyu.top/gthtebjtlk.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.hfpthk.cn/gtetoqwfgl.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.zhaomingkeji.xyz/gtxxvmjtxr.html

[H02] finally / ensure 收尾
来源：http://hz.dianchejie.cn/gtecmjsefn.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.pycfn.com/gthozgoxph.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.ybcxt.top/gtadjoigfd.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.pengpengdd.cyou/gtskbgqxtw.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.zhixingplan.top/gtcklsuylt.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.redwolf501.top/gtoqozfcle.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.xuetiantiany.cn/gtrluzmywb.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.zhaomingkeji.xyz/gtybqxqsts.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.xingfuxueyuan.xyz/gtkzwpczzr.html

[H03] 主动抛出异常
来源：http://hz.cashguo.top/gtotknwfgv.html

Py:   raise ValueError("错误信息")
来源：http://hz.sysykeji.top/gtqkppztlr.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.zycfv.cn/gthybtzafk.html

JS:   throw new Error("错误信息");
来源：http://hz.zhengqikj.top/gtevbmdvzq.html

TS:   throw new Error("错误信息");
来源：http://hz.cucudq.cn/gtjojgudtg.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.wangshuangyany.cn/gtbesgihhz.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.ehwqpu.com/gtgndieqsp.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.ydzc1.top/gtdcmjufex.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.snrcjt.cn/gtocxzfjhg.html

[H04] 自定义异常类型
来源：http://hz.jinqigfzy.top/gtizepwyvl.html

Py:   class MyError(Exception): pass
来源：http://hz.gzhubu.top/gtjkddlutm.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.xuetiantiany.cn/gtfjealdzy.html

JS:   class MyError extends Error {}
来源：http://hz.ydjk.org.cn/gtcezhzuqw.html

TS:   class MyError extends Error {}
来源：http://hz.hongshengwenyu.top/gturinhrph.html

Java: class MyException extends RuntimeException {}
来源：http://hz.gotoacloud.top/gtynvsmtut.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.birdmap.top/gtmxjublsm.html

Ruby: class MyError < StandardError; end
来源：http://hz.shanyushiyangtech.top/gtrdswysfg.html

C#:   class MyException : Exception {}
来源：http://hz.hywenlv.cn/gtguvcgfic.html

[H05] 捕获特定类型
来源：http://hz.zhaomingkeji.xyz/gtqrrbqqlv.html

Py:   except ValueError as e:
来源：http://hz.jyoumei.cn/gtxixlalup.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.tian-w.cn/gtlevpfdbo.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.haohaochexian.top/gtrcbyokcs.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.tanke756.top/gtjciodvmk.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.nanxinkj.top/gtyrpetgpv.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.0kj1m.cn/gtzuangqrx.html

Ruby: rescue ArgumentError => e
来源：http://hz.nanxinkj.top/gtbwpokfac.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.yj20258.top/gtczmroyih.html

[H06] 可选值 / 空值安全访问
来源：http://hz.xinyue.icu/gtgvagvdqa.html

Py:   value = d.get("k") or default
来源：http://hz.sysykeji.top/gtqveyfhjd.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.guannengcc.top/gtpvhcuuuv.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.hammf.cn/gtmfuecdrf.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.jinqigufen.top/gtccnifwfj.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.yj20258888.top/gtytfaeyvx.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.zhiwuduotai.top/gtuwukshqd.html

Ruby: d&.dig(:a, :b)
来源：http://hz.jinqigfzy.top/gtfxsspvtv.html

C#:   obj?.A?.B ?? default
来源：http://hz.nanxuanxn.top/gtmamlkike.html

[H07] 断言
来源：http://hz.tanke756.top/gtilutkbmy.html

Py:   assert x > 0, "必须为正"
来源：http://hz.andypj.xyz/gtdrhhyaix.html

PHP:  assert($x > 0);
来源：http://hz.yuxming.cn/gtawkhwggi.html

JS:   console.assert(x > 0);
来源：http://hz.zhiwuduotai.top/gtjzxzplad.html

TS:   console.assert(x > 0);
来源：http://hz.nanxinkj.top/gtgcyuuixx.html

Java: assert x > 0 : "必须为正";
来源：http://hz.smart0.xyz/gtndatmooc.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.daxiang520.top/gttiilkqqw.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.hnxiangtu.top/gtrrupwsop.html

C#:   Debug.Assert(x > 0);
来源：http://hz.tian-w.cn/gtzvzxkpey.html

[H08] 获取错误信息与堆栈
来源：http://hz.birdmap.top/gtpasogeln.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.aibaodan.cn/gtndbsvsnq.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.shuidangran.top/gtffozpwdj.html

JS:   e.message;  e.stack
来源：http://hz.zhengqikj.top/gthkkisrsj.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.jinqigufen.top/gtcnyiakcp.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.ybcxt.top/gtikqesyky.html

Go:   err.Error()
来源：http://hz.tian-w.cn/gtczmspnza.html

Ruby: e.message;  e.backtrace
来源：http://hz.yj202588.top/gtpjdcodnb.html

C#:   e.Message;  e.StackTrace
来源：http://hz.wangshuangyany.cn/gtvgxtzybd.html

[H09] 带错误码的异常
来源：http://hz.yangfankeji.com/gtbusbdxle.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.xylfe.cn/gtnnthfvtj.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.hywenlv.cn/gtcknfpucq.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.tian-w.cn/gtvdhzdtdt.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.wangdashe.top/gtfnrkkmcl.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.jianghu66.top/gtrtffpylb.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.ydzc1.top/gtrhfbbmce.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.dianchejie.cn/gtqfqnqbdh.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.zycfv.cn/gtfoholraw.html

[H10] 资源自动释放
来源：http://hz.52xcode.cn/gthicsspjh.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.hnxiangtu.top/gtomssbvgb.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.hywenlv.cn/gtvvujockt.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.xuanzx.com/gtjemjzheg.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.yj202588.top/gtfhcwfugx.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.chenlongwang.top/gtwfqfqvnv.html

Go:   defer f.Close()
来源：http://hz.shanyushiyangkeji.top/gtlrdpuwmg.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.sweek.top/gtaokacees.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.jlsjyb.cn/gtojjrphak.html

================================================================================
来源：http://hz.gaohongyu789.top/gtavryessk.html

I. 正则表达式
来源：http://hz.cqqwz.cn/gtxwdflxjq.html

================================================================================
来源：http://hz.cucudq.cn/gttbgxyakk.html

[I01] 判断是否匹配
来源：http://hz.guowangkeji.top/gtfpjdsobr.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.iojbl.cn/gtgeqxnljb.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.cucudq.cn/gtboukhwmy.html

JS:   /\d+/.test(s)
来源：http://hz.shzxlz.cn/gthsaeiawm.html

TS:   /\d+/.test(s)
来源：http://hz.nanxuanxn.top/gtzewlihlp.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.shuidangran.top/gtlnpnjafe.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.chenzaomai.com/gtkytbzzfl.html

Ruby: s.match?(/\d+/)
来源：http://hz.hammf.cn/gtxhhhamnl.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.guowangkeji.top/gtvyhksfpk.html

[I02] 提取所有匹配
来源：http://hz.vqdsnc.cn/gtvxwqxzmk.html

Py:   re.findall(r"\d+", s)
来源：http://hz.nanxinkj.top/gtlivtixyc.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.xingfuxueyuan.xyz/gtgcmzwxvw.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.cdnleiting.top/gtzukjajos.html

TS:   s.match(/\d+/g)
来源：http://hz.jqgufenzy.top/gtykzivlyq.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.52xcode.cn/gtsbmazpqr.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.yuanzhike.top/gtbymqpzhf.html

Ruby: s.scan(/\d+/)
来源：http://hz.chenjidiqi.icu/gtnhksfbto.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.52xcode.cn/gtmdgnesxk.html

[I03] 提取捕获分组
来源：http://hz.svipenyu.cn/gtmdmvuuav.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.chenzaomai.com/gtwhtwepup.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.gotoacloud.top/gtckxlbzhl.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.guannengcc.top/gtkoadrsma.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.yueranfly.top/gtuzldelgx.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.cheryme.top/gtvsztgkme.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.svipenyu.cn/gtuhkczmzw.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.xziqi.cn/gtzadhkqkf.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.iojbl.cn/gtkjdtpgfm.html

[I04] 正则替换
来源：http://hz.tanke756.top/gtvyxvyjvn.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.52xcode.cn/gtrqfkljeh.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.cucudq.cn/gtctrdsruk.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.yuxming.cn/gthlpemmpl.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.kuanghao11.cn/gtxoqjyaqs.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.9152youxi.cn/gtsquervra.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.chenzaomai.com/gtjoiokwwy.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.birdmap.top/gtbwstxgho.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.hongshengwenyu.top/gtyphoqlmg.html

[I05] 按正则拆分
来源：http://hz.smart0.xyz/gtlgukreqf.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.nanxuanxn.top/gtdvrmsoue.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.andypj.xyz/gtnymlomau.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.chenjidiqi.icu/gtyhuyxsih.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.jinqigfzy.top/gtbpotntnt.html


<!-- 参考信息 -->