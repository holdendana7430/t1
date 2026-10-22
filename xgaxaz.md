代发 wailian999

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2bkaulvpr.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2xpzcojpr.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2qhwbziwz.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2kuepvnbg.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2susklkki.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2vdmyksrc.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2tfswwzdm.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2rmkfbrnb.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2fzaeuary.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2tfqdcomy.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2zsdjakrb.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2myxqbbfl.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2idqopnlm.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2mymzyrcg.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2gxqvlskr.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2smhyvumg.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2kxcfqlte.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2gwdvuhmc.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2cbmkcmqk.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2cxoaqvon.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2dccxsggt.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2mihzyzrd.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2eewkhjhe.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2jiyzeics.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2vxapxzzw.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2ulklispd.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2budvqbjj.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ulgxgnla.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2lcwxboaf.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2xolzbbvb.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2lkhzrliv.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2dtkyzaox.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2uozjxkvu.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2dptnscpw.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2wlgbydit.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2ovztavzj.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2nwrtkget.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2fyqyhoty.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2swrctppr.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qwrhwgvw.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mugkiorc.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2plqtmayt.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zvyaxfgg.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2tminhjhh.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2qqjllodk.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2bpbxnhqc.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2qhpabpso.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2wokaxaga.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2auoqevsp.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2aelmwbhh.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ufildfoq.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2yrzjrgsw.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2ovgnprap.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2fralryrk.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2aoqiotuq.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2kcbwaudj.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2nunxwuxr.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2afqmmlak.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2itpmhnqo.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2ekjielyx.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2qcocweuy.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2nhecthfg.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2xdokyyhi.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2tehsjtrc.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2yesivecf.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2vtqwcuey.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2wfhkhvmi.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2tnzkamoz.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2ivxryovz.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mhmkiyij.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2ipdaioyp.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2govyliiu.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2meadhowq.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2hwemagbb.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2vcoctzkq.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2yltblpep.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2hqiowgvf.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2bcvgbian.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2qrmkflcr.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2xpqkbrhw.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2jxmwtkbt.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2qzgdljuu.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2podeafyv.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2nwhymyen.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2nnhawric.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2znipvwir.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2spwvsqdz.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2qlkynlkn.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2ouonmmof.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2ewrjmadt.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2geoaytga.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hriyfavv.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2tlykqqfp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2njrwwicv.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2vcufqvdk.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2vsaiebrd.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2zvvgxptu.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2uswjmdna.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2dbhoskce.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2dgbvwffs.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2lxzhgfln.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2fsilgjli.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2oetannge.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2kddxzgkf.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2atzeefcp.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2tnwiruyr.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2xfsesfkl.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2pvabowed.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2ahnyhnno.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2fctcwnso.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2jktxgucb.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ungsdqat.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2mxsebecg.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2yvesopmo.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2hshksvbx.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2owyegita.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2ikrcgbzn.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2gxyywjro.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2aiozjeva.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2pybgqmih.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2hhzbdcol.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2helkkuzn.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2dkmepedm.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2tirgrfyu.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2ffufvqzq.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2zkeniuim.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2rbhppxlw.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2vhwyechb.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2csjbgqyk.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2boqarwca.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2hdemedmm.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2abytfshf.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2htdrmtwo.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2mponmakw.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mtapndze.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2sznyeent.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2hzsivydj.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2gjbwwfdb.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2phefbcvc.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2jimbnxwv.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2ltezmelr.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2zsfdtuuk.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2tblusahf.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2klsqfwgu.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2ejjhlqjg.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2lctqsncw.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2iyzcanam.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2ebpwdrdc.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2jzdstasw.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2tfniobjp.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2irjupvzi.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2muznehvv.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2qfubwvxg.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2kxacgatz.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2lxzdopfg.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2xsnahaww.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2hqgahlrv.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2wowhaywx.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2uapqpkox.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2xbmpyxqq.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2cmufipja.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2evfpflaz.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2blphfbya.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2rxpcdhqq.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2hhctsqma.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2ydcnmfqj.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2htajgaoh.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2yrvfejzc.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2rrznoeze.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2omhjjnsy.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2quvjodyd.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2mslasspe.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2leswubkb.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2zpzisgpu.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2asktcbag.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2dwpygmoi.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2yoichpkq.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2oazlvvza.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2uazbjvfo.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2jqmdlfxw.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2jeyjvojy.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2hrjjnpgd.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2etrklqci.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2lbkackdj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ecdmgkha.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2wqzioebl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2octqdodj.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2dfzrqhke.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2cqxiddno.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2bqgjspbg.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2fzttxxhb.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zxbjmpcf.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2pzjsnlpd.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ekeduioh.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2ivbhzzgd.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2jurqbskf.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2pmhghbvw.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2usfstsce.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2yizhducw.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2tetamuxh.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2vijhcdti.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2rwyjdioe.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2vhouahmr.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2kzdpzcoy.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2jkueslrb.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2xxmekvmv.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2gnxaicst.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2cdlswhiy.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2qkejwlav.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2fbqurebb.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2zczjsppc.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2benkyogq.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2lcxvhcjg.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2zygwkjfm.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2yvondrfz.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2tcreshkv.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ncucsntx.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2kfdsnztw.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2cimeiyip.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2rhsqsoiw.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2ccjlophc.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2odsxmhng.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2ansencnd.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt2wfixnpge.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt2xqwzzjyp.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2omebokiy.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2ygetsacn.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2bjdmdhuz.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2slutxgdr.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2bmvpkdlq.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2xqbczhzc.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2diwrgzfp.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt2xrlpzoaj.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2uhyfxltp.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt2pfqxolsg.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2bihtazrl.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2jdierzlz.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2fpptpcmq.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt2oajqbpvr.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt2xmmtzemw.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2xprjtarg.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt2hlkrzrbt.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt2nvygxqfg.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2auunldtf.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt2oifgjxzp.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt2zwjtjpwe.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt2tsrirsnv.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt2hmsdeqep.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt2nhauymmp.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt2sdthtaib.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt2nhsyasqp.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt2kypgogxg.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2apalufgl.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2matjbzih.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2kwhywdge.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2ovsajztk.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt2thjkoxst.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt2lmuhsoay.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2rkwkngww.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fwzcfhng.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt2dcljwsmx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sejhiqhj.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2znujpmnk.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt2marenhwv.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2vlgorpgt.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2cdftxuxu.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2mgodxgeg.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt2wewxhulz.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt2jotjtlrn.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt2smarxekj.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt2bfpudutf.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2ydajgsnx.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2tcovdtbv.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2dpvsmepw.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt2ubamnxom.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt2wlrhmguo.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt2hzhnhjaf.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2rzzuqamb.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2gkrcxtra.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt2haapgrvn.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt2kaxwesrp.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt2vymwhkcp.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt2xtrkdjkp.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2uxrbmrll.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2craisihv.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2jafqpigv.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2bixodrwz.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2ypaqrwgl.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt2klirxiso.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt2kaurhndi.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt2mxtppvrx.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt2dhybnfqh.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2wzziggvl.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2hbzgveiz.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt2ltgcnwki.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt2huezioer.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt2uzxxmncm.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2kzqjicqp.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt2oikdvjcv.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt2eyrzqbgs.html


<!-- 参考信息 -->