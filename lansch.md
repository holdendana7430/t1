代发 wailian999

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.redwolf501.top/gttiuhqlfc.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.guannengcc.top/gtqepopkyq.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.chenlongwang.top/gtlnhzeret.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.ydzc1.top/gtvrynpbul.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.nanxinkj.top/gtguuephsz.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.yongpay.top/gtcsoieohc.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.birdmap.top/gtojpflutl.html

[F12] CSV 读写
来源：http://hz.guannengcc.top/gtvyouqnhk.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.jinqigfzy.top/gtafgrloky.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.snrcjt.cn/gtbtheouvu.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.ydzc1.top/gtyppmqutm.html

TS:   // 同上
来源：http://hz.xinyue.icu/gthoggehgy.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.ppjwa.cn/gthsjwlxoy.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.yonumen.top/gtfnqbvbng.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.sufxvd.cn/gtocfwbvso.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.zhijiandao.cn/gtuihcwomd.html

================================================================================
来源：http://hz.fengsongda.top/gtffocymdg.html

G. 面向对象
来源：http://hz.yangfankeji.com/gtnmjrmeqg.html

================================================================================
来源：http://hz.gzhubu.top/gtrkegbogm.html

[G01] 定义类
来源：http://hz.zdqjudy.top/gtqwllylbs.html

Py:   class User: pass
来源：http://hz.aizwys.cn/gtpkvprskt.html

PHP:  class User {}
来源：http://hz.zdqjudy.top/gtfpbenkrl.html

JS:   class User {}
来源：http://hz.yj202588.top/gtgdhayxxj.html

TS:   class User { name: string = ""; }
来源：http://hz.c1oappe.top/gtlluykesi.html

Java: class User {}
来源：http://hz.jyoumei.cn/gtzfgihsrp.html

Go:   type User struct { Name string }
来源：http://hz.52xcode.cn/gteoevgxzp.html

Ruby: class User; end
来源：http://hz.cheryme.top/gtqmkfkvbm.html

C#:   class User {}
来源：http://hz.zycfv.cn/gtcjwuyscl.html

[G02] 构造函数
来源：http://hz.nanxuanxn.top/gtzdcpfyxb.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.hfpthk.cn/gtphsnqnay.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.xinyue.icu/gtexgnsseb.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.hongshengwenyu.top/gtlckrfxtq.html

TS:   constructor(public name: string) {}
来源：http://hz.daria6918.cn/gtdjwmclsa.html

Java: User(String name) { this.name = name; }
来源：http://hz.gzhubu.top/gthmrvbzju.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.daria6918.cn/gtfzwoyfcq.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.chenzaomai.com/gtnqouwepr.html

C#:   public User(string name) { Name = name; }
来源：http://hz.9152youxi.cn/gthioemnft.html

[G03] 实例属性
来源：http://hz.xingfuxueyuan.xyz/gtebnpexja.html

Py:   self.name = "x"
来源：http://hz.zhijiandao.cn/gtftjhkmrq.html

PHP:  public string $name = "x";
来源：http://hz.meibo888.top/gthxdmiuuu.html

JS:   this.name = "x";
来源：http://hz.9152youxi.cn/gtxssuirjq.html

TS:   name: string = "x";
来源：http://hz.birdmap.top/gthvxazjih.html

Java: private String name;
来源：http://hz.shuidangran.top/gtmknzupwr.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.shzxlz.cn/gtfkatmwrl.html

Ruby: @name = "x"
来源：http://hz.ehwqpu.com/gtntalqtuz.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.cashguo.top/gtjigrtjqo.html

[G04] 定义方法
来源：http://hz.hywenlv.cn/gtzlybkrnh.html

Py:   def greet(self): return self.name
来源：http://hz.yanxiufei.cn/gtdccdbxwx.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.shuidangran.top/gtsnmdtqnl.html

JS:   greet() { return this.name; }
来源：http://hz.zhoulong.xyz/gtpwjsoarn.html

TS:   greet(): string { return this.name; }
来源：http://hz.shanyushiyangkeji.top/gtbylnnows.html

Java: String greet() { return name; }
来源：http://hz.andypj.xyz/gtodvbhuck.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.cqqwz.cn/gtbptsrnst.html

Ruby: def greet; @name; end
来源：http://hz.gotoacloud.top/gtieurreff.html

C#:   public string Greet() => Name;
来源：http://hz.dianchejie.cn/gtdryvvszx.html

[G05] 继承
来源：http://hz.zhixingplan.top/gtwxjqwqmw.html

Py:   class Admin(User): pass
来源：http://hz.yvedp.cn/gtatvvcxet.html

PHP:  class Admin extends User {}
来源：http://hz.0kj1m.cn/gtphayihtl.html

JS:   class Admin extends User {}
来源：http://hz.jianghu66.top/gtbxlyuion.html

TS:   class Admin extends User {}
来源：http://hz.cqqwz.cn/gtqqiuvyof.html

Java: class Admin extends User {}
来源：http://hz.kuanghao11.cn/gtjnrqrpwt.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.xylfe.cn/gtrxhyjydc.html

Ruby: class Admin < User; end
来源：http://hz.jianghu66.top/gtigzlpvts.html

C#:   class Admin : User {}
来源：http://hz.0kj1m.cn/gtfukaqzse.html

[G06] 重写方法
来源：http://hz.nanxinkj.top/gtxudpjvhn.html

Py:   def greet(self): return "admin"
来源：http://hz.zhengqikj.top/gtvmjxwakm.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.gzhubu.top/gtrkuphzch.html

JS:   greet() { return "admin"; }
来源：http://hz.316326.xyz/gtuhdmqseh.html

TS:   greet(): string { return "admin"; }
来源：http://hz.dashuyun.cn/gtwacupdkl.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.vqdsnc.cn/gttcrxlldc.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.gzhubu.top/gtuojrusxu.html

Ruby: def greet; "admin"; end
来源：http://hz.sxryk.cn/gtxboczhbe.html

C#:   public override string Greet() => "admin";
来源：http://hz.mhx1999.top/gtbqdggzxt.html

[G07] 调用父类方法
来源：http://hz.gzhubu.top/gtctevhiel.html

Py:   super().greet()
来源：http://hz.wangdashe.top/gtbkdvbcsf.html

PHP:  parent::greet();
来源：http://hz.xuanzx.com/gtyyghuehf.html

JS:   super.greet();
来源：http://hz.jqgufenzy.top/gtwzpvusit.html

TS:   super.greet();
来源：http://hz.wangshuangyany.cn/gtxwosawpe.html

Java: super.greet();
来源：http://hz.jlsjyb.cn/gtcouemvru.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.yuxming.cn/gtyhgsnfxq.html

Ruby: super
来源：http://hz.sxryk.cn/gtuhmrqqtb.html

C#:   base.Greet();
来源：http://hz.52xcode.cn/gtqwvzwxyq.html

[G08] 静态方法与属性
来源：http://hz.shanyushiyangkeji.top/gtrhwmywln.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.dashuyun.cn/gtfxyfltei.html

PHP:  public static function f() {}
来源：http://hz.tanke756.top/gthkqdjurz.html

JS:   static f() {}
来源：http://hz.cheryme.top/gtvyjrtglt.html

TS:   static f(): void {}
来源：http://hz.xuanzx.com/gtrjyytdue.html

Java: static void f() {}
来源：http://hz.jqgufenzy.top/gtsoixvnyz.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.shzxlz.cn/gtdvlmeatn.html

Ruby: def self.f; end
来源：http://hz.birdmap.top/gtvulzzipa.html

C#:   public static void F() {}
来源：http://hz.sxryk.cn/gtcapneqpt.html

[G09] 接口 / 抽象类
来源：http://hz.quarkkingdee.top/gtyxmcnwxz.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.yongpay.top/gtajlrxuct.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.hongshengwenyu.top/gteflyufel.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.shzxlz.cn/gtxircaqbw.html

TS:   interface Shape { area(): number; }
来源：http://hz.shanyushiyangtech.top/gtyetlwbzy.html

Java: interface Shape { double area(); }
来源：http://hz.jianghu66.top/gtiqijcmoi.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.jinyuanbaomall.cn/gtmbeofpwy.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.ivvv.top/gtmwuwcgiu.html

C#:   interface IShape { double Area(); }
来源：http://hz.kuanghao11.cn/gtbuwxeotc.html

[G10] 访问控制
来源：http://hz.cheryme.top/gthbjzqfwh.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.yueranfly.top/gtjesbjgrt.html

PHP:  public / protected / private
来源：http://hz.pengpengdd.cyou/gtwhnuphsv.html

JS:   #private 字段；其余公开
来源：http://hz.fengsongda.top/gtafpyszjh.html

TS:   public / protected / private
来源：http://hz.yongpay.top/gtbnlpguuo.html

Java: public / protected / private / 默认包级
来源：http://hz.daria6918.cn/gtjiulguuj.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.haohaochexian.top/gtutbztqwv.html

Ruby: public / protected / private
来源：http://hz.52xcode.cn/gtskrnnbrz.html

C#:   public / protected / private / internal
来源：http://hz.daxiang520.top/gtgzsiouqu.html

[G11] getter / setter
来源：http://hz.yj20258888.top/gteseupunp.html

Py:   @property 与 @x.setter
来源：http://hz.aizwys.cn/gtcomutrma.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.guowangkeji.top/gtvntasjse.html

JS:   get name() { return this._name; }
来源：http://hz.ppjwa.cn/gtdgcskwze.html

TS:   get name(): string { return this._name; }
来源：http://hz.chenzaomai.com/gtoukefamy.html

Java: public String getName() { return name; }
来源：http://hz.aibaodan.cn/gtqxtfktpc.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.xinyue.icu/gtchfyejua.html

Ruby: attr_accessor :name
来源：http://hz.xylfe.cn/gtnfpibruk.html

C#:   public string Name { get; set; }
来源：http://hz.cdnleiting.top/gtsgkfqjpy.html

[G12] 对象转字符串
来源：http://hz.ywan-chungtsiang.top/gtkdqbkcno.html

Py:   def __str__(self): return self.name
来源：http://hz.xziqi.cn/gtluywypff.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.xingfuxueyuan.xyz/gtyjgslvdt.html

JS:   toString() { return this.name; }
来源：http://hz.ehwqpu.com/gtyjdsvivc.html

TS:   toString(): string { return this.name; }
来源：http://hz.cheryme.top/gtaqontfno.html

Java: @Override public String toString() { return name; }
来源：http://hz.yanxiufei.cn/gtosohtpsc.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.jinyuanbaomall.cn/gtowlbpawz.html

Ruby: def to_s; @name; end
来源：http://hz.zhoulong.xyz/gtezkdfdfl.html

C#:   public override string ToString() => Name;
来源：http://hz.nanxuanxn.top/gtvcsbgeqk.html

[G13] 判断对象类型
来源：http://hz.yuanzhike.top/gtoppoibrc.html

Py:   isinstance(u, User)
来源：http://hz.mhx1999.top/gtwwsejfvp.html

PHP:  $u instanceof User
来源：http://hz.jiagoushi.top/gtezbdzons.html

JS:   u instanceof User
来源：http://hz.jyoumei.cn/gtfyvcifiy.html

TS:   u instanceof User
来源：http://hz.hongshengwenyu.top/gturpedclo.html

Java: u instanceof User
来源：http://hz.fengsongda.top/gtjslucelo.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.jyoumei.cn/gtzhbfjouw.html

Ruby: u.is_a?(User)
来源：http://hz.guowangkeji.top/gtutdboelm.html

C#:   u is User
来源：http://hz.dashuyun.cn/gtmdyalohu.html

[G14] 数据类 / record
来源：http://hz.316326.xyz/gtjoavizgw.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.jinghuilouyu.cn/gthsqgbudu.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.quarkkingdee.top/gtdfuermso.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.nanxuanxn.top/gtyrpyqedu.html

TS:   type User = { name: string; age: number };
来源：http://hz.yueranfly.top/gttxszbhyp.html

Java: record User(String name, int age) {}
来源：http://hz.jinyuanbaomall.cn/gtbbkswdct.html

Go:   type User struct { Name string; Age int }
来源：http://hz.guannengcc.top/gtoetrkqfc.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.sysykeji.top/gtiibwrzgp.html

C#:   record User(string Name, int Age);
来源：http://hz.0kj1m.cn/gtigtolyvn.html

[G15] 枚举
来源：http://hz.xziqi.cn/gtcavnzgqq.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.aibaodan.cn/gttwkdgruj.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.iojbl.cn/gthcwiwzaw.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.kuanghao11.cn/gteqwbjufg.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.tianlin.xyz/gtcvrgqsyd.html

Java: enum Color { RED, GREEN }
来源：http://hz.quarkkingdee.top/gtefnosehb.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.cashguo.top/gtizrfpety.html

Ruby: Color = %i[red green].freeze
来源：http://hz.dashuyun.cn/gtjwknvfwx.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.svipenyu.cn/gtrbbguwha.html

[G16] 对象转数组 / 字典
来源：http://hz.ivvv.top/gtvswruqfz.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.mhx1999.top/gtxexjuztv.html

PHP:  get_object_vars($obj);
来源：http://hz.ybcxt.top/gtxnjypqlh.html

JS:   Object.entries(obj)
来源：http://hz.aibaodan.cn/gtqvmtogmv.html

TS:   Object.entries(obj)
来源：http://hz.zycfv.cn/gtjaeidkdn.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.jiagoushi.top/gtijyomsov.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.ydjk.org.cn/gtnuzzwjca.html

Ruby: obj.instance_variables
来源：http://hz.nanxuanxn.top/gtsqoqubvw.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.yj20258888.top/gtekpxlmoi.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtfxblbgvk.html

H. 异常与错误处理
来源：http://hz.c1oappe.top/gtpyjmhzqb.html

================================================================================
来源：http://hz.svipenyu.cn/gtepaehdci.html

[H01] try / catch 基础
来源：http://hz.shanyushiyangkeji.top/gtkeqxzsyf.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.wangshuangyany.cn/gtiubhuuqh.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.tianlin.xyz/gtfhxytrdf.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.bjfxy.top/gtqcrzfkkn.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.yueranfly.top/gturbzlceo.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.ehwqpu.com/gttvqkmzwi.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.chenjidiqi.icu/gtvyvqyetn.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.ivvv.top/gtlivhopli.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.zhaomingkeji.xyz/gtgpaobgeg.html

[H02] finally / ensure 收尾
来源：http://hz.mhx1999.top/gtgkjdzfef.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.cqqwz.cn/gtktyystci.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.tanke756.top/gtxgmpccff.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.jinqigfzy.top/gtjteswrvj.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.ppjwa.cn/gtgkiselzf.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.hammf.cn/gtdgeqllyo.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.fzhhl.top/gtsmblvquz.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.redwolf501.top/gtfrjwsxov.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.sysykeji.top/gtliibexvb.html

[H03] 主动抛出异常
来源：http://hz.guowangkeji.top/gtctukmeob.html

Py:   raise ValueError("错误信息")
来源：http://hz.jinyuanbaomall.cn/gtcmyjkefi.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.shanyushiyangkeji.top/gtherdlgpi.html

JS:   throw new Error("错误信息");
来源：http://hz.havefunace.top/gtowbxtzqm.html

TS:   throw new Error("错误信息");
来源：http://hz.nanxuanxn.top/gtqcpbshcm.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.jinghuilouyu.cn/gthvglbpwe.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.pengpengdd.cyou/gtsiicidtf.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.fengsongda.top/gtwkhzwgbu.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.zhixingplan.top/gtlrsitgfa.html

[H04] 自定义异常类型
来源：http://hz.ppjwa.cn/gtognnlhbn.html

Py:   class MyError(Exception): pass
来源：http://hz.xinyue.icu/gtaldwoyvs.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.chenjidiqi.icu/gtyqkvgmbt.html

JS:   class MyError extends Error {}
来源：http://hz.guowangkeji.top/gtxcmqzpnw.html

TS:   class MyError extends Error {}
来源：http://hz.sxryk.cn/gtluwminso.html

Java: class MyException extends RuntimeException {}
来源：http://hz.fzhhl.top/gtkcxgyepo.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.yueranfly.top/gtvjbygskd.html

Ruby: class MyError < StandardError; end
来源：http://hz.gogol.net.cn/gtzougcaxh.html

C#:   class MyException : Exception {}
来源：http://hz.pycfn.com/gtaymusimm.html

[H05] 捕获特定类型
来源：http://hz.snrcjt.cn/gtguzeyjyb.html

Py:   except ValueError as e:
来源：http://hz.kuanghao11.cn/gtriwnybyi.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.meibo888.top/gtimqgkrbj.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.gotoacloud.top/gtbnlvzamc.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.dianchejie.cn/gtjknhtlhj.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.chenjidiqi.icu/gtkgmwyggh.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.daria6918.cn/gtpmlcdrmb.html

Ruby: rescue ArgumentError => e
来源：http://hz.hnxiangtu.top/gteosaeybn.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.mhx1999.top/gtlwbhtbyq.html

[H06] 可选值 / 空值安全访问
来源：http://hz.gaohongyu789.top/gtbujgdcxw.html

Py:   value = d.get("k") or default
来源：http://hz.yuxming.cn/gtppguiexg.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.yangfankeji.com/gtpvmbrrtt.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.ppjwa.cn/gtctlrdckb.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.daria6918.cn/gtdvchltmq.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.zhengqikj.top/gtgisgsvom.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.ehwqpu.com/gtvzsbgoht.html

Ruby: d&.dig(:a, :b)
来源：http://hz.svipenyu.cn/gtekwopznf.html

C#:   obj?.A?.B ?? default
来源：http://hz.shzxlz.cn/gtxizceuop.html

[H07] 断言
来源：http://hz.gotoacloud.top/gtqotbclkt.html

Py:   assert x > 0, "必须为正"
来源：http://hz.redwolf501.top/gteplwcmja.html

PHP:  assert($x > 0);
来源：http://hz.daria6918.cn/gtiqjagflm.html

JS:   console.assert(x > 0);
来源：http://hz.shzxlz.cn/gtijqnvvdb.html

TS:   console.assert(x > 0);
来源：http://hz.fengsongda.top/gtaknseaaw.html

Java: assert x > 0 : "必须为正";
来源：http://hz.chenlongwang.top/gtqftqfcxg.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.nanxuanxn.top/gtmwkjkrlf.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.haohaochexian.top/gtikgnysvf.html

C#:   Debug.Assert(x > 0);
来源：http://hz.sufxvd.cn/gtuiwmhxks.html

[H08] 获取错误信息与堆栈
来源：http://hz.sweek.top/gtvbexpehe.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.cqqwz.cn/gthibxqprj.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.c1oappe.top/gtfadelorh.html

JS:   e.message;  e.stack
来源：http://hz.andypj.xyz/gtuoycodbg.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.cheryme.top/gtoelwczys.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.jqgfzy.top/gtjjfwzqxj.html

Go:   err.Error()
来源：http://hz.hongshengwenyu.top/gtetofrweu.html

Ruby: e.message;  e.backtrace
来源：http://hz.yangfankeji.com/gtgwozvipc.html

C#:   e.Message;  e.StackTrace
来源：http://hz.cqqwz.cn/gtqzatatuo.html

[H09] 带错误码的异常
来源：http://hz.chenlongwang.top/gtpgiwrjyl.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.hywenlv.cn/gtihzsnuav.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.yvedp.cn/gtwsnbviio.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.dianchejie.cn/gtroihkgrh.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.kuanghao11.cn/gtwpgkqrua.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.cheryme.top/gtbcolwakx.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.shangyingyoupin.top/gtyjnspedt.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.yvedp.cn/gtroxiifjv.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.xinyue.icu/gtvqkcivyy.html

[H10] 资源自动释放
来源：http://hz.wangshuangyany.cn/gtyuzznjdq.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.zhaomingkeji.xyz/gtdznzcznk.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.cdnleiting.top/gtrkaakhey.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.zhiwuduotai.top/gtezqcmwul.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.aibaodan.cn/gtobacxrmf.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.dianchejie.cn/gtzagjwznj.html

Go:   defer f.Close()
来源：http://hz.yangfankeji.com/gtvxqyomgk.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.ywan-chungtsiang.top/gtyiwpljhm.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.yuanzhike.top/gtmvzrulmh.html

================================================================================
来源：http://hz.yanxiufei.cn/gtbeatkknp.html

I. 正则表达式
来源：http://hz.mhx1999.top/gtktoeuyby.html

================================================================================
来源：http://hz.svipenyu.cn/gtggagnadd.html

[I01] 判断是否匹配
来源：http://hz.shanyushiyangtech.top/gtqzkriqir.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.feifeiyinyue.top/gtvldllmwn.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.316326.xyz/gtxfiatafv.html

JS:   /\d+/.test(s)
来源：http://hz.cucudq.cn/gtxyjpjbfs.html

TS:   /\d+/.test(s)
来源：http://hz.ybcxt.top/gttcsrqieo.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.c1oappe.top/gtqsaqgeoz.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.cqqwz.cn/gtzouiyror.html

Ruby: s.match?(/\d+/)
来源：http://hz.sufxvd.cn/gthpcitigx.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.shuidangran.top/gtafkqucey.html

[I02] 提取所有匹配
来源：http://hz.zhijiandao.cn/gtylpzxdxj.html

Py:   re.findall(r"\d+", s)
来源：http://hz.quarkkingdee.top/gtbclkafhg.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.andypj.xyz/gtivkxxssz.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.yj20258888.top/gtvpxswpni.html

TS:   s.match(/\d+/g)
来源：http://hz.cashguo.top/gtxgdsifrg.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.9152youxi.cn/gtioqaapqm.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.daxiang520.top/gtarvakzjp.html

Ruby: s.scan(/\d+/)
来源：http://hz.guannengcc.top/gtirhranrq.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.fengsongda.top/gtogzvehet.html

[I03] 提取捕获分组
来源：http://hz.zhiwuduotai.top/gtcbeslfdj.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.birdmap.top/gtbbmnelnx.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.zdqjudy.top/gtbgarxqwc.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.wangdashe.top/gtqywfbwej.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.meibo888.top/gtxkvmfvew.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.0kj1m.cn/gtcrgelibm.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.haohaochexian.top/gtrcqpljln.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.ivvv.top/gtszxlnnsn.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.jinyuanbaomall.cn/gtltdyoxvk.html

[I04] 正则替换
来源：http://hz.quarkkingdee.top/gtuietrulg.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.zdqjudy.top/gtotdsvmaw.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.pengpengdd.cyou/gtrbfvntbg.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.zhijiandao.cn/gtfmnakyhr.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.316326.xyz/gtshjainke.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.zhoulong.xyz/gtdxdjxzvp.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.tian-w.cn/gtcngkpthn.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.guowangkeji.top/gthunvuzrt.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.jinghuilouyu.cn/gtumngibyb.html

[I05] 按正则拆分
来源：http://hz.xziqi.cn/gtkcgkvkva.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.hysaishi.cn/gtmkrvqrnz.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.jianghu66.top/gtifgzibgs.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.zhoulong.xyz/gtvctpfqew.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.zycfv.cn/gtdobpcixc.html


<!-- 参考信息 -->