代发 wailian999

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2owsderzs.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2htsuwlya.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2iwlkrqgf.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2nuzicivc.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2unkwdwxg.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2fizpndjc.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2dilanydg.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2gbzjslub.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2aqznfucz.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2mraybbjt.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2rumcjsam.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2nnpdsgun.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2puktqfuy.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2yuoyhgkr.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2qafasllz.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2elvoisam.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2ziwuyylp.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2nxflbrqm.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2njkhrdil.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2wbirtafx.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2qclsxiwz.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2stosctwh.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2lgrjlhun.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2kpasdvbc.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2suetyyrt.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2rqvtknmr.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2grqxzrtj.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2qbaijetz.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2qifhhaok.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lyzjyvkr.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2jlwkewuy.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2iaakmyik.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2zkjzlnjs.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2yivpssjg.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2htrkfpas.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2jgauxrks.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2croqudyj.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dlmywwnn.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2khltacip.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2bsgtvnia.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2uzkpahqo.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2gfqvilzu.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2jhrarykn.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2nvqetxvh.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2dkcrzuqt.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2eqkdbxch.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2fwrxusic.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2cpgvqnmw.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2zgtthcxd.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2yyejcocn.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2ytlhgnvx.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2ztamdxnp.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2xixqroum.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2bpnboldf.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2qtihyczd.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2yogbgwmn.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2zxtkxzdl.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2vbpgrsid.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2rljtxhad.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2mgpeuvpl.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2brxqjgee.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2mormnqay.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2jiixtbhg.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ndgdpcru.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2tgjnvgef.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2shkkhcnx.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2qdicfnlk.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2zxvdpuiw.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2nggobkgz.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2zvhzpubh.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2amcerofg.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2ubcehyqe.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2dcamcbwx.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2nndckfif.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2erxoimrm.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2afisctah.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2funiaylm.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2iszvzfpb.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2uwbbudeu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2aimgkchl.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2odtavvgc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ptgpnino.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2micpoooq.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2fdewxgmv.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2hpmckuaf.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2ivfyinqt.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2twcurydv.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2fupjhzrg.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2hozkekww.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2asiniqhx.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2lerekogp.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2jurxhdru.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2pjwevcyt.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2cvdpjyai.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2zwahurxs.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2akfsjfgw.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2ilbkfjxn.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2rygfiowd.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2xckszckt.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2houypcjv.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2qqsbkqdd.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2oevwonej.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2ufjhjtyp.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2dxhcutfb.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2wwvkhstz.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2pipsigxx.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2jdenvuzb.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2wojgwyfx.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2zpcggwft.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2imshnvri.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2uqkgtjgj.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2fqkqvirz.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2ixcxbmms.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2itiikaeh.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2xucskgab.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2xojlktki.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2cjpqrnmj.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2rbffbrzq.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2gdbcifak.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2bkxwedfa.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2mvbszcpk.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gnmblmfz.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2phafashr.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2ucrevumt.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2vyaxenph.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2mpxvqrlh.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2vjmlhxoy.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2xgmeialc.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2ssjfrizb.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2rftockgm.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2hixiohif.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2wzjcslrt.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2dkqjgrdo.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2yoyyvymr.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2vkqxulfa.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2zftcxkgl.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2imrsvmgv.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2mfcfgyqj.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2rlimyxfj.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2qjvkzmml.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2jjgnjtfv.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2vrxhkbos.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2atrvxlrf.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2nhxhzsac.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2urisspbo.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2ezcwzxve.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2rwzgilmz.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2ohkdzjdx.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2fgsndgjb.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2dmhwhzcg.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2bziyphnm.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2uidnhpfk.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2hujqmljf.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2xtggmpsp.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2dikdqjjb.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2lnmnueya.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2iqoaykui.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2ennbpkmg.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2rvpgmuwx.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2qhyuoftm.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2dpguzfjh.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2uayyctqj.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2yyqzamxe.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2kfobeshp.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2xdgqgclf.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2wvkcmxuo.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2zllqogbo.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2prtmhlmo.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2muaqolvf.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2hkyvvtkz.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2daymxaze.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ywzhtbvw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2npwusvyk.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2iccwgliz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bhfmedwr.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2kuvklilr.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2mrvguytf.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2fthsyxze.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2bdzgmfib.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2xgdaehyz.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2kqkllutx.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2ityzyfei.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2xyqzuszi.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2fetszitt.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2ttzbsusa.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2gixbgvhg.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2iwbfjiua.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2mbdsguve.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2aaxwiyzn.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2pivoerji.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2eoruzbml.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2oztpujdd.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2hlbiergs.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2kghpovgu.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2cmiydsex.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2gaibxodi.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2sdxpfdiv.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2nobmdvzk.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2jlonxosl.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2xlwhgxot.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2aigerztz.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2prprvinr.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2guexdfus.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2twxupbnb.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2plvngtcv.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2nruhtlhf.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2pvlbdaaj.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2ykzqoixz.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2dsckbist.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2rrhbuteg.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2wtkdigqe.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt2rqzxiuvb.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt2ubphzwfq.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt2luxqmkez.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2jlnpihuf.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2fefokeui.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2quraeijb.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2hyeebjso.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2dofropuu.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2ldycaumb.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt2jokyrraq.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2jhsgkgjr.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt2pyijzygq.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2ftnplmzy.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2zcdtpfoq.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2fqrcjlao.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt2klevzful.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt2tpjwmkbt.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2qfvtqeka.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt2uylvrjwv.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt2ugquieup.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2rpjufvxw.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt2orjazuid.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt2pbgmsbig.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt2cjxltxml.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt2pbdpkypf.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt2cdktcvzc.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt2sxtohmvd.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt2kzndwaqx.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt2ukmqmaat.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2zxokuvsa.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2abixmrao.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2lxkrapzg.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2ybljpzxz.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt2qqfxfeku.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt2kitcehva.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2uwbbaxar.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sgqcdgzw.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt2kfqulshs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mdsnmcbb.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt2mscabzzb.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt2xlzthszq.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2vnyddcgv.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2hcukqmay.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2delioecf.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt2ipwlwtou.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt2oqahyjyj.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt2chqlegex.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt2qnbglxur.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt2ejijvoae.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2psbaxpgt.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2hrrtoniv.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt2biifxoih.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt2xinwlsee.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt2eyczmtgr.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2lsummscj.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2usnfciac.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt2unrdjtyq.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt2fzahwxvz.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt2ohotyokv.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt2vkzuqnfs.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2uicnmmag.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2rbsphojf.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2shgrduzz.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2rqjdowfx.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2pqoryrcg.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt2mfronvcj.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt2wntefikk.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2ocryfbuj.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt2ojjkxjjo.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2hgoxqcdu.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt2gifyqzyp.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2ommytzkh.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt2zhhygifo.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2tzqnthpu.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt2vgohdehq.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt2yuyrkfha.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt2zfaiuvtr.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt2ikpfrcwf.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2pycvintf.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2dybdftea.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2eosidpju.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt2ahscdqcx.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt2eygztlji.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2jymmaurs.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt2euolibma.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt2hztlspqk.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt2izjlzyth.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt2lplzbonr.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt2zqgtjwzr.html


<!-- 参考信息 -->