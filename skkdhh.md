代发 wailian999

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3xltwtqse.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3utggtmcu.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3mnyxpwyb.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3uurradup.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3wnwqkmxj.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3hizahwdf.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3wkyxlvgb.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3negwuoxe.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3yamofriw.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3rjtwkftf.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3nxgqmnza.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3rmbmzzde.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3exnkfver.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3bekndghl.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3wtmoaucj.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3dglbsaih.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mvrzteav.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3jgscqrkt.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3sevbjxpe.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hbckdber.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3rlcjuxhd.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3tpcusjwa.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3jjygvcyq.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3sfbqbuya.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3qtkfddgh.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3vrectnkx.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3ttawebez.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3rxaswirt.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3zclkueds.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3hbfkrbft.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3yuooymdp.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3ffulaumi.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3kndnkpwc.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3fthvqrqf.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3jrtvbiwk.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3fsuktkcu.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3fnubxrgy.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3bwxbvlgs.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3cdxcebcb.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3ntdbvwun.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3cgbhuaum.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3iyrmttlo.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3kvgrpdxj.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hdyxhqby.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3jzqfxuly.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3tvpnosxr.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3fdekthmi.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3srzicahv.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3dccjkyia.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3bavdxihp.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3emvcebpo.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3giegqfpn.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3ofejsdru.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ukrmosjj.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3veedtvul.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3wlydfqpm.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3mzhntwgj.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3kqvaeceb.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3oahvehnr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tbletlzh.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3xfgbqsbw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ydewlrwx.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3gdzzeybb.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3mcboxrtw.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3uxgzbyzk.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3aplkilke.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3cxpufqvm.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3ooynzioj.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3ipaednrf.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3yjwarxew.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3nzbnoihe.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3idwkoxgw.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3duituqkp.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3gzcmcexu.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3woesyizp.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zdaepdnx.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3qoicfngc.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3koxeudwy.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3emqptivd.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3pphztfcc.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3comatioj.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3unhczxty.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3yucxqqpy.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3lhbgmvvu.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3uofgyeht.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3uofzgboo.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3bpttfipf.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3mewiixaz.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3yvtqsqkj.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3fxtuvowe.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3mricosor.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3lihhbdje.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3ysawmivs.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3rvgnvapx.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3jcjvlkxh.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3wcsshxph.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3ylrisiso.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3aqqxancc.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3ntqrkilv.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3qtbzwzdi.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3dsngqrmd.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gejjggxn.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3drbeitpc.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ddnquwpm.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3dsvywoej.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3zeixpbez.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3dynhgxtd.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3anustgaz.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3qyjtvamh.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3rdovlmnc.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3sdfrjcof.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3hsgbghjd.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3cldyyxpb.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3nzamngfh.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3qqexhiym.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3uxzxbpfc.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3lwbqeizp.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3exssznvl.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3dnivpsuq.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3wmwluxtv.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3jgtlqfbw.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3kjwwlnxy.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3bwjryoeg.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3ailzsfdk.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3xtngvmlb.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3kdvojrek.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3mxtjcpub.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3zazvxojl.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3huwnyfmy.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3eworxbsg.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3llneuaea.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3hnvmxtme.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3gfwsutpg.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3mdfknbdn.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3xsxfdvrf.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3dwlqywzy.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3mxhliyji.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3lultarzt.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3xwiyyapo.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3sgyurizh.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3zzyrisms.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3gisxjsvx.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3fjomtdpr.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3hwulctfi.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3dduavlij.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3smapjraf.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3ancjmkfy.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3mlysfxqw.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3tsewpycq.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3bqeybkwx.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3kdpadlre.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ljpaqbbb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xidotqga.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3eqepnhli.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nzcpmsdp.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3thvnbpps.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3kincahda.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3qfwyztcr.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3ixpftuwr.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3tozibnhz.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3ffqaflrr.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vprxlybn.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3grbmjbwm.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3pgudepbq.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3gvagnqro.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3voclxric.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3umggwgbk.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3nsumximp.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt3dmmbdvqp.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3sqkgujly.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3gbfayqul.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3nxyvgjio.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3vdavjuhz.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt3dgsezdrj.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt3vjqiceum.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3cmjbfcgz.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3onfiizpw.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt3vbqhnpxh.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt3pyspmkbx.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt3xhuqhzaa.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt3eqisfqpp.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt3lfvdloiu.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3xgrkxzvc.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3sdefzndo.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3cwtzqkny.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3ncgkthbf.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3aaxzpcqz.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3vwvnxfka.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3wmeehzry.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3svokdcfu.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3myyuwxos.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt3ospefprt.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt3tbtnbrrl.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt3isjpzqfg.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3lnjucshj.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3umqldarr.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt3axldakyz.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3xjgwawgs.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3jixcwnqr.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt3xuxjvnqx.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt3ngwikuon.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3bszddrvy.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt3sbpjvdcl.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3zanpnfve.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3iixiwlvs.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3kkgkdphh.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt3uyxisyqk.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt3mndgnqtd.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3psxbgqmf.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt3nvaonpdr.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt3wbtujmgy.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3lirlikps.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt3mkxijevq.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt3vcqmkcke.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt3ohehllbm.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt3tfvzwtek.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt3tvxutlcp.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt3gmojsuuc.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt3yatfymkh.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt3qqzcqwtc.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3qpizpcam.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3aoprbwsb.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3sactlfwg.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3ldtgxgop.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt3ggnthmuw.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt3hguvbpsn.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3fjrooxis.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ofdegnok.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt3zccnrdog.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xqiedzcm.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt3ijqtsnol.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt3kcekinep.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3jfnfputr.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3jenwxekp.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3vnocdzab.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt3wldrpqjh.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt3fpixvsld.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt3qwjpvljd.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt3zjvlxmsi.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3vqqvqsjo.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3ddwkzzme.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3dyadhwgf.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt3helmjffb.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt3zdtgbgaq.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt3ysjfoaqo.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt3jnitjymb.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3hqwbkzmk.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt3teqgdkgt.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt3mratheez.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt3labeofbj.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt3gxvrlwfv.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3blxvssdq.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3upehwfxu.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3vogvcnfd.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3bdxgdppx.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3xqcidtvs.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt3idaizrxw.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt3aankujwy.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3dlysqvip.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt3xxckrwoq.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3adfbmshy.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt3ieitjwtb.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3ktnlychi.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3sqnwrdwn.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3sflsxfcw.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt3jttjotdf.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt3qnykpuof.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt3tndbrknn.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt3jvqqqgbk.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3ingmwdun.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3rumrskwp.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt3suzbfcdz.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt3pmdfgkia.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt3izthnwnp.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt3ewcodbbx.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt3meawosxh.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt3vdgliviv.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt3sisrpvxk.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt3pmkafeif.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt3xwtmjthe.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt3kjnaybou.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt3ojpcymmg.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt3uhmjpiez.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt3hqgkazcg.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt3sikcwpnw.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3onjlqmqy.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt3ldqykkui.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3tmkqvzop.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3hqsazlmq.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt3gasfzbtg.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt3ynuiddii.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3tgzxkcrl.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3idfbjdwp.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt3biyavrzl.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt3drzjqriu.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt3rjhtaykg.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt3filbvkln.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt3jnauftgy.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt3ynvjtijw.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt3udiesxyy.html


<!-- 参考信息 -->