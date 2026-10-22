代发 wailian999

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2ivtswcuf.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2lfblaugw.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2ggqrrwis.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2yincikxg.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2wphlhyfx.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2ikpegpwu.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2uuctflgb.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2ffaigxjo.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2pqtmeknf.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2mqmfioqh.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2lcdmqfpl.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ymihzrqk.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2jssyeahl.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2gigtvnjb.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2rqscujrf.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2iinsrsmm.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2nabtablh.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2qpuegafo.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2tstkltch.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2zufqflfz.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2nbjdwdxd.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2dibhybuq.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2bawfunke.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2awyqefmm.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2tbuinswk.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xwmcpulw.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jlihqdcq.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2cezbdvhz.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2bpytvkfo.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2zwnrfamx.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2fzhfllip.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2isztiggb.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2wguohsht.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2unwefwol.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zehtakef.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2lkvbjedm.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2xicvidkh.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2nahcgjin.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2azudfvrn.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2bjwnjgwc.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2lcpabnlv.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2xxfvmxhf.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2ewcnikys.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2zwfxtdpg.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2sipsbwjp.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2gmhwcdif.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2srnlkxmn.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2pffijlnw.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2hzudbyif.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2ywhulpai.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2vngivjey.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2cpooqbqu.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2gjosffne.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2yyxgpeft.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2paummgfp.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2abirmsoc.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2vsmurdrm.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2cihvpgiv.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2ltybrcfg.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2ktdisgzl.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2yzybcyud.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2lkyspqvh.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2hphshhpt.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2kmqgnjwz.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2dohhfmyy.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2zdegkgse.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2rhmwzhjv.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2umoioleg.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2zsivlgei.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2uiprprgp.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2xlvhorua.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2nurgizls.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2alscrwqx.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2obcohotk.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2pyqltbxv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uvnymanq.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2yrtbwftd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xtdsspgx.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2uumhouoo.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2ovebixpm.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2tvsqhggk.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2vybsxaap.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2pbzewmjo.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2qqkdwhnw.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2gvtoxroj.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2fijjmnoo.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2dpehhyhc.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2cistrshj.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2xcgddpyc.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2hrlsqdkh.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ewgyqxjt.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2xjaafjhh.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2aoihmkws.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2uqblbsug.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2fstelrqn.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2hqyphbwb.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2edbqvocv.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2vbaistdx.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2pgyxbsmp.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2afazjrsw.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2vyvxueng.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2kramovdl.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2oluqlwwx.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2cspdbrsj.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2cucuynkj.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2jdpoazho.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2utilpcpa.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2jnjeeagf.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2wgajtdqu.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2ndwvbbxk.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2fkunwsig.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2taibzfom.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2xjhlppgr.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2jlnudhqc.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2uctskkvw.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2zvdpmrmu.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2pjmrbszx.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2uhscsdza.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jqopksxw.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2waolbrny.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2nswkodrk.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2ckongudp.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2icvmdfgy.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2lzviaoci.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2ajitydci.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2gjzcjfze.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2xbwqsias.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2rmsjtgwf.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2zgowaydj.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2bwsazovk.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2kxlgdxjg.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2koameixv.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2kturfrzw.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2zfbpkzrs.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2lzyddsny.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2ehntcrxf.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2lbsuvbrl.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2mtmuufut.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2gqyekisw.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2nwrmaoig.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2vywonnaj.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2rdcuyiqe.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2fldoiikv.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2zbbdrsud.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2vhkvwjws.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2yyuvzmlr.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2qixwovla.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2utcpdaph.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2nktqkzsr.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2wlzpzefb.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2ncvdlgpy.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2mpfoapcf.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2gsnrlleg.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2mmampytd.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2khvgzzuz.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2gqktfoty.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2npyeizql.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2yijqznoo.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2xjbdmdew.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2unqrrugc.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2dnenwcil.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2kstmzjyg.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2eevipkcj.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2qugzwroq.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2ermqdmqg.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2mmnpxwbq.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2etfnzrtd.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2rnnxxawq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jughlles.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2zxlwvvho.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rbhrqyuw.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2pzkkptxv.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2bglywrmk.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2slrfcgpc.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jkujkcxm.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2vbactlvy.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2iuoowwzr.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2srjzrlfb.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2fdenscst.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2jpgzgduw.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2pulvyxtj.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2iijqigae.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2fdzwaatc.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2xlailgis.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2uryovqum.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2gxhbxrmv.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2oxggelvr.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2hoxwqswx.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2kwmmxpjn.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2fdajyaro.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2yhsnubua.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2zzqtlbrw.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2pecuzbex.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2znmgvvpi.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2tmzttehl.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2dnlzsbmf.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2raofwtej.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2fmwqsrzs.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2zglwglru.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2euuiikmi.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2wfydyiag.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2ttzjywbl.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2kqklyjpc.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2hxehuunx.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2uxgkxvbc.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2dynoqico.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2svduycpm.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt2uhoopoms.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt2kmdcngax.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt2gnehxmcf.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2chhctdde.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2ctruxwga.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2osjjhcfl.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2kxvlnjcl.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2bdwisqfn.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt2yxddybvj.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt2uqxutjqv.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2bqqqrnxl.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt2izvtiuqn.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2wnfvazfu.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2vwagiqys.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2vgemshdb.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt2wvfneavz.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt2lgjqgltu.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2rpezcqlx.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt2ttmaoswl.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt2arfoumey.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2usoixmui.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt2rnrrdxbh.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt2cuxxtlva.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt2eznxdsvk.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt2jobegirh.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt2zzmadurq.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt2asrxzcxg.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt2dpcgmmkc.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt2aatdppxo.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2lvqaccxv.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2ooijbtsk.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2fvinsxow.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2xttpjiwh.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt2fnwntmvy.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt2ngdpcarh.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2ycwbzhvm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2eyrurxol.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt2sshujhcm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qnybophi.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt2zpkytbms.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt2dbudowpu.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2fuumatkh.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2itpzgsxw.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2jrzcgusa.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt2vxprzjsm.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt2lnskedli.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt2dfpkvpxp.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt2oztvwoqw.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt2nmaojkmn.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2gieszvyu.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2odkumbrq.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt2ulhrztpf.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt2jyngyrlp.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt2ymutceqa.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt2pjospjfb.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2zkuvupws.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt2hgjjqnfi.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt2seayxchn.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt2nbfhfije.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt2annhdvew.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2iqedufcv.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2upmqeozi.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2yilylisy.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2intwltng.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2njkpsahp.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt2snkljyer.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt2ulnomocq.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt2mizaiapb.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt2xloipscn.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2kuxiokpo.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2psngwtty.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt2jteybbwi.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2lcxlmjym.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2dkwizlxg.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt2pkgofsmz.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt2wpfricjo.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt2aonfdxsx.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt2ewzmghnp.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2rabfismp.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2avlfqgcj.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2barlskgh.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt2qdaxsvpz.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt2lpsfablf.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt2sftmmple.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt2gbpdpisf.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt2wdmcyljg.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt2tsjwhmtf.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt2moobvmds.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt2ixpdptms.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt2ciuwnokh.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt2eujwmowi.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2jxjhtwms.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt2cxdpdjja.html


<!-- 参考信息 -->