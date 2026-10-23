代发 wailian999

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ejobehpg.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3omfowbrm.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3fokrynvs.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vtpuawcv.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3evsqjkaq.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3tsxlvpgk.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3frvxgetn.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3memfiwqj.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3pyisqkth.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3yeulnrhe.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3mdtpjdph.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3bwwqpqcn.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3xikblxhf.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3hgtdhgwr.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3wafsuqvx.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ycrcjpuj.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3dfwaatej.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3huhavhxu.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3bwdkyxbn.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3anxjvbry.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3viqugjan.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3vwrdoxua.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3asshtfvx.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3ebtfukec.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3exjmtmzj.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3ejongyux.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3shvlxywo.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3njjftgfy.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3vybnwbmd.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3spcflimb.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3bbbukgua.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3ohjavrym.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3hwjunyvu.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ubqfzsfy.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3qixrvauj.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3iogzxafg.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3aslquxql.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3yyzcrlzm.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3mxvldtdj.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3kxnvwtct.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3wrscxrrr.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3mivopnja.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3lytbobbe.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3nlzosebs.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3tooacfsz.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3atxkgkze.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3huqxwnoe.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3skawezzu.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3gwjedwya.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3qlmgyrhi.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3xuvmfibc.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3fizzxzbu.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3savomrkv.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3hvuxzvpd.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3yhdhjjav.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3rpnchjjc.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3lpelniva.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3ctyhyddn.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3mhykoibg.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3ringfeyz.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3wphniqcz.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3zfuyuwsc.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3bnmmfagn.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3xjsxapul.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3wmxukasw.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3oxltabyz.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vmqbnvgg.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3molbkmxj.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3wvxyizoa.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3fydrxkve.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3qvlqhkxo.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3twaaidmx.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3mncrcrue.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3doarlupo.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3uvopcdxw.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3mtkugbbo.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3zvwakgno.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3kdnbgioc.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3bddxyrre.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3bopkmvdh.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3hlvbruev.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3uitcluxm.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3phqeqenb.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3nmskphcc.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3zkwholrx.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3emumkjym.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3ziivvvhy.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3jgdyqgby.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3zzsysvgd.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3ivbmbiai.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3totbrhdh.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3eswzfxmq.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3xnkmglgv.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3jbddwtwd.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3hrlafiom.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3munmifif.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3xfmjkrnt.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3xjhsqjyg.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3bvdrcarr.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bobqdqur.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3qsozohbq.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3gfxbfcxh.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3drqwlnqj.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3xzvdarxa.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3pxbdxnvu.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3gpajqngt.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3hxfxgfqu.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3ddfgsonr.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3akbtraan.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3nfmyzrqr.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3wlbyzsbo.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3aoqyvuha.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3ffhccehb.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3qybkaouo.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3otxcbkpt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hcirzfpv.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3tlcfzffd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mqlnvrhs.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3lpfqksvk.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3vgbhrjzr.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3lvfjoptl.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3xbpirggd.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3vxlppcpo.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3ximtwktm.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3kwwzjivb.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3gemejgqo.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3biwynfxy.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3vauyxpiv.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3ulzmocfe.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3unrmnkmk.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3litphkbg.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3dlwwtaqw.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3huveftdp.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3ylowyqto.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3orgwcxev.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3thamjhca.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3juvembwz.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3klkwknbr.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3fisdqkje.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3jcvlyfsr.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3thituhih.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3rtgplqyn.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3hlvddfmo.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3pssatjnk.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3pcemrkvz.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3trzajhwk.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3ztdkewty.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3vyrmzbgb.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3sqapjjhf.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3mcdfcfyj.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3epbqjjsk.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3uukfdajo.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3vsduloge.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3ixskujae.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3lmbxlpgv.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3wylqlark.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3mseuxohg.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wmcfdmkv.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3octqegkw.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kzjcstzm.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3snzrolig.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3ikfnkdml.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lcxffwvh.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3pgwcgrpj.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3slyphlre.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3jebdikbg.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3tjrojypu.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3ozgfhled.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3vcfifftt.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3knwgsqjh.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3emcztlpz.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3gpfjlaoy.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3cdlzbkue.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3ufacvmrr.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3hyuzxcqu.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3ppffndbq.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ixgfwrvo.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3fujblpxd.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3mrjzemtb.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3ybbofejy.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3jfyiuehr.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3hwbfsbxm.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3ctrgbcdh.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3dlccboux.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3yhfqjofc.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3tznbzpxx.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3lbktkjaj.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3wxghxleh.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3eviqzqbr.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3ccqawcgi.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3vfpqxjmc.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3pgpjqtfi.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3btzhqqiw.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3mkppyutq.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3yllfonzs.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3wluksrop.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3mmhmmxjb.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3lzzjsxph.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3nrdrmhiz.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3vnmtchtj.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3ohjmkiae.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3azcyimdt.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3lbtemqss.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3kuvfwxif.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3yclzinfi.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3gafoppyq.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3akhnxpbr.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3uhfrtbds.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xjvrpqsf.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3cgpofuto.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eooqtvun.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3ramkigct.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3nxpjsvdx.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3akhcmmai.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3ghfnlexq.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xhavzhso.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3vccsvfwd.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3nscnzjtl.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3uxyxpbru.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3cdwnvlgt.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt3lubmjykp.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3pkepsfwq.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3gevkwqcp.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt3sswgjgjs.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt3mdmhmygu.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3lkogeepe.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3sodoanng.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3okzyjscd.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3kasupywy.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt3ajohlknt.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zwycoovr.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3rwwgkdis.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt3ppscvkqx.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt3wddeivbu.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3uwmdzhjs.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt3vptrkyzt.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt3betlssnj.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt3npfirnfy.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3vgkbwbse.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3dsnbrozp.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3yigembob.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3dmzendga.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3ipurimxm.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3nilwwdex.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt3idtyovaq.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3xwblobqx.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3oisulnlf.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt3otteeayc.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt3lsqpbqpe.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt3ocwfzsam.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3suehpdce.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3jqhgbkbm.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3tbbleveg.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3fwsppgip.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3brpfrgzy.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3zyonbace.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt3pqlxdvqc.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3dqbnhppg.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt3oezxqqgs.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3bnjpuzah.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3clunprns.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3pmkilihg.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt3aqwxlgwx.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt3gsuxitqu.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3yoklnvlo.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt3ehxwdosx.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt3sofeumwp.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3flvrbakn.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt3ukahhquo.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt3uvcdzzwq.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt3kvqwsclu.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt3osurlbgj.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt3qrxxrovk.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt3powbfovw.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt3hnpthtpd.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt3pbpauypn.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3dycjoech.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3wnugxkuq.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3bjtfpbjx.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3jazsntxv.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt3rkzfvzal.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt3nmyeowhb.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3gqsvmxnk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3opaeubee.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt3ucvzdtvx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3twyljotb.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt3jwmhbhih.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt3xpmkewzy.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3iewtlpqv.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3tccdxtrd.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3rdvgthkh.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt3ldfitgey.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt3lltffjdc.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt3eisdafsx.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt3rftjttqf.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt3ygqwqfyx.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3mchmajpg.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3tphkitvn.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt3uxebbskn.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt3prrscfgp.html


<!-- 参考信息 -->