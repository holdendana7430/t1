代发 wailian999

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3sxupoxbr.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3tuebomew.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3pofxfuuv.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3emlfaqbo.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3qewcgdwo.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3xpvazhyb.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3ybjyncpw.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3rutzmlis.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3tfruhcmz.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3xpljcvlk.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3fuociihb.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3dqkkkidk.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3hddnjubq.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3jdkpyrob.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3afluuobq.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3mnmqydsv.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3zzwikcqq.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3plbtefcu.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3fbyoaktd.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3jkhcwkbr.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3vnnucohe.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3pmcdozki.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3bgtestuz.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3mfdidbhg.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3cvijpnsv.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3wailkrec.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3symoatro.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3wlptfwwv.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3ihtvxbbo.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3plluuifz.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3arklkajk.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3hksrqukx.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3ntvyydfw.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3rhwuxqkk.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3fnaqaorb.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3obvaxmpc.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3ehpcrlaw.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3wugtwsnh.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3qvsfpxqj.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3dlmtrpsl.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3obqsdlll.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3sfxwinnc.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3ougcdoku.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3mqwkqiak.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3hpgexxmv.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3rsrwgayo.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3dfnaxrhr.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3cfuckbgc.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3idulbrwd.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3fehetlia.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3ruemcdbq.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3czqqpwrt.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3qmwqweno.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3lbtivmlt.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3hwroqjqm.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3mtmakqwn.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3joxassqi.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3jdyuhdof.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3sviscyzp.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3ishfyier.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3glpfuvlw.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3otrtmron.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3mujysniw.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3qugiuggj.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3yyprrqpp.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3cziuqcet.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3kohpeqsz.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3hyvyemtg.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3zhczxwqb.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3nhzmpvvr.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3mzpirwtg.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3vadgcarj.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3hgnuccox.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3oscmyhci.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3arjxmwew.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ioyridua.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zogsjqmr.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3qkxiykvj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3brxndjjr.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3gztnwvjp.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3qgpnnktc.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3azxandmw.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3hmbznmjb.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3jumnurid.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3vegmrbco.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3jiiolpwv.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3ejywuqay.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3htmrksat.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3rziznvgw.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3obybshmp.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3ulxstqqu.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3aqbdrvmi.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt3xbronlza.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt3sorjeewr.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3duacdqhg.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3cfakywxf.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3vqfjiscd.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3xjzxnsno.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt3zlnmhpgh.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3kytcxqrs.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt3aqgomqhv.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt3jusnyqza.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3wjzcpcac.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt3geggrmwk.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt3xplzfydw.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt3enfxlwwj.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt3wfgqejeb.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt3vphzitcw.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3jnpkcnpp.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3zhrdxhhg.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3gslloxpw.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3hhcpckbd.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt3mmjnhfrh.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3dqmivhbk.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3zhtxxqiz.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt3xgsvqnbp.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt3abwbuiwu.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt3agnvqxxm.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3hmmujrxv.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3gjbaxhqw.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3qtuybntx.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3kmlqsqks.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3xqmtwbma.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt3qsylgfre.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt3rzmiqwct.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3rldxaaus.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt3zsnfguur.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3xfczafvh.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3rqwtsosj.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3zdwhehpa.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt3yoxbsoat.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt3wibekgmh.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3kxvtsqot.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt3sfnybxxx.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt3ccoyhggf.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3ltftruvv.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt3eivnxpmm.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt3qxxkyosz.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt3edcpqrjy.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt3gytcsddb.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt3difpcaxu.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt3leveuazg.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt3fehyllai.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt3kosaqxti.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3gerukizi.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3mtlduokz.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3vnjmkuwl.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3frkmmgue.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt3lbpzpudm.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt3oqydbjcm.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3zxgfpbvx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3haylkaqq.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt3rezqzicu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3okkaqyod.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3oodsgtxq.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt3foioalkv.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3kjrzibvk.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3enlgpwsh.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3ooggsrjn.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt3wtxexeyp.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt3mujcumoy.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt3wpintjoh.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt3qtdumigp.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt3kuhdiqva.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3cacewsxf.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3xcpgkwik.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt3jsfvsdau.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt3vfbtngff.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt3xjmebcpi.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt3mlnkckjm.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3qrqwjgey.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt3tvirlgsl.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt3yvkgvgcq.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt3trmovtea.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt3lzomjwkh.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3nflsrhmq.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3uuwdfzxq.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3rbpywnol.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3vclcvvel.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3bagdquox.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt3kqdauqwm.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt3aiuyffge.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt3ntdknppe.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt3axfotnbt.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3zoditkgc.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt3dzmxzuym.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt3snswsclh.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3fpbvikvs.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt3yogwxtyk.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3tjiwyanq.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt3tmcznqid.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt3njpumliu.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt3ctgoxthw.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3usylxegp.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3nklqjkrl.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt3majzwwlc.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt3dndfeqbp.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt3zxhkhuaf.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt3iuooclow.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt3wpqatcgy.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt3kcvqqxov.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt3ibhwrkiu.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt3vhieixfi.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt3myfgrvnr.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt3dgyxxipr.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt3iimoziyv.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt3zsfesaul.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt3gyosfema.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt3ysscsizn.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3vwnnhbsc.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt3wmiqtgwe.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3jdrpvcrf.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3cggwhwqd.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3tmdcwkhn.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3oilmxzme.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3tjbntsqs.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3lunzvnsp.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt3ecijtcam.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt3guolfrtl.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt3jyveobtg.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt3idztgicb.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt3hqwggsep.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt3guveiwnz.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt3zpvmqldi.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt3qsbedoth.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt3awjllszl.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt3vfnwfoed.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt3vidokavp.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt3cokmduqe.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3awffqfyx.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3ywijlgij.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt3qbtwekfp.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt3dubyuehn.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt3ecltiwye.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt3odzmfxax.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt3liclorfu.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt3balpjjnk.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt3pfjegtvy.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt3gebnhoqz.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt3jwxolzfm.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt3qbdmgfnu.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt3xkaqccxi.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt3rpmbtfcw.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt3fdytvgxm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3czqlscvf.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt3jcttdbsj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zjknlyik.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt3hqptqmea.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3odxitjdw.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3niprasip.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ecnfxgaz.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3erjojnum.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt3fsmftfjr.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ktutdlco.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt3qpwbgchs.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt3ibxqwros.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3obydsubx.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3yjxgkekb.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3gqywgkko.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xqecoypd.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3lzgyjpvj.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3mhmyeqii.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3vhdxacka.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3awtvccve.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3kqvlpsgz.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3qsbwxjbi.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3ebcltwkt.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3mkqanmxk.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3mjsqmzrn.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3gjqpnpth.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3cchzresr.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3yebudvjh.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3pxajwpgo.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3kcyvntjn.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3otgwyymt.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3ahszjdpr.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3lffwwpdd.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3pnrvwjxu.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3tfpojhgi.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3qjjgfjss.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3isptwpbu.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3opzlinku.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3zdhgcubf.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3kkykbvsh.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3goxihxnn.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3deanjcbf.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3acngvsla.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3uusthgei.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3xqluuanh.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3cekaesns.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3cxuqievl.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3xtetncni.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3qbhjilwz.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3jtybwjfx.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3kzqdbsue.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3zpxooknz.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3pnkswatg.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3ewijhuaw.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3lpaoarem.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3yrfmqklf.html


<!-- 参考信息 -->