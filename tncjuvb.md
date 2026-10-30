代发 wailian999

JS:   get name() { return this._name; }
来源：http://m.share.hesvh.cn/Article/details/gwhasmyoc.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.fehbvm.com/Article/details/gtmdupdcd.sHtML

Java: public String getName() { return name; }
来源：http://blog.fehbvm.com/Article/details/griofrzcn.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.zdbjq.cn/Article/details/gvvxbnmlk.sHtML

Ruby: attr_accessor :name
来源：http://3g.fehbvm.com/Article/details/guxdjbtxb.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.fehbvm.com/Article/details/ghdlowdcl.sHtML

[G12] 对象转字符串
来源：http://m.share.hesvh.cn/Article/details/gtopkxqom.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.hesvh.cn/Article/details/gfwpgncnw.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.zdbjq.cn/Article/details/grrnjaepg.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/gvuvtkald.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.fehbvm.com/Article/details/gdpcupzsw.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gpisjkgcx.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.fehbvm.com/Article/details/gsbfiiiut.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.fehbvm.com/Article/details/guchwggda.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.zdbjq.cn/Article/details/guspcyozk.sHtML

[G13] 判断对象类型
来源：http://blog.hesvh.cn/Article/details/gjfigmssf.sHtML

Py:   isinstance(u, User)
来源：http://www.share.fehbvm.com/Article/details/gacrtdhsv.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.fehbvm.com/Article/details/gpuczgxxg.sHtML

JS:   u instanceof User
来源：http://m.share.zdbjq.cn/Article/details/gokxvrltm.sHtML

TS:   u instanceof User
来源：http://www.blog.zdbjq.cn/Article/details/gssloxjat.sHtML

Java: u instanceof User
来源：http://wap.zdbjq.cn/Article/details/gujrngnxn.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.share.fehbvm.com/Article/details/gyrrcjgjk.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.fehbvm.com/Article/details/gzjwbwoki.sHtML

C#:   u is User
来源：http://blog.hesvh.cn/Article/details/grlgutldx.sHtML

[G14] 数据类 / record
来源：http://wap.zdbjq.cn/Article/details/gadjtfkbr.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.fehbvm.com/Article/details/ghbwzjiui.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.hesvh.cn/Article/details/gdtyfgils.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.hesvh.cn/Article/details/gzxrwqyrx.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.zdbjq.cn/Article/details/gcriuftmy.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.zdbjq.cn/Article/details/grejprbas.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.fehbvm.com/Article/details/gntnzwgrb.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.fehbvm.com/Article/details/gruatlkeg.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.zdbjq.cn/Article/details/glrgskfxe.sHtML

[G15] 枚举
来源：http://blog.fehbvm.com/Article/details/gwxlkaqgh.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.fehbvm.com/Article/details/gfmmyvnra.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.fehbvm.com/Article/details/ganofkusz.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.fehbvm.com/Article/details/gmrndnlzl.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.fehbvm.com/Article/details/gmiazhvqm.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.zdbjq.cn/Article/details/gmbhwepml.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.zdbjq.cn/Article/details/gqzctfnwp.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.hesvh.cn/Article/details/gtsksbinv.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.fehbvm.com/Article/details/gcxtysexr.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.hesvh.cn/Article/details/gfbysrpci.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.fehbvm.com/Article/details/gseijmjou.sHtML

PHP:  get_object_vars($obj);
来源：http://3g.hesvh.cn/Article/details/gmdfjqden.sHtML

JS:   Object.entries(obj)
来源：http://www.share.zdbjq.cn/Article/details/ghbeoccga.sHtML

TS:   Object.entries(obj)
来源：http://wap.hesvh.cn/Article/details/gnwatnqqm.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.hesvh.cn/Article/details/gzqzecleo.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.fehbvm.com/Article/details/gvczvpequ.sHtML

Ruby: obj.instance_variables
来源：http://m.share.fehbvm.com/Article/details/geoaxjpij.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.blog.fehbvm.com/Article/details/glhskqfoa.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/guvqfjkbd.sHtML

H. 异常与错误处理
来源：http://mobile.zdbjq.cn/Article/details/gcfxoolar.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gnvnchbwn.sHtML

[H01] try / catch 基础
来源：http://wap.fehbvm.com/Article/details/gicwnugyj.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.fehbvm.com/Article/details/gzjizbyug.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.fehbvm.com/Article/details/gsynwvitz.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://m.share.fehbvm.com/Article/details/gnucoazqf.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.zdbjq.cn/Article/details/ggtyhsnte.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.fehbvm.com/Article/details/gggnaddvk.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.fehbvm.com/Article/details/gstleqkbu.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.fehbvm.com/Article/details/gjxudyxua.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mobile.hesvh.cn/Article/details/gyesswzhr.sHtML

[H02] finally / ensure 收尾
来源：http://wap.fehbvm.com/Article/details/gmkqgaknm.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.share.hesvh.cn/Article/details/gkpelepwd.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.share.hesvh.cn/Article/details/gmagjrxey.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.zdbjq.cn/Article/details/gvezqbbtp.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://m.share.fehbvm.com/Article/details/gipaimsst.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.m.share.hesvh.cn/Article/details/gsgazyvii.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.share.hesvh.cn/Article/details/gzlsxbubf.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://3g.hesvh.cn/Article/details/gmbeygnii.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.blog.hesvh.cn/Article/details/gxkxftypj.sHtML

[H03] 主动抛出异常
来源：http://www.share.fehbvm.com/Article/details/ghyyafulb.sHtML

Py:   raise ValueError("错误信息")
来源：http://wap.fehbvm.com/Article/details/gwwcssjjd.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blog.fehbvm.com/Article/details/grjedyhwp.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.zdbjq.cn/Article/details/gedowiskp.sHtML

TS:   throw new Error("错误信息");
来源：http://www.m.share.fehbvm.com/Article/details/glsnpryfy.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.blog.fehbvm.com/Article/details/gzxmjxufj.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.m.share.fehbvm.com/Article/details/gtwnlpwev.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://baike.fehbvm.com/Article/details/gbtyfnfwo.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.hesvh.cn/Article/details/grgkbgvvs.sHtML

[H04] 自定义异常类型
来源：http://mobile.fehbvm.com/Article/details/gpdxiebya.sHtML

Py:   class MyError(Exception): pass
来源：http://www.m.share.fehbvm.com/Article/details/gpezqhvti.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://wap.fehbvm.com/Article/details/gcrkxxkri.sHtML

JS:   class MyError extends Error {}
来源：http://www.m.share.zdbjq.cn/Article/details/ggyhqwnec.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.hesvh.cn/Article/details/gbvbapvlj.sHtML

Java: class MyException extends RuntimeException {}
来源：http://m.share.zdbjq.cn/Article/details/gkwdmdzqq.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://baike.hesvh.cn/Article/details/gcbnajuif.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.zdbjq.cn/Article/details/gwarzkiix.sHtML

C#:   class MyException : Exception {}
来源：http://m.share.fehbvm.com/Article/details/gwnelmtsk.sHtML

[H05] 捕获特定类型
来源：http://blog.zdbjq.cn/Article/details/geainefqf.sHtML

Py:   except ValueError as e:
来源：http://baike.hesvh.cn/Article/details/gvfeixapa.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.blog.hesvh.cn/Article/details/gkiqrafmv.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://m.share.fehbvm.com/Article/details/gufdmehad.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://blog.fehbvm.com/Article/details/gnxyribmo.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.blog.hesvh.cn/Article/details/givxtkgep.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wap.fehbvm.com/Article/details/gaoqfuyie.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.share.zdbjq.cn/Article/details/gvnbpxcsu.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mobile.hesvh.cn/Article/details/gugrwiytr.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.share.fehbvm.com/Article/details/gbwnxlegl.sHtML

Py:   value = d.get("k") or default
来源：http://blog.zdbjq.cn/Article/details/goaazjuvs.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://3g.fehbvm.com/Article/details/gvrhcptkk.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://wap.hesvh.cn/Article/details/gyszbyzch.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://3g.fehbvm.com/Article/details/gkmcrwemo.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wap.fehbvm.com/Article/details/glawovsrl.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://read.share.fehbvm.com/Article/details/glyqhlgwo.sHtML

Ruby: d&.dig(:a, :b)
来源：http://3g.zdbjq.cn/Article/details/gjuweynxm.sHtML

C#:   obj?.A?.B ?? default
来源：http://mobile.hesvh.cn/Article/details/gzjjvqltp.sHtML

[H07] 断言
来源：http://mobile.fehbvm.com/Article/details/ghlftsfur.sHtML

Py:   assert x > 0, "必须为正"
来源：http://read.share.fehbvm.com/Article/details/guehjssgc.sHtML

PHP:  assert($x > 0);
来源：http://mobile.zdbjq.cn/Article/details/giiscbgpz.sHtML

JS:   console.assert(x > 0);
来源：http://mobile.hesvh.cn/Article/details/gdggtpfdo.sHtML

TS:   console.assert(x > 0);
来源：http://m.share.hesvh.cn/Article/details/gddbexytm.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.fehbvm.com/Article/details/gugqhwxjg.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.m.share.hesvh.cn/Article/details/gfufhbhpi.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://wap.hesvh.cn/Article/details/gwshuhfbl.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.share.fehbvm.com/Article/details/gzjchekep.sHtML

[H08] 获取错误信息与堆栈
来源：http://baike.fehbvm.com/Article/details/gapzeetlk.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://3g.hesvh.cn/Article/details/ggymxicic.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://blog.zdbjq.cn/Article/details/gsrymeuos.sHtML

JS:   e.message;  e.stack
来源：http://blog.fehbvm.com/Article/details/gqvvdukkh.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://blog.fehbvm.com/Article/details/gnlphhrgu.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://blog.hesvh.cn/Article/details/gszjqcago.sHtML

Go:   err.Error()
来源：http://www.share.fehbvm.com/Article/details/geovirkti.sHtML

Ruby: e.message;  e.backtrace
来源：http://mobile.fehbvm.com/Article/details/gfukhwqvi.sHtML

C#:   e.Message;  e.StackTrace
来源：http://mobile.hesvh.cn/Article/details/gnkclqtfk.sHtML

[H09] 带错误码的异常
来源：http://mobile.zdbjq.cn/Article/details/gftcukpxn.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.m.share.zdbjq.cn/Article/details/gkjyjwhok.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://read.share.fehbvm.com/Article/details/gpszpkucj.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://read.share.fehbvm.com/Article/details/grwbwncve.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://read.share.zdbjq.cn/Article/details/goqzqsfem.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://3g.zdbjq.cn/Article/details/gjkunxgqh.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.blog.fehbvm.com/Article/details/gesmvslkg.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://blog.zdbjq.cn/Article/details/gnqgqhiuq.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.m.share.fehbvm.com/Article/details/gugumykiu.sHtML

[H10] 资源自动释放
来源：http://www.blog.hesvh.cn/Article/details/gqizbcsqs.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.blog.fehbvm.com/Article/details/gydxmkpab.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.blog.hesvh.cn/Article/details/ghaasuzns.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.zdbjq.cn/Article/details/gywducyay.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.hesvh.cn/Article/details/gwlhqpzyz.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mobile.zdbjq.cn/Article/details/gzjhikpbo.sHtML

Go:   defer f.Close()
来源：http://www.m.share.zdbjq.cn/Article/details/guubcbcab.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://m.share.fehbvm.com/Article/details/ggoflgpuq.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://baike.fehbvm.com/Article/details/gwqthrkga.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/grixrkkvw.sHtML

I. 正则表达式
来源：http://baike.fehbvm.com/Article/details/gupjylwwn.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gihkdzbwf.sHtML

[I01] 判断是否匹配
来源：http://wap.hesvh.cn/Article/details/gkeufutxa.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.share.fehbvm.com/Article/details/gdmuddswl.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://baike.fehbvm.com/Article/details/gihuwieux.sHtML

JS:   /\d+/.test(s)
来源：http://mobile.hesvh.cn/Article/details/gexfrtctc.sHtML

TS:   /\d+/.test(s)
来源：http://m.share.fehbvm.com/Article/details/gvkstonyp.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://3g.hesvh.cn/Article/details/gelqsvxmg.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://m.share.fehbvm.com/Article/details/ggjyhxmyj.sHtML

Ruby: s.match?(/\d+/)
来源：http://mobile.zdbjq.cn/Article/details/gttnwfutz.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.share.fehbvm.com/Article/details/gbgbmfrti.sHtML

[I02] 提取所有匹配
来源：http://www.blog.fehbvm.com/Article/details/gacplkjnd.sHtML

Py:   re.findall(r"\d+", s)
来源：http://3g.zdbjq.cn/Article/details/golowivcp.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://baike.fehbvm.com/Article/details/gqpsjaesv.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.blog.zdbjq.cn/Article/details/gyplrcdiu.sHtML

TS:   s.match(/\d+/g)
来源：http://www.m.share.hesvh.cn/Article/details/gmmkviocr.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://baike.zdbjq.cn/Article/details/gytqhjfdz.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.share.fehbvm.com/Article/details/ghfwbuekw.sHtML

Ruby: s.scan(/\d+/)
来源：http://mobile.hesvh.cn/Article/details/gmikmkubm.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.share.zdbjq.cn/Article/details/gwtkfcnlf.sHtML

[I03] 提取捕获分组
来源：http://baike.fehbvm.com/Article/details/ghxacxgwd.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mobile.fehbvm.com/Article/details/gssxwwdmh.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://m.share.hesvh.cn/Article/details/gpsugyakg.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wap.fehbvm.com/Article/details/gbeeucckj.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://3g.hesvh.cn/Article/details/gjaqvcknf.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.share.hesvh.cn/Article/details/gtudtufuf.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://read.share.fehbvm.com/Article/details/gtneltzse.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://blog.hesvh.cn/Article/details/gkofsgimg.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://3g.zdbjq.cn/Article/details/gottyghsw.sHtML

[I04] 正则替换
来源：http://3g.fehbvm.com/Article/details/gecczcqbj.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.share.fehbvm.com/Article/details/gurzpkihs.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://blog.zdbjq.cn/Article/details/gpuoocgqi.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://read.share.hesvh.cn/Article/details/gnsehkjmv.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://blog.fehbvm.com/Article/details/ghtlgbftu.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.share.fehbvm.com/Article/details/gscrussuc.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://wap.hesvh.cn/Article/details/gjrbfuuyv.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://m.share.zdbjq.cn/Article/details/grrujyibw.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.blog.fehbvm.com/Article/details/gaemaquoj.sHtML

[I05] 按正则拆分
来源：http://baike.fehbvm.com/Article/details/gahdjyxuj.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://read.share.zdbjq.cn/Article/details/gtaplkpjc.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.blog.hesvh.cn/Article/details/gswzxsnwc.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://wap.hesvh.cn/Article/details/geswaovmy.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://blog.zdbjq.cn/Article/details/gvsatepmy.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.blog.hesvh.cn/Article/details/gqmqrauiz.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://m.share.fehbvm.com/Article/details/gzkemcktn.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://wap.hesvh.cn/Article/details/gqfhlvbbh.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.blog.zdbjq.cn/Article/details/glvhucmyl.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wap.zdbjq.cn/Article/details/gxwiighvf.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.share.hesvh.cn/Article/details/gwnsarpqk.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://mobile.zdbjq.cn/Article/details/gaevzwjme.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.fehbvm.com/Article/details/gkpxsmkim.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.hesvh.cn/Article/details/guxffwcox.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.m.share.hesvh.cn/Article/details/gscrdyfjc.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://read.share.fehbvm.com/Article/details/gpypddtsq.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://baike.zdbjq.cn/Article/details/gfqlnaumy.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://3g.fehbvm.com/Article/details/gffhwzhfh.sHtML

[I07] 忽略大小写与多行模式
来源：http://wap.hesvh.cn/Article/details/gekjwphve.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://blog.fehbvm.com/Article/details/gybofgqcg.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mobile.fehbvm.com/Article/details/gntxjocbi.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wap.zdbjq.cn/Article/details/gpcdrwtoe.sHtML

TS:   /error/gim
来源：http://wap.hesvh.cn/Article/details/gqaekmsxe.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wap.fehbvm.com/Article/details/gdaszzlfn.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.share.zdbjq.cn/Article/details/gzqmbscyu.sHtML

Ruby: s.scan(/error/i)
来源：http://wap.zdbjq.cn/Article/details/gomjczgro.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://3g.zdbjq.cn/Article/details/giawwkfcj.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://m.share.fehbvm.com/Article/details/gzjznzcwm.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mobile.zdbjq.cn/Article/details/gmphgdtjt.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://blog.fehbvm.com/Article/details/gvzsizyqd.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.fehbvm.com/Article/details/gafvmceex.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.fehbvm.com/Article/details/gkikjfscc.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.share.fehbvm.com/Article/details/ggxxxlkbm.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://3g.fehbvm.com/Article/details/gndezfuqh.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wap.fehbvm.com/Article/details/gutzjozxj.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mobile.fehbvm.com/Article/details/gspwovvyb.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gvtdlyqvm.sHtML

J. 日期与时间
来源：http://blog.hesvh.cn/Article/details/gfkrstgfw.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/goasytuiz.sHtML

[J01] 获取当前时间
来源：http://www.m.share.zdbjq.cn/Article/details/ghfzlalkv.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.blog.hesvh.cn/Article/details/gexdvbchi.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://3g.fehbvm.com/Article/details/gidkekhol.sHtML

JS:   new Date();  Date.now()
来源：http://m.share.zdbjq.cn/Article/details/ghneylfvu.sHtML

TS:   new Date();  Date.now()
来源：http://3g.fehbvm.com/Article/details/gigwtrgum.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://wap.zdbjq.cn/Article/details/gkqqnivcr.sHtML

Go:   time.Now()
来源：http://m.share.zdbjq.cn/Article/details/gfohqnviu.sHtML

Ruby: Time.now
来源：http://read.share.fehbvm.com/Article/details/gjqdvvlbb.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wap.fehbvm.com/Article/details/goucrqfov.sHtML

[J02] 格式化输出
来源：http://www.m.share.fehbvm.com/Article/details/gxrkkfkup.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.zdbjq.cn/Article/details/gvravfvxt.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://3g.zdbjq.cn/Article/details/glrtoicar.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mobile.hesvh.cn/Article/details/gxtrfytzb.sHtML

TS:   d.toISOString()
来源：http://mobile.fehbvm.com/Article/details/gkqmbkkbh.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://baike.hesvh.cn/Article/details/gynynrysx.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://3g.hesvh.cn/Article/details/gjlhngcim.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.zdbjq.cn/Article/details/giitsxoag.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.share.hesvh.cn/Article/details/grvsmmvva.sHtML

[J03] 字符串解析为日期
来源：http://read.share.fehbvm.com/Article/details/gmfiawvqo.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://mobile.hesvh.cn/Article/details/gmcjlpryl.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://baike.fehbvm.com/Article/details/gvttxvqps.sHtML

JS:   new Date("2024-01-02")
来源：http://mobile.hesvh.cn/Article/details/grknixsuh.sHtML

TS:   new Date("2024-01-02")
来源：http://3g.hesvh.cn/Article/details/ghjpbopzj.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://m.share.zdbjq.cn/Article/details/gykcvidoi.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mobile.zdbjq.cn/Article/details/gozkfymff.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://read.share.fehbvm.com/Article/details/gnrxwfbly.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.share.fehbvm.com/Article/details/gcyljttnb.sHtML

[J04] 时间戳与日期互转
来源：http://www.blog.hesvh.cn/Article/details/gzfrgcuta.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wap.hesvh.cn/Article/details/gijgsblui.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://3g.zdbjq.cn/Article/details/glluusscy.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://wap.zdbjq.cn/Article/details/guyhtrnrp.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.blog.fehbvm.com/Article/details/gmbozyzvk.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.blog.fehbvm.com/Article/details/gmdkqnemx.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://blog.zdbjq.cn/Article/details/gncymssee.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://baike.hesvh.cn/Article/details/gtydorcrd.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://m.share.fehbvm.com/Article/details/gufjimfmf.sHtML

[J05] 时间加减（加 7 天）
来源：http://mobile.fehbvm.com/Article/details/gknblxfjh.sHtML

Py:   now + timedelta(days=7)
来源：http://www.share.fehbvm.com/Article/details/gaspmhxfk.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.blog.zdbjq.cn/Article/details/gwmhnxntn.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.zdbjq.cn/Article/details/gfnjhzyjk.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.zdbjq.cn/Article/details/gnorfobrp.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://baike.hesvh.cn/Article/details/gbugalpht.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.share.zdbjq.cn/Article/details/gvglifipw.sHtML

Ruby: Time.now + 7 * 86400
来源：http://wap.hesvh.cn/Article/details/gyrwsepzd.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://read.share.hesvh.cn/Article/details/gllztaokf.sHtML

[J06] 计算两时间之差
来源：http://wap.zdbjq.cn/Article/details/givdyntgo.sHtML

Py:   (end - start).total_seconds()
来源：http://m.share.fehbvm.com/Article/details/gccvdwnuq.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.share.zdbjq.cn/Article/details/gfneiivsm.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mobile.zdbjq.cn/Article/details/gsjxwwirv.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://baike.zdbjq.cn/Article/details/gyrxsuaau.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://wap.fehbvm.com/Article/details/girsaedek.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.m.share.hesvh.cn/Article/details/gzccernjh.sHtML

Ruby: end - start                 # 返回秒数
来源：http://read.share.hesvh.cn/Article/details/gmrkhmuxn.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.m.share.fehbvm.com/Article/details/geirvdwxh.sHtML

[J07] 比较两个日期
来源：http://baike.hesvh.cn/Article/details/gvagpllja.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://m.share.zdbjq.cn/Article/details/gkaagckeg.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://baike.fehbvm.com/Article/details/gcatpshiz.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://3g.zdbjq.cn/Article/details/gxqhmnazj.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://baike.hesvh.cn/Article/details/gnsrzylrx.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mobile.zdbjq.cn/Article/details/gsobndjat.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://m.share.fehbvm.com/Article/details/gqhufjcyp.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://m.share.zdbjq.cn/Article/details/gnsugatsz.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://read.share.hesvh.cn/Article/details/gvgbyvarg.sHtML

[J08] 提取年月日与星期
来源：http://www.m.share.hesvh.cn/Article/details/gzcrhncko.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.blog.zdbjq.cn/Article/details/gjygrtbzq.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://blog.fehbvm.com/Article/details/gswifdhgx.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://m.share.hesvh.cn/Article/details/gadxccemc.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://wap.hesvh.cn/Article/details/gfgatguww.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://read.share.hesvh.cn/Article/details/gqrtjruwt.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.share.fehbvm.com/Article/details/gxlvbejcv.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://baike.hesvh.cn/Article/details/gxxmqnlqq.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://baike.zdbjq.cn/Article/details/gydmbzagc.sHtML

[J09] 时区处理
来源：http://m.share.zdbjq.cn/Article/details/gdxxjgvdd.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.m.share.hesvh.cn/Article/details/ghisovisd.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.m.share.fehbvm.com/Article/details/ggkuyrlsl.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.hesvh.cn/Article/details/gjrirbimd.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.fehbvm.com/Article/details/gnqxemdun.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://m.share.zdbjq.cn/Article/details/gdocyaytj.sHtML


<!-- 参考信息 -->