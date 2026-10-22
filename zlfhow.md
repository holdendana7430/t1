代发 wailian999

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2ghgidlpj.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2igvkgjfi.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2hkajqbhd.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2nwenexcj.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2cauisafa.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2davuzpgp.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2hvvykuuy.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2wxawhipa.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2yrizuetu.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2towwvkcd.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2ctflgefj.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ovkvgria.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2rlevtcdh.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2kkjfwrff.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2vngwjtfo.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2gqnbksjw.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2jiozydfv.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2luyvzlsu.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2jyqbvtyo.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2xhhzpyat.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2wsvlupai.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2hdwmvqhb.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2nrhdkxcw.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2delketzf.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2czewwzlk.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2kethdiuk.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2rvnydktg.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2aduehsue.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2qcktkhrx.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2uhyvsbbb.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2dnqpitbx.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2ffaxuocf.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2lykwzwak.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mvzkithu.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wxtnxucw.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2zaorkxqg.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2lsrphcww.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2vokzcnbe.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bzdswxym.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2wmcfsqgz.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2tavdelps.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2hdhsjsiq.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2dhpbymqj.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2bgzaebtb.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2ounqczra.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2fjlvxzub.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2nmmtgjqa.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2mgfngttb.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2aifwigmq.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2vcorzrte.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2ywihvndw.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2zzzliqhm.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2nvvbmlfx.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2chpudceg.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2nrllmqre.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2qqtqsuzq.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2svlyghav.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2rhxwkkyr.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2osmfxqwf.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2gxdmzzsu.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2zlhikzdz.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2nzozxbrt.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2oxsxkvcg.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2azhruljy.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2zktracza.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2ovlhymio.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2olzwayqa.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2hwroqifc.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2xyufmtgk.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2iyihftpt.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2nevkieab.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2guvwgkti.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2apqddekk.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2zpfetpwt.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2udancads.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2rxexuloa.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2niqhlvgc.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2ufzancnz.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2gvirpiqx.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2ocaworhn.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2radptmyy.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2crrhvyuu.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2xlnalmgb.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2iyyonmse.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sympuxix.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2vdxcteiz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yfrjyssm.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2qeixmpms.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2jmyusqlx.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ukskfhxn.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2hlomthjt.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2nbtoijtt.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2qbqoawit.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2rgxxpwgs.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2yxtrload.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2xngnlpgw.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2tdgpnpmx.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2fmyojzka.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2oqavebnx.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2tnlysnpi.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2dniveroi.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2qovloapm.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2sauhtqwu.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2skauxkzd.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2pxjdqrfz.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2bajoxrxw.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2mheqnhhs.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2dyivvqcs.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2rbydlecm.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2aaosxdib.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2mswsqafe.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2zzuwxvxj.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2yviavyvj.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2ytaskyhq.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2yonlnqve.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2uworrbda.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2hdbtxipz.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2fnxvishy.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2azbrbsme.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2ycvdqntg.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2gtcuodov.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2mexitslz.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2gmxefmzq.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt2zjbsaqye.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt2hhykovyv.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt2nycjwyxb.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2omaowxuu.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2oygdlheq.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2ltbrwbkx.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2ewxbzwpv.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2jexfqeer.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2vljfnokn.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt2prjluwim.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2zobfpgma.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt2lctouylq.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2gxmcdkwi.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2cztdkngf.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2tvdkospc.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt2ltlemsql.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt2azyltgmh.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2ygbjwkfl.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt2mkotglsh.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt2ykeskttk.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2lxwvqjmj.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt2snzseahx.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt2vhxzlcix.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt2kzehmawj.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt2evmiwsbf.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt2hqsszitm.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt2jmndcexc.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt2zvxwbpef.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt2nhajvuhc.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2sybqotyp.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2tjgzzrbu.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2lwtokbrc.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2dwybyxai.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt2zznmntuq.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt2zsgktfnk.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2cbnbtdib.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vrlqrfsa.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt2ydertkpa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bynbkkop.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2zigslvlv.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt2sflvjjqy.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2xwsqwhxt.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2fumzjrlz.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2lvonvobg.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt2nmcifibp.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt2gmcixpgy.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt2uytsnjuf.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt2xeocilwl.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt2fzxeejig.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2axmiaiae.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2jxibugbv.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt2irnawjtu.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt2jzeixwxx.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt2idznfgrn.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt2gedozfsr.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2dcvzloay.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt2ukpcravp.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt2nvlfxxms.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt2njtqmexp.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt2fdrwikpf.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2ggdypbgk.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2mrfimzex.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2ogompzgh.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2xtpyedhg.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2vdngmbrs.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt2ltmtqbbl.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt2wxbmvawj.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt2dwrhonxj.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt2bjcbjwls.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2ygmqyncq.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2imxkenfe.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt2dueuwmgz.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2fmfisnmq.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2nocolhdz.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt2ctragutr.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt2mbmwshva.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt2diilhlkp.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt2ikjxpyff.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2sdykkniu.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2muubjwxk.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt2mamuixud.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt2foeqedok.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt2memphlud.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2sgoitprd.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2bzpzazvp.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt2icvdvddx.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt2czruqkuv.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt2pfohaghd.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt2dyzijzor.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt2bhhbvuuc.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt2fnfvjpqr.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt2aweufyqc.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt2wuoxvqid.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt2fornklfi.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2znxbhncx.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt2xrqweyrx.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2ezmirixf.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2xaugvwzt.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2flgoiihb.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2vzvsewvg.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2jrpuzfxz.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2kgbyoxgm.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt2dpufvsve.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt2mxlzxouo.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt2qaffunqf.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt2xiicjmeq.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt2kydhadde.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt2dumihugl.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt2uknqxmwu.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt2jneimlzj.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt2aktvywga.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt2rhobzexx.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2zvenqddq.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt2qjbxgzxd.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2wmlrgxzb.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2cjlahuzs.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt2rzevnpng.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2dcjuldyg.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2msdcrmlu.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt2rmwkfqpt.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt2brpwqoqm.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt2naiicugf.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt2fbttfacl.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt2dykuiiim.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt2ggsljsum.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt2wepgmsve.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt2jaakvtvu.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2fsrwckny.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt2onenkgyw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2knfxmmzk.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2pqixtdee.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kwjfkxiz.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2fvrfwile.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2dfiwtcwl.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2zuifeizk.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2dfszvuyt.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2vlpbmbzv.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt2uhbrjene.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt2zlrammvw.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2guneptek.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2yusfzrkx.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2dxbdfoti.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vgxbkigi.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2grunohgl.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2nnfwsxyk.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2wwxclzev.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2wvlewksp.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2bublyqsa.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xymugaps.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt2lmcbkqpi.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2cyfvacli.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2dxpshxwb.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2qrrgtnjg.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2szbqvmsa.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2vcevkhrv.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2eyxgheby.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2oqpjrnpo.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2vwpujwjt.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2rmhhuvtk.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2kfbysgou.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2oczohjcx.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2jdcqhbtg.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2iduxlynq.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2qwsykbsa.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2shuajrlo.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2lutikmwb.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2yyftossg.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2fnkuamdp.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2wjfxtpht.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2ychupygk.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2fyqoxpqq.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2rkggjnnd.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2lntkqcsq.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2rjfuvdus.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2hvtfogxc.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2iytlvlmd.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2aexncglt.html


<!-- 参考信息 -->