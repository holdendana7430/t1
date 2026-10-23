代发 wailian999

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3fbuwhzie.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3eiypydgg.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3pqhwwesa.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jutomxwd.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3icopeeku.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3jauexdmg.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3rilkmged.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3prveykgc.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3ropfnvkh.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3jnqxouys.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3qemntmoz.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3rhkrfkjf.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3qtpugpel.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3vioadldq.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3dzqtghef.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3yjlgnrhv.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3ileehvtb.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3pcpwanea.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3tjbmpdsi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xxqwytjg.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3gtmuuijn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lkdenemt.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3uzhcsekm.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3inqtmjxi.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3wznqxvsu.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3bdhagazq.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3bnghbcfi.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3wbcfgrxm.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3dnngdaos.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3zxovzyyv.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3inguptbb.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3zbfmrvap.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3ljorbnfp.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3rhampena.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3elplgavt.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ijsikhyo.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3kydgkmxg.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3lahfffng.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3gxvtzphx.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3ixhbkqqn.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3kfnvfnya.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3xwkngdpu.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3jnihcnhn.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3cmexiadr.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3ucimpljn.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3ddezaxbk.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3hdkaubpb.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3vqejlxnn.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3sqfrkqbb.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3ygjqojpz.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3cltqcimo.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3xvqboske.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3vrvogvbb.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3smvrlshi.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3odfabzac.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3rcarower.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3cgjpbatw.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3ehudcvlg.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3vbptcmia.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3zbcjuoqz.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3kpvfeoup.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3nobevsoq.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3gnmrnihk.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mckwvsfp.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3dhliuxjc.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3qclmpytw.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dideqbsn.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3rfebbdhy.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3auwajnze.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3ztfglywa.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3osmrixxe.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3fcmrfeks.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3zeadgwfb.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3srivcuis.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3fqdwqrmv.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3fuwckzsi.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3erqkmhcx.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3fgxjfzzm.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3fmlczefh.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3mybvhzje.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3jfdtghog.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3spcrqxwq.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3ohqfdvar.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3fzpbamqd.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3auzvtsnh.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3gutxrsvo.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3eyocodcm.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3ugpqszsu.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3hdmmdlfu.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3jlqnsgax.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3kzrqcdsh.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3dxhtyege.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3hixczzlw.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3leakreha.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3hybpnatm.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3uwfyhdbd.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3mgyslakp.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3dxextiij.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3vlmgkqwy.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3gzpzuekg.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3hwvxalol.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3cblocgms.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3ymsdwhnc.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3drmmrqjg.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3wsosvhtk.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3gsprjamn.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3pqavtvzv.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3kjfmukge.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3pmgevjlm.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3tfqmizdk.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3hrrumhcl.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3flyyepvd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3abmsypxz.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3qazvyhus.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fdoyhwqo.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3xhtqvnui.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3nqgrhonh.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3suenadeg.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3exevxfdc.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zcxnxskw.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3txcdgrrh.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hmzttcop.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3mlhvopza.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3kzcjalxl.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt3fpsuhgik.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3uvxijwhg.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3ifxmsswa.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3zmolwzda.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt3itqxsmkq.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt3ebejhidf.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3yoapglix.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3fvgwwetn.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3ajyzawve.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3zknaserh.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3okqwdkas.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3alxnavqn.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt3gqtwknds.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt3twjmvngv.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3gwddweyn.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt3hhyenyvi.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt3ianxxagp.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt3fecgaidv.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt3bopnxexi.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt3bdifjkxe.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3bzlwqret.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3lhzhihbg.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3ahmipudq.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3pisfqkxl.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3aztmmhgi.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3kkkchizw.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3bbbihxqe.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt3omqstebf.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt3xwqpglna.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt3pigpdftr.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3krmqswkq.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3efezvqjm.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt3exiibeqk.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3dgjkvhrr.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3dfwwaigr.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3guvzzwee.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt3douhpcov.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3oqybirap.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt3oqvllqku.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3myhdchoa.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3gokbwisw.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3qlvznety.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt3fewrhzsz.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt3evehzpdq.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3tmjxiifi.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt3lkbcwirh.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt3zsceektc.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3nhnjmyxe.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt3ubsnxtzd.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt3ghsujrlb.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt3fiszlkxh.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt3qygwmxpd.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt3tnwhzfyt.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt3qemvetka.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt3jvfxpxcc.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt3qwbdfwpj.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3eocbraaz.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3ecofsgme.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3qjkqbzva.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3ygydsmtq.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt3qbbfsmke.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt3htprfyyc.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3bwufovey.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iofxmxrb.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt3vdjvowez.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nxfcjqfn.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3dhgekhrw.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt3hupfojst.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3uwxcxyga.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3fhtggsba.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3jtedtpfs.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt3ozjhaknf.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt3vxmyxxfb.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt3uvcenlad.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt3offnujcz.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3hziqeyxd.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3ktsezmwf.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3uouwnpep.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt3mogpidio.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt3eysembqv.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt3irdxrmqf.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt3cvbwmjpn.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3xeodopmx.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt3kshlsndk.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt3fjhwzivj.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt3ensgiisi.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt3ytzjauci.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3wsuyenpb.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3kpxsxtyr.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3jarodhak.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3hhvbfcxo.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3zxccnewp.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt3qrcqlssr.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt3ziplwfte.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3tkflhfzy.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt3ousmngar.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3zuqazawr.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt3nzhdsrkk.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt3sfdxqfmu.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt3sedhrrbm.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3lbqkookv.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt3rgbkrdmi.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt3qlvbpotd.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt3oisfdfgh.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt3hbspwtgw.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3kdukvpth.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3ekanlglq.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt3uafnsbrv.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt3yarlurkb.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt3iizuikgh.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt3mkswaibx.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt3anzpzppg.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt3dffxnequ.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt3iaiuczcm.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt3kdakduwl.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt3kzenqfns.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt3rryumrhz.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt3pjnilsga.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt3mmcxbtnb.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt3amnxjqww.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt3llrgepdm.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3ekcbztiq.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt3bntsqzzm.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3raushsmh.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3hvdmtise.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt3aiyftppf.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3zrtpsrnu.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3vzvtpkbk.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3uaawrqtv.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt3uizvsrqc.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt3fnrjpvkj.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt3exyvzjif.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt3iegddees.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt3cbvgcukr.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt3vyhinmky.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt3nkdkijnz.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt3pbpuoztx.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt3goacszrz.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt3gjmhcsna.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt3msbazgij.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt3gnzdxdbw.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3oolliunz.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3cuazirsi.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt3nzxzncit.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt3kmifxtic.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt3gftxgjqd.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt3jwfbwzlb.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt3wgwsbrlb.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt3yfiahont.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt3uqsehmcn.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3zglbcpvd.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt3zdloggtt.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt3rquusapi.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt3rvlptsci.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt3pnksiggz.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3irrxagtb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3irkhqutv.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt3lurkxahz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rjklribo.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt3nrdkdmfq.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3uqphadke.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3iyypfnkj.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3knbmknik.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3zcdiiydc.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt3abgggzuv.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3lxdbyiat.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3ozurkrkq.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt3rjwowtfa.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3ocghtuwh.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3bbeivpdx.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3sihcwcfb.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3hrifwrge.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3imnssyyu.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3annaygwv.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3ltagckfl.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3vnbiktyy.html


<!-- 参考信息 -->