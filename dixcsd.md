代发 wailian999

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2wpaldvio.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2zmfnwglz.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2iaeejdwy.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2lugnfyar.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2vzrigwgq.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2vdsnxrhp.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2lvvdpigf.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2gijapomv.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2epvyctcr.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2vhaxzczr.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2yvpxwjmg.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2yffvvusf.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2pghoqzwz.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qvbueigz.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2iqbrxtdn.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2elpevhdd.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2vbsxjybn.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2trpjxrwk.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2zwevlmxx.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2kecbfiqw.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2iikoebob.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2bokhobbl.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2jvacvvrc.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2dfkwxwlu.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2kyzyxywj.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2anqpxfdb.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2fyziqugn.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2dfddfzxa.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2sahqaond.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ohcexzgc.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2pufjczkd.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2vsbrlodm.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2afatnlzs.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2ztmsbbhu.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2evinqnli.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ojurlbtn.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2ccpxxvmm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lienxlcp.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2tjpbkcii.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2wabyzswe.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2gbdydjky.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2nmfppicr.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2hpkzuadc.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2blfftbul.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2gomkabpt.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2sictytnm.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2dudhinrv.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2vvjbmgaq.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2kiojxqpn.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2jfwihlls.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2epbmubxz.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2sioxtvna.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2kjfkfaxq.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2hswatyet.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2xsocvqwp.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2dmfycjbz.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2bmyttuvt.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2xnnajqzl.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2iozrakke.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2zogolwii.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2airecymx.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2rkuwwgoh.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2lszgpxvq.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2olriixwe.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2vljmnntv.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2ozsmqhrx.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2hbvibkgo.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2uwhgwigo.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2amxvcsxt.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2hrchgsbv.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2uodwhmxa.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2bdclvxae.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2adqcmrri.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2iytdetbb.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2clbcmqob.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2ihojnvwd.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2hhxivwqw.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2pjmokrxh.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2imymbpqn.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2cvtncclw.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2eesmktoj.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2dwnzjysb.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2rxfnkned.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2eoheospd.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2jjpvcnqn.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2efrohlut.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2hrbkuiyx.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2gezdczmo.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2ieuuxzoh.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2fjlwjdeo.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2urarojjb.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2bsockyas.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2tojrhsyy.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2kbtrzsue.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2beokxyhn.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2dietigbr.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2hnjdxsge.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2ykzoofox.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2hopbyrnd.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2hjyvvypx.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2yritubsx.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2udxclgnc.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2icxgywjv.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2mkrwaxli.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2yhjcrwwq.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2zvxghmwc.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2lyvksdrn.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2kspxbnip.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2slkahrte.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2dleprvxa.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2oasktdgo.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2woxfizyx.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2gzguaovs.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2mqfjvjws.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2eeukyfjz.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2cnbmekhs.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2yukzjhlb.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2myecqkvv.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2ervezdvq.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2zrwcqbxd.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2rssczimm.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2fzzdcxca.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2eonvdryl.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2uantooto.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2qsrsfcby.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2vxmoormr.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2dtoktsqu.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2udstxdlh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2phkxkwir.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2bilgnwxb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dzauwiss.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2uhvbdpgj.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2mhmddbbz.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2lnzfngzc.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kiznfbqh.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2qxmatbph.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2gznzgobu.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2fsitniap.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2rnekegoj.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2rzkslzxl.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2hwkqybny.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2lhkrxvpg.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2wnafvlqj.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2lfuynfxu.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2enntmszn.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2rawccmqb.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2mvzkgjmj.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2tkumlyky.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2zteubiai.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2dydevegg.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2zybtvhlf.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2zgoqvbvx.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2csqycdgu.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2zlxtzbzh.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2avvdfjpm.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2gigkifzh.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2snvssfyt.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2rsgptxfh.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2yotjvjag.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2opezuuim.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2dintpksu.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2cxmfblpg.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2omikiheh.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2gfrzexvo.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2qogyyyvj.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2xhhfplaj.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2mivikhxi.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt2kceqraps.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt2lretunsz.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt2jfoiamcq.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2etybofyq.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2sbpevspp.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2hxlvqgwn.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2hclqnaur.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2rrjgxccn.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2fcjipzrj.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt2aeqtsthr.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2mxcnvxmu.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt2gjmjobrd.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2evthavaj.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2dukktfux.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2dfsozoio.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt2soqlxyrv.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt2rtkbtywd.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2alrcdkei.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt2iwdqwhjz.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt2jcifzeyh.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2fjczrosq.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt2eolydqij.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt2tgvzucic.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt2sqfawjct.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt2ljcncwok.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt2jdxahalw.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt2kzwthcat.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ipwpvqdv.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt2rkmelaxy.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2vmbstmqh.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2kzjykcme.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2wwepdhqi.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2ydtqovif.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt2gwyrxphy.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt2cufyfbtr.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2ejjnolsg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cymicyks.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt2feqpagyn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fleppqxd.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt2ansgkqtt.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt2oggajqsv.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2qfzaheox.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2rqdgcprt.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2kyspglqy.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt2osyqpzjb.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt2zsbwknjv.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt2hwkllwjp.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt2shhzbjip.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2snmbrwtb.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2cbpkjrkj.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2iyasnqjg.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt2yalyxqsg.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt2rslsywco.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt2bueaokyx.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt2dzikxlqq.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2gufyerkl.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt2lopkycul.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt2nypzotfd.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt2feozmhqj.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt2lekgjsns.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2xivmrswv.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2butvdcla.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2oskipywm.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2pmyhpfbu.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2vmxlljmg.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt2dijxsugw.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt2rtawgaqh.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt2tsjufpqj.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt2qhhvzphv.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2jdheczfx.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt2opomsczw.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt2mbbimykm.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt2yckegkvs.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt2idioxydt.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt2lvahdogf.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt2fgdhhkzz.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt2nkllrftu.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt2vliymmfy.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2gzdjxhdj.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2gaqcdlby.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2vhgeopsr.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt2sfrecimp.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt2lfoaqqxe.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt2mblwzupb.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt2nsnyhbkr.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt2uqooqckh.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt2yihvlsvf.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt2gbxihcxl.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt2hfivizjj.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt2ajythafj.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt2irlfgqrf.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2ugquimuk.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt2jklvjlij.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt2zxwehrbk.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2dwiwbsri.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt2ermclzgz.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2rjbyhoxk.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2gkkpbucs.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt2tysrembm.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2lyjvqoib.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2tvhswipg.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2aatzpfga.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt2ftesbbdk.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt2byrarqnl.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt2thzkhxtc.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt2gzyvfuog.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt2vuwkuhfc.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt2szeyaklm.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt2bonuhokf.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt2aqnzaghh.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt2stvvcbua.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt2kzbpykkn.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2cvefjxkh.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt2vcttsemg.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2hgreqqez.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2sxocvnsj.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt2hpjgikgy.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt2rbneicrq.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt2oerkpplp.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt2pibnqjcy.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt2ycivhyxt.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2fvbngcpl.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt2fnvkkdat.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt2stgqihuh.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2iigzgona.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2tuqirdow.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt2lpvfadzo.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2kislfbhj.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2cqblisby.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2oxaldcrz.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt2bpzymyph.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2usrcvubb.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt2bplsbdhj.html


<!-- 参考信息 -->