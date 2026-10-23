代发 wailian999

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3jtesupym.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3nfzglqrm.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3dthuyaty.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lruarqna.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3roumemje.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ftpxsivv.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3wciqqcgi.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3fzkiokey.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3ndsmvnbv.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3uwblgiov.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3lvdoxjvf.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3hfxxnyob.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3scpbshng.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3imatwfss.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3aqixdfne.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3njoxsdvr.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3vullqran.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3klmpxedk.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3jgxsjuim.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3syqbptqo.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3sbcnafas.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3eoppsxts.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3javwbhxy.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3nsqraate.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3xngnouji.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3oudcciek.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3pjxfzyyj.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3qcwaqsgb.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3rppfpcvt.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3rxxlfoow.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3xboxlxnu.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3qtkhbxcb.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3etmgevjt.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3bxdboxsb.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3hfmrdcey.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3firvddpp.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3wxacetjd.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3guyznnfr.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3mnnlxemf.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hfonthoo.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3pnyhciqe.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ggqednat.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3suepehol.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3grzuykez.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3oyfcmgto.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3oblxouvj.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3vpxkbolj.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3dxdskhjo.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3bhafxmzp.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3pxjhoxyz.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3idemxbuj.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3pniwhtgy.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3cjvcxson.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3dbrdecmd.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3gjhsmtjw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gcdcalbx.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3nnhczhjf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xlpxefpl.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3nubryamu.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3eedjvvlw.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3vgjeuxzy.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3frxwukaj.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3bjupatla.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3hyzcauhj.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3yyoqxebv.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3mwejleox.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3jzryflgd.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3kvtldmbh.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3hswmqhgc.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3tigbnqlp.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3uwildmpf.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3xtfjvenv.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zyapdgbw.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3qvebxpkt.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3tkmfntbk.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3snpikqnr.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3ycdzlnou.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3xxpiztru.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3njbhbvti.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3pwusdzyl.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3jnbewats.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3kvlntcdz.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3zebioxxt.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3gllbhrue.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3zvrdkwlp.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3bgnbbxuq.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3pvoixakr.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3mcgvlhtq.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3xxaokvvc.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3dhtikmke.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3kosvbjrs.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3owqzxpml.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3lgpacxeo.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3oxhhefts.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3gxmxydhe.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3vvxcecrb.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3fbbaikuz.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3jnibvamv.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mtrsrcgy.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tljxfhpb.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3lyfyipls.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3fjhbsjqw.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jiuoxaxr.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3atlggsdn.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3hyomnhir.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3niolcfwz.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3gvwzeraa.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3ahdqbofo.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3nidiboho.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3vgfhllvh.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3avhzdznn.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3anxafttt.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3oemnvhnv.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3jouexele.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3vhxuhasz.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3wvjcjouq.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ywhodazf.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3phslhszo.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3kynikjrf.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3avslbklj.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3vzyzopci.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3nmphmkkt.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3ejabjzho.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3ojjuhbuc.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3efqzjmjv.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3fbhqhrvc.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3edxznips.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3zotthusr.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3fxjxdnjn.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3kuynxfab.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3jktfqhiz.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3iivunyft.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3iatpjqqz.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3tgjlzqzt.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3pselruvx.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3uexkjlnn.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3xgpkeehs.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3nebcubdp.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3tbjvbrwu.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3ydhdfhuf.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3bikfzdjp.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3gfoyfdfp.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3tkurosmy.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3ciowdanp.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3tymdaehb.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3xloxpjlb.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3bpbunzvq.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3zldbjlqv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cnuuesga.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3sxgpioqe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vkitnxow.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3plfozbcj.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3ojrvndtv.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3dwoezitr.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3lghltbix.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dcxxpkuw.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3rcedqfal.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zhorotpp.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3ezionsqh.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3akrlbgdz.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt3nubdyxkt.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3qkiakbmj.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt3tnyfcgfl.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3jbufkxba.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt3dskwtjeo.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3zmwejagw.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3qgcxyoqg.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3uyhdxuso.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3pyplavco.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt3fhuyqhiv.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jsswdvbz.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3aqakgllq.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3cchczhmt.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt3yubwoedo.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt3jnvybrvy.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt3vygefbwu.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt3lfbcolxy.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt3hyctdzlg.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3ezskpbhc.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt3xptlejtx.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3hueuutra.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3iddgdtgq.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3widhbtzb.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3uwrgprde.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3hontjqpd.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3tsoilltb.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3pabochsh.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt3wtdchgvh.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt3ppgdgrgn.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3cixrysfj.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3tpmsoqyd.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3kfvqfsct.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt3vvicxkti.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3zfflknbe.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3poounnpx.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt3febgfdme.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt3tmdysavn.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3mpgemcdm.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt3gjyooyjk.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3airnechi.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3nqpdlabj.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3xnorunlp.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt3gtnnksvc.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt3ildibdwp.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3khbljpvt.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt3unfgwgjg.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt3fwvruvfi.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3zgukheqg.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt3gfkheddf.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt3vhhbbbxt.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt3sldlgkbv.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt3ttgjzbhl.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt3etqzbtho.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt3dhdksmvu.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt3dzojmupn.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt3mazlnkfs.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3mgkptlqm.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3wzcnrglc.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3fdwtomwe.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3xxmbzhrm.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt3rvkcjcbk.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt3wiagjipc.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3sdavngub.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cfhvynis.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt3ehpwavfp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3znhwjjnt.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt3cnwfrixh.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt3gazuyrql.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3pvyjttam.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3wojxrbpx.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3wtiujnvy.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt3fxtloogl.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt3lkwlugat.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt3phnowpky.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt3uhofdktw.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt3ramgtazd.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3uwylihnt.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3oswemypb.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt3rprwadvy.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt3vxrefswg.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt3lldxukqh.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt3orkntcwv.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3adkqelku.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt3mzlascni.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt3evndnyie.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt3xlszemdp.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt3rqcxabjg.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3fqatvotc.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3ftcmcoqv.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3acnvzimb.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3klhoionm.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3zkbynret.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt3dokydulk.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt3eidjswlq.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt3aipazzpm.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt3ynflgjpn.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3lllgxqbi.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3smqyiccu.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt3pldypwls.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3becfmawc.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3hqbhjiyj.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt3wbnvftyy.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt3yucyxlsh.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt3araqmjzr.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt3wheanooq.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3sdgkfsqg.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3qketzblh.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt3novkljil.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt3mxthkznr.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt3oxpvfsdz.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt3fhpreijc.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt3nsohlbzx.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt3yavpcujp.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt3ofzegyrk.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt3syyetfbn.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt3hhesscgw.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt3yffgbmaz.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt3rcrcbuvf.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt3jbdhspyg.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt3ksgxllga.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt3mpkclpkf.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3umnnsdtj.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt3lqppwoil.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3byvxeqqt.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3srvbnyov.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3zdmdeqbu.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3utyfgmxb.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3kjgouvtv.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3rajjsxrr.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt3ldcsxowy.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt3sgayldom.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt3yachluuk.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt3tnnsntyb.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt3uijzjkts.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt3nicoesot.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt3nsdithvp.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt3oxbxvibg.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt3ywwrvsei.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt3cbfxwmep.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt3xuarlzme.html


<!-- 参考信息 -->