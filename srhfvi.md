代发 wailian999

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.hnqzz.top/gtxcbzcyhl.html

TS:   path.extname("a.txt")
来源：http://hz.haohaochexian.top/gthyhjkauq.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.zhijiandao.cn/gtockwklbe.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.tanke756.top/gtvfsemoxx.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.vqdsnc.cn/gtnyzwyxqa.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.chenlongwang.top/gtcwjfrugx.html

[F11] 复制与移动文件
来源：http://hz.jqgfzy.top/gtxepkfnoh.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.zhengqikj.top/gtvgzavzsp.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.xziqi.cn/gtgfzmfquy.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.kuanghao11.cn/gtqkkknbuj.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.xylfe.cn/gtckavkcxd.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.316326.xyz/gtfoomjlyu.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.ehwqpu.com/gtvinduhov.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.nanxinkj.top/gtdqqhvqtn.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.yueranfly.top/gtrjjjyoyt.html

[F12] CSV 读写
来源：http://hz.iojbl.cn/gtjbtvqxsl.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.c1oappe.top/gtbofuzifz.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.xziqi.cn/gtchkndlia.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.quarkkingdee.top/gtbacjaubp.html

TS:   // 同上
来源：http://hz.fengsongda.top/gtdmkfjsgq.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.meibo888.top/gtqutpmgwv.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.yj20258888.top/gtwfowzbgc.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.jqgufenzy.top/gtxvmektrc.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.yangfankeji.com/gtxdydzdas.html

================================================================================
来源：http://hz.ehwqpu.com/gtgjhubwph.html

G. 面向对象
来源：http://hz.zhixingplan.top/gtdwodbfaa.html

================================================================================
来源：http://hz.sysykeji.top/gtojmuisqt.html

[G01] 定义类
来源：http://hz.sweek.top/gtzshvbmye.html

Py:   class User: pass
来源：http://hz.gogol.net.cn/gtwazgscbo.html

PHP:  class User {}
来源：http://hz.yvedp.cn/gtzyhlclrd.html

JS:   class User {}
来源：http://hz.dianchejie.cn/gtswfaurjf.html

TS:   class User { name: string = ""; }
来源：http://hz.dashuyun.cn/gtsfohzwyz.html

Java: class User {}
来源：http://hz.pycfn.com/gtmepxxfhb.html

Go:   type User struct { Name string }
来源：http://hz.nanxuanxn.top/gtqteughev.html

Ruby: class User; end
来源：http://hz.gaohongyu789.top/gtuzgaynpb.html

C#:   class User {}
来源：http://hz.jqgfzy.top/gtswghwmsa.html

[G02] 构造函数
来源：http://hz.jinqigufen.top/gtzgoeteli.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.9152youxi.cn/gtyttxjgkf.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.yj20258888.top/gtpcrhnzjb.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.smart0.xyz/gtnwhjsgeq.html

TS:   constructor(public name: string) {}
来源：http://hz.zdqjudy.top/gtczstagvj.html

Java: User(String name) { this.name = name; }
来源：http://hz.zhengqikj.top/gtmeqyhuwn.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.cheryme.top/gteqobwpcv.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.gogol.net.cn/gtihnnrgvi.html

C#:   public User(string name) { Name = name; }
来源：http://hz.yuxming.cn/gtksgwcqit.html

[G03] 实例属性
来源：http://hz.yongpay.top/gttauzewby.html

Py:   self.name = "x"
来源：http://hz.jinqigufen.top/gtyolgvvzd.html

PHP:  public string $name = "x";
来源：http://hz.tian-w.cn/gtwuxsygfi.html

JS:   this.name = "x";
来源：http://hz.jyoumei.cn/gtbmywnmke.html

TS:   name: string = "x";
来源：http://hz.shanyushiyangtech.top/gtahwfxzli.html

Java: private String name;
来源：http://hz.wangshuangyany.cn/gtkumxwwip.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.yj20258888.top/gtlskcxteq.html

Ruby: @name = "x"
来源：http://hz.nwbrower.top/gtotvrvlhg.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.meibo888.top/gtpjqpbjyy.html

[G04] 定义方法
来源：http://hz.xingfuxueyuan.xyz/gtkjyqywxd.html

Py:   def greet(self): return self.name
来源：http://hz.hywenlv.cn/gtyubxppca.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.yuanzhike.top/gtoheemcgv.html

JS:   greet() { return this.name; }
来源：http://hz.yuanzhike.top/gtrwrbzmfk.html

TS:   greet(): string { return this.name; }
来源：http://hz.zdqjudy.top/gtzihjxxfl.html

Java: String greet() { return name; }
来源：http://hz.jinghuilouyu.cn/gtojwfyioj.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.cdnleiting.top/gtpjfswuom.html

Ruby: def greet; @name; end
来源：http://hz.ppjwa.cn/gtlvlfksyq.html

C#:   public string Greet() => Name;
来源：http://hz.jinqigufen.top/gthkjbzrbe.html

[G05] 继承
来源：http://hz.tianlin.xyz/gtvkdylmyb.html

Py:   class Admin(User): pass
来源：http://hz.xuanzx.com/gtvfryfyxp.html

PHP:  class Admin extends User {}
来源：http://hz.yangfankeji.com/gtkhvfiscn.html

JS:   class Admin extends User {}
来源：http://hz.hfpthk.cn/gtbfrjlzwq.html

TS:   class Admin extends User {}
来源：http://hz.zhiwuduotai.top/gtgrkjmkvd.html

Java: class Admin extends User {}
来源：http://hz.xziqi.cn/gtkhuimrjw.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.quarkkingdee.top/gtpigwesyc.html

Ruby: class Admin < User; end
来源：http://hz.hammf.cn/gtoylrscpc.html

C#:   class Admin : User {}
来源：http://hz.fzhhl.top/gtcuohcsdy.html

[G06] 重写方法
来源：http://hz.tianlin.xyz/gtloruakuz.html

Py:   def greet(self): return "admin"
来源：http://hz.c1oappe.top/gtcqcynxuc.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.yuxming.cn/gtrrdpnyjn.html

JS:   greet() { return "admin"; }
来源：http://hz.hammf.cn/gtobrqvbgh.html

TS:   greet(): string { return "admin"; }
来源：http://hz.fengsongda.top/gtlqhbwlaz.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.zhijiandao.cn/gtxnzunzlb.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.zdqjudy.top/gtulxvlndl.html

Ruby: def greet; "admin"; end
来源：http://hz.gaohongyu789.top/gtsxweqpxr.html

C#:   public override string Greet() => "admin";
来源：http://hz.ehwqpu.com/gtgdrfyogb.html

[G07] 调用父类方法
来源：http://hz.ppjwa.cn/gtrtjhffrd.html

Py:   super().greet()
来源：http://hz.fengsongda.top/gtcgmthvpw.html

PHP:  parent::greet();
来源：http://hz.tanke756.top/gtykddispw.html

JS:   super.greet();
来源：http://hz.jianghu66.top/gtqttavlvt.html

TS:   super.greet();
来源：http://hz.sxryk.cn/gthlgvfycq.html

Java: super.greet();
来源：http://hz.zhiwuduotai.top/gtkotixlcq.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.yangfankeji.com/gthnojvrqw.html

Ruby: super
来源：http://hz.c1oappe.top/gtrxhwkvhe.html

C#:   base.Greet();
来源：http://hz.ybcxt.top/gtjfmegidb.html

[G08] 静态方法与属性
来源：http://hz.sysykeji.top/gtdgqanjyc.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.xuanzx.com/gtocbaodvh.html

PHP:  public static function f() {}
来源：http://hz.jqgfzy.top/gtsvmpondq.html

JS:   static f() {}
来源：http://hz.gotoacloud.top/gtjhiqjyfn.html

TS:   static f(): void {}
来源：http://hz.yanxiufei.cn/gtyynjmyfa.html

Java: static void f() {}
来源：http://hz.dianchejie.cn/gticsgpygg.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.daxiang520.top/gttbgarbxy.html

Ruby: def self.f; end
来源：http://hz.smart0.xyz/gttzohibvl.html

C#:   public static void F() {}
来源：http://hz.cheryme.top/gtnvoneadh.html

[G09] 接口 / 抽象类
来源：http://hz.yuanzhike.top/gtuhzezibp.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.dianchejie.cn/gtsxlrqeqk.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.yangfankeji.com/gtniztvszz.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.cucudq.cn/gtgnqzbusg.html

TS:   interface Shape { area(): number; }
来源：http://hz.52xcode.cn/gtposkiobs.html

Java: interface Shape { double area(); }
来源：http://hz.kuanghao11.cn/gtvkqfeiuh.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.yangfankeji.com/gtwumfyfgz.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.fzhhl.top/gtvtepofuy.html

C#:   interface IShape { double Area(); }
来源：http://hz.fzhhl.top/gtstgmrlhv.html

[G10] 访问控制
来源：http://hz.yueranfly.top/gtfpqlyaoc.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.mhx1999.top/gtxgmxlkod.html

PHP:  public / protected / private
来源：http://hz.yuanzhike.top/gtsdxlmpre.html

JS:   #private 字段；其余公开
来源：http://hz.tanke756.top/gtbuguczdq.html

TS:   public / protected / private
来源：http://hz.jyoumei.cn/gtpscdzzrn.html

Java: public / protected / private / 默认包级
来源：http://hz.shzxlz.cn/gtlyfpqcfu.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.hnxiangtu.top/gtuymkzbdb.html

Ruby: public / protected / private
来源：http://hz.cdnleiting.top/gtcsydqhdd.html

C#:   public / protected / private / internal
来源：http://hz.shanyushiyangtech.top/gtqdbsmgfy.html

[G11] getter / setter
来源：http://hz.ivvv.top/gtkajgfvne.html

Py:   @property 与 @x.setter
来源：http://hz.yuanzhike.top/gtiharmbuq.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.cdnleiting.top/gttqyciapl.html

JS:   get name() { return this._name; }
来源：http://hz.52xcode.cn/gtbqcdxyfe.html

TS:   get name(): string { return this._name; }
来源：http://hz.smart0.xyz/gtlhintaiw.html

Java: public String getName() { return name; }
来源：http://hz.zdqjudy.top/gtmtfredlf.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.wangdashe.top/gtinsiiapq.html

Ruby: attr_accessor :name
来源：http://hz.zhijiandao.cn/gtldzumfgi.html

C#:   public string Name { get; set; }
来源：http://hz.hongshengwenyu.top/gtvpglukuw.html

[G12] 对象转字符串
来源：http://hz.sweek.top/gttjmfctmj.html

Py:   def __str__(self): return self.name
来源：http://hz.sweek.top/gtebvcaxcr.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.zycfv.cn/gtfcnlbrgr.html

JS:   toString() { return this.name; }
来源：http://hz.zhijiandao.cn/gtvreclffa.html

TS:   toString(): string { return this.name; }
来源：http://hz.chenlongwang.top/gtbrjidpzl.html

Java: @Override public String toString() { return name; }
来源：http://hz.xuetiantiany.cn/gtvehakuam.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.c1oappe.top/gtentxpklk.html

Ruby: def to_s; @name; end
来源：http://hz.c1oappe.top/gtwybadagw.html

C#:   public override string ToString() => Name;
来源：http://hz.tianlin.xyz/gtzqdtfnit.html

[G13] 判断对象类型
来源：http://hz.zhaomingkeji.xyz/gtragegtgc.html

Py:   isinstance(u, User)
来源：http://hz.snrcjt.cn/gtzmvudgwb.html

PHP:  $u instanceof User
来源：http://hz.gaohongyu789.top/gtssikwpow.html

JS:   u instanceof User
来源：http://hz.feifeiyinyue.top/gtwgsajfoh.html

TS:   u instanceof User
来源：http://hz.svipenyu.cn/gtlqtoldrk.html

Java: u instanceof User
来源：http://hz.yuxming.cn/gtexndqaun.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.jlsjyb.cn/gtgvmepjaw.html

Ruby: u.is_a?(User)
来源：http://hz.daxiang520.top/gtalykverk.html

C#:   u is User
来源：http://hz.ywan-chungtsiang.top/gtuebasoqs.html

[G14] 数据类 / record
来源：http://hz.andypj.xyz/gtqhrjxcsv.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.kuanghao11.cn/gtplilogme.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.cdnleiting.top/gtuynhcqas.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.quarkkingdee.top/gtbvayvowa.html

TS:   type User = { name: string; age: number };
来源：http://hz.pycfn.com/gtmetmgogd.html

Java: record User(String name, int age) {}
来源：http://hz.jinqigufen.top/gtuvticumg.html

Go:   type User struct { Name string; Age int }
来源：http://hz.guannengcc.top/gtyqjphfdv.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.yanxiufei.cn/gtevulmrzu.html

C#:   record User(string Name, int Age);
来源：http://hz.yangfankeji.com/gtahvioqxy.html

[G15] 枚举
来源：http://hz.yuxming.cn/gttfiysgdk.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.svipenyu.cn/gtjclyiwqc.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.yj202588.top/gtopuudlgm.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.jinqigufen.top/gthafcmhtc.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.jianghu66.top/gtpljthkrp.html

Java: enum Color { RED, GREEN }
来源：http://hz.iojbl.cn/gtfyngktoa.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.guowangkeji.top/gttmpuzqiu.html

Ruby: Color = %i[red green].freeze
来源：http://hz.tanke756.top/gtzfrhitbh.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.pycfn.com/gtbmvmuros.html

[G16] 对象转数组 / 字典
来源：http://hz.sysykeji.top/gtfkxqvxuv.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.cucudq.cn/gtekwrozbk.html

PHP:  get_object_vars($obj);
来源：http://hz.snrcjt.cn/gtcxudmcsw.html

JS:   Object.entries(obj)
来源：http://hz.xinyue.icu/gtfugspbht.html

TS:   Object.entries(obj)
来源：http://hz.hywenlv.cn/gtwuuurrrm.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.fzhhl.top/gtzmwsonbo.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.cheryme.top/gtyflemnjv.html

Ruby: obj.instance_variables
来源：http://hz.nanxinkj.top/gtfrzlrkeg.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.jlsjyb.cn/gtuvrtonxz.html

================================================================================
来源：http://hz.hfpthk.cn/gtfgfqvpmr.html

H. 异常与错误处理
来源：http://hz.quarkkingdee.top/gtsacmxqhi.html

================================================================================
来源：http://hz.tianlin.xyz/gtzyyuueop.html

[H01] try / catch 基础
来源：http://hz.vqdsnc.cn/gtqovabzmm.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.gogol.net.cn/gtdptyfgct.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.jqgfzy.top/gtziintjty.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.gotoacloud.top/gtathgzirh.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.hnqzz.top/gtxpomhezq.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.xinyue.icu/gtayicswho.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.52xcode.cn/gtixzlwcrt.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.shuidangran.top/gtzlxeynsb.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.yuxming.cn/gtpjboxmuv.html

[H02] finally / ensure 收尾
来源：http://hz.cdnleiting.top/gtwtafdvui.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.c1oappe.top/gthxrthxxd.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.hfpthk.cn/gtzsancvwb.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.hnqzz.top/gtllfztoay.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.zhixingplan.top/gtsqzqcdgy.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.xziqi.cn/gtfjmaxfue.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.ppjwa.cn/gtepnyxujv.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.jlsjyb.cn/gtfalmulvt.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.hongshengwenyu.top/gtynpwmxyq.html

[H03] 主动抛出异常
来源：http://hz.ivvv.top/gtzchhoklx.html

Py:   raise ValueError("错误信息")
来源：http://hz.guannengcc.top/gtfqsckysl.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.yj202588.top/gtnnluxozm.html

JS:   throw new Error("错误信息");
来源：http://hz.iojbl.cn/gtpuwulzfu.html

TS:   throw new Error("错误信息");
来源：http://hz.svipenyu.cn/gtscdcezrv.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.chenjidiqi.icu/gtoprezxwr.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.aizwys.cn/gtifjmlwpi.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.hywenlv.cn/gtgeyfthxr.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.nwbrower.top/gtazfvnfsc.html

[H04] 自定义异常类型
来源：http://hz.316326.xyz/gtvqmdsuup.html

Py:   class MyError(Exception): pass
来源：http://hz.cashguo.top/gtgazgdotj.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.guannengcc.top/gtkjlrygoh.html

JS:   class MyError extends Error {}
来源：http://hz.shanyushiyangkeji.top/gtfsvozbbw.html

TS:   class MyError extends Error {}
来源：http://hz.cqqwz.cn/gtnvojikno.html

Java: class MyException extends RuntimeException {}
来源：http://hz.cashguo.top/gtqfdfyvhz.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.yonumen.top/gtunbvfqos.html

Ruby: class MyError < StandardError; end
来源：http://hz.xinyue.icu/gtszoicrzh.html

C#:   class MyException : Exception {}
来源：http://hz.mhx1999.top/gtthgovnpn.html

[H05] 捕获特定类型
来源：http://hz.yvedp.cn/gtxsluvfya.html

Py:   except ValueError as e:
来源：http://hz.wangshuangyany.cn/gtjeqehcjb.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.cucudq.cn/gttfphdrqb.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.yuxming.cn/gtxonfipay.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.shanyushiyangkeji.top/gtcibpunlb.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.xuetiantiany.cn/gtkplhlppa.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.zhaomingkeji.xyz/gtbqpkqjqe.html

Ruby: rescue ArgumentError => e
来源：http://hz.hongshengwenyu.top/gtgvafwcvc.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.feifeiyinyue.top/gteltibolc.html

[H06] 可选值 / 空值安全访问
来源：http://hz.yj20258888.top/gtzfanmhje.html

Py:   value = d.get("k") or default
来源：http://hz.jinghuilouyu.cn/gtwqjclymp.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.yonumen.top/gtxhcguqzh.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.ybcxt.top/gtwqbdzzoj.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.havefunace.top/gtydjxbmbu.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.bjfxy.top/gtzslgkeif.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.redwolf501.top/gtpvrlokji.html

Ruby: d&.dig(:a, :b)
来源：http://hz.tian-w.cn/gtxcjklmro.html

C#:   obj?.A?.B ?? default
来源：http://hz.ywan-chungtsiang.top/gtobgaipuw.html

[H07] 断言
来源：http://hz.meibo888.top/gtwmqiiyuf.html

Py:   assert x > 0, "必须为正"
来源：http://hz.redwolf501.top/gtiiacfnnj.html

PHP:  assert($x > 0);
来源：http://hz.guannengcc.top/gtwdtbkytb.html

JS:   console.assert(x > 0);
来源：http://hz.guannengcc.top/gtqgjyxsgc.html

TS:   console.assert(x > 0);
来源：http://hz.cheryme.top/gtluuxegey.html

Java: assert x > 0 : "必须为正";
来源：http://hz.gotoacloud.top/gtiqurdxqc.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.jyoumei.cn/gtaswmuyfl.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.hnxiangtu.top/gtmmbxafqw.html

C#:   Debug.Assert(x > 0);
来源：http://hz.fzhhl.top/gthkyjiybv.html

[H08] 获取错误信息与堆栈
来源：http://hz.gzhubu.top/gtmxdasniz.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.jyoumei.cn/gtcrsmlsef.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.yueranfly.top/gtipqwiskp.html

JS:   e.message;  e.stack
来源：http://hz.jinghuilouyu.cn/gtgngqhlot.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.redwolf501.top/gthnpfgsbf.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.jqgufenzy.top/gtitsftrhp.html

Go:   err.Error()
来源：http://hz.nanxinkj.top/gttlxppwwx.html

Ruby: e.message;  e.backtrace
来源：http://hz.pycfn.com/gtvjcwbcgn.html

C#:   e.Message;  e.StackTrace
来源：http://hz.zhaomingkeji.xyz/gtiasisogt.html

[H09] 带错误码的异常
来源：http://hz.redwolf501.top/gtdsghtuhj.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.zhaomingkeji.xyz/gtlxgaxssf.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.dianchejie.cn/gtcrtjvwob.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.redwolf501.top/gtjzrknzqa.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.haohaochexian.top/gtiukobalb.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.bjfxy.top/gtjolzjshl.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.zhengqikj.top/gtskxifyui.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.52xcode.cn/gtsxwesmcm.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.jlsjyb.cn/gtolgoawox.html

[H10] 资源自动释放
来源：http://hz.pycfn.com/gtatowwequ.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.sweek.top/gtozoikcyk.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.mhx1999.top/gtfcjqpfuu.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.dianchejie.cn/gtwidwjmdm.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.quarkkingdee.top/gtykplxjju.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.hongshengwenyu.top/gtcplhilke.html

Go:   defer f.Close()
来源：http://hz.gzhubu.top/gtyopemoxp.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.jinqigfzy.top/gtyqxoiotk.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.guowangkeji.top/gttmmdrrrr.html

================================================================================
来源：http://hz.sweek.top/gtczykermg.html

I. 正则表达式
来源：http://hz.chenzaomai.com/gtjpnirzck.html

================================================================================
来源：http://hz.dianchejie.cn/gtpmwepmer.html

[I01] 判断是否匹配
来源：http://hz.xylfe.cn/gtraqgasvs.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.yuxming.cn/gtdrocvchs.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.yj20258.top/gtqhlrfqvr.html

JS:   /\d+/.test(s)
来源：http://hz.jinghuilouyu.cn/gtvwhdanbc.html

TS:   /\d+/.test(s)
来源：http://hz.sxryk.cn/gtkidiardo.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.aizwys.cn/gtjeexixlf.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.fzhhl.top/gtdemzwaqc.html

Ruby: s.match?(/\d+/)
来源：http://hz.ivvv.top/gtvimjmadd.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.jinyuanbaomall.cn/gtjzenjwls.html

[I02] 提取所有匹配
来源：http://hz.guowangkeji.top/gtzdtiarjm.html

Py:   re.findall(r"\d+", s)
来源：http://hz.zycfv.cn/gtequegurq.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.shangyingyoupin.top/gtelgahipo.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.cucudq.cn/gtpqzacjtq.html

TS:   s.match(/\d+/g)
来源：http://hz.kuanghao11.cn/gttccnxuir.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.shuidangran.top/gtbgovxtnu.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.tian-w.cn/gtkiqhmkei.html

Ruby: s.scan(/\d+/)
来源：http://hz.zhiwuduotai.top/gtakafeaks.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.jlsjyb.cn/gtmwyeozyh.html

[I03] 提取捕获分组
来源：http://hz.xuetiantiany.cn/gtbryhzswm.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.cqqwz.cn/gtpscrfotj.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.jlsjyb.cn/gtxysdjdtp.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.xuetiantiany.cn/gtetudahxe.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.zhaomingkeji.xyz/gtwmeekruq.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.jyoumei.cn/gtnkzznftd.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.jinqigfzy.top/gtrlkipjuq.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.ybcxt.top/gtzsjiypum.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.zhengqikj.top/gttlokrhbt.html

[I04] 正则替换
来源：http://hz.feifeiyinyue.top/gtuibyrous.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.chenzaomai.com/gtpeoimcnj.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.gaohongyu789.top/gtyecucbeg.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.wangdashe.top/gtrojhcjfa.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.yj202588.top/gtzurjygbv.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.wangshuangyany.cn/gtsuqvrrpr.html


<!-- 参考信息 -->