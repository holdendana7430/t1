代发 wailian999

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2vqdrcjus.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2zkarlyrw.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2bbtfukir.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2vjmjrlqq.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2gymlrfps.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2kercjlwm.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2uqerkiri.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2lljfvrdx.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2fztbvyfn.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2aqdvwuxn.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2rppmzkoi.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2owahlnol.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2wyeswkdk.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2ouopqiyz.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2gidpvaqw.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2lyymlzeg.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2iymrqhhu.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2uufrlxcn.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2fveebdhg.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2nrjjmfnu.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2fkzhkgwp.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ebtxoxnp.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dbswdahc.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2wqifjigw.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2rekjrerk.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2hrukrtja.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2tatoqfcv.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2xdgjebfi.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zgqxagoi.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mybdpsde.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2fvufqooe.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2aaucxvvk.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2xcgtizhh.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2isemgvbj.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2yebdowbj.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2yrzmqkkm.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2gykclocz.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2xrxqtawo.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2idoezawi.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2iypqqecw.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2woxnxqqj.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2dmegrzwj.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2ytyiodpl.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2blwmkkev.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2fkgmqrvs.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2tygqgkkj.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2nhanjzpj.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2ltymxgpw.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2itubtzfk.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jahyzdur.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2lrgtybqu.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2cwenaxnc.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2xdhvqypn.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2kqpyylbs.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2gnoamzdj.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2qpdoksgb.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2cezitklh.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2mfzrlnrg.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2wtsrgeap.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2xitrmitt.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2hshwehxw.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2dgzwbukd.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2pepnerma.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2frzltlft.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2ykzbdozg.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2jfdwlhja.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2htwahpgx.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2jojrlfnz.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2llvzwrwe.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2gojyoynv.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2siwdxrvb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2almyfkgm.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2pgsvzgrk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kokdyyuy.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2xtxuiqjh.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2sbodqanj.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2srkmacbh.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2mszkfowr.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2rpbtploj.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2aoukxjtn.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2hplgumkk.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2wfsaiyvr.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2seerwroo.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2oeuilbht.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2fybphfxl.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2eaayvjdb.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2svuiakuz.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2lftmtltp.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2mgpbngyx.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2kpjawqyr.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2jnhtpdwm.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2uxzezxam.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2xxpggfez.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2bcyyltoz.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2syyabvka.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2camwuhcl.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2twcegdjk.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2mwdvqaff.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2hkpqmqfs.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2mjosmgxx.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2wrxzptpm.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2lzfdmgyd.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2qbpsrylk.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2zfbanfap.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2pklzwcru.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2biiezmpx.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2qlfcgojy.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2fcselhgu.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2dvizcokq.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2bauzrpoa.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2ortbrnmh.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2pnrlhtmt.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2dspjmpvv.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yjzrsmbx.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2dilbipwf.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2vfashjmq.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2zbzoxscu.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2ixojbhyx.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2jolujwpe.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2hiqdbjcj.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2gkjhqigp.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2vhgoligg.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2xpydbjvb.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2oyvvpggb.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2pnspbtph.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2edruvqki.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2yunfgasx.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2tfxldzml.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2zlpkiafx.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2ylmrcyur.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2evrxqxev.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2lywmqbaz.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2eotuwxqm.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2uvtzynuu.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2hiuvpuih.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2dxnbbhjz.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2upoifica.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2yqqhilmt.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2iznrsffk.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2rbwhwemv.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2rvxdtsxo.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2obhogxmi.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2fdtciwka.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2zqwdwvop.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2wfbihogi.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2cluygcot.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2hfemdikk.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2dqqtrgeu.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2gdrcurxd.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2vhrylfmd.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2uhlgobpj.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2alcfubtz.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2opkmdhmz.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2oxfludbl.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2wskifmhr.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2jdbhrhif.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2mfvkkhwa.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2zulrdzdi.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2donisaeu.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2rtakwuak.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2sgdwcpnu.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2baxydwru.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2gwwyrcgk.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2bstiqrhq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qnaplwcm.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2uhyvfzud.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zuxjgwht.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2umwpxocr.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2fglbigdk.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2rayscrfu.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ahveqsdd.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2sfxxkxtq.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2cxtabhdk.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2zuukftri.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2kykcnnax.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2mknwbwdj.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2rgsmyraw.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2entmqnwf.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2zpjjjlys.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2gntmkyin.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2ihtcvvku.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2pflcwsam.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2kqittzjn.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2kdvnexxq.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2kayzttrt.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2aoxzoqha.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2tyrammmw.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2prwsguwc.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2wqxfbtdz.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2gcsvimfo.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2cxjvwaoi.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2jnaqlsht.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2arncogfc.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2nvtqvlkq.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2pwtgjcau.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2ttdgssfv.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2kdklifjj.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2zqunyesp.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2ridwqgrk.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2ncrpeeyi.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2kohoruhc.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2stzohlpk.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2yindidsy.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt2oqwtgghn.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt2ythhfnzo.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2nttipfxb.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2izebfayp.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2yienadwi.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2jppejaxj.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2vsttkbqi.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2umdsubkt.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt2ifzjmokt.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt2oovnzkov.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2ogodqvbz.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt2vdflfary.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2curyxdkq.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2hyvjjttz.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2njqflmeq.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt2pxuxwmoe.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt2sdghwnii.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2vpheyqic.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt2wcackfer.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt2fuetwntb.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2zsjryhcq.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt2fburxxzs.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt2mblchftb.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt2geynwnyz.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt2rxmxbhai.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt2thoddmvg.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt2nmqztdty.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt2uaahtmrf.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt2dqxjgbwk.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2gwkrhojr.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2hltgofyp.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2xhecjiqc.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2lhuwjydl.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt2alkcaltv.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt2zjdgfmad.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2ybtczheh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2spfzzgml.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt2zpqluatn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cbfuwlko.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt2qpgchwqk.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt2fkwrmvhu.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2zhazjqbl.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2hovxqyux.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2tpwukzwn.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt2kjvpnvrg.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt2edgdlxuu.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt2qmsyqtcr.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt2bgusrofc.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt2fzwqeoxo.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2ejoojspe.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2ilywordj.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt2dxltyuxt.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt2jmxrlxlq.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt2aqvdvsyl.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2iktgcwiw.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2brlhiryl.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt2ailwefdd.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt2auxcpbhe.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt2kuntzvha.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt2fwkvvtum.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2vciltnai.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2vpsxozea.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2crkuovcz.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2duppbomm.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2vtyfnuli.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt2gesdboiu.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt2lxwkuxqk.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2eblrkkoq.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt2rrmguyam.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt2ovfuhjwz.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt2mgrrvoyb.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2kwpeclmq.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt2vsuazhes.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2stobfgqh.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt2ixifmmis.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt2fxlqfbjs.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt2uokklozg.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt2rfzconsp.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2fxjqwjuv.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2oreqwelj.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt2irtwdfaj.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt2jbqjhwzi.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt2samfoxil.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt2rppofhbh.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2jwnzkogw.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt2vonvgwyf.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt2meecfuhl.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt2emkeccpb.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt2ulepkgpd.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt2wszqmvbs.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt2nequzlvj.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt2iugrtyfi.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt2vvzqtnwf.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt2rdhoozgb.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2emnxbhci.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt2iohmmrci.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2ivrmyckl.html


<!-- 参考信息 -->