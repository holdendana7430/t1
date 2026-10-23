代发 wailian999

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3qpnqquff.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3pqwhoxkj.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3zrtdande.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3xlqdvhrp.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3japjpxov.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3fpqmbksb.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3clbcpqeo.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lldcryqf.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zjvjzenc.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jqeazkmi.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3kstdwhdg.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3gtqurtgc.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3eydaptfw.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3elfltdla.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3ajmvejqa.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3nupdxtnz.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wzxjdhqv.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jpluzyfv.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qchjowto.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wopkopfl.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3ehqbqhbn.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3kwixnvwh.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3sexqgcrh.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3oleoenms.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3dmsiqmdc.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3wfbkrvzh.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3lgaddryv.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3rrtgbemt.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3ututwfgw.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3qzwtvjwc.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3kqbgrejn.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3sraqjxmg.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3egatbdph.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3zlsdhpty.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3cqukycxf.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3rnkvisie.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3sfnlvpwc.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3ykddabrg.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3ztvfrvuc.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3ahclwxjd.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3syqdnjcl.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3hsbkbrgp.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3lrzfainm.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3wshtoxqh.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3maevoykm.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3xqgbcoxu.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3tofndxkz.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3umgheezz.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3hgavmkib.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3uyvisizt.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3pzmorxto.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3qbhxughv.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3etxiunxw.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3punoztjl.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3qlzhsdkq.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3qhkvbskr.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3kpxkngfk.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3aotdqnab.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3fisakfpz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3exnomkcl.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3apdfoait.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3szpgkzzz.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3fjaomwqb.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3rxkjzqnv.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3thknwcpb.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3drbfsazh.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3tzryguuu.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3vhwkfpxj.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3xwkghhqa.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3riqrnjdd.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3djqcjpvg.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3xsxnlzkf.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3tltzrqpc.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3vxvyweaj.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3lflvgmgv.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3xjlgsteo.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3bhenehab.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3xioqugkn.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3ffvnzvjd.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3rqiketdl.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3vutqpeiw.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3gytfdcgz.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3epxocdeh.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3vaittafp.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3frxxypek.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3ofdrpefk.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3lbooyvwa.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3jmpiwzuu.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3keewwlwc.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3dvdgyvug.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3zchziibs.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3vpdghtkl.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3sctjetjx.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3hmbmqahf.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3nzxnkeov.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3rokxdems.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3tswdocqx.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3xlkhnuok.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3ukcwivmc.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3bqolhxye.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3ilunebbv.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3aabyqvuj.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3obxbhiww.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rcdadgzu.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3pnyzzprr.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3gymywhow.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3jvwqjury.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3jvraetjy.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3zgwlooxf.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3banqhejf.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3tqwzavih.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3aikrfpit.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3gaefkzdu.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3hernqexy.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3qdnenpsh.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3icllfqop.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3bdwrdcos.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3fxgosglp.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3rymwdgjo.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3bydeflew.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3xqfkwddu.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3xnkztrup.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3xbssnnmb.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3eufdmsde.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3pnqfpypx.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3nfrzrfsr.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3xlgxwzcg.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3adjitvqz.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3kvzaskzq.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3giojhbel.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3cfcuvwzj.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3dyhqneos.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3elgcllhv.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3njamntbd.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3hhbxaatl.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3cdbmfuge.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3vnqqnokf.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3mzuottfz.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3kcvvnvfb.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3xfwkasjb.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3nqefvcbl.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3nivwovjz.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3lncaxfrg.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3invvxysx.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3nbylkkjp.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3qtjlrikh.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3hypwussg.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3kgnqcmnz.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3szzknwtf.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3xfrzxfio.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3vytcmedm.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3sztlohfj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dogbrujf.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3dfesrglb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gaxxises.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3cwoxbepz.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3ofvmzaml.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3blthmqtv.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3tfzhcvge.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3lgerviad.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3zvlklkew.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3bxhuvkvf.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3ubxttkot.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3xzhzgzud.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3gnxzkahl.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3bmeayhyw.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt3wbctpvjg.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt3djnqysgo.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt3flowrwcd.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt3wseqwjgv.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3hnaclgxq.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3aqixlfhy.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3zlwczamc.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3miiorxnx.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3vjthehie.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3gfenwqqp.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3ncdooudp.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt3mjrgsoyn.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3ttzhmvtz.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt3jucdgbui.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt3xbljxcre.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt3hzlwxadu.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3cahqjfyb.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3hpdwlhyx.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3uwkzdwvx.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3ucicrcma.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3vvlqdzec.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3gapbgvym.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3udosdhtj.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt3kuynjroe.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3rlefxpes.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt3sjuoahyw.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt3qnimpzlf.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt3jfcmkauf.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3vlusmwkh.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3cugnkgte.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3quwqrnwj.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3zmixtxct.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3ylumkpdh.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3qusntfoh.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt3hykwpqxt.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3pelvnbnk.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt3lizawvjj.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3tjcdxgcb.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3apuheebs.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3qsoqzgig.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt3jyeucoeu.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt3kevdbajd.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3qsveejhm.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt3rwwykpro.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt3ronvjpax.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3gsglrcct.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt3qwccsuep.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt3ykbcuitc.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt3oynaunln.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt3ogtzlnii.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt3yqqywkem.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt3vpvlkybr.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt3kqscleac.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt3ehtvwgyt.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3khhlxvux.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3vlglundl.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3kolxdevf.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3tayvskjv.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt3cwegomwb.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt3tkzrsksp.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3qmxfudml.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ymsyunph.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt3qepykanj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3oqjrpdnj.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3ykzazzeg.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt3qoxftvno.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3kpykzcql.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3szmcetmc.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3jqctfydd.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt3hgqblkrj.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt3yngfwrzf.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt3dqhwvvol.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt3unhcttnt.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt3gthrxvac.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3dkjdffmk.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3vmnixkuv.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt3qmtqppra.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt3cemywqxa.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt3lqgxmlbs.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt3eovisqwb.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3dweraurr.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt3qlkrsotj.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt3nsntfaje.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt3myqfocip.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt3zqplabcw.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3gfgmniin.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3xzxnxvri.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3cetigczt.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3kpirhaha.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3rfesnevt.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt3nrbkcadn.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt3gxfnrayk.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3iwojhymp.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt3ewhzzuff.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3foylhfiz.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt3ppwfjnxy.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt3mlezgcta.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3pgtexeen.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3btgxvtfr.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3nsklybcs.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt3yvnqkhhl.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt3fdclwmon.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt3tsyqydtp.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3qzytfmaw.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3sdjtqfwg.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3taztcctp.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt3agrepibf.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt3hbsawelw.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt3gnpqeide.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt3bdoexsej.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt3qpxumpbd.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt3pvekoydi.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt3neoywklj.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt3kenppkqf.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt3dojdktwg.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt3gsrlzbgc.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt3xstzvquw.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt3honssqqg.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt3wqyqizoh.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3zzsaekgm.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt3xyfulaft.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3ypesbbnn.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3azozhvha.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3uqkhqeqv.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3orosolse.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3tymxhzfn.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3peuvgpcf.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt3ynchuwnd.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt3lrwsccpx.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt3cfatpiha.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt3vwxuqfky.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt3smcefmnx.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt3fhqqomyj.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt3voyqlcdm.html


<!-- 参考信息 -->