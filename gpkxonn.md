代发 wailian999

[G10] 访问控制
来源：http://3g.hesvh.cn/Article/details/glejfqxus.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.fehbvm.com/Article/details/gkejtxlyg.sHtML

PHP:  public / protected / private
来源：http://m.share.fehbvm.com/Article/details/gajihjlpl.sHtML

JS:   #private 字段；其余公开
来源：http://wap.fehbvm.com/Article/details/gtezesocm.sHtML

TS:   public / protected / private
来源：http://www.m.share.hesvh.cn/Article/details/gfrxemjwv.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.fehbvm.com/Article/details/gqosddvfi.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.hesvh.cn/Article/details/gfelhlppn.sHtML

Ruby: public / protected / private
来源：http://www.share.fehbvm.com/Article/details/gathimcbi.sHtML

C#:   public / protected / private / internal
来源：http://blog.zdbjq.cn/Article/details/gnwortguo.sHtML

[G11] getter / setter
来源：http://www.blog.hesvh.cn/Article/details/gfeaetgcq.sHtML

Py:   @property 与 @x.setter
来源：http://blog.hesvh.cn/Article/details/gvrvgkhli.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.fehbvm.com/Article/details/gqkigkeuj.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.fehbvm.com/Article/details/ggtryijwo.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.zdbjq.cn/Article/details/gnbmjpxnd.sHtML

Java: public String getName() { return name; }
来源：http://wap.zdbjq.cn/Article/details/gxgrpwfsf.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.zdbjq.cn/Article/details/gifmvboiy.sHtML

Ruby: attr_accessor :name
来源：http://wap.zdbjq.cn/Article/details/ggszdljfa.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.hesvh.cn/Article/details/ggtmblgfe.sHtML

[G12] 对象转字符串
来源：http://mobile.zdbjq.cn/Article/details/goenymkrl.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.hesvh.cn/Article/details/gwlrpfozt.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.hesvh.cn/Article/details/gfqjnoifg.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.fehbvm.com/Article/details/ggfduosmn.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.hesvh.cn/Article/details/gohfubpvd.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.hesvh.cn/Article/details/gzxbygzpz.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.zdbjq.cn/Article/details/gpgndyxku.sHtML

Ruby: def to_s; @name; end
来源：http://blog.hesvh.cn/Article/details/gthaourmz.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.fehbvm.com/Article/details/gpliewwzf.sHtML

[G13] 判断对象类型
来源：http://m.share.hesvh.cn/Article/details/gbaakllbz.sHtML

Py:   isinstance(u, User)
来源：http://m.share.fehbvm.com/Article/details/glxlvewwt.sHtML

PHP:  $u instanceof User
来源：http://www.blog.fehbvm.com/Article/details/grymaisuo.sHtML

JS:   u instanceof User
来源：http://baike.fehbvm.com/Article/details/gflgbgkgz.sHtML

TS:   u instanceof User
来源：http://wap.zdbjq.cn/Article/details/ggcrnoicu.sHtML

Java: u instanceof User
来源：http://read.share.zdbjq.cn/Article/details/gfqelmgtv.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.zdbjq.cn/Article/details/gjqdkragh.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.fehbvm.com/Article/details/gkwahmjjz.sHtML

C#:   u is User
来源：http://m.share.hesvh.cn/Article/details/giqonsgjr.sHtML

[G14] 数据类 / record
来源：http://blog.zdbjq.cn/Article/details/gywnzsebu.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://baike.fehbvm.com/Article/details/gaxhpdlas.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.zdbjq.cn/Article/details/gxyuwpmcq.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.hesvh.cn/Article/details/gcolwxtxv.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.hesvh.cn/Article/details/gnykhypis.sHtML

Java: record User(String name, int age) {}
来源：http://read.share.fehbvm.com/Article/details/grwmylzfz.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.zdbjq.cn/Article/details/gxniisqyv.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.hesvh.cn/Article/details/gmesiwyns.sHtML

C#:   record User(string Name, int Age);
来源：http://wap.hesvh.cn/Article/details/ggylhfcig.sHtML

[G15] 枚举
来源：http://blog.fehbvm.com/Article/details/gtvifjkih.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.fehbvm.com/Article/details/gxfdglxmc.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.fehbvm.com/Article/details/gptkagmtn.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.fehbvm.com/Article/details/gdjtezxkb.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.fehbvm.com/Article/details/gieefjdka.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.hesvh.cn/Article/details/girgfhuux.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.zdbjq.cn/Article/details/gzyntfthb.sHtML

Ruby: Color = %i[red green].freeze
来源：http://read.share.hesvh.cn/Article/details/gzgpwtymb.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.zdbjq.cn/Article/details/gnpgrcexz.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.hesvh.cn/Article/details/gaawmiwoa.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.hesvh.cn/Article/details/gubppvvoz.sHtML

PHP:  get_object_vars($obj);
来源：http://blog.hesvh.cn/Article/details/ggtrnqqgd.sHtML

JS:   Object.entries(obj)
来源：http://blog.hesvh.cn/Article/details/gacbvysdr.sHtML

TS:   Object.entries(obj)
来源：http://read.share.fehbvm.com/Article/details/glidmzpdj.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://m.share.zdbjq.cn/Article/details/gudkhtjdj.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://3g.hesvh.cn/Article/details/gxcqimvez.sHtML

Ruby: obj.instance_variables
来源：http://m.share.zdbjq.cn/Article/details/gmqjafypf.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.hesvh.cn/Article/details/gcyukshjs.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gorbvaecz.sHtML

H. 异常与错误处理
来源：http://www.m.share.zdbjq.cn/Article/details/gjtpjkwny.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/grqveqrqz.sHtML

[H01] try / catch 基础
来源：http://www.share.fehbvm.com/Article/details/gipbyyhcw.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.hesvh.cn/Article/details/gcsujabmr.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.hesvh.cn/Article/details/gmdbsodnn.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.hesvh.cn/Article/details/ganaifmxb.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://3g.zdbjq.cn/Article/details/gunfduqox.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.m.share.hesvh.cn/Article/details/gywomukwe.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://read.share.hesvh.cn/Article/details/gnpwcyvrw.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.fehbvm.com/Article/details/gxkmlagjg.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.fehbvm.com/Article/details/guajmasig.sHtML

[H02] finally / ensure 收尾
来源：http://www.m.share.zdbjq.cn/Article/details/ghskxszgt.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.share.fehbvm.com/Article/details/gwxklgcwo.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://mobile.zdbjq.cn/Article/details/gcsvmnbow.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://m.share.hesvh.cn/Article/details/gkhktgesv.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.hesvh.cn/Article/details/giouvcxdo.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.hesvh.cn/Article/details/glxmlqmsg.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.fehbvm.com/Article/details/gjeldsksx.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.blog.zdbjq.cn/Article/details/gxfjxlxba.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/gopkkogkw.sHtML

[H03] 主动抛出异常
来源：http://baike.fehbvm.com/Article/details/gpjzpzqus.sHtML

Py:   raise ValueError("错误信息")
来源：http://read.share.hesvh.cn/Article/details/gqgwjnuup.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.m.share.zdbjq.cn/Article/details/guxgavznx.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.zdbjq.cn/Article/details/gbhyiycci.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.zdbjq.cn/Article/details/gcdfuhlha.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://baike.zdbjq.cn/Article/details/gdhjidjkx.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wap.zdbjq.cn/Article/details/gkjreywoo.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.blog.zdbjq.cn/Article/details/gdspjkoht.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://wap.zdbjq.cn/Article/details/gvcvavxgu.sHtML

[H04] 自定义异常类型
来源：http://blog.hesvh.cn/Article/details/gqxgkuoaw.sHtML

Py:   class MyError(Exception): pass
来源：http://wap.zdbjq.cn/Article/details/gxzdwsial.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://mobile.hesvh.cn/Article/details/gvlssspbu.sHtML

JS:   class MyError extends Error {}
来源：http://www.m.share.fehbvm.com/Article/details/gdlgoaags.sHtML

TS:   class MyError extends Error {}
来源：http://wap.fehbvm.com/Article/details/gqiudwocl.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.fehbvm.com/Article/details/gtwdhxcgf.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.share.zdbjq.cn/Article/details/gozzaohmc.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.hesvh.cn/Article/details/gkdfvaatz.sHtML

C#:   class MyException : Exception {}
来源：http://3g.fehbvm.com/Article/details/gkieydljm.sHtML

[H05] 捕获特定类型
来源：http://www.blog.hesvh.cn/Article/details/geroyrhyo.sHtML

Py:   except ValueError as e:
来源：http://www.m.share.fehbvm.com/Article/details/gxuwbhpsv.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.zdbjq.cn/Article/details/gxfcskiys.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://m.share.zdbjq.cn/Article/details/gfytrcfmc.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://wap.zdbjq.cn/Article/details/gygiskkir.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://wap.hesvh.cn/Article/details/guxqrqhtr.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mobile.fehbvm.com/Article/details/gsvdxqnie.sHtML

Ruby: rescue ArgumentError => e
来源：http://read.share.hesvh.cn/Article/details/gwodblgda.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.share.hesvh.cn/Article/details/gqgngesig.sHtML

[H06] 可选值 / 空值安全访问
来源：http://blog.hesvh.cn/Article/details/gqzbotkhi.sHtML

Py:   value = d.get("k") or default
来源：http://blog.hesvh.cn/Article/details/gbquvbthz.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.blog.zdbjq.cn/Article/details/glywnsrll.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://blog.fehbvm.com/Article/details/gdvabbrym.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://mobile.hesvh.cn/Article/details/gjbcmlswe.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://baike.zdbjq.cn/Article/details/glzbhancm.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://blog.zdbjq.cn/Article/details/gwnqxyhxa.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.blog.zdbjq.cn/Article/details/gwhntowvc.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.share.zdbjq.cn/Article/details/gphjrhhro.sHtML

[H07] 断言
来源：http://baike.fehbvm.com/Article/details/gswjrglle.sHtML

Py:   assert x > 0, "必须为正"
来源：http://3g.hesvh.cn/Article/details/glafaqckk.sHtML

PHP:  assert($x > 0);
来源：http://www.m.share.fehbvm.com/Article/details/gyueuirfw.sHtML

JS:   console.assert(x > 0);
来源：http://blog.hesvh.cn/Article/details/gubixcttj.sHtML

TS:   console.assert(x > 0);
来源：http://blog.fehbvm.com/Article/details/gxrfujlvt.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.share.hesvh.cn/Article/details/glgjhkhxa.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://blog.hesvh.cn/Article/details/ggrauqdgs.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://blog.zdbjq.cn/Article/details/gxerarwol.sHtML

C#:   Debug.Assert(x > 0);
来源：http://read.share.fehbvm.com/Article/details/gxsmshbec.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.share.hesvh.cn/Article/details/gunznnzvg.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://3g.zdbjq.cn/Article/details/ggdpnvkrq.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://baike.zdbjq.cn/Article/details/gbolzsvfv.sHtML

JS:   e.message;  e.stack
来源：http://www.share.hesvh.cn/Article/details/gmqrxshcb.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.m.share.hesvh.cn/Article/details/gqbdkgymz.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://read.share.hesvh.cn/Article/details/gxqnstvxc.sHtML

Go:   err.Error()
来源：http://3g.zdbjq.cn/Article/details/guupzwtrx.sHtML

Ruby: e.message;  e.backtrace
来源：http://baike.fehbvm.com/Article/details/gbczonzmd.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.blog.fehbvm.com/Article/details/gcwnrtzjq.sHtML

[H09] 带错误码的异常
来源：http://m.share.zdbjq.cn/Article/details/gwnlcgari.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.m.share.hesvh.cn/Article/details/gqaokocaw.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://wap.fehbvm.com/Article/details/gxmyycvke.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wap.fehbvm.com/Article/details/gbvcblzij.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://3g.hesvh.cn/Article/details/gplrsjhgw.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://m.share.hesvh.cn/Article/details/guvdlatcr.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.m.share.zdbjq.cn/Article/details/gczzwqcvv.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://read.share.fehbvm.com/Article/details/gbfmarqdc.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://wap.hesvh.cn/Article/details/gmmcirchf.sHtML

[H10] 资源自动释放
来源：http://3g.zdbjq.cn/Article/details/gtlpxiyzb.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://m.share.hesvh.cn/Article/details/gcknphtut.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://baike.fehbvm.com/Article/details/gsyjsiezm.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.hesvh.cn/Article/details/gtnwaelco.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.zdbjq.cn/Article/details/guujfefdc.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://m.share.zdbjq.cn/Article/details/gtzshlreg.sHtML

Go:   defer f.Close()
来源：http://read.share.hesvh.cn/Article/details/gblletwle.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.share.hesvh.cn/Article/details/gjktbfcyy.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://m.share.hesvh.cn/Article/details/godrgcpls.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/guhvgqnlo.sHtML

I. 正则表达式
来源：http://blog.hesvh.cn/Article/details/gnfsqoegr.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gavwujpbj.sHtML

[I01] 判断是否匹配
来源：http://mobile.fehbvm.com/Article/details/grvcuuiil.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.m.share.hesvh.cn/Article/details/ggilwyooo.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.blog.hesvh.cn/Article/details/gaayqayea.sHtML

JS:   /\d+/.test(s)
来源：http://wap.fehbvm.com/Article/details/gecotfzdp.sHtML

TS:   /\d+/.test(s)
来源：http://read.share.fehbvm.com/Article/details/gtxnoxfmp.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.share.zdbjq.cn/Article/details/gjelhyojf.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.share.zdbjq.cn/Article/details/glahkkmfl.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.blog.fehbvm.com/Article/details/grnygunxj.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.m.share.hesvh.cn/Article/details/gfwlkyxze.sHtML

[I02] 提取所有匹配
来源：http://blog.hesvh.cn/Article/details/grhujwsip.sHtML

Py:   re.findall(r"\d+", s)
来源：http://blog.fehbvm.com/Article/details/gimxntpcs.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://blog.hesvh.cn/Article/details/gmyrvjgac.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.share.fehbvm.com/Article/details/gsfnhpojx.sHtML

TS:   s.match(/\d+/g)
来源：http://wap.fehbvm.com/Article/details/gxchmbdyo.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gpkimxzwi.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.m.share.fehbvm.com/Article/details/gbdhjtcal.sHtML

Ruby: s.scan(/\d+/)
来源：http://read.share.fehbvm.com/Article/details/glffmdbyp.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://read.share.fehbvm.com/Article/details/gvhchyhab.sHtML

[I03] 提取捕获分组
来源：http://read.share.zdbjq.cn/Article/details/gyfllsbps.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.m.share.hesvh.cn/Article/details/grrdlwwgi.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.blog.hesvh.cn/Article/details/gbqtyelss.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mobile.fehbvm.com/Article/details/guzidsutr.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.m.share.fehbvm.com/Article/details/gritchbzq.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://blog.zdbjq.cn/Article/details/ggldpywvd.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wap.fehbvm.com/Article/details/gctmclgwg.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.m.share.zdbjq.cn/Article/details/gikczkfmu.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://m.share.hesvh.cn/Article/details/gpifiejhe.sHtML

[I04] 正则替换
来源：http://3g.hesvh.cn/Article/details/gfiyzeqzn.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.share.hesvh.cn/Article/details/gcuihgknw.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://m.share.zdbjq.cn/Article/details/glqrkmrxd.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://3g.hesvh.cn/Article/details/gtuqrayve.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://baike.hesvh.cn/Article/details/gmnaxaomq.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.m.share.hesvh.cn/Article/details/ggnxhfsfq.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://m.share.zdbjq.cn/Article/details/gyzpbizsv.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://baike.zdbjq.cn/Article/details/geqtiwucw.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://3g.zdbjq.cn/Article/details/ganjgloxg.sHtML

[I05] 按正则拆分
来源：http://www.m.share.zdbjq.cn/Article/details/gejskfubf.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.blog.hesvh.cn/Article/details/gmuvrkanl.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://3g.zdbjq.cn/Article/details/gvrtdgaot.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://3g.fehbvm.com/Article/details/glihmwhrl.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://wap.fehbvm.com/Article/details/giryqqcog.sHtML

Java: s.split("\\s*,\\s*")
来源：http://wap.hesvh.cn/Article/details/glfkznflx.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://blog.zdbjq.cn/Article/details/gammddpxy.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://read.share.zdbjq.cn/Article/details/gawxtsgcd.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://read.share.zdbjq.cn/Article/details/gcjkgvqmz.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://3g.fehbvm.com/Article/details/gwsugmcjc.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://mobile.zdbjq.cn/Article/details/gbsmecutp.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://mobile.hesvh.cn/Article/details/gtpxxkyst.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.zdbjq.cn/Article/details/gamsdupce.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.zdbjq.cn/Article/details/gtxwquwir.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mobile.fehbvm.com/Article/details/gyvnobsax.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.share.fehbvm.com/Article/details/ghpbvosqq.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.m.share.zdbjq.cn/Article/details/gewilrnee.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://3g.fehbvm.com/Article/details/gqodpzcsn.sHtML

[I07] 忽略大小写与多行模式
来源：http://wap.zdbjq.cn/Article/details/gefldlkhx.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://blog.zdbjq.cn/Article/details/gvsbxloto.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.share.hesvh.cn/Article/details/gswdgvqil.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://read.share.hesvh.cn/Article/details/grdrkkfzc.sHtML

TS:   /error/gim
来源：http://www.blog.zdbjq.cn/Article/details/gnrckogzn.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mobile.hesvh.cn/Article/details/gwdfedtnw.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.blog.fehbvm.com/Article/details/gbshnmanv.sHtML

Ruby: s.scan(/error/i)
来源：http://3g.zdbjq.cn/Article/details/giczrqsun.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.m.share.fehbvm.com/Article/details/gjkbmqzvw.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://baike.fehbvm.com/Article/details/gvxhylftx.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.blog.fehbvm.com/Article/details/gdszylxsn.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wap.fehbvm.com/Article/details/gzhifmiqa.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.hesvh.cn/Article/details/ghnwgrffu.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.hesvh.cn/Article/details/goezwvojr.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://wap.hesvh.cn/Article/details/gmmjxungm.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.share.hesvh.cn/Article/details/gnuzmpdim.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wap.zdbjq.cn/Article/details/gggrqqsik.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://blog.zdbjq.cn/Article/details/gjfzjjlbo.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gnrsyuoul.sHtML

J. 日期与时间
来源：http://blog.hesvh.cn/Article/details/gyxunlzct.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gpuxcmayc.sHtML

[J01] 获取当前时间
来源：http://blog.zdbjq.cn/Article/details/gylmxfdih.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://blog.zdbjq.cn/Article/details/gyiuzlbtm.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.m.share.zdbjq.cn/Article/details/gjifnaajo.sHtML

JS:   new Date();  Date.now()
来源：http://wap.zdbjq.cn/Article/details/gorerrccz.sHtML

TS:   new Date();  Date.now()
来源：http://blog.fehbvm.com/Article/details/gyplkrsxw.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://m.share.hesvh.cn/Article/details/gbvpevsiy.sHtML

Go:   time.Now()
来源：http://baike.zdbjq.cn/Article/details/gqykrhxby.sHtML

Ruby: Time.now
来源：http://www.share.zdbjq.cn/Article/details/gccnmujjx.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.m.share.hesvh.cn/Article/details/gvixmshxh.sHtML

[J02] 格式化输出
来源：http://read.share.fehbvm.com/Article/details/gexcpokor.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.hesvh.cn/Article/details/grmbwilfd.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wap.zdbjq.cn/Article/details/gtkrybqth.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://m.share.fehbvm.com/Article/details/gxzjevnoe.sHtML

TS:   d.toISOString()
来源：http://www.blog.zdbjq.cn/Article/details/gdmuljmwp.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://m.share.hesvh.cn/Article/details/gawbvqzak.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.share.fehbvm.com/Article/details/gnqqpoxfv.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.zdbjq.cn/Article/details/gqljstdhi.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://mobile.zdbjq.cn/Article/details/goxibaetk.sHtML

[J03] 字符串解析为日期
来源：http://www.m.share.fehbvm.com/Article/details/gcywbqrof.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://blog.zdbjq.cn/Article/details/gasetlvlm.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://baike.fehbvm.com/Article/details/ghnkpipvy.sHtML

JS:   new Date("2024-01-02")
来源：http://blog.hesvh.cn/Article/details/gnkebcsuh.sHtML

TS:   new Date("2024-01-02")
来源：http://baike.fehbvm.com/Article/details/gaegzjcob.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.m.share.fehbvm.com/Article/details/gztubhugp.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wap.hesvh.cn/Article/details/gaeuobkoj.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://m.share.fehbvm.com/Article/details/geyvphlqh.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wap.hesvh.cn/Article/details/gogzvqbmh.sHtML

[J04] 时间戳与日期互转
来源：http://mobile.hesvh.cn/Article/details/gbgubbmdo.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.m.share.hesvh.cn/Article/details/ginfhobcx.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://3g.zdbjq.cn/Article/details/gvdwxoaxf.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://3g.fehbvm.com/Article/details/gpcsqwvey.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://read.share.hesvh.cn/Article/details/ggfihzcsg.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://wap.zdbjq.cn/Article/details/gcdcumqro.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gwzkxbbob.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://baike.fehbvm.com/Article/details/gzjwjxpqq.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.m.share.zdbjq.cn/Article/details/gczzrxzil.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.m.share.fehbvm.com/Article/details/gqquyuvlp.sHtML

Py:   now + timedelta(days=7)
来源：http://mobile.zdbjq.cn/Article/details/gcrukpwjj.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://3g.fehbvm.com/Article/details/gazuwvrbp.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.zdbjq.cn/Article/details/gjcrrqubl.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.zdbjq.cn/Article/details/gcdazeijq.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://m.share.hesvh.cn/Article/details/gvjqkbtwa.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://baike.hesvh.cn/Article/details/gfumkzyua.sHtML

Ruby: Time.now + 7 * 86400
来源：http://baike.hesvh.cn/Article/details/grtnnqudc.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://mobile.hesvh.cn/Article/details/gxjcundrd.sHtML

[J06] 计算两时间之差
来源：http://wap.fehbvm.com/Article/details/grlcbplbp.sHtML

Py:   (end - start).total_seconds()
来源：http://blog.zdbjq.cn/Article/details/glkcksvij.sHtML

PHP:  $end->diff($start)->days;
来源：http://baike.fehbvm.com/Article/details/gisklhqti.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://3g.zdbjq.cn/Article/details/gjzuwnidi.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://blog.hesvh.cn/Article/details/gtihabyvs.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://wap.zdbjq.cn/Article/details/gsenmvzxj.sHtML

Go:   end.Sub(start).Hours()
来源：http://read.share.fehbvm.com/Article/details/gxvsshqyd.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.share.zdbjq.cn/Article/details/gvbdhqlkp.sHtML

C#:   (end - start).TotalSeconds
来源：http://mobile.hesvh.cn/Article/details/gkutekbtb.sHtML

[J07] 比较两个日期
来源：http://wap.hesvh.cn/Article/details/ghpvjilhd.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.share.zdbjq.cn/Article/details/gibjfacnn.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.blog.hesvh.cn/Article/details/gemwejnuy.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://3g.fehbvm.com/Article/details/guqyhlepl.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://3g.zdbjq.cn/Article/details/ggjwzzuna.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mobile.zdbjq.cn/Article/details/gwalaavgc.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wap.zdbjq.cn/Article/details/goeclpxtj.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.share.hesvh.cn/Article/details/glbdmjcir.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://blog.hesvh.cn/Article/details/gzkizdayv.sHtML

[J08] 提取年月日与星期
来源：http://www.blog.hesvh.cn/Article/details/gimbexolj.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wap.fehbvm.com/Article/details/gtctivfvr.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://3g.zdbjq.cn/Article/details/gtoqhlkyn.sHtML


<!-- 参考信息 -->