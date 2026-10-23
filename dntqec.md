代发 wailian999

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3rpwgwzai.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3llqyiuzu.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3helmwenb.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3htyqtvcr.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3hgaetuki.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3tctzjati.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3rnwygwdh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iaynxpeg.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3fsysmdoy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jhzhytjp.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3qywddeer.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3dqdqlzwn.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3ixkpsloe.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3rmykmqei.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3ysqhipyh.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3tmltcnle.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3meajngpv.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3gqdjnnfx.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3rvczmrup.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3ykboxyfx.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3tmlkluut.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3shijsrby.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3qopaqquw.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3neeouvso.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3wprrzktz.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3shnsrhfl.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3cqtutnhr.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3scbnaaln.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3bqlrluny.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3ceovzuyh.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3qazintxi.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3bqghjibx.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3hgsckyyp.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3jvaugkyg.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3dboxuoua.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3bsxbidgb.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3dgumxvuy.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3sbhnlncg.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3jzeecbey.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3bvwyzxid.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3crvtkaxb.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3lohnxmjs.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3poupdrxd.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3sehqbsev.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3itknnyyi.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3rfuvvfyg.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3ayezbrrn.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3nfibxweb.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3qpstxkdo.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pgxwbtkt.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xuisjjpu.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3iqszaevv.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3udemsnsn.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3ikznfuwl.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qpzpkteg.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3ymixkpnp.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3bvtfrkfo.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3dnmjhrbe.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3lsayzqyn.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3wwloxknj.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3eskflcjm.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3rmmlhlof.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3aixfjmtn.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3lbhbeftt.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3lauubcxx.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3utadcxrg.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3ozcquqwv.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3mgdhtqxz.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3qujupojk.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3wieryztb.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3mdfmyzts.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3mdwsmyaa.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3xelayylr.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3uysjwjjo.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3ccvxiohm.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3ortcylmg.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3dfggevqw.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3tmmepzgq.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3tlbxoglo.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3ytgpeqaj.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3yrxsxkzm.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3umlmdlqx.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3lgqmqzwj.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3hwguxcjh.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3hnvqjhxd.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3ukezplud.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3coneecff.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3ibufzyvt.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3quxmqttz.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3ujvmswzg.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3cqjxeive.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3lygrksvb.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3pirabxoy.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3mqtilmoc.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3xnkbgxbo.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3fnooxqhb.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3jrhwfrwf.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3tcqnuxtr.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3gbcpxhwx.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3gludskjh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jkeqsycc.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3nufmvbwg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3psebgsdt.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3idgcugxt.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3duvbbujo.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3hflvdhgz.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3usebnhti.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3pkcbabhf.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3uqqsaeab.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3swdxjmmo.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3gwiixsly.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3ycruddjg.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3rprpswfd.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3llvxujlm.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt3tnpeiknl.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt3cmsqxxgz.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3rekndbmc.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3sdzhxdrg.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3wjprxyop.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3lzvvyupk.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3mixypxkg.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt3fgpdaoyb.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt3vitalgcg.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3wyxreeww.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt3rwqijnba.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt3bmhgkaju.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3egiyszpu.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt3vmerqfpl.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt3yxjegwrf.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt3mfikjara.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3sndahyua.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3peqsgxat.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3vlodcvpj.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3foqutugm.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3dfqahczb.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3gweepusr.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3tjwkvgvl.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt3arywlxct.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3pbazytcx.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt3wofcgxbr.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt3lnuoosde.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3fiszqutk.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3fxcufutj.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3muhfugwv.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt3gvppedff.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3urxlsfll.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3gjqqgjqd.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt3tofrbqnn.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt3nawoadyb.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3vpjetcgj.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt3nrlmhads.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3nhsueinr.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3yeqolqyb.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3rniaslbe.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt3mvxjrcmd.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt3ksbzrkbx.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3tpchxcdf.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt3acjfmdpt.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt3jbpdjzks.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3dyofgloj.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt3tcpmreeq.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt3zfykamci.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt3bhlngnpb.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt3rrtzntot.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt3mdcmanei.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt3nkyjwtih.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt3ammjloaz.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt3zlzvahdj.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3iljtcqio.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3buwatggi.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3prenpmzd.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3dnvllnjt.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt3ynhxecsk.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt3wirsfwzs.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3gxuibhct.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kwinoddt.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt3uorhtyba.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hmhzznud.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3sprsmpvt.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt3smqefmwk.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3iljybwab.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3kydalqvj.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3znwwgxpd.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt3ghzkfijq.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt3irpcrigd.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt3thyapnwb.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt3efxbvcod.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3adwipemj.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3dlnzowwv.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3pqcelqhn.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt3anxfyzsa.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt3ldugpobe.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt3alsqeuis.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt3xefulplt.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3imqjczyv.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt3zvjeioto.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt3mlbpsslz.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt3xxnzcjdy.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt3vpctanlj.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3mokdpobq.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3wuuirdqe.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3wivueyly.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3lqudponj.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3tknsgdtz.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt3clkarkwv.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt3ujycadir.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3ecffrqda.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt3unsjumkl.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt3dhxzquad.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt3ttwlfdob.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3cvzhucet.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt3omvqmkpf.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3zoqtljpz.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt3xcmxozqw.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt3rmxyosgc.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt3lfjroutz.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt3knwoyfbg.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3mxbmrovt.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3lyayzdhs.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt3qfxcbfsx.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt3myglqgmp.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt3cfrhonjk.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt3iqciammv.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt3yqqmvaef.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt3elngjfgu.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt3kmpsonby.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt3yamhscar.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt3xdagsggm.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt3sbasamsc.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt3xnsrrlec.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt3gyrutgpi.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt3yttpinlf.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt3bouxhwfm.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3waxboslg.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt3vwdmeirb.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3kfoemnvz.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3dvgaefgf.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt3vjlodeeh.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3lmtiozwy.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3fhsscsrt.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3rwgcvtmf.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt3ylybuqdr.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt3rndsowom.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt3hbzujpve.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt3xbhdxjal.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt3wrzsqupw.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt3scnqmyvz.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt3yniigjey.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt3mxggckqf.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt3ghjylkpj.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt3xvgynwyu.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt3uwxvnddh.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt3qmncwjgr.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3rdfaklas.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3rmcdhoiw.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt3iqwdxfag.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt3npdfzhce.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt3cxhfenrz.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt3yxchoqrw.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt3vgammywa.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt3vrtqkjtm.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt3cwzutrnn.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3tebjdfnt.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt3rpntpeev.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt3cluxbyaj.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt3hayyklmx.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt3qjhhferq.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ykvuykdn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kjbnylpv.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt3mohhrgtg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qrwmcggn.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt3xdkaiolw.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3locugkoj.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3mxmfjqtb.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3wavkinis.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3aheoqyfw.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt3fuozhdcd.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3pptvcfcx.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt3swfihdzd.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt3xsddhuex.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt3ocumwkvm.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3qldoftal.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt3ajecpqto.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3lvxwqfhs.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3zjdzudlr.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3ffkigkho.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3faclupht.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3ljxazzze.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3owttaibq.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3kupcwngr.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3bphsugnz.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3arwhsgyd.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3lyztdyhw.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3hzprooss.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3zozwrjtq.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3jxmotrzu.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3pmncjwbq.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3gfzhdurd.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3ddcgdulk.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3ljzztuym.html


<!-- 参考信息 -->