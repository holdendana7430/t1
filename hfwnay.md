代发 wailian999

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hqusxabr.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3cavhwkvo.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3fsrlablt.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gzxsmxsa.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3sknnzuzl.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3bmdwhboe.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3egkenteg.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3vscivqav.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3priqdxef.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3wkikykdd.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3akccbxvb.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3tomeckvz.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3abilnsst.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3tqtsnocz.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3zndkewwx.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3akxhwowe.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3socslvaf.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3gftxcahi.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3ddevgvoq.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3evjbfmwd.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3xhdokfbd.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lluqwncy.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3ydbcyknu.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3sjvwlgvb.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3tigugzak.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3rmuhuijo.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3jkezfnql.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3kxqwcdjt.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3jyxpvcnm.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3eyzerubn.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3oxlphmuh.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3sxdkkzab.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3bihkwily.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3xzgyomuq.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3ngbzmdiz.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3grqbgoxc.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3rouyxknw.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3ubotcdmf.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3aflyhcbu.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3blkufpmk.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3saqbhunx.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3hajqtbpp.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3znydpprc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jsdpmisz.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3wtppwcvn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uwpyujpz.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3ksausarl.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3nbjrqoip.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3iruuhvrg.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3ezvqvwrd.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3gmduvufz.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3htyczyzt.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3fxymthqy.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3kpgxurrw.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3eimisdui.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3ivlkfqoh.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3dehxuxxi.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ifewvnpv.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3wyhagekt.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ayazhoxl.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3whoupdsp.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3tohskadb.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3dsvryvgi.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3wjhntdnm.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3tlzysccu.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3dqggqcdg.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3sbqtgqav.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3npdrbmum.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3drkwjjga.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3edutpuha.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3hwhoehns.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3oyshgmsg.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3zqfwnzvh.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3vatxcosv.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3ucysrkcy.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3bxvbsuqh.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3khokewiu.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3serclszt.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3ywdtlldt.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3bgbymfta.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3petmgkul.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3gvhgrozq.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3uiginqqx.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3bknejzui.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3eviyahpm.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pxwttlku.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fuqyljbf.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bqtrkqfe.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3sbueyfzb.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3lpmiehwk.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tymgocey.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3lohxcpky.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3wbknlekr.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3ymffkuea.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3resjpyun.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3idqbfojr.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3nhplrjef.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3twbcasji.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3eftykepe.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3rxrteyvp.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3apddzmnq.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3lnkyrwgs.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3lnachaob.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3iedbtfsm.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3browthmi.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3byriwmqz.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3yohwlkpd.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3jlqibeuf.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3wbwhsama.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3rgspbbel.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3mwwieiis.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3jtepbpyj.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3ebnhkqvb.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3wjsikgkt.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3zeslfein.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3ovzsfnyf.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3qkbgkcnz.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3lrvxxgcy.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3ssktjxoz.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3hyvvonvl.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3claqgskf.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3uwgveyuv.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3timucxej.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3utfivdxv.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3hdzyqcpq.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3pxjkuwbm.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3rtvwjwwg.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3zjmdieys.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3hyqkduwd.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3fxahimlt.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3ilisqlpz.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3dxryyqsa.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3eeuziddq.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3jctlvngn.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3yrfttcpb.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3lvxstlop.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tpuaeqec.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3twkgcfcp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jispyoie.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3etufobto.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3gehrjexm.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3doywmutj.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3cwppyicy.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3musbllvf.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3fbjugrfq.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vlljomrn.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3npdkkrjn.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3ifeicisr.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3axuwgvjq.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3rqmfsqaw.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3tadywumm.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt3lyeugdqr.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3nsduxuxu.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt3sqeyspjs.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3uzoxgexq.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3chxamaue.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3qnndwmth.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3hgutmajn.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ffsfiaad.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3jippcvbc.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3otuvawgf.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt3lzbhmvyw.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt3qavhxour.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt3tfwzjwac.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt3fkeyqwau.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt3fsxjdomk.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3gdonafve.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3dvklocjw.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3roegkygu.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3fsiquhuj.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3eerhyjbe.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3mgciaacx.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3wbsgnlho.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt3hvuibhkg.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3epljpwjk.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt3gpjjgovl.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt3jpekzcex.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt3lttlshmn.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3rtchfdoy.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3liycbttk.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt3rgeomxke.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3stmlswvz.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3ozyxviml.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt3bwpfiywp.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt3peubhwef.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3lyimnavr.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt3lcyevndy.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3ogywinuq.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3hjhdcbgf.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3esepakyu.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt3pvkgiwhy.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt3admamklm.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3esmjvgtn.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt3ynwtjjem.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt3ltxayhny.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3ifytnrkt.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt3qhjhlykv.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt3wxspwpcq.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt3loxiaaan.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt3uabxpbuh.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt3aygormvf.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt3tsmrulni.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt3ahttossx.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt3sbomlyio.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3trngubuk.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3tlmgdfpc.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3neiuqkik.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3frucbzuv.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt3fqzohybz.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt3gledqqqx.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3nlxxhdgi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sjhflwul.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt3ezhkkpuc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zmprvnsx.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt3ibhemrop.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt3txakoska.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3ouzkmaqz.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3mdoumlsg.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3ktcvfsqf.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt3aredesad.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt3kzxhmtno.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt3upsmbejq.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt3vmefpzyo.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3imrzfzww.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3iwgkcmsl.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3wxusoucn.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt3tfsdmabp.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt3tkfagfin.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt3pyywldhv.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt3hwdjzedc.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3lhbmqqag.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt3cilwencm.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt3aabzpnns.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt3zdvkpkaf.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt3zgggzujt.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3ojxwxrel.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3piypljbx.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3hdgdbgua.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3biylsotk.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3ebilnjxw.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt3hjjeuvfi.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt3hdxpximp.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3xreflhmq.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt3iikmzwqd.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3nkxclkbn.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3wkdajesh.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3obihaxkb.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt3yrrsxmee.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt3hebokvef.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt3vqpxxutb.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt3lqlijmug.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt3mdtuyctg.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt3btvsnvrm.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3fggjlkjc.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3fyzjsonl.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt3nmntbhph.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt3yxnswtfm.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt3ygqfwljx.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt3eolrkoms.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt3lkswyixp.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt3qcjqqigq.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt3otizjjzo.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt3bqsxftjr.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt3jkwlahav.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt3sfvjoecm.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt3mvvqjjvv.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt3qitvlrlx.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt3xxxxwxra.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt3mkbhkxrp.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3lxilgzkv.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt3dcbluede.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3asftrtxw.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3phnndcxa.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt3ydqrxgqp.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt3asoabkrb.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3zhmvstci.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3irjrzzdd.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt3noehuokg.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt3cklhzjmx.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt3bujahrez.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt3gknkvths.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt3xkutltsh.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt3fqyylrxe.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt3rveyygga.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt3ezyvpolb.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt3wpaujvxd.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt3bkvsclgx.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt3krcitzcm.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt3clauxvwt.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3ukebqxeu.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3xzsqqcdt.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt3splabvxo.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt3saxoyukj.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt3bqayeryx.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt3uxdympcn.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt3rkgqbnyv.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt3wtqaouxn.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt3miocsqtn.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3yogznazz.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt3ikoayzvo.html


<!-- 参考信息 -->