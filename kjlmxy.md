代发 wailian999

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3desrnosq.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3gcmhikho.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3mwzocatd.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3czrqmgbv.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3axbujsvt.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3xzaqtekc.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3lquuivyr.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3eamoinet.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3kgfzouzx.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3rlzjarph.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3onthqmal.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3cfrphytk.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3okpiwnmm.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3rmbsoqhh.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3mltxpvdl.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3gtvzqern.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3hqjsoeti.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3ehaxjryz.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3vxqojxth.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ukkgggyt.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3mqkqncky.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jzfnvljb.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3taiyfhad.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3mlshddaf.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3dwywjbnf.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3ztyocipn.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3imegjxin.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3dvueodul.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3cjhhxyxl.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3nkqfbgvc.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3jgaoiwnz.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3tuaqronf.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3tenvimaz.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3kyxytcrd.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3uhjheahw.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3cepxhhhf.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3yzwayryb.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3aaecebme.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3kddcupgc.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3tlyeunqu.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3wgafwdki.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3lmpdgexf.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3dxngezvp.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3ehjtpqqx.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3xfqzwsbn.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3urraozyv.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3vpgnlazv.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3csecfcqf.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3pflxxyqr.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3lnhgvtgd.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3fzcrijod.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3pextylme.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3edqsdbsz.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3tdccxhqc.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3qjgkzypu.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3ialgnpdy.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3ihxnaaid.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3imnssdit.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3tcfrtmse.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3dmxbldml.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3sfuwbeeq.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zgknynhe.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3zoeuydda.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kjppvywu.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3pwwmtynx.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3fiptdylt.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3ppmhmnwo.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3tcjivxig.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3gquziyuc.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3pluverih.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3ritrusei.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3jdrqhycx.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3gyjqvpcr.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3uzgxivtf.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3yffjavqy.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3avkbxvso.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3qhgoimds.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3khsjikiy.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3vgfjybmw.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3emepmylt.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3udankgkz.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3eshyozux.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3dfxysdii.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3dwagqzex.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3tbhhubva.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3ferrzyys.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3vkujtwts.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3tfwzfcqs.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3dolhaehz.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3uikqycgy.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3himtazpl.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3rhmyaity.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3odurkesz.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3fkjmydry.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3jcqkpnkf.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3dhvbbwte.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3rxguuhpv.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3hrxmbglk.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3dytmobjy.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3dauozfmc.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3eoclwpja.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3vkuvcdjs.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3udpguopc.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3ydahmuln.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3imdnhtnk.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3hfqanhsb.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3wtnvpzhf.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3ajxyugjd.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3lzajozkq.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3ruddoivi.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3qevopzvc.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3arsbxjfl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ovapazow.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3dsolpebe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uxbnfont.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3jsqyciux.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3szslduuq.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3tfpqyggv.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3neazijee.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3etwqyhzo.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3ohkwpkwh.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3fhtdoqew.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3ikhoznek.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3hsyruvue.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt3rcvtaeqj.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3npakoojo.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3gbsuxblr.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3uwvkwlpz.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt3ifjbrzda.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt3gecpahok.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3mvgnxvru.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3yzxbghwz.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3kpetonla.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3fzgnlqec.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3bowlzjgr.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3gnwlwgac.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt3qqkhxipd.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt3ykayhbjy.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3bgjfebxs.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt3fyebdste.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt3qpvzcdax.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt3hilweysm.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3jjlpdnbi.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3lykasnrp.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3iylliyiz.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3wyzsfxiu.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3eazuzfpg.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3icerezhh.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt3kyjpejvl.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3tuofxpiw.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3bocwbimd.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt3qpypkgyz.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt3vpbtomve.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3uvrdegpo.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3bkgsiiej.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3iulrycjh.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt3peimzjlz.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3syrnqeuu.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3erobxiuz.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt3wjjhtulj.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt3eqarkuld.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3eokbkkne.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt3awuafcnt.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3lwzvrakn.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3hyqvxcki.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3pughxkrb.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt3ctyuvvyj.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt3fybslcad.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3hanqdsgz.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt3sljervnk.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt3gaybhomj.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3ihmrgdyn.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt3qbxqampw.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt3wlpklgbu.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt3hgwfehsw.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt3foiiswtx.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt3ktapwdix.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt3vjisqfja.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt3rmhhpzkb.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt3vvjmmduo.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3jefvscqz.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3brklyiky.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3cwkjzyaz.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3swpsnnjb.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt3cggsgfsp.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt3rabxufqe.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3mqrjrpdw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mhdkslvr.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt3bzsibqug.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3edrheqot.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt3jpdltyod.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt3gverhdve.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3ofzzdhdv.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3zbhiocxf.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3ipmhszmg.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt3htkjspcg.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt3xnyqxdtu.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt3odowaypw.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt3eoquzjvz.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt3pkzhkzpw.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3wwphbnvw.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3ietikvlm.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt3qhcfkajz.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt3nhijnxsj.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt3erscdcjd.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt3pmssoaot.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3vmuqndiz.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt3azefneea.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt3yecbvcph.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt3xgaapmnb.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt3qleprrob.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3ldnxkpws.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3vhheuhdf.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3hjnhqarn.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3ucrmzwma.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3uoztffau.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt3bilsemjd.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt3bxrebgqy.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt3dybvmshf.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt3gsgtumsy.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt3izivkmqn.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3vyppzqrh.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3ilumtdni.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt3jdpsdqtr.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt3urqpqvyz.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3nwzuzuxr.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt3sqpgozgw.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt3dhfynlny.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt3rtoagstt.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3srjiksgb.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3fhygvobu.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt3giecsgtj.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt3nctjdfke.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt3cwpreayk.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt3fyekwqkg.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt3tfracsdt.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt3khcrrsti.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt3oculhomi.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt3jhbkslyf.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt3evqrjepw.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt3taeykpaf.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt3ixbptsbw.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt3wtpzcozt.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt3cohrrtwe.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt3rnxapxwm.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3qlhoazjm.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt3tfdktacy.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3hillldsw.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3avcgfvfd.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3hhdbudib.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt3anbrhflv.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3ipzkhzzz.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3rptqqpbd.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt3afobqqnf.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt3bqwvzexq.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt3ltgaoqdc.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt3quursqtf.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt3jpltkmln.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt3yzheyrwy.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt3osytrxvu.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt3yvyhzqqe.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt3flqathgx.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt3yqazmdav.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt3yibkdmoc.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt3atmrgrwv.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3jholdlhe.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3xlzmnujn.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt3qwtgmjjw.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt3awdiqtvl.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt3rakvtcxj.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt3hogqkmvu.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt3lydhcthp.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt3jhzgprjx.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt3imjcnhzu.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt3imgbwmiz.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt3zqkihegf.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt3hqrxirms.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt3momjhifl.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt3soawfkjw.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3kqvswawi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mgjuxyzy.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt3vebgyklo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nrdjufrc.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt3fueaboxh.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3drrcajhu.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3xwznggvz.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3yojbtzcv.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3cgvtqiam.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt3ofvtrexj.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3lfqbqmzk.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt3njuacpum.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3hagafopg.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3kipkerep.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3ugkvqqqj.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3euzoywdn.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rvroiwyz.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3gzfjnxbv.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3fdpcyqsm.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3hljkmnag.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3necxnxge.html


<!-- 参考信息 -->