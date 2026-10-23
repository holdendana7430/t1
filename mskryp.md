代发 wailian999

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3buffklky.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3gqkcpxqh.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3whjlxvkm.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3dmyrhjov.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3cghqnhyn.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3vjgiejyz.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3dknbfvyj.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3drlsjojv.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3bmgkpnob.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3fifbuhwm.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3rchfozyl.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3ivkemklr.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3xakndhnb.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3urtjvuhh.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3cdnacycl.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3xksprukj.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fhdrcybq.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hgpylmja.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3uolmtssn.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3wdkrizsr.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3esphlicm.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3vhbldcnf.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3mrpnstwh.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3trfjudvw.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3ooxhciom.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3sdadeykw.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3lvsybvzh.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3fwaifhtx.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3kweujwqw.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3jxekastc.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3sowlwidx.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3dtapctqo.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3uyruacyq.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3iqjagjff.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3khcgeutx.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3fshyuero.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3vqcfrwrc.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3vlbviejq.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3aixgbgzv.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3zygrejap.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3psztliop.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3wqmmtgtc.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3qtnaqsnp.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3sezwxhai.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3akxdubmb.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3hfybmqli.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3oducwfdx.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3rjfearbp.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3buvmwrmf.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3wbfwulsk.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3dlevkivh.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3vajpwfyg.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3grtairce.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3homyzxnb.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3zufxkwda.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3ovttmgqa.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3lipljzaf.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3eqdwmzkc.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3eooetdug.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3njchtmxp.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3iwodzuou.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3likzagln.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3ntaydlhk.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3gizbddrm.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3athflmmu.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3kzhhrtgb.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3kzwlmvga.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3rajxgdzj.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3fzhyzliw.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3cbjffasf.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3ecaqjkqx.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3bnpjpmdo.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3vhgvinhx.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3dlczwnjk.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3lqmrbiqh.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3rhadeuga.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3pxvkcqad.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3kfobigdn.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3lqlebjie.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rjplvrks.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lludijmd.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3cnoevbki.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3zmgfifqe.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3wxfymjdt.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3qglcdkmy.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3oitrzyja.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3zcwtamni.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3qbxqczmy.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3gojawphp.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3poynbnjh.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xcbusvxj.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3tstokyup.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3znefqvfq.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3pdpvbtde.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3sieiadjq.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3rehzmhoq.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3kwevfztb.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3jaurpznh.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3dhpnqkkq.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3gbkgloog.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3smposqiq.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3uwxaoxsa.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3sttcgqea.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3icgofwjk.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3qdoyslfl.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3xajxjltu.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3lvprhlfr.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3jonjxabk.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3fdamwgnv.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3skteelrm.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3hlbxefwy.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3ilerjqlj.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3ljqxpasq.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3hgaoomcv.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3tyzdnphs.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3njdvihem.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3onljftzk.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3cozkdqlp.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3xqifblty.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3mlhsajjp.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3mpnxbpdz.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3exdyxhav.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3uczmgcao.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3oqlgeqxr.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3sgtjhgsb.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3zpzgdksw.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3rddxomtb.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3gkbxyajh.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3hqfjmgtq.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3qykpkbei.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3bmdlngkx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3euprovrf.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3hxsytvkr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nbpkqmno.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3mugskvhm.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3ucpxctii.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3znjxpedn.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3locxxijx.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3tvhgnqno.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3sfxqzsjp.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3mqdgtgrq.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3ppeipkpa.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3jfizkgqm.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3xyyodfjm.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3qtfeskbr.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3ipoksbdg.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3bghaxynd.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ndoxmcjo.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3hrqepgua.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3hvsbhcbr.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3hdbadwlz.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3wewfrqem.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3mwslvycq.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3gchzjfnp.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3dwqchrfq.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3urcdsydk.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3dsgabsah.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3ryyzkkjv.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3rpuefghh.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3azmrpxvb.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3cckhuxol.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3kttwhalu.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3sjcfgmav.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3tcsjrepy.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3tdklgdoq.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3oetjyopc.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3xedakdyr.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3bleaolxi.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3fjmcmtpf.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3bxlamnvb.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3rcgeagys.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3euseqyrv.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3rdggzywo.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tmvkbnsi.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3wvqdvlam.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ijokiljr.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3caodmpnc.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3tibxtjgh.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hlppnfxp.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3pfwqfuvh.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3tbbqtyoj.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3dzvronto.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3bgrfrvqn.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3zkcnaivc.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3txijectx.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3dbrwtswe.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3vpmvaasn.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3pfpifycb.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3rlrwuqbu.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3mexalsae.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3nhcwegyd.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3gyjayzts.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3vsthneqk.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3svqhfavc.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3aplcxcod.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3buvarmdi.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3uvnkiqut.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3xhygeors.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3qomcljke.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3isemegyd.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3osewovjh.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3qbdmbstr.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3uzoaqxeo.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3npncfdca.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3ybqkgakn.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3vbxmqqhn.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3fpqghzzr.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3uuchqtuy.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3juqbcqaw.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3gyrcyoxv.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3dfagmhzz.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3vjwvuogg.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3ssmsprag.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3cybgqndz.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3dzizgcxt.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3bzqravvh.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3qxjimpgs.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3vgoryrhh.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3vobinycl.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3wrvlzpfs.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3zrqgyrzv.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3zvzehaba.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3vlweqfdw.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3fxstsbvm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mkmxrahm.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3iqrdzodx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wedphqly.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3klnytqzm.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3trhduuuw.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3cmytrcbk.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3fietelaq.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3eqipruuw.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3rizzmnhx.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3ivvutqrv.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3keunlvas.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3kdgmkmqe.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt3yzeeaays.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3hylplhrv.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3jkdgaxlr.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3lewuqgvz.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt3qnwcfphp.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt3jskcsapj.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3ugnymzim.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3jruuhxql.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3qkfpbijq.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3gxnmmlpu.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt3moewhcse.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3dbczuaxk.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt3odabzwff.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt3atshmoer.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt3cysjmsuv.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt3afxdepje.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt3cefduayf.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt3mthhmakl.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt3qgoyuvqj.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3npgmsuwt.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3femnrpfu.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3cwocrugy.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3enbwdrrq.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3nxsxbija.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3etypexya.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt3phlcvgom.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3peszxdst.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt3whyovlwi.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt3mpyofzcc.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3spcrvviv.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3rgwkqptz.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3dbbafesw.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3bpmdveip.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3axmvrnrt.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3tepluafq.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt3prlewcnx.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt3xdoucylb.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3yximdorn.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt3lwufxzia.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3vxibiuuj.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3vrfghxcz.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3qhbzbrcm.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt3enwszjkv.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt3nqtuefsx.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3qeuxpqsr.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt3errvwvij.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt3vniuyseh.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3vapxrfvd.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt3lsidicsp.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt3xmufmcfr.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt3buozmhsv.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt3kwbeibxm.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt3pcqshqha.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt3aljxopva.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt3obauoizb.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt3isoxumym.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3gahghtrs.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3ikjggiwj.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3lonjongi.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3xacjtnlb.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt3yinibajp.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt3lreyzchm.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3hcbzfgaw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fvkbexfi.html


<!-- 参考信息 -->