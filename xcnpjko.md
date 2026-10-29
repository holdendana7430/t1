代发 wailian999

TS:   constructor(public name: string) {}
来源：http://3g.zdbjq.cn/Article/details/gysctqhus.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.zdbjq.cn/Article/details/gcqbrvcip.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.fehbvm.com/Article/details/gpbnpgocl.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.fehbvm.com/Article/details/gofxnwqhn.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.hesvh.cn/Article/details/gdqdnhnsa.sHtML

[G03] 实例属性
来源：http://mobile.hesvh.cn/Article/details/gavtkbybl.sHtML

Py:   self.name = "x"
来源：http://www.share.zdbjq.cn/Article/details/guiwsbrlq.sHtML

PHP:  public string $name = "x";
来源：http://m.share.zdbjq.cn/Article/details/gwbwkuvbc.sHtML

JS:   this.name = "x";
来源：http://3g.zdbjq.cn/Article/details/glmwellwk.sHtML

TS:   name: string = "x";
来源：http://www.m.share.hesvh.cn/Article/details/gtztugtmo.sHtML

Java: private String name;
来源：http://www.share.hesvh.cn/Article/details/gcnirjdzw.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.zdbjq.cn/Article/details/gkicwrite.sHtML

Ruby: @name = "x"
来源：http://baike.zdbjq.cn/Article/details/guzujknkc.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.fehbvm.com/Article/details/gcirupjpk.sHtML

[G04] 定义方法
来源：http://read.share.zdbjq.cn/Article/details/gdhjlzfch.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.fehbvm.com/Article/details/gqmfrcape.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.hesvh.cn/Article/details/gajfkflqf.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.hesvh.cn/Article/details/gnokntsng.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/gbbtlolps.sHtML

Java: String greet() { return name; }
来源：http://www.blog.fehbvm.com/Article/details/grafsziwk.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.zdbjq.cn/Article/details/gxmbxynfv.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.hesvh.cn/Article/details/gufdzcsqs.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.zdbjq.cn/Article/details/gpccufffl.sHtML

[G05] 继承
来源：http://3g.hesvh.cn/Article/details/gxnzigkyr.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.hesvh.cn/Article/details/gbpcardlj.sHtML

PHP:  class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/gashyjcef.sHtML

JS:   class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/gvqbjkppd.sHtML

TS:   class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/gjlfzmmng.sHtML

Java: class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/gzgroxjub.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.zdbjq.cn/Article/details/gkkydhlbs.sHtML

Ruby: class Admin < User; end
来源：http://3g.fehbvm.com/Article/details/gtspjmdiz.sHtML

C#:   class Admin : User {}
来源：http://www.share.fehbvm.com/Article/details/gtjhyyzwh.sHtML

[G06] 重写方法
来源：http://read.share.fehbvm.com/Article/details/gjcekfdxh.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.zdbjq.cn/Article/details/gxldrpmff.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/ghufpceyr.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/golorsztn.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/gdifuxhha.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/grjuqwrpc.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.fehbvm.com/Article/details/glxactpwx.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.zdbjq.cn/Article/details/gyqvutynq.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.hesvh.cn/Article/details/gqnkssitp.sHtML

[G07] 调用父类方法
来源：http://www.share.hesvh.cn/Article/details/gelotvtpi.sHtML

Py:   super().greet()
来源：http://blog.hesvh.cn/Article/details/gkdclliiv.sHtML

PHP:  parent::greet();
来源：http://wap.hesvh.cn/Article/details/giqsuzylf.sHtML

JS:   super.greet();
来源：http://www.blog.zdbjq.cn/Article/details/gyxdjmhuy.sHtML

TS:   super.greet();
来源：http://mobile.zdbjq.cn/Article/details/gtykmximp.sHtML

Java: super.greet();
来源：http://3g.hesvh.cn/Article/details/gesrcllbr.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.fehbvm.com/Article/details/gxhpyvihk.sHtML

Ruby: super
来源：http://read.share.fehbvm.com/Article/details/gnedacgkp.sHtML

C#:   base.Greet();
来源：http://www.blog.hesvh.cn/Article/details/glryqolmr.sHtML

[G08] 静态方法与属性
来源：http://m.share.fehbvm.com/Article/details/gjereuiau.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.fehbvm.com/Article/details/ghnjgadmo.sHtML

PHP:  public static function f() {}
来源：http://mobile.hesvh.cn/Article/details/gybevowpd.sHtML

JS:   static f() {}
来源：http://mobile.fehbvm.com/Article/details/ghlbfdoyo.sHtML

TS:   static f(): void {}
来源：http://m.share.zdbjq.cn/Article/details/gmwljmghe.sHtML

Java: static void f() {}
来源：http://3g.zdbjq.cn/Article/details/gchdbnywp.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.hesvh.cn/Article/details/gukzvpzls.sHtML

Ruby: def self.f; end
来源：http://blog.hesvh.cn/Article/details/gsqfwtaiz.sHtML

C#:   public static void F() {}
来源：http://mobile.hesvh.cn/Article/details/gmlvovbro.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.fehbvm.com/Article/details/gcubsunai.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.zdbjq.cn/Article/details/gqtwstsmq.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.zdbjq.cn/Article/details/gjhhjulno.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.hesvh.cn/Article/details/gaceoabkj.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.fehbvm.com/Article/details/gwlhfhigw.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gnqtopnzw.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.hesvh.cn/Article/details/gjzpzepdw.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.hesvh.cn/Article/details/gdlejgzpy.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.fehbvm.com/Article/details/gxqnrlnmi.sHtML

[G10] 访问控制
来源：http://baike.hesvh.cn/Article/details/gzuiluolx.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.zdbjq.cn/Article/details/geryrehai.sHtML

PHP:  public / protected / private
来源：http://read.share.zdbjq.cn/Article/details/gblwzovdp.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.fehbvm.com/Article/details/gempybyce.sHtML

TS:   public / protected / private
来源：http://mobile.zdbjq.cn/Article/details/gbwgekxmp.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.zdbjq.cn/Article/details/gozusadjm.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.zdbjq.cn/Article/details/gvduljzrr.sHtML

Ruby: public / protected / private
来源：http://mobile.hesvh.cn/Article/details/gmtkmwfqw.sHtML

C#:   public / protected / private / internal
来源：http://m.share.hesvh.cn/Article/details/gkainbkrv.sHtML

[G11] getter / setter
来源：http://baike.zdbjq.cn/Article/details/gmbmujcxa.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.zdbjq.cn/Article/details/gkllwqlzk.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.zdbjq.cn/Article/details/gkiuhlcth.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.zdbjq.cn/Article/details/gbiozqzdh.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.zdbjq.cn/Article/details/gvnwsxuia.sHtML

Java: public String getName() { return name; }
来源：http://3g.hesvh.cn/Article/details/gvutufdep.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.fehbvm.com/Article/details/gdsxgnudr.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.fehbvm.com/Article/details/gqnuxhymu.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.fehbvm.com/Article/details/gnhkhtypz.sHtML

[G12] 对象转字符串
来源：http://wap.zdbjq.cn/Article/details/gxetnqphg.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.hesvh.cn/Article/details/gfglrjowc.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.hesvh.cn/Article/details/guqvqfufj.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/gelhtusdb.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.hesvh.cn/Article/details/goxsdielp.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.zdbjq.cn/Article/details/goryqgwgx.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.zdbjq.cn/Article/details/giiediwmq.sHtML

Ruby: def to_s; @name; end
来源：http://baike.hesvh.cn/Article/details/gpbvrdxpg.sHtML

C#:   public override string ToString() => Name;
来源：http://www.share.zdbjq.cn/Article/details/gjbdacith.sHtML

[G13] 判断对象类型
来源：http://baike.zdbjq.cn/Article/details/glqokbyod.sHtML

Py:   isinstance(u, User)
来源：http://wap.zdbjq.cn/Article/details/gwfikytcd.sHtML

PHP:  $u instanceof User
来源：http://www.blog.hesvh.cn/Article/details/gqqlnmegh.sHtML

JS:   u instanceof User
来源：http://wap.hesvh.cn/Article/details/gvanihpla.sHtML

TS:   u instanceof User
来源：http://m.share.hesvh.cn/Article/details/gcmoidxnw.sHtML

Java: u instanceof User
来源：http://baike.fehbvm.com/Article/details/gvdqjnfzr.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.hesvh.cn/Article/details/grwfahwok.sHtML

Ruby: u.is_a?(User)
来源：http://blog.zdbjq.cn/Article/details/grsyrqyiz.sHtML

C#:   u is User
来源：http://wap.zdbjq.cn/Article/details/gsqrtlkdc.sHtML

[G14] 数据类 / record
来源：http://3g.hesvh.cn/Article/details/gmwoykusv.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://baike.fehbvm.com/Article/details/gwxzimkch.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.fehbvm.com/Article/details/gcoqwpkpu.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.fehbvm.com/Article/details/gsndbsica.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.zdbjq.cn/Article/details/glmwjkrfl.sHtML

Java: record User(String name, int age) {}
来源：http://3g.fehbvm.com/Article/details/grxauykfm.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.fehbvm.com/Article/details/gksdxxlll.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.fehbvm.com/Article/details/gbrreqfzm.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.zdbjq.cn/Article/details/gdtuqsqyz.sHtML

[G15] 枚举
来源：http://m.share.fehbvm.com/Article/details/gakoqgqsn.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.fehbvm.com/Article/details/gkvmjszne.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.hesvh.cn/Article/details/ggzmardqu.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.hesvh.cn/Article/details/goggbqjlv.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.hesvh.cn/Article/details/gwelxcdpd.sHtML

Java: enum Color { RED, GREEN }
来源：http://m.share.zdbjq.cn/Article/details/ghvnrxsrp.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.hesvh.cn/Article/details/gqouxbmfb.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.fehbvm.com/Article/details/grvznlkue.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.fehbvm.com/Article/details/gtydueykl.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.hesvh.cn/Article/details/gsfkneapq.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.fehbvm.com/Article/details/gwpqynwwf.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.fehbvm.com/Article/details/gvinvieai.sHtML

JS:   Object.entries(obj)
来源：http://mobile.zdbjq.cn/Article/details/ghviezhto.sHtML

TS:   Object.entries(obj)
来源：http://www.share.fehbvm.com/Article/details/gxqqdmmhl.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.fehbvm.com/Article/details/gwicqslqn.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://wap.hesvh.cn/Article/details/ghyfmmrde.sHtML

Ruby: obj.instance_variables
来源：http://read.share.zdbjq.cn/Article/details/ggecxyjqg.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.blog.fehbvm.com/Article/details/gnixfcwyp.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gsiipnnwb.sHtML

H. 异常与错误处理
来源：http://m.share.fehbvm.com/Article/details/glbvmwrhd.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gjwkhvtox.sHtML

[H01] try / catch 基础
来源：http://www.m.share.zdbjq.cn/Article/details/gbehnkbwn.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://baike.zdbjq.cn/Article/details/gyebbiplk.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mobile.fehbvm.com/Article/details/gvcknibzl.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.fehbvm.com/Article/details/gdgmqerkt.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.m.share.zdbjq.cn/Article/details/gkwkuuswi.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mobile.hesvh.cn/Article/details/gwmxqyiln.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://blog.zdbjq.cn/Article/details/gthkryjii.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://blog.fehbvm.com/Article/details/ggiuyvhrc.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://blog.hesvh.cn/Article/details/grlymhkev.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.fehbvm.com/Article/details/ggwbmouqf.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://read.share.zdbjq.cn/Article/details/gqokeyuye.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.m.share.fehbvm.com/Article/details/guukpstzf.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/gppunsswr.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.share.fehbvm.com/Article/details/gixcbcfhe.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/gvdbhyaiw.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.hesvh.cn/Article/details/ghrlofvkx.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.share.hesvh.cn/Article/details/gdxyblcdu.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://3g.hesvh.cn/Article/details/gasiuqzwj.sHtML

[H03] 主动抛出异常
来源：http://baike.hesvh.cn/Article/details/gwkqzzkwf.sHtML

Py:   raise ValueError("错误信息")
来源：http://blog.fehbvm.com/Article/details/gxogtzicn.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.fehbvm.com/Article/details/gmgwaucae.sHtML

JS:   throw new Error("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/gcaurirei.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.hesvh.cn/Article/details/ghvzxtjgl.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.zdbjq.cn/Article/details/ghytrwlzy.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mobile.fehbvm.com/Article/details/gladxonom.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://mobile.hesvh.cn/Article/details/gycypyril.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.hesvh.cn/Article/details/gilcxvmee.sHtML

[H04] 自定义异常类型
来源：http://baike.hesvh.cn/Article/details/geojvhwjv.sHtML

Py:   class MyError(Exception): pass
来源：http://www.blog.hesvh.cn/Article/details/gxutuldbq.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://3g.hesvh.cn/Article/details/gxdlmbkkr.sHtML

JS:   class MyError extends Error {}
来源：http://3g.fehbvm.com/Article/details/ghtrfishr.sHtML

TS:   class MyError extends Error {}
来源：http://baike.zdbjq.cn/Article/details/gaaotggui.sHtML

Java: class MyException extends RuntimeException {}
来源：http://baike.fehbvm.com/Article/details/gdmrjlnbi.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.hesvh.cn/Article/details/gidlxqotm.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.share.hesvh.cn/Article/details/gjgbfcfrs.sHtML

C#:   class MyException : Exception {}
来源：http://3g.zdbjq.cn/Article/details/gkhogsiuq.sHtML

[H05] 捕获特定类型
来源：http://www.share.hesvh.cn/Article/details/gjrgdxlif.sHtML

Py:   except ValueError as e:
来源：http://3g.hesvh.cn/Article/details/gjibfydvf.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://read.share.zdbjq.cn/Article/details/gdssmhhus.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.share.zdbjq.cn/Article/details/gmvyzpznl.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://m.share.zdbjq.cn/Article/details/gatduaiiw.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://mobile.fehbvm.com/Article/details/ghdojebgv.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://m.share.zdbjq.cn/Article/details/gnidjqiwn.sHtML

Ruby: rescue ArgumentError => e
来源：http://mobile.zdbjq.cn/Article/details/glybbnttd.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mobile.fehbvm.com/Article/details/gfgsqtiuy.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.blog.fehbvm.com/Article/details/gwpatnccx.sHtML

Py:   value = d.get("k") or default
来源：http://www.m.share.hesvh.cn/Article/details/gutvekvku.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.m.share.hesvh.cn/Article/details/gxiktuhjc.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.zdbjq.cn/Article/details/gyneqpnau.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://wap.hesvh.cn/Article/details/ghqdddlqa.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.blog.fehbvm.com/Article/details/gujmifink.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.share.zdbjq.cn/Article/details/glnvtfkyw.sHtML

Ruby: d&.dig(:a, :b)
来源：http://3g.hesvh.cn/Article/details/gngqmcprr.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.share.fehbvm.com/Article/details/gxqkozysm.sHtML

[H07] 断言
来源：http://read.share.zdbjq.cn/Article/details/gojutvqeq.sHtML

Py:   assert x > 0, "必须为正"
来源：http://wap.hesvh.cn/Article/details/girykjjdt.sHtML

PHP:  assert($x > 0);
来源：http://www.m.share.hesvh.cn/Article/details/gurheqevb.sHtML

JS:   console.assert(x > 0);
来源：http://read.share.hesvh.cn/Article/details/gigutwyoc.sHtML

TS:   console.assert(x > 0);
来源：http://www.share.fehbvm.com/Article/details/ghbuvrcfn.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.hesvh.cn/Article/details/gnjfoxkby.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.m.share.fehbvm.com/Article/details/gwxmbfuys.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://wap.zdbjq.cn/Article/details/glqvlfkud.sHtML

C#:   Debug.Assert(x > 0);
来源：http://read.share.zdbjq.cn/Article/details/grgmawzzd.sHtML

[H08] 获取错误信息与堆栈
来源：http://3g.hesvh.cn/Article/details/gmxdlcjqg.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://mobile.hesvh.cn/Article/details/gzexjcnbz.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://3g.fehbvm.com/Article/details/gcrbrgsso.sHtML

JS:   e.message;  e.stack
来源：http://read.share.zdbjq.cn/Article/details/giczvfwja.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.m.share.hesvh.cn/Article/details/grjauxpjp.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.blog.hesvh.cn/Article/details/gbsxrueyg.sHtML

Go:   err.Error()
来源：http://www.share.fehbvm.com/Article/details/gdztagunu.sHtML

Ruby: e.message;  e.backtrace
来源：http://m.share.hesvh.cn/Article/details/gyhowgdnp.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.m.share.zdbjq.cn/Article/details/gwbnotbcm.sHtML

[H09] 带错误码的异常
来源：http://m.share.hesvh.cn/Article/details/gcfsghwos.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.m.share.hesvh.cn/Article/details/gekvjwgvm.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.blog.zdbjq.cn/Article/details/ghzohyygd.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.m.share.hesvh.cn/Article/details/gegmxpjqz.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.m.share.hesvh.cn/Article/details/ggytjoypb.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.share.hesvh.cn/Article/details/gqnzhmbof.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://baike.hesvh.cn/Article/details/gjvwwszao.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://read.share.zdbjq.cn/Article/details/grmnicbjx.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.blog.hesvh.cn/Article/details/gvadbjbfq.sHtML

[H10] 资源自动释放
来源：http://wap.hesvh.cn/Article/details/gldclmqvf.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://3g.hesvh.cn/Article/details/gjoethwyd.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://read.share.zdbjq.cn/Article/details/gdecwitqu.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.fehbvm.com/Article/details/gncszqcei.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.zdbjq.cn/Article/details/giueelkkp.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://3g.fehbvm.com/Article/details/gzbjspkik.sHtML

Go:   defer f.Close()
来源：http://3g.hesvh.cn/Article/details/gxgajqajh.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://3g.hesvh.cn/Article/details/gezqtmwns.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gwbsgwugc.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/ghxbvujxr.sHtML

I. 正则表达式
来源：http://wap.fehbvm.com/Article/details/gjqjqntzh.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gjmghegvw.sHtML

[I01] 判断是否匹配
来源：http://www.m.share.fehbvm.com/Article/details/gptvperwc.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://3g.zdbjq.cn/Article/details/gdpudryhi.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.share.fehbvm.com/Article/details/gkvzresft.sHtML

JS:   /\d+/.test(s)
来源：http://mobile.zdbjq.cn/Article/details/gykbrcaup.sHtML

TS:   /\d+/.test(s)
来源：http://wap.hesvh.cn/Article/details/gzahhyhhs.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://m.share.zdbjq.cn/Article/details/gnxztduee.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.blog.hesvh.cn/Article/details/gulmgmhlr.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.m.share.hesvh.cn/Article/details/gyanmqrix.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wap.fehbvm.com/Article/details/gsfybonta.sHtML

[I02] 提取所有匹配
来源：http://www.share.fehbvm.com/Article/details/gesbwkbrd.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.share.fehbvm.com/Article/details/gsjkholqb.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://m.share.fehbvm.com/Article/details/gshnjytjj.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://blog.hesvh.cn/Article/details/gsdrskvwc.sHtML

TS:   s.match(/\d+/g)
来源：http://www.m.share.zdbjq.cn/Article/details/gtalpxtov.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mobile.zdbjq.cn/Article/details/gqkjoqfyr.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://m.share.fehbvm.com/Article/details/gprlroemf.sHtML

Ruby: s.scan(/\d+/)
来源：http://mobile.zdbjq.cn/Article/details/gsvzhwapf.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.share.zdbjq.cn/Article/details/gwwmhepvc.sHtML

[I03] 提取捕获分组
来源：http://baike.fehbvm.com/Article/details/gjggnsdbv.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.share.fehbvm.com/Article/details/guwlkzslf.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.share.zdbjq.cn/Article/details/gfecbgxkh.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mobile.zdbjq.cn/Article/details/gbmeiumus.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mobile.hesvh.cn/Article/details/gayscgpmh.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.blog.hesvh.cn/Article/details/gldvxoipa.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://3g.zdbjq.cn/Article/details/gmlfjovzs.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wap.zdbjq.cn/Article/details/ghhaxywxf.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://m.share.fehbvm.com/Article/details/gwqextsnb.sHtML

[I04] 正则替换
来源：http://read.share.fehbvm.com/Article/details/gonhfpggg.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://m.share.hesvh.cn/Article/details/gtrrumrhb.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://3g.zdbjq.cn/Article/details/gynhgqgey.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.share.zdbjq.cn/Article/details/gsxuimmod.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://mobile.hesvh.cn/Article/details/gtbeoynjp.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.share.zdbjq.cn/Article/details/gcpvnyukr.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://blog.hesvh.cn/Article/details/ggvpjqslv.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://wap.hesvh.cn/Article/details/grlbeystj.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://3g.fehbvm.com/Article/details/gyqekklto.sHtML

[I05] 按正则拆分
来源：http://m.share.fehbvm.com/Article/details/gpkipmraw.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://baike.zdbjq.cn/Article/details/gxyspmkid.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.blog.hesvh.cn/Article/details/gmjubuvkw.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.blog.zdbjq.cn/Article/details/giampufws.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://baike.fehbvm.com/Article/details/gbgjgntrl.sHtML

Java: s.split("\\s*,\\s*")
来源：http://mobile.hesvh.cn/Article/details/giyqnacks.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://mobile.zdbjq.cn/Article/details/guabpgkmg.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://blog.hesvh.cn/Article/details/gsimopjgn.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://baike.fehbvm.com/Article/details/gfggwzvxs.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://baike.zdbjq.cn/Article/details/gulzwcyur.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.blog.hesvh.cn/Article/details/gzlvcrrxd.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://blog.zdbjq.cn/Article/details/ghaguxznq.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.zdbjq.cn/Article/details/goghdfxju.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.zdbjq.cn/Article/details/gfqechfav.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.blog.fehbvm.com/Article/details/gjpoqrhct.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wap.hesvh.cn/Article/details/gbnuscvvf.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://blog.fehbvm.com/Article/details/gkgudwlof.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://m.share.fehbvm.com/Article/details/gsprhwjfy.sHtML

[I07] 忽略大小写与多行模式
来源：http://blog.zdbjq.cn/Article/details/gqterqiuc.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.m.share.zdbjq.cn/Article/details/gxubeycsu.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.blog.fehbvm.com/Article/details/gxcftlxeu.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mobile.fehbvm.com/Article/details/grnhthpuy.sHtML

TS:   /error/gim
来源：http://www.share.fehbvm.com/Article/details/gxvkknmos.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.blog.zdbjq.cn/Article/details/gechtkfem.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.m.share.fehbvm.com/Article/details/ghskqxdfv.sHtML

Ruby: s.scan(/error/i)
来源：http://m.share.fehbvm.com/Article/details/gbdcbgjfy.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://3g.zdbjq.cn/Article/details/gewxffgic.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://mobile.hesvh.cn/Article/details/gxqjafwwc.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://m.share.hesvh.cn/Article/details/ggwyikndq.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.m.share.fehbvm.com/Article/details/gyzyhvwtd.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.fehbvm.com/Article/details/gvxyerrct.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.zdbjq.cn/Article/details/gqusnrotl.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.m.share.hesvh.cn/Article/details/ggswduzdf.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wap.zdbjq.cn/Article/details/gihunieib.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://3g.fehbvm.com/Article/details/getmnqlmu.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mobile.fehbvm.com/Article/details/gekujonti.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/goahtxhen.sHtML


<!-- 参考信息 -->