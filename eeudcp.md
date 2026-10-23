代发 wailian999

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3mhgcggpx.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3vbzynbka.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3nyrmlvcz.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3ryvxivqy.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3iwgfkwel.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3iitvxwpx.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3frdbrrir.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3peuawzeu.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3dfhhgbxs.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3maehrtqm.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3kgadwsrr.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3lziapius.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3eikmupoy.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3cqymzqsj.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3vhjtfbwx.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3atxipmiw.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3qwlvujwb.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3fayyraco.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3sbfidmjp.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fknmpzdi.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3yjmeypft.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3zjgopjpu.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3ziuxlsir.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3vpvmkbkg.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3lbhiqgeq.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3pxyzcboy.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3xbrgmzdg.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3ixkfavqt.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3nbfianuh.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3kswzwlhq.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3hdzvqqsk.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3cekemgjj.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3csqqrapw.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3jilzqdii.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3zypezxje.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3lfmlpklj.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3rvgiuxnu.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3xxcemuct.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3jhxetqwh.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3gsgtaeid.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3uvcjeqjp.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3cqclivwv.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3dtkidzfe.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3eeoxitdr.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3iwqnaulb.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3poznvoet.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3dexlaqam.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3gcwpsyob.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3xkbiesmn.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3fgyuxxbs.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3losvgqce.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3hkwfiriv.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3hljfudpg.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3xhwcogod.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3wgdaiona.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3dvhhbfgj.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3pjavgjst.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3pqglchhl.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3cxwkaaad.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tmroylrv.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3selheknd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ildsymjb.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3jcoixqhy.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3gtqkdsmn.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3msdkmxlo.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3lvwydzvx.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3zsuvivym.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3tjlxbmvc.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3tmxjlqis.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3piuoovon.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3dbbfyuuw.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3vhrnnxhl.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3ailkeavy.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3vnzbvjrj.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3fgvndmtg.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3amprubjr.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3fsjtlpny.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3xqywzrnq.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3xnazrhfz.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3uymygsmg.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3yvanzjli.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3gzjpaaxk.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3rvecrvpy.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3fartgmsz.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3tusnmsnu.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3xsizyssv.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3ebcbutbh.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3bqcrkqoo.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3apwijjsz.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3vhnynqwa.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3avnzjsqj.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3nikyqqcz.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3gwgftngt.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3odlsaqrk.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3eutszbwg.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3tfdwbfix.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3ksrxdwsn.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3eeditdkd.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3pfmxcxce.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3bsnsmsta.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3ezkqcvkx.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dadfyyww.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tnmdvtso.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3wmrcesft.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3seaeanbc.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3orfcrsjr.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3uotuktqp.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3oddoknwi.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3jxhimdne.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3tlyaoice.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3fqgoqjbn.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3olbtzmbr.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3kuruskzb.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3xvmxzxjy.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3tbeafxik.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3wknqpvxo.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3qwntrptm.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3ytzrudjf.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3nigcpozt.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3tvbuaypr.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3mwgggmpx.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3atpzauom.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3boanpwln.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3tigxiubf.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3yqfetgfn.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3qhmjlijo.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3qylcvezo.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3uicimdfd.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3likoeyez.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3xtwphqyi.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3ndwsguel.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3uhwwrubl.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3isbijghh.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3olvbhbvz.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3gblamllu.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3fgpbxwvo.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3pdnwrmhg.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3ikhafzss.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3fptchrxf.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3dxlmktgy.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3tjwyphcg.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3ivmwupqt.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3ukfbqofx.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3dehcmnrg.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3khgkwkgw.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3rhfypjzr.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3vvakvdle.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3wwltnvbo.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3luqmdduv.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3ujnixtji.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3uyektalb.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3gredtbcv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lywjplrm.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3pcmzihvs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uklnfpcs.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3wmayczyh.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3ugrppspt.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3gfmfjskk.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3gwqyafts.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3kptnkfzv.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3mnbsgqqc.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3iwaweuvq.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3pgoglvkv.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3kcvkcgyx.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3arkanhau.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3mmxumobz.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3cpqlsqiv.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3aucxxfwk.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3nfxddcar.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt3satqacqr.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3qolxbwgl.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3yowshcyj.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3udyudxbi.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt3fwoyxjwr.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3znwkbesv.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3wwhqqnpk.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt3wervhssz.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt3dnaqbnqu.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3mexxnjjz.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt3ejnjykrp.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt3eehdyyjf.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt3bjdjlzyj.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt3ftgwrdpf.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3hflvuqsp.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3nsefvbgz.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3wakifizt.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3ckbxwchx.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3vogkcnem.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt3rbzygehp.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3pbjhplpx.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3ztskicpk.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt3kapqmshj.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt3lspxtaju.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3gqvqcnpz.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3ohhibwyr.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3fcayuvgx.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3afvylrfj.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3fugguucx.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3cmensbyg.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3misrthjq.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt3wwggniiv.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3oefzumto.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt3cceupgvz.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3saulfxxj.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3eydypugk.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3hsvhyolq.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt3onyohgen.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt3imwonqnv.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3nnrtqpgj.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt3wpjwnixe.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt3mxjaowys.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3srtbedwa.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt3pujlvyms.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt3ruuhgccq.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt3bpwhuyqf.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt3ieoxwzjz.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt3cjhyfjph.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt3tjloedis.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt3kvlngzan.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt3sodpbncr.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3sllxbeqt.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3hshikdda.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3zptclnho.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3lmuvirmg.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt3rqoirvtr.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt3ioyfqvkx.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3djbdqhgu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qwjouxsh.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt3mqqzqbyw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ywxvcvqs.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt3tpjwabnu.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt3fhtkecfb.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3tbiddenu.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3jnbwmocw.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3ipzbtdgu.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt3laeoqhfo.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt3udrtdljp.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt3tibexcqb.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt3kodwriwt.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3xkbveavh.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3vwgfoqhd.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3zencbtbp.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt3ducqvoam.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt3xplbqrny.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt3edwlmrhu.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt3qdqtumug.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3qwwdktfl.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt3kmzgosko.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt3kewlczqs.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt3dugrllrp.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt3cdeuwcnd.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3kzghbxvl.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3vfywrjfx.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3jrbnpjoc.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3jnyylqfn.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3bpqwmqnb.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt3phnafbzv.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt3dfhlhhwm.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt3iuxhpxrt.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt3uyfxhfvp.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3vshkbqnh.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt3yuyckgki.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3iwtwyksi.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt3upuswxbd.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3gbznmhcw.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3rcklboja.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt3rxnihlft.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt3icsmcwyg.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt3knpmsajr.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3aiamheny.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3rxxmngdg.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt3dxefjgdi.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt3kihaebpk.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt3eqoscvlj.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt3ftbzsyqu.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt3rvnqeiet.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt3tmkaycic.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt3disvspol.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt3dolrjuda.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt3qecdgikp.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt3aecuigcs.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt3wqzdyede.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt3ezzszacj.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt3nzmouhrv.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt3dztwvswd.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3nbaztxdk.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt3ltgobeid.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3pdepaqat.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3sayovpcj.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3buuihvhh.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt3hpqujewz.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3zxxykxkp.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3bteiosqs.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt3hxzfsejh.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt3pvwqyssm.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt3souqpxhe.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt3laqkdxbb.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt3czibmzbh.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt3nlytzqjn.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt3mvxvqocm.html


<!-- 参考信息 -->