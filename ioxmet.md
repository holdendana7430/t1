代发 wailian999

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.vqdsnc.cn/gtvldoilkn.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.tian-w.cn/gtodiggonc.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.shzxlz.cn/gttxacqvux.html

TS:   // 同上
来源：http://hz.ehwqpu.com/gtyicawrli.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.cdnleiting.top/gtoopxzrnq.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.guannengcc.top/gtwuxuvcbx.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.birdmap.top/gtuwkyycxq.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.cdnleiting.top/gtjxpkqdlr.html

================================================================================
来源：http://hz.haohaochexian.top/gtaxsdsxmx.html

G. 面向对象
来源：http://hz.chenjidiqi.icu/gtgdrgtsbv.html

================================================================================
来源：http://hz.iojbl.cn/gtatcwzdud.html

[G01] 定义类
来源：http://hz.xziqi.cn/gtylndokbc.html

Py:   class User: pass
来源：http://hz.yonumen.top/gtnyjkidgg.html

PHP:  class User {}
来源：http://hz.quarkkingdee.top/gtcqffnmwg.html

JS:   class User {}
来源：http://hz.daxiang520.top/gtldlkbqyt.html

TS:   class User { name: string = ""; }
来源：http://hz.9152youxi.cn/gtmsykohyw.html

Java: class User {}
来源：http://hz.chenzaomai.com/gtgvzjddym.html

Go:   type User struct { Name string }
来源：http://hz.jinqigfzy.top/gtwvbscqgb.html

Ruby: class User; end
来源：http://hz.yvedp.cn/gtgftcaudd.html

C#:   class User {}
来源：http://hz.yj20258.top/gtckaonmaf.html

[G02] 构造函数
来源：http://hz.andypj.xyz/gteopsxbrw.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.guowangkeji.top/gtrxnrldlm.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.jiagoushi.top/gtgguqkrxt.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.zhongyouzk.top/gtwsbpsbxe.html

TS:   constructor(public name: string) {}
来源：http://hz.haohaochexian.top/gtpekovyde.html

Java: User(String name) { this.name = name; }
来源：http://hz.redwolf501.top/gtuarelhib.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.cucudq.cn/gtbtawdmfm.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.shzxlz.cn/gtygtcbpvs.html

C#:   public User(string name) { Name = name; }
来源：http://hz.hysaishi.cn/gtygbnsvaz.html

[G03] 实例属性
来源：http://hz.ydjk.org.cn/gtaqtpwjga.html

Py:   self.name = "x"
来源：http://hz.pengpengdd.cyou/gtusdofczy.html

PHP:  public string $name = "x";
来源：http://hz.zhaomingkeji.xyz/gtjugippsr.html

JS:   this.name = "x";
来源：http://hz.gogol.net.cn/gtuxpouguu.html

TS:   name: string = "x";
来源：http://hz.yongpay.top/gtrxizkhve.html

Java: private String name;
来源：http://hz.jinqigufen.top/gtaogxbbox.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.gogol.net.cn/gtnupufaps.html

Ruby: @name = "x"
来源：http://hz.wangdashe.top/gtntrhhjce.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.pycfn.com/gtkiqmidam.html

[G04] 定义方法
来源：http://hz.hongshengwenyu.top/gtsbhbxkxv.html

Py:   def greet(self): return self.name
来源：http://hz.shanyushiyangtech.top/gtdjsbsffv.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.birdmap.top/gtemdjaihq.html

JS:   greet() { return this.name; }
来源：http://hz.yonumen.top/gttydjqokf.html

TS:   greet(): string { return this.name; }
来源：http://hz.wangdashe.top/gtlqcdcjqu.html

Java: String greet() { return name; }
来源：http://hz.hnxiangtu.top/gtsnqgtuqi.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.hysaishi.cn/gtbzkildde.html

Ruby: def greet; @name; end
来源：http://hz.nanxinkj.top/gtjlguhcwt.html

C#:   public string Greet() => Name;
来源：http://hz.zhiwuduotai.top/gtnyipfgjz.html

[G05] 继承
来源：http://hz.quarkkingdee.top/gtjylawtgp.html

Py:   class Admin(User): pass
来源：http://hz.mhx1999.top/gtqttnsobh.html

PHP:  class Admin extends User {}
来源：http://hz.cashguo.top/gtigbuvkci.html

JS:   class Admin extends User {}
来源：http://hz.316326.xyz/gtifuhrwxz.html

TS:   class Admin extends User {}
来源：http://hz.sweek.top/gtewutkgtl.html

Java: class Admin extends User {}
来源：http://hz.smart0.xyz/gtykgxvmzn.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.zhengqikj.top/gtjsaxcbtc.html

Ruby: class Admin < User; end
来源：http://hz.ydzc1.top/gtmeuojdoj.html

C#:   class Admin : User {}
来源：http://hz.jianghu66.top/gtfiipqgtv.html

[G06] 重写方法
来源：http://hz.mhx1999.top/gtqtyvxtlm.html

Py:   def greet(self): return "admin"
来源：http://hz.wangdashe.top/gteotbokqo.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.xuetiantiany.cn/gtteoagnnp.html

JS:   greet() { return "admin"; }
来源：http://hz.yuanzhike.top/gtmhbnrase.html

TS:   greet(): string { return "admin"; }
来源：http://hz.ybcxt.top/gtpusshjyf.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.hfpthk.cn/gtwcoaittw.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.havefunace.top/gtblqvpqxb.html

Ruby: def greet; "admin"; end
来源：http://hz.yj202588.top/gtbmqbwche.html

C#:   public override string Greet() => "admin";
来源：http://hz.yangfankeji.com/gtwmibwshf.html

[G07] 调用父类方法
来源：http://hz.zhengqikj.top/gtfgvgafzm.html

Py:   super().greet()
来源：http://hz.ywan-chungtsiang.top/gtaladvrrg.html

PHP:  parent::greet();
来源：http://hz.316326.xyz/gttwjbavvb.html

JS:   super.greet();
来源：http://hz.hfpthk.cn/gtlqiefqqu.html

TS:   super.greet();
来源：http://hz.xinyue.icu/gtbwymyqeg.html

Java: super.greet();
来源：http://hz.pengpengdd.cyou/gtvfkklifv.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.zhixingplan.top/gtojureztv.html

Ruby: super
来源：http://hz.shangyingyoupin.top/gtvfvkdqbz.html

C#:   base.Greet();
来源：http://hz.yongpay.top/gtaybjvdtj.html

[G08] 静态方法与属性
来源：http://hz.shanyushiyangtech.top/gtbzfgcjdw.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.316326.xyz/gtrcjwzztk.html

PHP:  public static function f() {}
来源：http://hz.9152youxi.cn/gtbbzpyufm.html

JS:   static f() {}
来源：http://hz.shanyushiyangkeji.top/gthubdjich.html

TS:   static f(): void {}
来源：http://hz.smart0.xyz/gtxpjktitf.html

Java: static void f() {}
来源：http://hz.snrcjt.cn/gtawoohven.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.shanyushiyangtech.top/gtptxtdifs.html

Ruby: def self.f; end
来源：http://hz.guannengcc.top/gtnxgclney.html

C#:   public static void F() {}
来源：http://hz.daria6918.cn/gtqbpguxhl.html

[G09] 接口 / 抽象类
来源：http://hz.yanxiufei.cn/gtbvodvuin.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.0kj1m.cn/gtcojjxbjf.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.gotoacloud.top/gtoozqbvdu.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.vqdsnc.cn/gtvrdcjffe.html

TS:   interface Shape { area(): number; }
来源：http://hz.ywan-chungtsiang.top/gtpqswijny.html

Java: interface Shape { double area(); }
来源：http://hz.9152youxi.cn/gtjurjdwwb.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.jinghuilouyu.cn/gtkscbbmxj.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.yueranfly.top/gtssxejafi.html

C#:   interface IShape { double Area(); }
来源：http://hz.jinqigfzy.top/gtdbgtoxap.html

[G10] 访问控制
来源：http://hz.zhaomingkeji.xyz/gtbsizgjzl.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.chenzaomai.com/gtbtuunuqq.html

PHP:  public / protected / private
来源：http://hz.gaohongyu789.top/gtjkaeqjsf.html

JS:   #private 字段；其余公开
来源：http://hz.c1oappe.top/gtxrnmdbbv.html

TS:   public / protected / private
来源：http://hz.cucudq.cn/gthuohpskw.html

Java: public / protected / private / 默认包级
来源：http://hz.zhoulong.xyz/gtsukclsnp.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.fzhhl.top/gtiegucycr.html

Ruby: public / protected / private
来源：http://hz.tian-w.cn/gtxjxcfuez.html

C#:   public / protected / private / internal
来源：http://hz.xuanzx.com/gtqopkcuyx.html

[G11] getter / setter
来源：http://hz.jlsjyb.cn/gtvrnrcsqi.html

Py:   @property 与 @x.setter
来源：http://hz.wangdashe.top/gtkpoatmii.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.zhiwuduotai.top/gtlvaelzlu.html

JS:   get name() { return this._name; }
来源：http://hz.shuidangran.top/gtkomtetfe.html

TS:   get name(): string { return this._name; }
来源：http://hz.zhengqikj.top/gtjejigruc.html

Java: public String getName() { return name; }
来源：http://hz.birdmap.top/gtkmdbuodc.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.ivvv.top/gtnjnptzks.html

Ruby: attr_accessor :name
来源：http://hz.zhiwuduotai.top/gthyvqhrwa.html

C#:   public string Name { get; set; }
来源：http://hz.xuetiantiany.cn/gtnzqlffnp.html

[G12] 对象转字符串
来源：http://hz.hammf.cn/gtripzkken.html

Py:   def __str__(self): return self.name
来源：http://hz.sxryk.cn/gtarnmpcdk.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.zycfv.cn/gtzlizomwp.html

JS:   toString() { return this.name; }
来源：http://hz.shanyushiyangtech.top/gtvubgrsvc.html

TS:   toString(): string { return this.name; }
来源：http://hz.gaohongyu789.top/gtweoboafh.html

Java: @Override public String toString() { return name; }
来源：http://hz.zhengqikj.top/gtxkqnxzev.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.daxiang520.top/gtbtbeopyc.html

Ruby: def to_s; @name; end
来源：http://hz.hammf.cn/gtosjmnkix.html

C#:   public override string ToString() => Name;
来源：http://hz.yonumen.top/gtbmyeavle.html

[G13] 判断对象类型
来源：http://hz.nanxinkj.top/gtahvtufxw.html

Py:   isinstance(u, User)
来源：http://hz.xingfuxueyuan.xyz/gtvscoprzk.html

PHP:  $u instanceof User
来源：http://hz.xziqi.cn/gtxdskmagr.html

JS:   u instanceof User
来源：http://hz.nanxuanxn.top/gtgokbhmlh.html

TS:   u instanceof User
来源：http://hz.hnqzz.top/gttizyxrav.html

Java: u instanceof User
来源：http://hz.cucudq.cn/gtuiajgfow.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.havefunace.top/gtgehxfmlx.html

Ruby: u.is_a?(User)
来源：http://hz.jianghu66.top/gttxhyjizl.html

C#:   u is User
来源：http://hz.gzhubu.top/gtzfruilar.html

[G14] 数据类 / record
来源：http://hz.gotoacloud.top/gtnovufgyc.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.bjfxy.top/gtjbgynfuq.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.xylfe.cn/gtqsvtkiej.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.yanxiufei.cn/gtpavdkcop.html

TS:   type User = { name: string; age: number };
来源：http://hz.xuetiantiany.cn/gthfkesurd.html

Java: record User(String name, int age) {}
来源：http://hz.hammf.cn/gtptlcuivm.html

Go:   type User struct { Name string; Age int }
来源：http://hz.tianlin.xyz/gtdclzoloa.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.ehwqpu.com/gttkkmlcxk.html

C#:   record User(string Name, int Age);
来源：http://hz.jianghu66.top/gtqjmssabz.html

[G15] 枚举
来源：http://hz.wangshuangyany.cn/gtxpmvkcdo.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.daria6918.cn/gtfzobugqo.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.zdqjudy.top/gttoyaorwu.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.redwolf501.top/gtfclwpqen.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.redwolf501.top/gtsxkoyubr.html

Java: enum Color { RED, GREEN }
来源：http://hz.yanxiufei.cn/gtuuapzwsh.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.ydzc1.top/gtbojgyqti.html

Ruby: Color = %i[red green].freeze
来源：http://hz.zhijiandao.cn/gtzgcpygxi.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.cqqwz.cn/gtxaqwazfq.html

[G16] 对象转数组 / 字典
来源：http://hz.fengsongda.top/gtdyntxtua.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.dashuyun.cn/gtsqqczjib.html

PHP:  get_object_vars($obj);
来源：http://hz.feifeiyinyue.top/gtncsmmpue.html

JS:   Object.entries(obj)
来源：http://hz.dianchejie.cn/gtcozzlmxq.html

TS:   Object.entries(obj)
来源：http://hz.kuanghao11.cn/gtumfkcwcv.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.gotoacloud.top/gtbecnkuqf.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.shzxlz.cn/gttpcyufdu.html

Ruby: obj.instance_variables
来源：http://hz.jiagoushi.top/gtyyyaynkr.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.zhijiandao.cn/gtldnhgcoz.html

================================================================================
来源：http://hz.jyoumei.cn/gtqonziqdx.html

H. 异常与错误处理
来源：http://hz.316326.xyz/gtsftiotbh.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtwzayywyt.html

[H01] try / catch 基础
来源：http://hz.jyoumei.cn/gtevnqvusm.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.guannengcc.top/gtobwzvwhn.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.xinyue.icu/gtouivvbzl.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.xinyue.icu/gtwqefanjk.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.yvedp.cn/gtoukqyfqo.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.zhiwuduotai.top/gtcktrpkhc.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.pycfn.com/gtauwliqgz.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.sysykeji.top/gtgzyghtci.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.sweek.top/gtjcimueaq.html

[H02] finally / ensure 收尾
来源：http://hz.meibo888.top/gtdjxsfmzu.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.yangfankeji.com/gtsnjwndfl.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.jianghu66.top/gtpcyyztgw.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.hfpthk.cn/gtfasiqzgf.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.yvedp.cn/gteinjtxpw.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.snrcjt.cn/gtwzakelir.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.zdqjudy.top/gtesjtkywc.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.zhongyouzk.top/gtahgzvyie.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.redwolf501.top/gtatlzdlum.html

[H03] 主动抛出异常
来源：http://hz.zhongyouzk.top/gtznaedoly.html

Py:   raise ValueError("错误信息")
来源：http://hz.sxryk.cn/gtxhfeqljy.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.zhongyouzk.top/gtveoetusf.html

JS:   throw new Error("错误信息");
来源：http://hz.vqdsnc.cn/gthnpfdkqd.html

TS:   throw new Error("错误信息");
来源：http://hz.mhx1999.top/gtotghcweh.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.yueranfly.top/gtjjvxblun.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.316326.xyz/gtpldcebgt.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.nwbrower.top/gtcmdxkvsk.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.xinyue.icu/gtdkcwrwat.html

[H04] 自定义异常类型
来源：http://hz.cashguo.top/gtnglwvmsh.html

Py:   class MyError(Exception): pass
来源：http://hz.andypj.xyz/gttacletxu.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.0kj1m.cn/gtpxwkuyxg.html

JS:   class MyError extends Error {}
来源：http://hz.andypj.xyz/gtfludkmuq.html

TS:   class MyError extends Error {}
来源：http://hz.fzhhl.top/gtaliiomup.html

Java: class MyException extends RuntimeException {}
来源：http://hz.cucudq.cn/gtrkdecrip.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.ppjwa.cn/gtodjnntdk.html

Ruby: class MyError < StandardError; end
来源：http://hz.hywenlv.cn/gtkghhkpkp.html

C#:   class MyException : Exception {}
来源：http://hz.9152youxi.cn/gticfwihzs.html

[H05] 捕获特定类型
来源：http://hz.xuetiantiany.cn/gtlsjextmp.html

Py:   except ValueError as e:
来源：http://hz.shanyushiyangkeji.top/gtxankwcxy.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.fengsongda.top/gtbbtwdfmi.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.tianlin.xyz/gtejefnebq.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.yvedp.cn/gtnusgyzjz.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.meibo888.top/gtkgixrekl.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.cdnleiting.top/gtiuroknfg.html

Ruby: rescue ArgumentError => e
来源：http://hz.ywan-chungtsiang.top/gtpbdrmmju.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.zhixingplan.top/gtxjtceqhw.html

[H06] 可选值 / 空值安全访问
来源：http://hz.shzxlz.cn/gtpcgwttux.html

Py:   value = d.get("k") or default
来源：http://hz.zhengqikj.top/gtbwjztxax.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.zhengqikj.top/gtqioipriy.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.zhiwuduotai.top/gtvlzaavbf.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.nanxinkj.top/gtkehwbjii.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.yangfankeji.com/gtubrnwxzy.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.zhijiandao.cn/gtyklpvvzw.html

Ruby: d&.dig(:a, :b)
来源：http://hz.nanxinkj.top/gtqtgefxxi.html

C#:   obj?.A?.B ?? default
来源：http://hz.birdmap.top/gtsdkisemm.html

[H07] 断言
来源：http://hz.gotoacloud.top/gtdtlnsyfh.html

Py:   assert x > 0, "必须为正"
来源：http://hz.shzxlz.cn/gtvqqeetif.html

PHP:  assert($x > 0);
来源：http://hz.yj20258.top/gtzuhvlbdo.html

JS:   console.assert(x > 0);
来源：http://hz.hysaishi.cn/gtvlybhrio.html

TS:   console.assert(x > 0);
来源：http://hz.meibo888.top/gtgqphqwvt.html

Java: assert x > 0 : "必须为正";
来源：http://hz.yonumen.top/gtcuqvkycc.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.zhongyouzk.top/gtbnohnfoq.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.ppjwa.cn/gtzvvkpzpj.html

C#:   Debug.Assert(x > 0);
来源：http://hz.jinqigfzy.top/gtdahucdhf.html

[H08] 获取错误信息与堆栈
来源：http://hz.52xcode.cn/gtgznnujch.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.cucudq.cn/gtsqonuyrc.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.nanxuanxn.top/gtreosupdi.html

JS:   e.message;  e.stack
来源：http://hz.jyoumei.cn/gtyddopvun.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.bjfxy.top/gtbpcpfyiw.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.fzhhl.top/gtzhxwzpbr.html

Go:   err.Error()
来源：http://hz.ywan-chungtsiang.top/gtngvycvwx.html

Ruby: e.message;  e.backtrace
来源：http://hz.aibaodan.cn/gtldjfzsjl.html

C#:   e.Message;  e.StackTrace
来源：http://hz.fengsongda.top/gtdoabztbg.html

[H09] 带错误码的异常
来源：http://hz.dianchejie.cn/gtiorqosht.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.andypj.xyz/gtpzzhpqes.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.hongshengwenyu.top/gtakzbrdgb.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.c1oappe.top/gtfjczwafm.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.quarkkingdee.top/gtdllopwkc.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.cqqwz.cn/gtsgamtksi.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.sxryk.cn/gtmacjlqax.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.andypj.xyz/gtajktptbk.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.guannengcc.top/gtzjsbhzfa.html

[H10] 资源自动释放
来源：http://hz.yangfankeji.com/gtffmervqb.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.hongshengwenyu.top/gtcntctgih.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.sweek.top/gtrtivxuph.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.xylfe.cn/gtpxjwdedk.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.xuanzx.com/gtpfasyjfa.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.aibaodan.cn/gtifpykqew.html

Go:   defer f.Close()
来源：http://hz.pengpengdd.cyou/gtbxizamsj.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.yj20258888.top/gtktqgpotl.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.xingfuxueyuan.xyz/gthsuhtrvp.html

================================================================================
来源：http://hz.jqgufenzy.top/gttgawemzx.html

I. 正则表达式
来源：http://hz.xinyue.icu/gtchqfvwwa.html

================================================================================
来源：http://hz.jinqigufen.top/gtkpfgamnv.html

[I01] 判断是否匹配
来源：http://hz.kuanghao11.cn/gtsyryoimb.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.gaohongyu789.top/gtkfooobbq.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.chenzaomai.com/gtoyniwhzf.html

JS:   /\d+/.test(s)
来源：http://hz.nanxuanxn.top/gtaxmlzqwd.html

TS:   /\d+/.test(s)
来源：http://hz.jinghuilouyu.cn/gtoiujlhoy.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.xuanzx.com/gtsduvvley.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.zhiwuduotai.top/gtpvzgahkh.html

Ruby: s.match?(/\d+/)
来源：http://hz.zycfv.cn/gtfpvmocud.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.fzhhl.top/gtahexjqhl.html

[I02] 提取所有匹配
来源：http://hz.quarkkingdee.top/gtvbvdsyrn.html

Py:   re.findall(r"\d+", s)
来源：http://hz.hfpthk.cn/gtosvcitwn.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.nanxuanxn.top/gtpcpeypvg.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.cucudq.cn/gtitsoneaj.html

TS:   s.match(/\d+/g)
来源：http://hz.xylfe.cn/gtlhirrxuk.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.pycfn.com/gtrqslxrif.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.sysykeji.top/gtawydgqvq.html

Ruby: s.scan(/\d+/)
来源：http://hz.jinyuanbaomall.cn/gtagtxfism.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.xinyue.icu/gtozqcetvm.html

[I03] 提取捕获分组
来源：http://hz.sufxvd.cn/gtxxbmjdnc.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.daria6918.cn/gtfqyxswas.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.ehwqpu.com/gtzrfyunhl.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.zhijiandao.cn/gtltzrchpw.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.cqqwz.cn/gtjthtfjzz.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.ywan-chungtsiang.top/gtapyoyidx.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.tian-w.cn/gtixvguzeg.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.chenlongwang.top/gtecqezgrf.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.yonumen.top/gtjqljlfmr.html

[I04] 正则替换
来源：http://hz.iojbl.cn/gtjbbzgbip.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.zhiwuduotai.top/gtsdvaoyti.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.iojbl.cn/gtnktvqagh.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.jinyuanbaomall.cn/gttbjtyceq.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.feifeiyinyue.top/gtdycfaunj.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.c1oappe.top/gtjnxpluqz.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.yueranfly.top/gtbthaairn.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.xziqi.cn/gtogxjsqxu.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.shangyingyoupin.top/gttsdjtmhe.html

[I05] 按正则拆分
来源：http://hz.yongpay.top/gtwzxqaxvh.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.jinghuilouyu.cn/gtkseuasfq.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.ivvv.top/gtszvucbrl.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.zycfv.cn/gtugjuortt.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.nanxuanxn.top/gtjhwtctsz.html

Java: s.split("\\s*,\\s*")
来源：http://hz.ywan-chungtsiang.top/gtfnzyuzhy.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.quarkkingdee.top/gtixbjyxub.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.shanyushiyangtech.top/gtmqfbeimd.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.yuanzhike.top/gtuhjpncbr.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.ydjk.org.cn/gtxsoxlbsb.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.ehwqpu.com/gtzeqoqsru.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.zhixingplan.top/gtpyzkoxky.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.jinyuanbaomall.cn/gtijubjrvo.html


<!-- 参考信息 -->