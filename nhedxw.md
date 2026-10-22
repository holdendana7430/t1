代发 wailian999

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2xslpndzn.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2gxhxmtgi.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2fwkzbulg.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2haixgvep.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2ezyrzfhz.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2nhckjvcj.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2sksqvkxr.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2eeseuaet.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2ybctvqky.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2kkcxptpc.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2rexttrmx.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2pmrasktu.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2efujipyv.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2cjznzwam.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2lmlcepxj.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2zcnofgtw.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2dsmtpvxh.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2wunzzakh.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2slechise.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2urabpxgf.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2fjzctwqq.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2aijodmhv.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2fxgikvmc.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2oedupzuy.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2tpooxdoe.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2poubzgtn.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2ckrvcppt.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2sddgsqke.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2jokntqch.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2szdwfuvz.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2izhtwnfq.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2zfoerpzm.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2ucpgnbpr.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2jqbedpyw.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2wfpuchqo.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2imhxcydf.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2zjvdnpnu.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2xvtydcus.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2oamjgblp.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2inexfbnn.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2kknkpfta.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2hkvkjdky.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2hsfbiqtf.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2jtvdodwg.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2wqewzerq.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2yxuszxbn.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2ifmgfwgh.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2dnbtduef.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2vuntxomy.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2dzcwexgz.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2wthhsyqn.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bimutcds.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zdzeklbw.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2baiullzo.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2sluioumk.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2bxpqldge.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2fndaabvw.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2luvdpebw.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2oenuxowm.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2fonilhhw.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2urxmzbvk.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rxwtafwo.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2kvvwshgi.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2mlepdhvh.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2nxbzsqoc.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2fpowewcq.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2nzhsldpc.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2vlurnlxc.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2fjesgsyo.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2rqlwspux.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2eiissuxb.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2mmnfimya.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2ltucvivd.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2tgjsltio.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2umvjebtw.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2zhxydplp.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2bftespjh.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2mxggnipr.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2oqcsoamk.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2nzsfauvw.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2uezscqav.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vpnzefjf.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2bufxadyr.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2hkkbqbjo.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2lizutpxu.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2blfzcdlr.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2aedgdqgv.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ttrplxdy.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2msesnxmd.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2avqlyxmu.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2fgodjhzc.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2ucubxqqa.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2reekwozc.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2ttpjucff.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2gbglfwuy.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2nlsqlytd.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2ydbgumjv.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2qgxfjqqa.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2zlnnjfmc.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2shwfumce.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2wanlcdxr.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2fjwpmzhp.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2magiwdbi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gojqvhez.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2rjpojdoh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cehqowtd.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2emciiasg.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2fteqoqah.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2kigjuqee.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2yccxrbol.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2cozxisbm.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2mamiizrj.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2tzrduotj.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2stvgltvi.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2ylrkqkzj.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2vtahmhqn.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2ofnhepwy.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2rhynmlpi.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2gwukhjpq.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2hzoprwvr.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2crtoaklm.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2wafglfzm.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2mfzycslr.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ocryycjj.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2oqhzeztt.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2wqrmpprr.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2sjdirplb.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2jogmbhzc.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2mavvbhzm.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2lfvwbmuf.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2tomrjczg.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2fnovsmwd.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2tzngiwgt.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2ryczlcli.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2oimonsjy.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2xlcbwuvl.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2geahgrsb.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2zcrkfreo.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2vrktmznn.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2nuodhzvi.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2xsjjmdhf.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2zebvcocq.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2gqlhnmcx.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2nmmozomh.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2gowgftqh.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vtkybyfk.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2togqgszp.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2laasrizm.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2bkjqlock.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2ckttszbz.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mncgyjgv.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2bdhptsln.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2wirlzkoa.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2jitdqlcw.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2fhjnqsas.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2xyntbktj.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2sxqxdyfp.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2egbtlnva.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2dbpyxcez.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2xpnmtdam.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2kdkxnlqn.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2safevbwj.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2hjnnigqh.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2zxyieowy.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2vvhmfagw.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2mmpyjsnm.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2dmfchcgm.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2kvwlzsqn.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2jqokkfxm.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2mkyuwcvj.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2vniqxume.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2fubknzjg.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2kamyufvx.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2kuyaghkj.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2uzhquhtx.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2yqilsbmn.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2spbrrlkt.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2zwyljhsy.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2xsfuqell.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2mozzlozn.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2inahygbk.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2wcamkabn.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2ieqzozww.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2tojiteqz.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2zzdlsfmr.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2enxhnhem.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2zsgexvsn.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2yzpnbivq.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2mgnnsscn.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2ykkvwluo.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2pcgzxkfi.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2plarhiem.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2zwgtebdj.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2psplwyqa.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2jqeiwuak.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2puwadkai.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ewszudiu.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2vhsibrwc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wpgpnavr.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2sfatesfy.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2roewtwuh.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2lfythoxb.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2eqzgvcem.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2dlmiuzzs.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2xufmxgjv.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2kdhufcoj.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2ffokunvh.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2yslnlkyp.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ebpkwexh.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2drrlhcqu.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2muuknrpb.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2psnlksyg.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2jmraizat.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2dxdjruuv.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2wbyiveeo.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2woromdnf.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2ogzbeyco.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2thyqpcbm.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2swulqcye.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2wwytjqwt.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2lejvunyl.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2bahulvew.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2omlxafin.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2gqztzgzt.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2bimfdldh.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2bvtqhtsg.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2byouxfqp.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2glkkaisn.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2nfaylbvr.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2mjefbulf.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2rcbfquze.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2wemhtdhw.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2lbfoqpnn.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2votxhvbw.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2xvlozpwr.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt2tyexqobo.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt2tdywirso.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2qemcwzeh.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2hvxfkxpq.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2gfevgqot.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2xbolufer.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2yshcovwn.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2qszmiwjz.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt2qlbbjfzq.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt2mvhorjsx.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2omrnijnd.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt2lqxubnbv.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2nmhocyqd.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2wgolthcz.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2wuignlyn.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt2hjfroaem.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt2hckoutww.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2fsocyypj.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt2zndlttkb.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt2zjopougx.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2kkrisnsa.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt2pfjheghl.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt2xiuwrjsb.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt2kpckeowj.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt2gngjwhab.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt2nrcsietr.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt2sncfutkj.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ctwfvjam.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt2cskjzwnl.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2xqnggeow.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2ehjvhrgd.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2vxmltxac.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2cmjvqwfs.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt2eoqndtyw.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt2cwncnomt.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2uojsxagu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2stbgdryl.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt2pczscfrc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pwgzrcys.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2figfeppp.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt2gghdvfic.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2ybdkmuhb.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2xovtmmol.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2fbmukjvg.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt2qqltszjs.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt2eicaaplf.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt2xipkycqb.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt2zbihapci.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt2hcpahejn.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2vzpexatc.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2bbejymjp.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt2qmgbzlle.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt2pzebfcnm.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt2czyjwsja.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2brpdbzvs.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2jccdjcak.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt2dmlkerki.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt2snmixwki.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt2fdtnfshx.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt2xwppvrgf.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2ypstfgvn.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2apscudge.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2ebpwbcth.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2khoffpli.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2uprjasfl.html


<!-- 参考信息 -->