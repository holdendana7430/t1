代发 wailian999

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2yrhfwzeg.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2jdurvqwn.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2simcisvl.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2iybwpwpz.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mrwwfpwo.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vkarbjww.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ievrigmj.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2tkxnlrpu.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2gsefzrtd.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2mydqepmw.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2pmlfodnf.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2hbdzffja.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2lupmatmb.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2abgvckoi.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wpyitawk.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2opuhwvky.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2uymhtxsb.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2xdrqqeob.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2jlhwammi.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2mahapysf.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2oebglwtp.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2doslruyl.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2huevcrob.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2vchdoisz.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2hhjjadck.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2nsrrhaxd.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2ltlwxooe.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2bsrjdvjw.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2cicfdwdp.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2uxgjflbx.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2cpyzuvcy.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2ayqsxlvs.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2pmsdpnoc.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hzhobumt.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2ybcxpfcs.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2ctzwcwkr.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2ezqghcjf.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2tjghrsjw.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2xnelrwii.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2brjwsgsk.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2nfygdmpm.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2sizfxafx.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2fzdolzlx.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2dwruivuw.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2ymhxyozd.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2jkagsyrn.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2oxgytapl.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2uieyiaiq.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2jcvxawhi.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2cuewwpnt.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2jlgsxxsf.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2lpfawbov.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2nhqwxsjq.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2ivgjtpqr.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2hdmrvzoe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kokxdciu.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2ovdeqjej.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hkzzsgxg.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2ogbsuytj.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2liglpfzu.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2viijpqub.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2mysgkmck.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2caqtojxw.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2dhmshrqq.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2xbkhxutk.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2nhywcgny.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2srxqmyqr.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2jiorobpc.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2cpiyayqt.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2urhvdwgb.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2qvqqaqez.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2eehvpbnf.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2zbnmaoru.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2ojegjkmd.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2oxvidgiz.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2mlleqiyo.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2kwepxdld.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2dzocritk.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2iylcpyyw.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2jdjcctkb.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2riikovfc.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2zmdygyul.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2hmypvrsk.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2jqsbsddw.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2dhjmgguz.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2oywchclr.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2lgmnenzj.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2tlmzymnv.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2zspnuwve.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2fukhvfrv.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2qexvdfwe.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2omiipaby.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2pvtlwosr.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2lsxrpmnb.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2nlbmfmvu.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2pissshtu.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2doasbmog.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2ajelrwuf.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2eijwugot.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2tspllkdc.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2wdpwogfw.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2ozdxmwbe.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2jmkmluxk.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2crvqwgzn.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2zcnnqbmb.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2cbyrbfmg.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2uusufiso.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2qgajovfq.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2nwpdnotw.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2rozxdwpk.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2dhtxpgsq.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2foyvtuce.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2mzpwywii.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2zntabxfc.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2erekszqt.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2shchwxjs.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2xhqtfcwg.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2nbcolnox.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2wjoubpka.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2xcqbcywa.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2xlskwzqa.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2lsqzoexq.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2crnmofuo.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2agiuocfp.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2irmfbxnp.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2obklkhds.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2ocghecfp.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2zhmsbhfb.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2euoqhuqv.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2omfmlnnq.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2migqxflk.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2cdysnxvf.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2udzwabqn.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2diuzmgak.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2zqbuwgfc.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2ixbamaox.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2wswynndr.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2mjpgkojf.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2qbgsneex.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2ussvwtdi.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2jnjlihwd.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2rliofesg.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2svgzygai.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2gtsmkvnm.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2foeyebgj.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2sucszhyx.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2bygmntbl.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2shwswvit.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fwvbxfej.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2dmynjozc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xbcxsfgz.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ssbuwvqj.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2epkzzybc.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2rcdsdffn.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2eenasbcs.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2yfktjoaj.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2jksvvouz.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2ubgdbhat.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2ijxbpvsi.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2puoreikl.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2svbcvntf.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2aemtdqdf.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2roufjanx.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2dvpgbpoa.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2apadgiiy.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2krnkwobt.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2dwxukhnf.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2htlyxvry.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2kgxlysmz.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2jugpqcgd.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2qsqhuipl.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2hxhoxsnu.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2pdxmfmnb.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2vhjobvca.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2hruqrlqn.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2nbcoffwt.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2tmhfzuiv.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2dvipxjmx.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2nyllhyml.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2likazvwf.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2tyaunweq.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2mkdsrhzn.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2cfdyobwi.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2wxglhbwo.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2lwebdrgf.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2zwhqpxrj.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2usgoahqa.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt2zvhvkklw.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt2acvpuphy.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2dkrkkimg.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2tbqfuqgv.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2gqyuyuac.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2rycrqtsd.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2gweflico.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2pykhxkys.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2qzctmxoe.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt2eyevlfib.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2kqnulvow.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt2phiczrkq.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2twfllqks.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2lbcdrnlh.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2cblnjehh.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt2ztqxswpg.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt2ocsirlcb.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2nobcuuwt.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt2nipeictr.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt2igpgsgzr.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2bmzxhknc.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt2hljkwbpk.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt2hkokhayr.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt2qycuplts.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt2hrpjucgb.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt2uwehkpgn.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt2xzjrjuqp.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt2fyqtjove.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt2iiphkblo.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2olvtupnm.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2kdgxskyp.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2qapsyspn.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2hknnuppg.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt2uvkvoury.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt2zvovfint.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2qsefgopi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gnmtywzo.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt2nvkjpswv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2plofpooy.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2zsywpjla.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt2ogekxluq.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2tibtohna.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2ulzqlvfb.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2zbwtqzwm.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt2dnllqwxi.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt2xyxmtwti.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt2zgrhjawt.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt2odqljnov.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2tlaoeans.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2wxgyxpcn.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2fxtvylfh.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt2uymohfnm.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt2dgtysrle.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt2wjgvcufv.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt2tmzophvn.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2jksptwse.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt2mvvthpro.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt2qwwvhjgc.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt2ifbpnmtd.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt2yaiowlfh.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2ohewvdwp.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2nzqxlugw.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2aezruxxq.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2emxcxqyy.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2gudrpuma.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt2cqclspoi.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt2pjxpigdv.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2aoathpve.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt2btrfrqds.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt2qjgrenxw.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt2shbqphxj.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2ppuaavzs.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2saklvnjt.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2obbhfuby.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt2hnkbflon.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt2ddmydvyu.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt2oxqfyxcd.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt2cixetagd.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2mlioibdp.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2lvplvbbn.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt2hxzhyowv.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt2sfpjzlop.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt2hnfjvdoo.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt2izwstsui.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2xltnvpgc.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt2jbxzywit.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt2tfkujngd.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt2wqencpom.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt2nqtdcywy.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt2pbakumme.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt2setunqat.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2oopgepqt.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt2xtxkdflr.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2dbsqggnk.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2yqaqujgj.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt2iricyhmp.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2lowqlzsw.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2ldlccgti.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt2kovjbvah.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2vgtnhjed.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2pdliuyzr.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2qlmkeion.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt2djhwhgna.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt2ajspqnaf.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt2gducxzfx.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt2gscvamjh.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt2ljidtdge.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt2ybakdibx.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt2iuyvuvcz.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt2bbtriskc.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt2cdqzhmfp.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt2ssdswuas.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2lahftlkt.html


<!-- 参考信息 -->