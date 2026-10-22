代发 wailian999

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ssavzrrd.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2alirehbv.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2ulztjhje.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2cdmgjopb.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2dclcrkkf.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2agnkrazx.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2rzusptut.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2rfkgxveh.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2txzfmzac.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2dxzpeqfk.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2zdzopdlb.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2muypptgu.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2qbnmwcft.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2qixavxad.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2sxaqixoq.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2guyhccbv.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jtgmlgth.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2ksevllcp.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2rahykajz.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2kcjjpwai.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2awphwgln.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2axrnfqfs.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2ivruuowp.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2tczumjuz.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fstkyjgf.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2lwifmxdj.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2axjbawpt.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2hknxwepa.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2snfyxxzc.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2zaellqbu.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2lrnqknzs.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2gmvnehic.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2ktymfbth.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2kotasnax.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2jdivnjnq.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2pjoscbsw.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2zjcwnfdh.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2iaqnmxwz.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2viyoprwe.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2dwbfzjrj.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2ykkyerdu.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2kymarvwz.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2qdravjlh.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2yhbpmbdi.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2mcwaqaec.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2ubbbbixa.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2ghjlcefk.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2buxcmtag.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2leilruqs.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2rzswyios.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2tvsddqxw.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ybzguzpd.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2gnmsgwvg.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2lvuamfyv.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2jmyhfsxl.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2ugychlfp.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2odmsdafl.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2xeftgotr.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2cestjece.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2iqrnuedp.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2cebyghqy.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2fxiqofqn.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2cedzphaa.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2ezzzuxwi.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2lldjlobh.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2lrrnjtui.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2vanugpvu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2amnnvpph.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2phfahedx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gitucbao.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2lwpgbxex.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2xauafglz.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2iyfvkoie.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2phnkunit.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2cbjsfptz.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2jeafjxow.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2evbtwqnf.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2nbzsdmwp.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2youuwxqz.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2bvnbrlpw.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2rtdpxcuk.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ebebwlyl.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2kotkpywy.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2slbkhpll.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2oypaussi.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2jvppbqvy.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2vnjqseng.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2hwsamvui.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2sfwuxynu.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2lunmhfiu.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2uyvjfvpo.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2nziatjuu.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2ivnugfru.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2emrftmjk.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2bqbyrdhu.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2vhjtktlx.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2kgklxynm.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2wrvdbsqi.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2ehfpuagt.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2vlidplaj.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2epqpjwho.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2cbxmfnvi.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2wsnvhveq.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2ymizcdjr.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2jbnljnvb.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2xwmugygs.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2fhmazyrx.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2bubyectc.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2hmoclfod.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wafusxcg.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2kdrwlndg.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2blvshwhe.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2vdcetmnd.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2zvaifcqv.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2mnnoowev.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2mroxjzty.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2ddwzckxs.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2hrdjdjxr.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2bxpnuamc.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2itppvxxk.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2zrfqkgbr.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2ymfdpljy.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2lelumnai.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2ogwxqthu.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2saurmcsp.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2czpotcuf.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2nhklkkfk.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2yiqwnbmr.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2efnhyqox.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2ywuernmb.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2acikeuft.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2nmlfvinn.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2apictzqq.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2naswtrde.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2qppmbyet.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2gbhvupss.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2hpumigoj.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2tidvnbfu.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2byvmbeto.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2kjnanxxa.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2zqvdvpwd.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2gixzxvmx.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2bxcatfgv.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2zrvynkbz.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2kyaqkruz.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2wqsmnwbx.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2oidakgkj.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2imrrpsqi.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2fmqxyxlc.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2wiyjyzhf.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2pqcmkann.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2izbnjyae.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2mgnnfcrq.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2afkiamkq.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2uennptek.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2ofpgadiq.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2qbqjttac.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2fnozfein.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2vhwoubcc.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2udxyesjc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jaewyfqz.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2ibohoptt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2njyadlwq.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2vdzdyopx.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2tkavtbqp.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ktqnvkps.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tawhxfuo.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ylrdgqka.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2lwsibwux.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2jvfcpgit.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2vzuqxoza.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2zjjflvmz.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2qarkvkfb.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2yunetved.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2enimahbf.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2bpwvzztd.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2zaehnarz.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2vtryvaoo.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2ivltoqaj.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2brfefamt.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2vjvkcsrq.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2qtespkrg.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2eyweizki.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2makyxanb.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2divxpvgi.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2tgevwuke.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2myamoqpq.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2qtqihrse.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2ufjgegbv.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2xmbaryhu.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2jwzgtrrh.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2broadmcx.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2xzbvphpr.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2thcurvhk.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2fqtkxdmz.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2crdixfhy.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2bubhxvbv.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2hwnfrgjm.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2mtqjpjjw.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt2kqxcrtkp.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt2opfomupv.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2uijqussm.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2jpkexckf.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2jhdnlagx.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2raukioeu.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2efpsefzc.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2upgursym.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2kassihrs.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt2stslgbqf.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2kvjmapzu.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt2kapjmxxw.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2msxrsbyl.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2inhwpgfg.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2mvcdhqxf.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt2bqqoejxu.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt2avgvoqvs.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2ykhzvsqu.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt2ucfzuxcp.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt2gwzvlbqn.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2pkhezpof.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt2vppkxsch.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt2ondaiode.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt2emupayhl.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt2femdplsj.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt2hrbbooqw.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt2vsxtpgvl.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt2qwxnlaxe.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt2dfikzkja.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2jxegxymr.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2xhskvwuj.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2dwiqqnoy.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2ujgziwxb.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt2gbbhbkja.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt2cbxefjbx.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2gwwttezp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ipmpynvg.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt2xswjxmpf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kuizbffr.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2cpejkyqc.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt2wfgkflsg.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2bticiuhg.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2hzkabkqq.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2sbsayxeq.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt2gfcwdvem.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt2fnlwykpi.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt2gkpcedqs.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt2mcegbfvv.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2leqlmdwi.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2kqxwkwml.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2qftvfqzk.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt2kxhdchjn.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt2yphxvcco.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt2muvohnha.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt2grqmsrxw.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2nmibfxts.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt2jeqlpckj.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt2eiwhbfbq.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt2xqnjrdvu.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt2ntgovrje.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2xkonrtfg.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2yhttjkfa.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2gixkxfpt.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2jucoomjl.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2fnccsypr.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt2dbqrftoh.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt2onxuaakf.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2pgdmxbmn.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt2gzimexnl.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2xkucihnp.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2smqsjqyy.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2ejxtbmfc.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2sscmsmbg.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2dpwetatl.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt2jxphniwz.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt2rczglufm.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt2ndjhfzuv.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt2wfrhxsnh.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2yvqjalve.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2yzaafsth.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2mduvrvmr.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt2hxutskjl.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt2avazbruc.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2fbctksrk.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2rlqidcjw.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt2btgrflnu.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt2gibfeajd.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt2nvspsvog.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt2cxfsbdia.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt2vsiojuzj.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt2ztcuzwlh.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt2guqwpftb.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt2qcymjqqn.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2cgayxqxk.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2fxehlebn.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt2chtcyvao.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2obfjubvl.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2vvljacad.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt2zwpqscxq.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt2deubniqz.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2agteikvj.html


<!-- 参考信息 -->