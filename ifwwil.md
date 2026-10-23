代发 wailian999

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3wpnkvoru.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3wmyntkoo.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3wjsmssaq.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3akzvxwvl.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3qeigzfsa.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3rjnzvgax.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3zzvsnxuj.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3gqsvgkgc.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3yutkplvf.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3zofcyxvq.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3luikjcly.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3dlhiguik.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3xuqffibj.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3qmbfcrwl.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3fvsefjcu.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3xwlzilhi.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3liphythb.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3vnpfgskp.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3xqiffpia.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3ottcqwja.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3gisczijw.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vslcmvan.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3cvzcxdxv.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3yqxftgoh.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3iddksjbi.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3gqyzbttt.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3wxdmmujl.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3ydwrwrnp.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3oxkopnpn.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3zsygjtev.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3ynrvqfwk.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nszhtoui.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3jvbcrkpg.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3bcvhohxg.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3bnupwyko.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3cuhbpxoa.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3sbyotzau.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3lsetwssk.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3ezfcjlaz.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3bvnnhxps.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3tkjvzrcw.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3ccunxljg.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3qtlikcys.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3uxybmxnq.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3jihysrfx.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3ucgmckwq.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3vtuskept.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3gitnebiu.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3lxashmpb.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3dureabqr.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3wakhtvnj.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3cuzkwsgk.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3wjobrddm.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3scynmvvz.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3tftlkcgq.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3ynfgpqvs.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3aiyljluc.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3odixraut.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3vbtnwaev.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3wjwgegrg.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3kuvoidoo.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3gqihstvw.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3mxsjineh.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3ylwelrcy.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3wdaqvxwb.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3yjwbfwud.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3yyodcawh.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3xoaanzso.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3rwpairhe.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3hnsrhyhh.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3lmffajgn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lnoabapa.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3dxeetcsf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vmyiuojs.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3hkuvvmzc.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3sglrsgmu.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3xxgglutw.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3fbzcrebr.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3abartdvq.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3dnnctamo.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3kuzrtgyx.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3yxrkbqsa.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3utzwazzw.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3toqxsgzh.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3hxhxrnqf.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3qhmaebgo.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3loaakiep.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3tjpnctgp.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3tbjctltn.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3qqqpdqgm.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3spdhdtgy.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ncztiyyn.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3wfbbfosy.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3lithtcjh.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3hhqnzzxa.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3tponbrlm.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3bslbdusb.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3yebwaenr.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3uaikvpxt.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3qerxxdkz.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3zlwyeoil.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3ipobkmvd.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3gcelduey.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3trosxtbu.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3upnlnobp.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3tepmfehu.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3rbfxtfns.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3susnomxh.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3rdnctumq.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3arykdfhw.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3cqjyjpaw.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3eokomxjc.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3pcvxdifx.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3askrksao.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dkapkvrt.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3imkltfbw.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3gznqaxdp.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3uwbeexdh.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xfntkake.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3zginoutf.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3wmfzyfrt.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3cqtbwuym.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3zinvikkv.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3fsbenxzl.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3xhyfcfyg.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3jgcyawvd.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3jpicidpw.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3goezlskk.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3polpdeob.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3ztcyskzp.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3fndkpztq.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3nwvfqynf.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3eyqxrmmp.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3ppsmmedc.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3vjrwqkfu.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3ivmbrnmm.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3vdzmater.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3snxhsnqh.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3olzjuode.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3lrafzzaj.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3flbfrppu.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3faxmcfre.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3qbjonwrk.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3chmuqner.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3wbrgpfmh.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3lmbuioii.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3ususnnzu.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3resniwxn.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3vzduuret.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3bpsfzkiu.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3slzwnyii.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3pwazwnvu.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3ydtjemka.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3orszhttl.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3ajatcojt.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3nwtptger.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3tafhufxv.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3upfxcvvb.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3eilvlsyu.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3mdkkelqo.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3gkhhicue.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3aqjphyhe.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3tnyocrvd.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3kceggyye.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rbtftosg.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3jjuwghgk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zqlujccz.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3mhtmgpgs.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3xyuwtuak.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3ocnovjcs.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3tywicbno.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3sfeytchz.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3vyjdupye.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3fpxllnnh.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3xofjnieh.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3kuiijiel.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ogmdzlxd.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3gwfnhldo.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt3blriwfhl.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3fkywgmwa.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt3rlpgpjus.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt3auboyzhs.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3yihtspas.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3yxwmnyzi.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3tjcfazbb.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt3jdxjrskb.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ilkooomh.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3tijdhnfm.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3wlbazsgw.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt3keysklff.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3pnojedyb.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt3iwgmioxb.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt3svczmesp.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt3habokrfb.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt3pxdzroao.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3evqyfyci.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3zzrcmgqc.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3slvtciwx.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3ysnbmecq.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3euchevkd.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3fszindxa.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt3kypkuckk.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3gfizjimd.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt3htoxghsp.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt3asfvpmbq.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt3fpbpmsvr.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3tqraeejz.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3xevtmbto.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt3wsizduwu.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3qpombbqy.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3xhgetcqb.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3krqmejog.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt3pemlbzaj.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3lpdaawhr.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt3rigguuat.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3yayjqxvr.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3ongbmhbu.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3qegtkhtp.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt3frubqsli.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt3jqtjsxdn.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3tqxgqfit.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt3eoxycqup.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt3ekjdcozt.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3hosmieux.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt3noqysiup.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt3ebliwsgb.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt3csybwhmz.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt3ddwahhtf.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt3qjwmelvz.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt3ilgxrqem.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt3oxnpzjqj.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt3rlxjaeen.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3ikunbbzd.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3vnyuopvy.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3kvcwtlqr.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3alpebqif.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt3saexbsia.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt3pqmeljfo.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3wehrmvlg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bzavbswd.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt3weguwlvl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jajrstmq.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt3zdqrabkv.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt3wyxcdrbn.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3jinikzee.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3wufkczlr.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3crprbyxr.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt3jalrmgjr.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt3sadireki.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt3olftynyi.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt3aclcsajc.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3cnxtmgmr.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3bdatunyu.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3xpodwwyb.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt3wbppwrie.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt3pxmfkacg.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt3ucovutce.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt3hqxcwowo.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3vfynckdf.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt3hprtxcym.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt3vdsdcnan.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt3vhucubye.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt3knrqlqgi.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3dwcmwxdm.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3kopznbpy.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3hndbfiyy.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3dthjcuao.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3vugolkgt.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt3rwwmryxk.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt3jkbzgzyk.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt3elwcemdp.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt3oxuycxbo.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3cwoecfgk.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt3mojcdnjs.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt3dvqhijmq.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt3rsppyeoc.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt3drlulzrh.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3pliddvsv.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt3ufqqoxpo.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt3axpdqofv.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt3pkbazfwv.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3ydznehad.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3zkkllcsg.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3skikygti.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt3flmrszpu.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt3risvstsj.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3tppbfhxm.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt3hksoyunv.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt3gjvxjuhd.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt3jsyxhfwn.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt3znzzxymu.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt3qgisbjbe.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt3wacpkeqy.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt3owyxwvbz.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt3qkyofyaw.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt3xaliophp.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt3qezymdmt.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3psktnqbq.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt3ygotyfnc.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3vxzixxrm.html


<!-- 参考信息 -->