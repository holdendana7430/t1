代发 wailian999

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3ijfkfwxp.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pjvqnijk.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3pwwligyw.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3lvgmmhmg.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3vrkgqrbj.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3siulhxpf.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3vvvqulxc.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3yhytaqdi.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3wekgcpvk.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3kvvgtkfs.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3airyphib.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3bkztpokj.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3pdvvbxhg.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3gndrsyvs.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3jgnjgcka.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3uhkczrth.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3sxyzujfp.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3jjpixvhm.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3twgzkktn.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3cphqjmbz.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3hjemticu.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3fkgrlmru.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3jrrzhqah.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3pdlguduh.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3ivzhatmg.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3faumqszu.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3vhnouujb.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3ktaiyswj.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3wsgvgvnl.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3ogqazapx.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3urlmhhii.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3rnxiptzo.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3lhoxbvhz.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ktvayjlz.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3evnfexus.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3yooilefg.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3qnoffgoh.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3jgwqpoqo.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3lfqzicip.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3pbcvmesp.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3tvnvsvky.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3nfiiebeq.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3xohtndov.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3rgazfnhk.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3mxrwmwwr.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3hgftscjf.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3nzpwsyke.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3abzqtdpg.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3osvshpct.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3ftozdygp.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3itlxtqmr.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3udbcdoak.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3wrmcrvpe.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3wodtjayw.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3sluunbna.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3jtlorclw.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3ifyhplwk.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3vjiiriej.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3oapduwhi.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3cdzuxcjd.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3adosndlb.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3fwltsjcv.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3ogcckwax.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hfmmdyct.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3mskmatfw.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ktusjuoo.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ajsbnkfz.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3hkreqovi.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3jluyrfuz.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3fzodkxzs.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3sdcanytw.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3pjxyxlrd.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3gqlczlkc.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rorqlygs.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3titrvwcx.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3fxxirehp.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3ovbigifu.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3sugfwuph.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3pqduhjgc.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3fbgphvuj.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3befqmuth.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3dlcvgwpd.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3fgjeykin.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3pkrmvilw.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3besqrwfv.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3vswczqdo.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3nkxxqwai.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3ycqgpfbq.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3rsugkwit.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3ztptzzjj.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3svcghbhp.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3mddcgrhp.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3ixelvuao.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3hbhqpdwe.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3psyqjskc.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3wxsbvihw.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3uppqeeza.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3ugomwjfm.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3geavkqcy.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qywanofs.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3jfdfpgqk.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ztgwholk.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3xebhrafi.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3wtltoyjl.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3syxgweqj.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3rvnfwjbu.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3pczkfvat.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3gfyrglxn.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3jpytqlsj.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3kkhwdlfd.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3dyusrwex.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3ycuxtyxd.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3fvqjvhqv.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3hdybyaqq.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3uwamlzku.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3enligjsk.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3enxhvsdi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ihfvohho.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3imazytdg.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3xgmokhpk.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3cbjrplvd.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3tsvcxfvj.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3txfjxjbx.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3cjntphaz.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3apfslnle.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3tfyxdgbq.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3tlskvfdi.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3sgvvbbxd.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3adqiazyc.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ipgftosn.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3fsvcbgxf.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3xysaemkw.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3xflyfumq.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3orczvdyr.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3mkylkqww.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3vfxljmjq.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3gowhxyti.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3pypnomyi.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3cuvuhypp.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3tyzmjqhq.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3wvekgfkd.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3jmxxbtjm.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3aeazswto.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3cjsgejef.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3kziruwnn.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3lqofbbgs.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3fpwezmhw.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3yqmyojrk.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3qcvadfsc.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3gzypdpfi.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3xcpibbyg.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3pgelpbys.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3zhmgctzt.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3gcnjpyvc.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3jthapebr.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3zkqztocv.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3fxgnidsv.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zfdqzjza.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3emxsfzvp.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qemylcuu.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3puzatudn.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3mnhppmat.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ztaprqep.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3ennkgqku.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3kdhrjwwf.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3ifniqfwz.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3mfvwuwgg.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3akjbyzvf.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3uemyfzqx.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3zblrycdu.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3brpnaxpj.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3cqsxnhax.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3eybhzrqu.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3vzevxyoz.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3mxmwcpoz.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3kfjhluyf.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3zxjocabk.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3qopnhwye.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3robbpmci.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3lvsboblb.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3xpieirxb.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3sbgplmny.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3cggvlrpo.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3rzzsenzo.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3mlwxabkd.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3kxjhqber.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3lrqgwxaj.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3msymxler.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3xjnoesvk.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3ovewzqkx.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3yngdruzk.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3kwepurmu.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3kkfhxswm.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3qtgwjkcz.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3vlalubxg.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3bwthgdnd.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3cfvzvymp.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3lqbusfpe.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3jdagcphh.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3jlnfgngc.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3fsdbyluk.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3qvyormgs.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3bddtozax.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3gsiheicm.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3kyifajpc.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3srswiavo.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3usulaowy.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3etzbjytp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ypmhxgkw.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3yabsbppi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3talzeugl.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3bqjsjuot.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3opwsaemr.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ibhauhxx.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3owhgzpal.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3yhxmyxdh.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3zpnxevrf.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ahyehhua.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3glvqpoqf.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3mbrlueho.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt3mujsmetv.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3rdegrieu.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt3tjjfjcst.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3obocjmsg.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3qwwkjzha.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt3vivjgaza.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3uquktbom.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3qqkobgku.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3dqgmdugm.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt3kydklbfi.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3glsfqicr.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3rijyymkq.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt3lwhofkti.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt3lhaaskkg.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt3zfzzyvzd.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt3sdmdopkr.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt3ldyrpdwq.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt3cvrfsrwf.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt3zfoprbvs.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3xcsprjpj.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3lyxvjytn.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3czncacti.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3ubwkefzc.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3hsnkzdud.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt3azofyqok.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt3luwylhax.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3zpmlzxab.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt3icqvrgjn.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt3gvkeufbp.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt3yminzxel.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3jlxxqutf.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3dyirdwqx.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt3pqoocxoz.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3izzcwgzz.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3imszbqjr.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3yfcekomk.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt3tvxonqvu.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3nmdkyume.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt3exflzlyo.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3rkfkitmn.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3thcakgce.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3qgoiktxp.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt3kboeuqoc.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt3qmakrwuq.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3zhybnhxv.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt3jiolghqi.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt3evvycsvu.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3hattzwpr.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt3qmhcaycb.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt3bvmilhvq.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt3kqczkdth.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt3ntnhfitg.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt3pnmkabwh.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt3bqtffzlb.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt3vswozbnr.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt3pwvcabph.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3njuxnzbh.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3aqlsstni.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3zjwubykx.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3sohbvhvb.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt3cvzjpiby.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt3ettelafb.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3qihypuza.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bdjvrxor.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt3gqiapsat.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kdvchxgh.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3iyokmxft.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt3fodrojad.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3xvbzgxvj.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3ncbdibyu.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3ufzmjbih.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt3jkbehefv.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt3izhnbwnz.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt3kbifjopd.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt3bdgnjxol.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3arzvnvip.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3fkdizuwd.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3vryjdjwq.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt3uygvntfk.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt3heyfpegx.html


<!-- 参考信息 -->