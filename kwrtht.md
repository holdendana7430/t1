代发 wailian999

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2upuveueu.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2kumhldkp.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2nsgebujv.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2zmgdvcne.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2pwkobxjb.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2uofszabs.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2xddipfjy.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2cphxwxgx.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2jfsqquho.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2cbyzjfqv.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2fwczagvs.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2dugqwnla.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2uvqgdyva.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2bkysngjf.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2uzwjotsy.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2gjvabhml.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2uggxaapj.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2tvfdlbiv.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2rnretiyq.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2angxlqkq.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2wbydqqjc.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2zhaoepuq.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2vrztowkp.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2vspxaxmt.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2twunrqch.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2nnqufvtj.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2uusqwlia.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2ghjaygll.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2xwzjclmk.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2dvzsfsmn.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2upyzderg.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2payemvuq.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2vwtdlwtq.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2gxvkrowv.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2tbvddapz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rejlrfhv.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2rxnktzei.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uuucakkg.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2lhdvmwjc.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2jbrqrhdu.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2yeowxqsd.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2wsqjikxk.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2rmudtnmt.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2wqkvguer.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2kxvavmbw.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2lurqsxnt.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2ulfdzbow.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2lpfspoah.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2zvtlojla.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2gednpuvr.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2rudjdmvp.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2leeroibl.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2jbryvxas.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2nwpwjwci.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2dafucoit.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2aqahzykn.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2oaduqyvg.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2vtjgjclu.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2iukesnpx.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2mjvppifb.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2pzuekxxu.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2zlkufllo.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2nxunogpx.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2qhnpkblv.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2fiyeqlob.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2ngdypcfq.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2gfvfhjov.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2osnkkhab.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2ixfxhpic.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2dtbmlgyz.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2zlnktlty.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2mjmcotmt.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2tgjghuuo.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2hklxakob.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2eawxemcu.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2clbafvgx.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2whbqvwmr.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lirapbyb.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2onolcuhe.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2tqyjoqmd.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2xtdvwutj.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2jatgkyzv.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tykzuxxf.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2jzejezbi.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2mloymfcc.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2xboxdbrc.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2yqmpsxsg.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2brnvxojq.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2luxlqqqj.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2qmjyctdt.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2meqzivur.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2ovxmjolh.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2dxtbbblm.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2njpekyza.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2gmkeqlbx.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2qjksmicp.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2cgxxucdx.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2ydrwyivn.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2cyjgbroz.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2icolliro.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2pjwqyacx.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2fkyhrmup.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2eevjefll.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2pbxoiang.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2znzsispt.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2cdbfcnyi.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2vshkbyjt.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2eupvnmld.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2sxswjgku.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2vxzfxiwt.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2tgxjoset.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2tywesxqt.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2cbbwmtgr.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2hwqrdvns.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2izhhclis.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2srflcsxu.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2kovegdxj.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2hmpzqhhz.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2avqpnsbn.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2ccmilymj.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2jhmdahkn.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2kqsdnxfz.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2oqodwbeb.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2qlshpwyd.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2hpsufwdg.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2lobyssii.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2mwqzfdrg.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2hdxggldw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qldbdqzu.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2fydokkif.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nzhfovxq.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2jwakocle.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2myhottsk.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2dlglcxyw.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2faccdcoe.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2yxlfamog.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2gqrjlyxt.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2sazuvyrq.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2fwgqbgwz.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2rmbyxkfb.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2ushedhll.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2vyubkkda.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2odrnqdyi.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2qwohkuta.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2kvonklvl.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2lzdxwcbx.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2jpjzaquv.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2yljvytuu.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2mbgndbhe.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2xxitvanm.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2wuetrfzv.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2uevnftjf.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2qlipjrzv.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2wwdtpkjo.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2lvchithg.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2herywzwt.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2mgcprrxu.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2kvtsoqew.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2meqwrlux.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2ijyzppli.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2eqdsdcwq.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2hrddbanh.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2ffqtlxvr.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2aprvesar.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2ddlcclew.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2zmbkwvee.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2umlbebnp.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt2vktlzuph.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt2kpnqmjub.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt2ynbnrvga.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2ytcogweu.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2znyqeerb.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2vldriolq.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2abcxlwnr.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2vptvzecf.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2fkdxflgr.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt2hxrafabp.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2plpktclo.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt2ylqseaom.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2mxhurtsj.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2fyltnnxw.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2ijmrlfal.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt2zmhjdjur.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt2rfxivbes.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2vhlghgfz.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt2iawnerpw.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt2nqigdetj.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2zgdlliir.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt2iquqnxzy.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt2laitpbjr.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt2nodxcaps.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt2wccowxwu.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt2mrmlnekq.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt2jrhwqfls.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt2lglytyne.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt2tkoxtmlc.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2otrrurle.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2wmiummva.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2mazxicmd.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2yozwkhpa.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt2ajrxygrm.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt2hmiquram.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2hlclzqoh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rynqosdq.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt2hbrlbpii.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2foajmgoj.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2knogoxym.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt2jyulofmw.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2lurtkvmp.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2xfrllaxf.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2inxrzrcq.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt2qmzymdce.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt2ngiojjiw.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt2dbslqunf.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt2tnttwtmh.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2umdkbdfw.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2dsiufatl.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2ugyzggfw.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt2hrufujak.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt2pqzgelyg.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt2ahlrjibf.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2qhzzytfr.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2kpkjqcse.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt2tirdbtza.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt2grgkmyqf.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt2zyhowfbj.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt2irspplwt.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2iblsiarv.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2wiagdbyb.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2kexyqqpy.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2pxufsqru.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2ixyxsleh.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt2jeefamex.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt2vhveefnn.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt2aqgfdtab.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt2oibmuxgf.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2agyaogbr.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt2cpedqjrc.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt2sqqjgxoy.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2fwmflozc.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2zskdwntz.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt2oxvcesqu.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt2fasiwmjo.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt2tfrbskwb.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt2higdlzwy.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2sbifrpxu.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2gjdhhlob.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt2fcwluxku.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt2ecnyxxme.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt2soljgwqh.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2tbcmkzus.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2upzzchns.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt2kisibmeu.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt2muuuqxpv.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt2hqpkisij.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt2jhgflfsb.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt2xckcffdc.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt2zexlviry.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt2ichblxih.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt2ggbkrluj.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2cvfvdpam.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2ezmvllmv.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt2eumzaxkl.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2rfsisano.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2oraqewfi.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt2goeguvxx.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2ewbrwtvs.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2ndxkieer.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2ydhiezmw.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt2frcbadkq.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt2kyaalske.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt2hdbykaee.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt2dotsqpgc.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt2osykyviq.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt2iqhocnbg.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt2olmsrjdp.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt2synzbswo.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt2eufcvfkd.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt2fzhfaxac.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2psirljdg.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt2ghdysutf.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2pczsrkcw.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2qmgcwsfd.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt2xujaylgn.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt2ksqmphhf.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt2jadraycf.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt2mnatfjwl.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt2jitfoztw.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt2pdigawpv.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt2mvdmkxcw.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt2tkopggdq.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt2imbtyofb.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt2lyavguft.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt2vqdedgiv.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2udxnuupj.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt2buxtrguo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jlyqlwnz.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2ontgfwrm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dtefljac.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2kbtgvuih.html


<!-- 参考信息 -->