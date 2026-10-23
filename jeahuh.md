代发 wailian999

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3xvqdqtfi.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3gghncnuo.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3wdyfmfje.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3woaizcse.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bbdjabrj.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3hgstoiya.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wlgpwmlu.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xxxoubeu.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3lcaeelai.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3pmbbrhue.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3kflecfrn.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3rvrobluo.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3ssbhmykv.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3xshvdopm.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3hoeytidr.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3trnvnrdm.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3zxwydkid.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3sxipmghn.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3degbemem.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3gkakwdiw.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3ostzsfhx.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3cnhlbpwl.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3hyqhkgby.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3jazarfol.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3gqfxbkpd.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3ehghuqov.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3jfxgbrvx.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3jhyehgke.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3oswnyagd.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3xnfsvuge.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3csimjhac.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3qdcguhlw.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3gzqkmlli.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3osqqzrcj.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3hhbwhrmu.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3ohtjgbzx.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3cjnegvqb.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3fudetuht.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3oybfpkih.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3qckawyro.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3sxacqdbf.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ozzxjqya.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3kcgplrvo.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3fkuymaqw.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3aljuwsnw.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3lfrijtys.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3blpqwdzf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vfsezzqx.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3tzvsqrcj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qyjipqhy.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3orfhethh.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3ifgvtdgl.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3tpgkinpa.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3lbldcnxl.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3dazavfhj.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3qvbqqdnx.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3tfbkervx.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3cgfifebe.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3pbmprrzp.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3xhriqqoi.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3advadhzk.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3tbwgnmpd.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3aijkjbvc.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3xzwwesex.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3vrpzcriv.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3nitranvr.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3wjbnqlsb.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3tpcnwqpr.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3kudcevky.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3iimfdlum.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3eqsnflkq.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3lpdawssc.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3wgwwjsgd.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3ewcfuhvi.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3tjutnwon.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3fdkjmhdz.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3vlxxabhv.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3htazlyqv.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3mzjxrqqv.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3hpeelunh.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3dtfsumfv.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3oapixndb.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3xzngmqzt.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3gavhavls.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3amfnwjnt.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3cccssvxn.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3clxdwaul.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3cwzvikdt.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3unddzlgk.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rqhsjatf.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3mwymnmlt.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3eiaoxhxi.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3ytpmsmnk.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3gwnwdxup.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3hkrniakw.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3ywffwqdd.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3znbwigsn.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3xzqyymrb.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3xiixtfwa.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3ydtvcfjf.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3rhnksqfr.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3akzeyrjk.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3zqwbjhbl.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3wvamofoy.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3nvqydjcz.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3tgzfnbey.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3pbssmkpz.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3dwbjnobk.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3yvxturpu.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3shjxiynn.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3gnnnvoiv.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3vjbyezqw.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3wyqroriy.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3uckzwxpx.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3lbkionpp.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3wnftwakv.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3xnzqndpu.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3qzyvmgzt.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3cbxutqrc.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3najroyhv.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3clvmfapn.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3iuibwqbw.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3fovdqwbl.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3onjnpaly.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3uobetycf.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3fsvpwwtl.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3wcpdtgij.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3bxzckxxm.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3ccheixwb.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3cfkdonkl.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3ellbugzq.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3pdgkzzlq.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3ehezzhmv.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3dpjgkrwp.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3lhxpziph.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3pwmpzlqm.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3jjzjxssz.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3ohlvejea.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3haxxtvfv.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3akpaywfb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nxpanhgk.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3xzmkekqj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ssmxfvid.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3fttydhbw.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3dpuhzudx.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3rddqqjxc.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3yqqqqepw.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rtvetyiy.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3igjjifgf.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3sybpzhpv.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3rdmdmhmb.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3uzyebylx.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt3kloyksqh.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3dgssgaqv.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3uwvklzqm.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt3ynpzsfzk.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt3xfftxcch.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3tgrtijpj.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3mysbfhkr.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3fogpnzpu.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3hmqondim.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3dgnibepu.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zbafzyii.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3fradhdji.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3abulrqmo.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt3xrlwasux.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt3zajulqww.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt3ubbvjavt.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt3ztipkhvk.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt3drmyvgzi.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3dvyzoypd.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3bstyfwyq.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3cnrhnflf.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3hvepfwaj.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3kxzkvbvk.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3tppshydi.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3entknxqq.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3pykzwkgo.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3qkgkxksf.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt3wztxnojf.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt3cvnjlwby.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3zkunkabk.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3guzitfsf.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3qyjuemmn.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3spelghvt.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3aidmcmab.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3zyhcwtxu.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt3orzkjviv.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt3jcihqbor.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3pejucbov.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt3uxstjgye.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3ewyocyou.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3magivsdp.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3jhvtujvs.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt3qerhnekn.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt3rosazguc.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3rtecgbft.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt3ldtumzhi.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt3goyrgqzv.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3qehxfdte.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt3nactebze.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt3bamvxzaq.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt3bqpgwesj.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt3mmbiykqs.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt3ddxyqowt.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt3cddyoidh.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt3rkvtsstb.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt3ttqgirtd.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3vqihrinn.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3pdohdtmy.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3pvzjomnr.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3ivmnouby.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt3uqevhhfo.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt3frgysqwd.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3zugikdkc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3drnuohut.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt3ftijmbzb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3slwcleui.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3zydvwtci.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt3qugcygqr.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3odnmiczm.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3zlzynqdw.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3bgbqvphd.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt3stkitvww.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt3muvtsnot.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt3dgcvsunp.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt3ecwvbmil.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3eovmfpka.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3rbzsiyqb.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3dhqgoxac.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt3zmerdusu.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt3ljzvquyf.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt3eiczijmj.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt3oczlgoyi.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3tlvuqssx.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt3hueeewhh.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt3iklxdune.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt3kyxhlrfl.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt3klqnxblg.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3uvtqfbdr.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3kilvxzar.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3ovejfhsb.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3mqbcrfrl.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3bqqjivie.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt3hvgsopkb.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt3jlulcoez.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3ewcokcyb.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt3pnwvdqqa.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt3ccaptbib.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt3skhzqjis.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3edfdqtbk.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt3ytmbiesq.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt3ijxqiesw.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3uhozlsxl.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt3cbsrevow.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt3qegmsiuq.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt3ivuywyvi.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3wmmulmpn.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3hmwkchiz.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3ojmawdkz.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt3ludurzhg.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt3rmeuthmb.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt3jlsdbenb.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt3vhrtkoqy.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt3lwksswdp.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt3sruwertc.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt3tnosompd.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt3kjpydfga.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt3rmxbriot.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt3bdcmnlim.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt3ndpskurq.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt3pfpjeidh.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt3cmdoohqz.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3atwbqwuf.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt3xuhyijrv.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3kgvjdepo.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3nffcaown.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3jnoftjlp.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt3mnrndxzx.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3rpsbezhh.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3gbviauah.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt3mkiihlle.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt3zemkvqxd.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt3lhxgsgpc.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt3wlgbcmdb.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt3amcdfsug.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt3ezefptzc.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt3ubgmfmom.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt3xwxbpeha.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt3iheevdsm.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt3hxkblswd.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt3lhjuvmwl.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt3zotenhrn.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3qyielnri.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3fdfbuusb.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt3tbefswdq.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt3qysczbih.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt3nsefwmwk.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt3ndemlzml.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt3sqyqubxb.html


<!-- 参考信息 -->