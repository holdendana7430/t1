代发 wailian999

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.cucudq.cn/gtajkcckjc.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.jiagoushi.top/gtizwkwjcm.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.nanxuanxn.top/gtstipfhzy.html

[F12] CSV 读写
来源：http://hz.0kj1m.cn/gtcgidzzaq.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.gzhubu.top/gtspcjzlda.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.nanxuanxn.top/gtkhbfekun.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.cdnleiting.top/gtnuseabej.html

TS:   // 同上
来源：http://hz.cucudq.cn/gttnqsztye.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.wangshuangyany.cn/gtnoniteda.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.ivvv.top/gtklibisfm.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.yj20258888.top/gtfxgqpajy.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.gotoacloud.top/gtvhagilrq.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtciobdkil.html

G. 面向对象
来源：http://hz.bjfxy.top/gtmtvlggdv.html

================================================================================
来源：http://hz.jqgfzy.top/gtwnsyvzji.html

[G01] 定义类
来源：http://hz.birdmap.top/gtdihycthq.html

Py:   class User: pass
来源：http://hz.ehwqpu.com/gtpukapjju.html

PHP:  class User {}
来源：http://hz.ybcxt.top/gtqzuoapyz.html

JS:   class User {}
来源：http://hz.ywan-chungtsiang.top/gtkhhroknr.html

TS:   class User { name: string = ""; }
来源：http://hz.chenzaomai.com/gtbhgwedde.html

Java: class User {}
来源：http://hz.sysykeji.top/gtckwczzgk.html

Go:   type User struct { Name string }
来源：http://hz.ppjwa.cn/gtpdqggjkc.html

Ruby: class User; end
来源：http://hz.cucudq.cn/gtqlkfcspp.html

C#:   class User {}
来源：http://hz.yuanzhike.top/gtzeljlqxk.html

[G02] 构造函数
来源：http://hz.shanyushiyangkeji.top/gtwwookjqi.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.havefunace.top/gtaiwsnmxq.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.9152youxi.cn/gtlophjsbd.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.nwbrower.top/gtpyysucpd.html

TS:   constructor(public name: string) {}
来源：http://hz.ivvv.top/gthmbzovpj.html

Java: User(String name) { this.name = name; }
来源：http://hz.yanxiufei.cn/gtpunohxxn.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.jlsjyb.cn/gteqfksxvf.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.xinyue.icu/gtjxaszuig.html

C#:   public User(string name) { Name = name; }
来源：http://hz.tian-w.cn/gtottrdalu.html

[G03] 实例属性
来源：http://hz.tian-w.cn/gtfnlcepen.html

Py:   self.name = "x"
来源：http://hz.gaohongyu789.top/gtlioecrhz.html

PHP:  public string $name = "x";
来源：http://hz.zhaomingkeji.xyz/gtwbuwmezs.html

JS:   this.name = "x";
来源：http://hz.shanyushiyangkeji.top/gtdzysqtaq.html

TS:   name: string = "x";
来源：http://hz.yj20258.top/gtczuvicsj.html

Java: private String name;
来源：http://hz.nanxinkj.top/gtmmmxhbad.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.zhiwuduotai.top/gtsraijlco.html

Ruby: @name = "x"
来源：http://hz.shzxlz.cn/gtkswnchln.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.chenjidiqi.icu/gtwjzeiujz.html

[G04] 定义方法
来源：http://hz.ywan-chungtsiang.top/gtasnhcbfo.html

Py:   def greet(self): return self.name
来源：http://hz.jqgufenzy.top/gtdorxiabw.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.daxiang520.top/gthihdlkgw.html

JS:   greet() { return this.name; }
来源：http://hz.xingfuxueyuan.xyz/gtirmbpxys.html

TS:   greet(): string { return this.name; }
来源：http://hz.yj20258.top/gtgefilmcp.html

Java: String greet() { return name; }
来源：http://hz.birdmap.top/gtnjagjplv.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.jinyuanbaomall.cn/gtiugjshty.html

Ruby: def greet; @name; end
来源：http://hz.hnxiangtu.top/gtaiplmjou.html

C#:   public string Greet() => Name;
来源：http://hz.mhx1999.top/gtiyesulzr.html

[G05] 继承
来源：http://hz.pengpengdd.cyou/gtwruyavzk.html

Py:   class Admin(User): pass
来源：http://hz.hnxiangtu.top/gtsclybsuz.html

PHP:  class Admin extends User {}
来源：http://hz.hywenlv.cn/gtbvjqutce.html

JS:   class Admin extends User {}
来源：http://hz.hywenlv.cn/gtwhxewciv.html

TS:   class Admin extends User {}
来源：http://hz.wangdashe.top/gtbxspfjpu.html

Java: class Admin extends User {}
来源：http://hz.ppjwa.cn/gtkrpcfmpg.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.ydzc1.top/gtweqrqosx.html

Ruby: class Admin < User; end
来源：http://hz.tianlin.xyz/gtsaedtpwe.html

C#:   class Admin : User {}
来源：http://hz.haohaochexian.top/gtaxrxxnkx.html

[G06] 重写方法
来源：http://hz.sysykeji.top/gttzkjyerm.html

Py:   def greet(self): return "admin"
来源：http://hz.shzxlz.cn/gtdprisqjy.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.sweek.top/gthagtepiu.html

JS:   greet() { return "admin"; }
来源：http://hz.zdqjudy.top/gtkpfqchew.html

TS:   greet(): string { return "admin"; }
来源：http://hz.pycfn.com/gtdedgexcz.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.xinyue.icu/gtayhplaan.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.zhijiandao.cn/gtkxjtpjol.html

Ruby: def greet; "admin"; end
来源：http://hz.zhoulong.xyz/gtnmoellwq.html

C#:   public override string Greet() => "admin";
来源：http://hz.dashuyun.cn/gtlebbxgzf.html

[G07] 调用父类方法
来源：http://hz.zdqjudy.top/gttzzfcqjx.html

Py:   super().greet()
来源：http://hz.hnxiangtu.top/gtezichvwi.html

PHP:  parent::greet();
来源：http://hz.zhijiandao.cn/gtckcenlsf.html

JS:   super.greet();
来源：http://hz.guowangkeji.top/gtducljmgn.html

TS:   super.greet();
来源：http://hz.sweek.top/gtkrtnzriq.html

Java: super.greet();
来源：http://hz.tian-w.cn/gtgtbouehl.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.zhengqikj.top/gtdsscdbhe.html

Ruby: super
来源：http://hz.xingfuxueyuan.xyz/gtzxguryyw.html

C#:   base.Greet();
来源：http://hz.zycfv.cn/gtvexzdjca.html

[G08] 静态方法与属性
来源：http://hz.52xcode.cn/gthttbwsjl.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.cdnleiting.top/gtqqzldqya.html

PHP:  public static function f() {}
来源：http://hz.vqdsnc.cn/gtrhmkaxoe.html

JS:   static f() {}
来源：http://hz.shanyushiyangtech.top/gtwhmnhiwm.html

TS:   static f(): void {}
来源：http://hz.chenjidiqi.icu/gtxswqihfz.html

Java: static void f() {}
来源：http://hz.meibo888.top/gtejykqjgg.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.shuidangran.top/gtzpsjqvgf.html

Ruby: def self.f; end
来源：http://hz.sysykeji.top/gtkgnupnpk.html

C#:   public static void F() {}
来源：http://hz.tian-w.cn/gtyfqrcqnf.html

[G09] 接口 / 抽象类
来源：http://hz.chenzaomai.com/gtezkipohs.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.ppjwa.cn/gtqfrdwcuh.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.shzxlz.cn/gtapvthtmw.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.52xcode.cn/gtzgkdvnwb.html

TS:   interface Shape { area(): number; }
来源：http://hz.quarkkingdee.top/gtgphwuweg.html

Java: interface Shape { double area(); }
来源：http://hz.nanxuanxn.top/gttjeohozt.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.shzxlz.cn/gtmgjstonm.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.shzxlz.cn/gtdhgjsomr.html

C#:   interface IShape { double Area(); }
来源：http://hz.sufxvd.cn/gtunceappt.html

[G10] 访问控制
来源：http://hz.xingfuxueyuan.xyz/gtnhxusgbf.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.ybcxt.top/gtxryfcida.html

PHP:  public / protected / private
来源：http://hz.sufxvd.cn/gtmecbrnaj.html

JS:   #private 字段；其余公开
来源：http://hz.zhongyouzk.top/gtrcrvnyae.html

TS:   public / protected / private
来源：http://hz.daxiang520.top/gtxnvelacx.html

Java: public / protected / private / 默认包级
来源：http://hz.shuidangran.top/gtkisztyec.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.ivvv.top/gtcuadbnrw.html

Ruby: public / protected / private
来源：http://hz.xuetiantiany.cn/gtsuvhyqby.html

C#:   public / protected / private / internal
来源：http://hz.hnxiangtu.top/gtqoofxpan.html

[G11] getter / setter
来源：http://hz.xziqi.cn/gtiintboll.html

Py:   @property 与 @x.setter
来源：http://hz.sweek.top/gtdddkrybu.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.aizwys.cn/gtiihbiody.html

JS:   get name() { return this._name; }
来源：http://hz.shzxlz.cn/gtsasxaavi.html

TS:   get name(): string { return this._name; }
来源：http://hz.andypj.xyz/gthpuwucfo.html

Java: public String getName() { return name; }
来源：http://hz.jinyuanbaomall.cn/gthvonqnnr.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.iojbl.cn/gtpsepzqor.html

Ruby: attr_accessor :name
来源：http://hz.jinqigufen.top/gtobkoxwuk.html

C#:   public string Name { get; set; }
来源：http://hz.nanxinkj.top/gtrfvwxzgw.html

[G12] 对象转字符串
来源：http://hz.hywenlv.cn/gtbaeckpth.html

Py:   def __str__(self): return self.name
来源：http://hz.yj20258.top/gtwxzflacp.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.yongpay.top/gtmaqcuugw.html

JS:   toString() { return this.name; }
来源：http://hz.xingfuxueyuan.xyz/gtzunhilsd.html

TS:   toString(): string { return this.name; }
来源：http://hz.0kj1m.cn/gtomnvosgb.html

Java: @Override public String toString() { return name; }
来源：http://hz.haohaochexian.top/gtexccomgq.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.sweek.top/gtpvibmtvy.html

Ruby: def to_s; @name; end
来源：http://hz.zhongyouzk.top/gtvuggoguq.html

C#:   public override string ToString() => Name;
来源：http://hz.shanyushiyangkeji.top/gtgntxwifg.html

[G13] 判断对象类型
来源：http://hz.ydzc1.top/gtznnlfvll.html

Py:   isinstance(u, User)
来源：http://hz.xuanzx.com/gtqnqzgnll.html

PHP:  $u instanceof User
来源：http://hz.jyoumei.cn/gtwwboxwyd.html

JS:   u instanceof User
来源：http://hz.ywan-chungtsiang.top/gtaayrwonn.html

TS:   u instanceof User
来源：http://hz.zdqjudy.top/gtudhrnipj.html

Java: u instanceof User
来源：http://hz.yanxiufei.cn/gtedvdcnbh.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.shanyushiyangkeji.top/gtawtysbgg.html

Ruby: u.is_a?(User)
来源：http://hz.shuidangran.top/gtddggotao.html

C#:   u is User
来源：http://hz.ivvv.top/gtlvsvxodw.html

[G14] 数据类 / record
来源：http://hz.guannengcc.top/gtsifmzzyu.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.mhx1999.top/gtbursbbpt.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.hnxiangtu.top/gtwthajkgv.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.xinyue.icu/gtuyctdsqw.html

TS:   type User = { name: string; age: number };
来源：http://hz.hammf.cn/gtbhdtleba.html

Java: record User(String name, int age) {}
来源：http://hz.chenjidiqi.icu/gtfakrvnpk.html

Go:   type User struct { Name string; Age int }
来源：http://hz.pengpengdd.cyou/gtnklarvcr.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.hywenlv.cn/gtteplmphy.html

C#:   record User(string Name, int Age);
来源：http://hz.jlsjyb.cn/gtlwulmzig.html

[G15] 枚举
来源：http://hz.guowangkeji.top/gtcsmwkguh.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.dashuyun.cn/gtqvahufgl.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.yuxming.cn/gtcmdbmyqj.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.hnxiangtu.top/gthtbicsjo.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.redwolf501.top/gttueddfkq.html

Java: enum Color { RED, GREEN }
来源：http://hz.haohaochexian.top/gtgpoghakm.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.0kj1m.cn/gtuzizpzcf.html

Ruby: Color = %i[red green].freeze
来源：http://hz.tanke756.top/gtdsoodqes.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.ivvv.top/gtdynmhqxu.html

[G16] 对象转数组 / 字典
来源：http://hz.andypj.xyz/gtzzdyyyms.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.0kj1m.cn/gtrvoqjuat.html

PHP:  get_object_vars($obj);
来源：http://hz.yongpay.top/gtzsubhubh.html

JS:   Object.entries(obj)
来源：http://hz.aibaodan.cn/gtafvngewg.html

TS:   Object.entries(obj)
来源：http://hz.shzxlz.cn/gtutdbeogx.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.shanyushiyangkeji.top/gtbevcxojr.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.bjfxy.top/gtalfqunxo.html

Ruby: obj.instance_variables
来源：http://hz.mhx1999.top/gtmdmwzmdi.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.zhiwuduotai.top/gtagfqrmvj.html

================================================================================
来源：http://hz.c1oappe.top/gtsxevvnma.html

H. 异常与错误处理
来源：http://hz.zhoulong.xyz/gtdifwhxlh.html

================================================================================
来源：http://hz.shzxlz.cn/gtvmnblfhr.html

[H01] try / catch 基础
来源：http://hz.jqgufenzy.top/gttovaurxz.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.birdmap.top/gtjzglkbok.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.pycfn.com/gtphmltlpg.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.guowangkeji.top/gtfxbqigff.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.quarkkingdee.top/gtletdntce.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.c1oappe.top/gtjmcmwsbo.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.tanke756.top/gtgkklwhav.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.quarkkingdee.top/gtgeupodkx.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.chenlongwang.top/gtjvlxjnhy.html

[H02] finally / ensure 收尾
来源：http://hz.hammf.cn/gtohlblxgp.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.jinqigfzy.top/gtbibyevps.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.havefunace.top/gtigoxcnxx.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.shuidangran.top/gtxxrdhosy.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.yangfankeji.com/gtigujjceb.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.hammf.cn/gtzxqiljde.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.jqgufenzy.top/gtovsdznir.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.tian-w.cn/gtmxfclzcj.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.cheryme.top/gtrpkzdtmh.html

[H03] 主动抛出异常
来源：http://hz.fzhhl.top/gtulljoslx.html

Py:   raise ValueError("错误信息")
来源：http://hz.52xcode.cn/gtuhnopodm.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.ydjk.org.cn/gtmesnrapn.html

JS:   throw new Error("错误信息");
来源：http://hz.guowangkeji.top/gtqlejkxyg.html

TS:   throw new Error("错误信息");
来源：http://hz.hywenlv.cn/gtwkvwibvw.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.cucudq.cn/gthfgtmoam.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.yj202588.top/gttisqmcsp.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.sweek.top/gtoagocmnx.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.mhx1999.top/gtzwknnbxj.html

[H04] 自定义异常类型
来源：http://hz.wangshuangyany.cn/gthdhoiwyw.html

Py:   class MyError(Exception): pass
来源：http://hz.wangdashe.top/gthrjauzmr.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.feifeiyinyue.top/gthekctllw.html

JS:   class MyError extends Error {}
来源：http://hz.gaohongyu789.top/gtmcsvncht.html

TS:   class MyError extends Error {}
来源：http://hz.aizwys.cn/gtqknopwrk.html

Java: class MyException extends RuntimeException {}
来源：http://hz.gogol.net.cn/gtlqxkqvlr.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.cashguo.top/gtbgjzxdri.html

Ruby: class MyError < StandardError; end
来源：http://hz.iojbl.cn/gtrfcyytde.html

C#:   class MyException : Exception {}
来源：http://hz.jinghuilouyu.cn/gtorbqtvxs.html

[H05] 捕获特定类型
来源：http://hz.tianlin.xyz/gtdrwdyafs.html

Py:   except ValueError as e:
来源：http://hz.yongpay.top/gtrbvayuhb.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.wangdashe.top/gtdzygrpkq.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.sweek.top/gtxkpbuidx.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.hywenlv.cn/gtxrscmkgp.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.vqdsnc.cn/gtfydxsfox.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.xylfe.cn/gtugnozvrt.html

Ruby: rescue ArgumentError => e
来源：http://hz.xziqi.cn/gtujinozge.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.hammf.cn/gtsbyxbjnw.html

[H06] 可选值 / 空值安全访问
来源：http://hz.haohaochexian.top/gtlhxjrnro.html

Py:   value = d.get("k") or default
来源：http://hz.9152youxi.cn/gtcvqopqtd.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.shanyushiyangtech.top/gtkwdpuyaq.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.xuanzx.com/gtkcljjcov.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.shanyushiyangtech.top/gtatqwchlv.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.pengpengdd.cyou/gtvzlwsfcq.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.yvedp.cn/gtrzqjgxtl.html

Ruby: d&.dig(:a, :b)
来源：http://hz.andypj.xyz/gtgsbzprmp.html

C#:   obj?.A?.B ?? default
来源：http://hz.jinyuanbaomall.cn/gtjljvwtyi.html

[H07] 断言
来源：http://hz.andypj.xyz/gtpsacuvlb.html

Py:   assert x > 0, "必须为正"
来源：http://hz.sysykeji.top/gtwdwssyei.html

PHP:  assert($x > 0);
来源：http://hz.yonumen.top/gtlcgxxgkp.html

JS:   console.assert(x > 0);
来源：http://hz.yueranfly.top/gtryfvhotn.html

TS:   console.assert(x > 0);
来源：http://hz.sweek.top/gtmnkrhpyq.html

Java: assert x > 0 : "必须为正";
来源：http://hz.jqgfzy.top/gtyknrdehc.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.yueranfly.top/gtpjnsjmud.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.andypj.xyz/gtyykuswvi.html

C#:   Debug.Assert(x > 0);
来源：http://hz.zhengqikj.top/gtksyywxkz.html

[H08] 获取错误信息与堆栈
来源：http://hz.havefunace.top/gtbqglfiqw.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.sweek.top/gtjcodljts.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.kuanghao11.cn/gtadqmgsfi.html

JS:   e.message;  e.stack
来源：http://hz.hnqzz.top/gtncygtabr.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.yuanzhike.top/gtzbbynhzc.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.daria6918.cn/gtmfbpetml.html

Go:   err.Error()
来源：http://hz.jqgfzy.top/gtwszfwisj.html

Ruby: e.message;  e.backtrace
来源：http://hz.jlsjyb.cn/gtpeavnbeg.html

C#:   e.Message;  e.StackTrace
来源：http://hz.haohaochexian.top/gtnoyhdxsa.html

[H09] 带错误码的异常
来源：http://hz.jinqigufen.top/gttcqebwuc.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.sufxvd.cn/gtpluvqfxz.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.jinghuilouyu.cn/gtfdnfhtxv.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.shuidangran.top/gtwurshyhy.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.yuanzhike.top/gtkwlaakah.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.yonumen.top/gtwgibuqhs.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.haohaochexian.top/gtuordipbx.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.dianchejie.cn/gtlelnuqln.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.jinqigufen.top/gtnkjulyth.html

[H10] 资源自动释放
来源：http://hz.zhengqikj.top/gttuzeisqi.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.guowangkeji.top/gtabivpsfm.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.pengpengdd.cyou/gtyaaqaxif.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.xylfe.cn/gtyeykolir.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.haohaochexian.top/gtmxdkulnv.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.sysykeji.top/gtnmwxiyqe.html

Go:   defer f.Close()
来源：http://hz.xuetiantiany.cn/gtokmdqihn.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.dianchejie.cn/gtvhqkdyhn.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.zhongyouzk.top/gtdwxfuhgl.html

================================================================================
来源：http://hz.cashguo.top/gtlxfhyims.html

I. 正则表达式
来源：http://hz.yangfankeji.com/gtvpqdyeey.html

================================================================================
来源：http://hz.hnqzz.top/gtgmagljnu.html

[I01] 判断是否匹配
来源：http://hz.zhengqikj.top/gtzuwrvncn.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.yj202588.top/gtefyrjzns.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.zhengqikj.top/gtiuldnfpf.html

JS:   /\d+/.test(s)
来源：http://hz.jyoumei.cn/gtdxvwcozr.html

TS:   /\d+/.test(s)
来源：http://hz.ybcxt.top/gtnjxlxkfl.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.ydzc1.top/gtxfzbctjx.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.shanyushiyangkeji.top/gtqbbovkji.html

Ruby: s.match?(/\d+/)
来源：http://hz.ydjk.org.cn/gtigivrhbd.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.zhijiandao.cn/gtwfbsfxhe.html

[I02] 提取所有匹配
来源：http://hz.cqqwz.cn/gttarnzyci.html

Py:   re.findall(r"\d+", s)
来源：http://hz.ydzc1.top/gtnkmcypir.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.sxryk.cn/gtqfvwoiza.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.chenjidiqi.icu/gtiytnupac.html

TS:   s.match(/\d+/g)
来源：http://hz.yonumen.top/gtibouxfgp.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.cdnleiting.top/gtjofivijx.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.yanxiufei.cn/gtbenmzvvk.html

Ruby: s.scan(/\d+/)
来源：http://hz.hammf.cn/gtcatvjgym.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.cashguo.top/gtdfhqduor.html

[I03] 提取捕获分组
来源：http://hz.fzhhl.top/gtpbtwdupi.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.smart0.xyz/gtmumrufon.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.wangdashe.top/gtpvqjnofj.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.zhixingplan.top/gtqcleqebd.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.daxiang520.top/gtebjjwfsf.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.xuetiantiany.cn/gtuigreaew.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.tian-w.cn/gtaaqbisys.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.zhijiandao.cn/gtaqbzighf.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.nwbrower.top/gtxmmvltmi.html

[I04] 正则替换
来源：http://hz.guannengcc.top/gtaydmycar.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.jqgufenzy.top/gtzldrawdg.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.xinyue.icu/gtlrwcrjnn.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.birdmap.top/gtwnpdbmai.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.jyoumei.cn/gtcuejcppn.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.gaohongyu789.top/gtaelksmcy.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.hywenlv.cn/gtpavvqrst.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.cqqwz.cn/gtenjqimzu.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.316326.xyz/gtuyphrthx.html

[I05] 按正则拆分
来源：http://hz.pengpengdd.cyou/gtpjvyatnw.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.316326.xyz/gtrklejhur.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.hnqzz.top/gttdxvvmji.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.jqgufenzy.top/gtxujaeykw.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.vqdsnc.cn/gtcteyrgvp.html

Java: s.split("\\s*,\\s*")
来源：http://hz.nanxuanxn.top/gtqofgsowk.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.gotoacloud.top/gtknwurjmb.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.aizwys.cn/gtqlijxorb.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.yuanzhike.top/gthdszpgkl.html


<!-- 参考信息 -->