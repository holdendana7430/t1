代发 wailian999

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2skmdieos.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2qmmxubsz.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2zyluujqi.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ppujwryf.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2rynstjmp.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2tgribtqv.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2sxkacaia.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2pchqfhre.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2zniderwh.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2jzzjskir.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2cnmdhtex.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2viqubazv.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gmtewgzd.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2xuixjdby.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2wgucanzr.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2rrlqhysq.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2ghnogepq.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2borzcszr.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2ehyjgwrz.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2iqhvcxjg.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2qjscpjkw.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2gyylnrkw.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2cbefjyll.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2ldzwxfrc.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2moxnebbd.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2kiyfucey.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2qddgekac.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2nrlpjudg.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2ppafwaoi.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2mislekbg.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2fvqsruhc.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2rloerhsy.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2zylimyja.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2eymrnjvb.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2emuarokn.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2zkyogbje.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2fsyaopgg.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2dqmgovqd.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2gaamnbhz.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2lfzhwach.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2dwjjecug.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2ndjmfiaj.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2oyridfkm.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2rmpqoomj.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2abllgdba.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2sncgtubz.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2tarxqygc.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2iwdjorbk.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2tdpxgsfe.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2dyhmwgma.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2xmidizko.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2dtnwsppj.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2nvocidbq.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2wjgxiyoy.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2zobbdefp.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rakwlxgo.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2wnqbkxio.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2vrxmsnic.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ikfstbae.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2jysvwbqo.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2drwytgan.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2bzfeqfim.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2caoazliw.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2yjfetvfh.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2siaqalag.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2soejylby.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2acvjfpaq.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2vhzofpxp.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2nqldiduy.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2wqpytddu.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2elzznsyr.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2gsadrsvv.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2bvlmyuqm.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2bvzecvpn.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2quukpwyu.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2bzybhkvx.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2tpschuwo.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2urnvyeso.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2ngueywyo.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2vozvvjoc.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2odsjpzgl.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2hzhasrve.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2chwcdetq.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2zaradvxq.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2rcwfopna.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zrshjxnm.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2flmkjtwc.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2dyzdpbwf.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2iyzedtsv.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2txyhzgyo.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2yykeuuvl.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2lsvtwfhx.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2duikbtbc.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2xyqpqaxl.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2intavbyq.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2rcbnjptg.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2sqlzxrfm.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2jnqobiqs.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2roppnhlg.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2qjkcknxj.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2neaoviqj.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2gayeufpn.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2iiempjzl.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2suezjwnw.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2harfubnj.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2zbglsbvs.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2bjwxyaga.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rryhvqwu.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2numxwbjw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2otzughox.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2vjubhpni.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2hyxkqzzv.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2oafhlall.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2bqsjecdu.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2ryfoaldr.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2lvxdlfyt.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2twtstgii.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2prbygpdl.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2whrvdgkx.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2jaexwnba.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2tqdmeuax.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2onmpdxxo.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2oegudyzw.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2iqywruol.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2iudoeauj.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2bzffbdcs.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2vfskirvk.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2ttspuxpz.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2pivhicju.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2ontrhvbe.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2anhlwenc.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2skdokrrk.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2ftpahtzz.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2gtmhueza.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2zcwspypr.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2lfowmgri.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2gerruzab.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2xoxaducv.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2tzpnfhlu.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2ifqwioaf.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2fdeyciuy.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2vhismpkq.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2iylcrmkq.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2sipkcsij.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2tghgltrq.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2vkwifovx.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2qsyrhqxb.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2uzbtafai.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2jfszorhw.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kuwqfxov.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ptzaybfg.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2vcukzdku.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2lozgnwtu.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2dyhhikng.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2ypchsojd.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2gdxvkdhb.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2rabrmksg.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2mqvdcenj.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2cpikiils.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2ommyzhdi.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2njcrezqm.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2deejfimr.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2ckuevmua.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2gihlwhtn.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2ahpsbfda.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2jvjpjqsc.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2rfdtkiwt.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2ahdddvnw.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2cyolpmhk.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2ypekhspm.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2dimzqmmx.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2xeyneiht.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2aguoztmo.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2cvfaasli.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2dhhnevaw.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2grcguper.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2hcwooyma.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2phhvssry.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2wwqatcza.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2xtqvpenb.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2awpfprod.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2rscerjbh.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2ytxcgxsz.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2lshlassh.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2lbjfoane.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2jbyqpvbx.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2zpsdavzk.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2zchqhpjr.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2tgccmoio.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2bxcrtmrg.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2dkfinvrt.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2qbaaoydy.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2lnbpuklz.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2eenvewms.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2egkrzajb.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2rgfbhvzb.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2nwlwpcih.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2pyqvuwvb.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2kcocshvf.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2hmknvsts.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mmncvbes.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2qfqepemz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2euxjwgkb.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2zwdqnzbr.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2ekaqklgt.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2gftspaur.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ldjiomwe.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xzamqwkh.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2lukcmzrx.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2yzueziwv.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2gulyfnir.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2auxdufqe.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2fvpfqntl.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2gtzoicdh.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2vqkipmyt.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2nymkklkv.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2slzokiqb.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2iukziylr.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2vpepikzg.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2qtninwjf.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2xcvfvqpy.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2orngocmz.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2hyjmmckx.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2ysatkhsh.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2fekburqc.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2xvgknvsq.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2eniwewro.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2acewkvxi.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2kxjgrbsh.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2atuchzec.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2qjfnnjdx.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2qtfrcoue.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2hzsfifez.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2nkddehea.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2plmbuhgh.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2ejodieuc.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2ujtahxhi.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2dpnjwojk.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2sbpckfmh.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt2dhcgnxrz.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt2jyxaldpu.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt2uogxpeff.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2seumybfm.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2oedbulib.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2slgjvyxy.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2wdasffhf.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2bvuibcku.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt2ltyrwkyo.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt2tnqhtfsm.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2apahsbca.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt2skrpjset.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2ielhbsxs.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2kyosiezr.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2slbuestn.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt2nlkfrnmx.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt2rvynxpjx.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2jfryaqjs.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt2hpaapaax.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt2rxhdqkxz.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2breaxngi.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt2rxtmzjrc.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt2ismocbxu.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt2qfznnwqq.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt2dfaczwlp.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt2rinaqevm.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt2mmgmhcfw.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt2qntagtpa.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt2lzbwsryu.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2sfrgditc.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2rvsgdsrb.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2rxbmuams.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2ymgjgydd.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt2ghmrbbxf.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt2xtbxjqfl.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2wlwpofyw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jfysrigw.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt2bdkmfvcu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mpxzhjld.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt2jlxpifrc.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt2dmjfqbuq.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2azdlbdrr.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2lkjneovc.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2lgwcrews.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt2xabxeufy.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt2cheujnxs.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt2fjpdgdlw.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt2grrdcjug.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt2ykmmhztm.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2fktvwron.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2phudlotb.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt2pjdnitxp.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt2joakhpua.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt2iwbqfroj.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt2iyklzskc.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2yxikshok.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt2lvwnepsv.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt2atnndstt.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt2zhczryel.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt2ilrikvyc.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2rwnizdrs.html


<!-- 参考信息 -->