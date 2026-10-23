代发 wailian999

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zwaahdgr.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3zlffzjme.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3rknnyugx.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3jiekypwz.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3qhzryzcu.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3rvhhhorg.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3zaglsivc.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3fucjjmqc.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3uixomhvp.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3ulwbrnib.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3iwolblwb.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3zkkkvqqp.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3odxudcrs.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3ofuppjdw.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3ejeuysra.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pwzpipxw.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3qszkqpgy.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bklsekob.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ntalyyhq.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3sgalklkp.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3fucoqcns.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3hadehnby.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3mapgvdnw.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3msxwtqmi.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3gexttbop.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rqhupcjm.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zshzurrm.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mfmidxfu.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3vtffessw.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3elbvalyd.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3oaunrnxz.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3wocinfxa.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3zhyunubt.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3kxgncarz.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3dsxvesis.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3ndwikxxw.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3lvhtesfw.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3hxggynnm.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3caweuyap.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3ypseplsg.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3boouyggy.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3atenhsbl.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3yrfhoved.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3lznqnjmk.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3uebxpzbt.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3sblndwll.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3txfvpekt.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3qgzhopfb.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3bjpycnlb.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3xevcjgxa.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3zuffaisr.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3zfesqugm.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3yfnqakyz.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3oocsqgcy.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3uwpddeyr.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3crhcvbjm.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3nxtsflot.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3wkhjxzvq.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3vzttibho.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3stytezxl.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3cgupwgjh.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3xtxagxnj.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3lodaosbm.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3eftidsgh.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3cqljzpnz.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3tsxzptml.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3livvzqgn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3feblcfkj.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3ooyfypyt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jjyynhrd.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3xevbngda.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3rmueedgh.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3dbcriqcc.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3tcxenpxw.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3siuavgwp.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3dumpvaou.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3xkxwvreo.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3winhuxoy.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3uhqxwhnm.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3vojdwpax.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3xbbdnuxy.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3jiricozb.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3oowywmqn.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3koncnzln.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3btfjoibb.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3itkypixw.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3croudxbt.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3iwutsayg.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3zsoejsyj.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3canbkgks.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3fmynefii.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3guswccxm.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3axfjyfcn.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3vjelwiwc.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3exkniyam.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3bkpqprdp.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3wtfajobi.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3iozfqgzd.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3rjbrsedn.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3sizbkfhq.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3wapocavq.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3abvwhsyy.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3lztcoesu.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3hlaxkenb.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3pzditsfx.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3amjdvglj.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3gsyuksaa.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3fkgbevoj.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3qszspvhd.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3saahchci.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3svmlsrft.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3tirpopnb.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3ewtmzihz.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3ilghvvny.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cemmwnyj.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3ltaczrgg.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3mrwznvfc.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3eaxxmufm.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3eagrwqxc.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3dsgshfwo.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3eahtlnad.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3ajhbskdl.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3rgyolkup.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3aowbuuix.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3xerzbtok.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3gthkgshx.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3ukfforjc.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3emerdicq.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3evzcadmh.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3okrcxwmi.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3xfrrtwcn.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3nbkczpik.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ylfebrvu.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3ornwjcfl.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3vfybktea.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3mjwsvsaz.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3yptmhvsv.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3hogeaiye.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3jqedfjne.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3yxqaljor.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3fejawpxa.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3mfzpppst.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3ichqbwwm.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3duwjkbpx.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3zfdcbhsc.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3zdubgjxw.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3ofublxeu.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3lnfqfocd.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3mmjeefmg.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3txhxmbwo.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3mrawhfoa.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3xbhfshjj.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3krffdooq.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3valcuuqp.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3zmthgsxr.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3zpeinfgx.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3dacvvmxt.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3cdunbzmz.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3kwmrgeyi.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3phmqlhfa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xfpgepdf.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3ahyquhuk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sbmxohox.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3noxevotk.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3nonkxsaj.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3koepetoa.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3rjlkddze.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3ilbiznae.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3nhglgbto.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3lmlgnrjn.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3gwytlwqe.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3mrcucess.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3kglkiznj.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3danoedln.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3wxbmxqvh.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt3txotstto.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt3rbgawwmt.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3pmxicyvl.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3imundamf.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3thuveqzs.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3nfmcqoxz.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt3horxpbbw.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3qrvjhqst.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3zqpvgkkw.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3xspazlwe.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt3tzuldpsh.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt3yaxhluxn.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt3mhtfuhal.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt3krbbqivr.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt3xsoprbqh.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3obckrver.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3puiwotot.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3uluvswqz.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3fgyboxwb.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3hekcwebw.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3odrfgdzb.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt3sxabjzjk.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt3jzjkuzmd.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3kekqrtgn.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt3leksideo.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt3zrlvikma.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3jtvzbvuh.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3qwdyqlgw.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3lfxdtzny.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3fdmzrtvx.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3izdzinxf.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3evsuhuyx.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3htdlsvjd.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt3cexrcqlj.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3haodzhuz.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt3kbisfnzk.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3rykqmgsk.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3rgnjwjhc.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3wvkwixvi.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt3rceaotsm.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt3rjeuiadp.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3uzovuorb.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt3vyosrgeg.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt3zsfvviql.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3lqfpuvrr.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt3zzgaxngq.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt3dxsiyiks.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt3yrojihcw.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt3amvsklhz.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt3yshvgljd.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt3fyaavpgf.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt3oafdmhtn.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt3xkvpmbvu.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3mikcpapd.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3mxjmjpqn.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3vccoqxad.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3gnavxojf.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt3xcokkbgr.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt3lkyauwdb.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3umdndkny.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3exawnebn.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt3eviwhrzc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dwxcevnh.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3idxlmywz.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt3rdigtlfe.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3oavfewak.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3tlbjezme.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3sgzkxbap.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt3hsumjgkp.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt3tgwolbee.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt3gsolgwfy.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt3gtcfffax.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3hoqkgmnt.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3jqjzxpzq.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3gqbvyslt.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt3ditutkay.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt3qbpcttky.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt3dvohtuqy.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt3uiqphfgs.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3gsvlhyln.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt3cqklljit.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt3haabtmkb.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt3cucwyayo.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt3svfiadck.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3ancpffiv.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3mnwrbbce.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3tieourfu.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3nohmyjyr.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3umsbhxsw.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt3swjvwqrq.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt3rvnmogvy.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3bipyofdb.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt3wjdycavv.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt3unlxfdwb.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3gwmwcmpu.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt3csdzdaun.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3mcscpzut.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt3sfnozubs.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3erjypwhr.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt3iowasxmk.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt3vusoztfa.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt3apdmnufe.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3twwjrqkk.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3calinphv.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt3atfnbsay.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt3veftvkwu.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt3oqkxpzll.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt3lfeguefa.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt3lgmgctxv.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt3vgpudtyh.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt3msfowbup.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt3kfzybltk.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt3zvtjpbmn.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt3ybyuiyth.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt3qzhiboyl.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt3kbmcwzro.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt3rtbgyfnk.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt3rmgwvqsb.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3lrqydxgu.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt3lhfkvrse.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3srfhtvmv.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3somcmdlp.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt3zocnyrod.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3lvbneamc.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3pifkjstu.html


<!-- 参考信息 -->