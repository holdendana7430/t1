代发 wailian999

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2qsxnlutu.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2jmxmdhlg.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2xoxworzb.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2jdquhxqf.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2iykakfto.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2xeqlrhoh.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2ilzxiytj.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2xxafljlt.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2eidfhsev.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2cwiiyqtw.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2uxfjwuhh.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2gtujiydj.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2qanyaxwt.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2dfhdzfvx.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2itlitggi.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2nxvzgbwd.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2yutwdwss.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2bqljnplt.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2azfjvdxh.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2plpltovt.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2siolcpfq.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2embwshoy.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2kzdighic.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ufguexyf.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2faselbwg.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2loyzkrbl.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tlifplmt.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2hjlpqkqv.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2ebofypcb.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2fcowridd.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2axlhfcoy.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2htdmyaom.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2msmztlkq.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hgrtrvkc.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2oqqapuop.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2agktwqzb.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2yoohcrrw.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2yrgjpjer.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2vzzzstxx.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2glluotlq.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2qlimirga.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2hpcblgbe.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2cemizqqa.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2dkrcfmkj.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2yubajmni.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2itdovegf.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2ulwcyrej.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2pqtgrzgj.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2atzhmjak.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2zogusvlk.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2vcmntmap.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2swbpgjhe.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2fqixvrwl.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nutoudmr.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2blxzabkg.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2trglpqwf.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2ykzesbej.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2fkkprqgy.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2hhhgktrg.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2frimelhh.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2wgxxsanv.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2elibznfj.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2vdsuzgxt.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2wzfgggsa.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2kwcwjqvv.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2sccapinj.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2yujygbvz.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2yezyniel.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2sybyeipy.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2jjbgffat.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ijsywecc.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2swkfdqhk.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2vpkoxntf.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2rzimjkvd.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2onrtyqyy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jxayfhkl.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2oxgknsym.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2omzztdic.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2nbwynczu.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2rbnkerhu.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2lcscfuek.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2lwsfijdt.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2ykcmpbph.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2glvdaqzv.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2cqgqdlpf.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2xkzsvsju.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2qqyaqrou.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2klodpyjg.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2wvehkfuy.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2edsfajvf.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ksykxril.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2bxbomqxs.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2zkyxelbo.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2wyuadbyk.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2gaonhovu.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2mmztoxjr.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2qmseegmg.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2iwajnuec.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2jqscgcyw.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2ugekedkk.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2zrhtbqrd.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2whlaigil.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2hnctapui.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2auxlbrxo.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2muvtgsfl.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2pzgbroke.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2laqjncjq.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2kbalppsc.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2euvaspri.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2vsslrhag.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2ddqiptcw.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2glfajzxm.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2bmapxalr.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2wcsftmgw.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2kwlmkfmu.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2snrtcedp.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2dwrrcjqj.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2ailiizkn.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2iyziomxx.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2uscrzzzo.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2tdimlbas.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2uaswmsrn.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2ogiwtffv.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2lhtmnfvk.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2hfpzvavk.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2sinolybs.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2ipdnfcfr.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2xyvsjipc.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2ubdbtkfv.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2ytxglcir.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2ioeqbdkm.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2ynblwdfg.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2yukwkvwi.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2zzudxvka.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2zaehmcvj.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2cpnitppg.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ktfxexaz.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2qqoaiqke.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2xttwghoo.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2swiztlng.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2fwscwwtc.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2xzbltbvx.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2ogzjlbya.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2hstquqei.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2bxqnztcx.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2rlmdfmgk.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2apnoigzn.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2ykfelmll.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2dxkzfcca.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2oelrwmxp.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2dkuyndrd.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2logvwexd.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2btlnxoih.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2doiraoiu.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2mhzxmsrj.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2sqdqitum.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2ywdsjiko.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2gmutrmkg.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2wjuvyhti.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2hvkznlns.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2uqeqovqj.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2ogtbcmfv.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2gohpryye.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2sbaqzxju.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2bzykwfjk.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2pxvupvvf.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2ulblpugf.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2cqwmsroj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vmhmfowu.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2xhskctrx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2relbokvl.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2fyiyibbg.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2kxiylozl.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2gezgsann.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2ynsnqaqk.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2unictrbf.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2zvlblrvq.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2ifwqjmdo.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2nnnyaorz.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2xtfrpyqb.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ncmxrdob.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2uuwkspsz.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2ktqqhrwo.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2vctiepiz.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2llpjzvve.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2mdgjjrzb.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2rxiauijw.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2skdtszcl.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2gvmooxet.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2ldlwirgu.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2vnpktgsx.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2qyonmwsc.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2irznezqt.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2bmmlnijn.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2fxhuntku.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2dhaditrq.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2pgxvwmem.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2cjewcgml.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2ogeimfub.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2zhefqisl.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2fmlhlzbm.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2zfrlvmmf.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2jxdcbbaa.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2zxuwygvq.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2vzxhamca.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2hrbbpgmr.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2bnxtqzvo.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt2tltdzwfn.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt2aclketio.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt2lpsudzhh.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2xsgydbsb.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2tvuppjhj.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2katazxwn.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2pxsurtni.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2bzjassia.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2yzcbmpqo.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt2ayvzlpph.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2azgdlnad.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt2niqkszju.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2wqgocjfb.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2rzyfzbqn.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2xutejush.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt2kcuhdazn.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt2ytrddeak.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2jfsxlagl.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt2tiikowkh.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt2fymtmcff.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2zpmkzqdc.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt2qjywhugi.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt2fqdnzcgq.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt2gqbztsre.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt2uqurkhzn.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt2xdssgkpw.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt2ccnkidab.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt2rwylcvrk.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt2lpkppcfo.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2hdqttjly.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2ysvabaix.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2ipgazxcs.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2xntjghmg.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt2yimcjsyr.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt2pggebckp.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2xkarimrk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rvezqpzc.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt2kjhhdlgq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tftkaxil.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2fhopqjpn.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt2rrakjojl.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2lseipvpk.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2kveqqphm.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2majmwvox.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt2uzywrtor.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt2lpprarta.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt2hjfpwbld.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt2dmbkwxhd.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2cpmgehir.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2wyuxfijh.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2oqdybnfa.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt2qyinkzgh.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt2rypqijge.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt2frkhjrhg.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt2ojxlipls.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2avuihyru.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt2corrtenj.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt2pmerpyiy.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt2bwmwziva.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt2knsmbjqi.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2rdzmfilr.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2gjojkibh.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2zrpyszod.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2tsfwfadr.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2gjrebdmo.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt2xqkuygdn.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt2kylphjuf.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2xovikylx.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt2jhgtuptr.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt2xaruwmxu.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2hyzrremr.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt2dsplvsnr.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt2ctqdlzkj.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2azdtpujq.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2qltrgnlw.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt2awsfwcsv.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt2mtmihmoy.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt2uurzrqbv.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2nbouyodh.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2fjnilscm.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt2lxabsyqd.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt2bfvakqdb.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt2fsxvacvt.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2weszgost.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt2tqzrssur.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt2olqxrdja.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt2awodywvh.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt2jrdqcydf.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt2blozxgfm.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt2xkuamogl.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt2uramrmvg.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt2qvjyppnp.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt2ccvolkmy.html


<!-- 参考信息 -->