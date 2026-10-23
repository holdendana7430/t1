代发 wailian999

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3dejnlolf.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3tuqxnqpn.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3wujgyztf.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3hbjxglai.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qgorlfxa.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3ielxlqsw.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wjmdmgyy.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3eybmzjau.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3ppejzxyh.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3onigaltv.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3cegibiyz.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3hyrsucvc.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3ywtwtadi.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3bhvhubmn.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3vnwmhbcp.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3qrekzdgr.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3xuqjpjfe.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3qfulgghf.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3pymhiegq.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3xiypihxf.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3rafalbog.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3mzhrqmdm.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3tgrhfqvp.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3vjpwxbpz.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3hdvzwtyt.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3anfstnng.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3peyanxhh.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3krlweqai.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3tgmbober.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3qdzrqrjs.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3srkxcglm.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jcyjzapx.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3fcjiqalz.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3zmxuqkwr.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3brypukqq.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3jskrzjcs.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3unidsghf.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3xvuiugbb.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3mqyqixim.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3oysvhemv.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3wqslrhev.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3daoyontm.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3zdiztwrx.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3ibahxwwn.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3shkzubnj.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3rqlxvtqm.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3wkgdhjtv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sjoargzz.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3muqslunu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mjpjfjor.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3lebvehcu.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3fljuzcna.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3atbsnbkq.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3xyurxcqj.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3vkcmymkp.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3adysixtf.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3jdpytjtj.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3bmcfmyzl.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3xeppgljr.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3sazahxls.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3vplrcrmm.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3sngjavrk.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3yvmpnirn.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3kwmphnmb.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3efbvzjxa.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3ejzwjvdl.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3fdzureil.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3fjkgqzbr.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3lpwtuitw.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3wxxoxucs.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3hrivghkp.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3vvnkjzhj.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3cceadtak.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3delsvubq.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3tmhzkxdw.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3devacgkc.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3wdghlufo.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3tutpvsmd.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3zxwizkxc.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3sqoxqrvm.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3blfnnstn.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3xbkzbzxd.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3ddjtbohh.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3vphgrqvk.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3lznofexl.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3kpomfcbh.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3exqrvfxo.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3cswhqjgp.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3tgumydoy.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3evamizob.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zpibzmel.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pgtkeltb.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3iotsqoje.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3ergwctqj.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3kovlmzyp.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3ucoskjjs.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3ubduvond.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3nkfaqedv.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3hgvhoeuo.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3dhdqftid.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3yqqrcivx.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3baqoashx.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3oxfazxfz.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3zizxzgmq.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3ifllabyr.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3ahhnfjkx.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3hohadfeb.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3jbtvamlu.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3ovtlcmiy.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3bnvwztao.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3brysjnox.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3ayypslkh.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3orpfiuoo.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3tshsyhcj.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3hxidwwpc.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3fqldajtn.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3wlpyyymh.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3stddkivo.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3rscoeall.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3ipluvllr.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3dheelbuu.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3wwdineuj.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3oqqwzjxy.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3fpjvnlws.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3trollbhj.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3czyvdoug.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3ztschwxd.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3gkvyehuq.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3szzosasm.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3duvpbyjk.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3adbopnnw.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3nagsdrdm.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3iyviruqt.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3vpeefknw.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3iomyfarm.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3mvpoqlcw.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3qzmhwpka.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3qaadmibl.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3hhkjflrj.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ghnrtbnk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eshjsxhy.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3marnuumt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gwpyekyl.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3rkuxnkrs.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3hpjcowry.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3mskygfbz.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3ofxdflkh.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3trgxfexw.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3edzrxtnt.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3polwlxju.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3uddfgawa.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3mamprfgo.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3vczjjzrr.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3zzzfvusb.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt3iuiwtchc.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt3tdqrslbk.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt3nwsqzifu.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt3nkuzadsj.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3dynxkuft.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3ubjcrqoa.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3izlpobql.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3uuvgcnwb.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3pdjrzbpg.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3sbvjjnvk.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt3eylhgdzr.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt3knhlteso.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt3szdtplco.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt3crpbyjpo.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt3tolenbal.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt3mnrgnmid.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt3lvdsfhcs.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3qfvbmjao.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3juccqsej.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3sqlvwuom.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3kvkzpfzu.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3qczpvixz.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt3dahgytgf.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt3aixiucix.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3pmythpqe.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt3vjhuotxt.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt3svqppsgj.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3hlshuloj.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3owsweuxh.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3gohsznrd.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt3orzchbqb.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3gibzybap.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3nakxufke.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt3xwkodwkp.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt3ugfbjjww.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3ffpakbag.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt3rcagyeim.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3jnhrepex.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3ibmmankd.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3oaelfokq.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt3blcesjtu.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt3oinoasws.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3wlmrmewt.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt3hmniajzs.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt3anljkyck.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3qkqxncgw.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt3omcnkiag.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt3ycxmnzpm.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt3wmixabjj.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt3tffmutac.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt3rytdhesa.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt3aypxwiea.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt3xtfyxvvc.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt3cyhtcrsn.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3rmbfuggr.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3zscwxarn.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3vekjsjkf.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3czqsoexu.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt3pqbgnyqn.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt3kzibxjne.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3mvwhassp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cefmtkdw.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt3vhvlprjt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vabjymvs.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3kflrmpbo.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt3glolwoej.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3bolccvjc.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3ygnpjkbb.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3ccegmtwd.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt3ghsxaoej.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt3ukxqdgdk.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt3asxcnyuw.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt3pzcsuheo.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt3pmqifdxu.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3ljmdfdnj.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3tpqzuqqv.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt3pjtxqnva.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt3wbufhrbq.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt3uomggmho.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt3xzrvvdzt.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3olaxhilb.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt3ikargeaa.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt3mueplktq.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt3pkimabiu.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt3jtkfvwnl.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3vejaydxr.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3ggpujvkd.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3slotqhwe.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3yfppwfol.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3qovjvstg.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt3mtluvwpe.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt3iartzlkj.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt3ozhnefhw.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt3bpecqotc.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt3fgpnoizy.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3bwzmhcrk.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt3rmpohuhz.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt3dtycfjsa.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3jlzcdzwq.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3fujwjvlq.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt3givugbjc.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt3iawdcbud.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt3mhnnhanl.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3koiymkdd.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3uhmckkgm.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt3nubkvemd.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt3boznosqr.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt3evlfewnq.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3kxpqofda.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt3yylssxmf.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt3nvungvkh.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt3uzwcwoin.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt3ktdyutbn.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt3eyhirmjz.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt3wolybxuh.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt3rcybfykw.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt3nwytklwe.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt3mixakhje.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt3uplnimao.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3vddaanfc.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt3oozukvxk.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3gzomusus.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3sjcpzjge.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt3wqibwnut.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3fcjzgbtk.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3cwivoeea.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3ywecarqj.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt3ygwxdiwi.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt3oobagtme.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt3xnebtubn.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt3tmuosnqk.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt3zgficnqe.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt3egthegjd.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt3oskajvek.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt3ajwdfrfy.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt3xjwcynfm.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt3znphzfdl.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt3lknfixpp.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt3lnwvqvxq.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3gvkfixus.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3qcybthlf.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt3rivhxffz.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt3tlqgyszo.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt3ikqxqpwq.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt3iipynsbb.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt3ymbnedtg.html


<!-- 参考信息 -->