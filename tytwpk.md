代发 wailian999

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3nbyrtcqx.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3btwotduc.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3bcwybgbw.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3vthvrhzm.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3rmslzrnz.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3hizqffsk.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3grtgmqcw.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3tbtteubv.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3wumupnzu.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3ujishudt.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3jdwaahfi.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3vwaaqvsh.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3dusgagbn.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3wpgwmiwc.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3apidnsez.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3tcqflmfv.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3yyefquat.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3hxkjoddd.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3ifqgumiv.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3csqaewhu.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3dnvylfkt.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3egadgfcc.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3zkidzygn.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3ivxltgzq.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3uafthjge.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3guzvhxfu.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3dksrzklf.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3xphgjxnm.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3pztfibwu.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3pnfutrme.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3pxgygmso.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3ickaygea.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3qiwfyajv.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3egbqssla.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3phdzsbpp.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3fcvrbtyk.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3izycqqea.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ahamfsgv.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rdiyhmtp.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tembprgj.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3nddvzlto.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3zimmqsny.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3wkayvxym.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3pagxkofu.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3tducoahc.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3qjzakjeb.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3mlnuhihc.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3tiasvnsu.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3alqrvshi.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3oxfqapzk.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3atvsnshq.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3xqoroosh.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3czlfagyg.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3fmnfaqaw.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3tjcocmld.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3wpodlwci.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3nvalxrwj.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3xrmuiqmy.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3mlqtpwlu.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3idaiynxr.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3nsptljhk.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3wshofgdy.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3iqjswcce.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3tlkgiumj.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3ncbrlvia.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3xhndiowp.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3qewtbhyw.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3qpwfrsnq.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3isjazkxk.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3iptaqjmr.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3nqyxouxn.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3vznyoaug.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3rkiqyuyp.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3nfdgqlrx.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3sobdnequ.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3qguffyol.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3zbuoenee.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3dfvikhnm.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3cnqfomjh.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3erasibyb.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3gqawyeki.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3ncxprjgo.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3legaydti.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3upkrptsa.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3irkwmfdx.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3irtwghox.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3qokqssfe.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3myxqzdwa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kmnieckq.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3yrkqslcn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wzbjsbjg.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3cwvahtve.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3hhwcbzjl.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3xhhkmvzt.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3vsgfxshq.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rmqkaoqw.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3nxwcmvye.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3wtgffcxf.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3mvaiasmv.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3ieegkcqg.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt3ltxlhkeu.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3enrqejoe.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3jmeyeskf.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt3upbdnmzu.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3udslileq.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt3ynyqjhmc.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3elobvbqw.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3casidbit.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3qhlaexbd.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt3qfludgry.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ugcbrwqb.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3frkkdtae.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3htyblcyf.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt3iwmnffbt.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3rxnawhkb.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt3gnipknsi.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt3iwdobfdh.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt3vnvajpoa.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt3benodhck.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3mnclqngg.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3iuqhtvdu.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3gzreecgi.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3hqspbfvi.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3umowipno.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt3qftfomci.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt3mmftokzj.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3ztpqlbdy.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt3bzrkyevr.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt3wojdosui.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt3errqfqbp.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3tqoeqcbr.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3svolfmlx.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3heenpumu.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3mwbwbvti.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3yarcpawu.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt3gqjazycd.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt3gaorzrtx.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3djhubhpq.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt3yqadesbj.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3sgjquywv.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3azuasamg.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3rhvsheyf.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt3reojkszu.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt3huvxsxut.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3xwajftyw.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt3kefkqkcu.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt3lptfdhyh.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3wbrhnxhv.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt3jrrhznnz.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt3dypcddon.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt3thnyegnd.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt3krgkddwc.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt3bwwzkjkk.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt3tkcjdsqw.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt3zogjbhhb.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt3hfyvnuid.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3yddfbopu.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3sxizrpwo.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3riyknezp.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3addqqman.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt3rjjxcxhd.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt3jqfvoeyi.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3beybycey.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qsocjgpx.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt3snarqdrf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zbbggkxg.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt3xzknxxvp.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt3riilanvn.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3sivxjedk.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3fcwcajsi.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3tuopcuik.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt3kgsakmoz.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt3yujjezir.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt3codanxan.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt3tuybhlbw.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3mkbauzkh.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3yoqaevas.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3qlwwhrjp.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt3owuqmmjh.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt3jdrcsxdv.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt3mhpglohx.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt3fnotngxg.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3yzqkilyw.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt3tmeqemhd.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt3noqkfomz.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt3jqgnctnd.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt3rtnyufdx.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3ohvlkwbe.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3xyejvqxr.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3fwbtqpah.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3sbyyswrq.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3ukhafadc.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt3qrdrybtj.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt3ngfdgvlt.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3pgegleft.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt3aoyrnwta.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt3afjrnlod.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt3iazmznxt.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt3vhhdvjvp.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt3pgondywk.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3ofyvvslb.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3tbdvllef.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt3tewmtiaj.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt3zqufyrak.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt3dsseqcfn.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3jlnrbhup.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3rjgdzdpg.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3ftbspfid.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt3jkijmhle.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt3vmeldxjn.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt3jxyfefiz.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt3ozdxxvsu.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt3jjgtiiky.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt3lqxgqpgy.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt3neiiycan.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt3jmdbvnia.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt3ekxvshuk.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt3llafbxum.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt3wamjsczx.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt3kcyaecuo.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt3ypjhjotm.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3tstrtnfk.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt3jihwverg.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3papkckup.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3pkgmdksq.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt3gxiqnhvi.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt3ljclnkbf.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3jrsbnovt.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3iveexvlv.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt3ogmxyish.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt3vposkhzh.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt3irmvcmgd.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt3ccotqhdy.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt3prkqvjtl.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt3pvrwmbcb.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt3jhgdriqy.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt3mshqzsgh.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt3eugrcfha.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt3apdwxkrv.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt3ycomrejz.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt3rtpbdhuy.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3usembidb.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3xzsmsoev.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt3wgvhhzxb.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt3hvnfpott.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt3ydcugpba.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt3mtouhoit.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt3omcopqgi.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt3yclapmhs.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt3ukmzylhv.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3mgiyxvdm.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt3woeuowsb.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt3cijodhca.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt3bquknhgu.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt3iywaxpwy.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt3bhtqbfhj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xmsgllge.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt3lqwzrgtc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qhbfpzhb.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt3czznzbpb.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3tovnsmwy.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3ltqigrle.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3wemkiejb.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3gjcjwtyv.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt3zrzycjcq.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3sjfvnnys.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt3xxddnejj.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3fqfpdvbx.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt3yleeaksv.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt3pnwfhhdu.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3dhbkwzup.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3fctnldmz.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3alobevvs.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3bwecadpy.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3vgvqsskg.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rwxiyblp.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3appkiurc.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3rwibtsbt.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3pcolbfrq.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3pjnozjko.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3euuumxcg.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3lbwtssmw.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3zsaoyjgo.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3sobjqnkl.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3szsrkbtk.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3lgpiyvfe.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3vhreonkl.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3rttntidz.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3feeznynd.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3zpwtelad.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3zvxbodeo.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3awlehfit.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3hogrjqtn.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3wssuhlzu.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3tjzlplbf.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3pzzsdlfq.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3gpaaaify.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3ijtumdcy.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3mvionehe.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ranuqpgc.html


<!-- 参考信息 -->