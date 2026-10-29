代发 wailian999

JS:   class MyError extends Error {}
来源：http://www.blog.zdbjq.cn/Article/details/guifphukg.sHtML

TS:   class MyError extends Error {}
来源：http://wap.hesvh.cn/Article/details/gaqrtvnim.sHtML

Java: class MyException extends RuntimeException {}
来源：http://wap.hesvh.cn/Article/details/gtaaxsapn.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.zdbjq.cn/Article/details/gjvkmneog.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.hesvh.cn/Article/details/ggxoayzdv.sHtML

C#:   class MyException : Exception {}
来源：http://3g.fehbvm.com/Article/details/gwuadslea.sHtML

[H05] 捕获特定类型
来源：http://wap.zdbjq.cn/Article/details/giflhirfq.sHtML

Py:   except ValueError as e:
来源：http://wap.hesvh.cn/Article/details/gvaakdqei.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.fehbvm.com/Article/details/gfuhoiimb.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://m.share.fehbvm.com/Article/details/gfgikrltl.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://baike.zdbjq.cn/Article/details/gowdkzunl.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://blog.fehbvm.com/Article/details/gypmiuhpi.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mobile.zdbjq.cn/Article/details/gchcuhios.sHtML

Ruby: rescue ArgumentError => e
来源：http://read.share.hesvh.cn/Article/details/gzhjsargx.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://blog.zdbjq.cn/Article/details/gnawkddnr.sHtML

[H06] 可选值 / 空值安全访问
来源：http://mobile.fehbvm.com/Article/details/ghsacfexm.sHtML

Py:   value = d.get("k") or default
来源：http://baike.zdbjq.cn/Article/details/gfcowklim.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.hesvh.cn/Article/details/gyoowwdka.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://read.share.hesvh.cn/Article/details/gsmaesqie.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://wap.zdbjq.cn/Article/details/gbqbbdfpv.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wap.hesvh.cn/Article/details/gghvdkede.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://m.share.zdbjq.cn/Article/details/gmdtpnudw.sHtML

Ruby: d&.dig(:a, :b)
来源：http://blog.zdbjq.cn/Article/details/gchxaabqe.sHtML

C#:   obj?.A?.B ?? default
来源：http://mobile.hesvh.cn/Article/details/gpqqmwfmn.sHtML

[H07] 断言
来源：http://baike.zdbjq.cn/Article/details/gmjqdtjal.sHtML

Py:   assert x > 0, "必须为正"
来源：http://3g.fehbvm.com/Article/details/gwylrjjln.sHtML

PHP:  assert($x > 0);
来源：http://mobile.zdbjq.cn/Article/details/gapsiaxjf.sHtML

JS:   console.assert(x > 0);
来源：http://www.m.share.hesvh.cn/Article/details/gxkoliaut.sHtML

TS:   console.assert(x > 0);
来源：http://3g.hesvh.cn/Article/details/gcespnlip.sHtML

Java: assert x > 0 : "必须为正";
来源：http://m.share.zdbjq.cn/Article/details/glwbwsvyp.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://read.share.hesvh.cn/Article/details/gtbuwywdj.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.m.share.fehbvm.com/Article/details/gxfobecjj.sHtML

C#:   Debug.Assert(x > 0);
来源：http://3g.zdbjq.cn/Article/details/ggpxkpbts.sHtML

[H08] 获取错误信息与堆栈
来源：http://blog.hesvh.cn/Article/details/gwmhsgnvc.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://blog.hesvh.cn/Article/details/gbwiqtgna.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mobile.hesvh.cn/Article/details/gheusgkbf.sHtML

JS:   e.message;  e.stack
来源：http://baike.fehbvm.com/Article/details/gygimhhdh.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://wap.zdbjq.cn/Article/details/geccrzizr.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://blog.fehbvm.com/Article/details/gatjqcsob.sHtML

Go:   err.Error()
来源：http://www.share.fehbvm.com/Article/details/gmqdpedmx.sHtML

Ruby: e.message;  e.backtrace
来源：http://read.share.hesvh.cn/Article/details/gynnixhwn.sHtML

C#:   e.Message;  e.StackTrace
来源：http://baike.zdbjq.cn/Article/details/gvljnvulg.sHtML

[H09] 带错误码的异常
来源：http://3g.hesvh.cn/Article/details/gecsedzrl.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.share.hesvh.cn/Article/details/gtgujdzfp.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://m.share.hesvh.cn/Article/details/gzsxuxgkd.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://3g.hesvh.cn/Article/details/gcacsoqiq.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.blog.zdbjq.cn/Article/details/gfxqagott.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://read.share.zdbjq.cn/Article/details/gcdcdbmsw.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://baike.zdbjq.cn/Article/details/ggkvpeefh.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://read.share.hesvh.cn/Article/details/ghmwbfipk.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.share.hesvh.cn/Article/details/goiydvnpd.sHtML

[H10] 资源自动释放
来源：http://m.share.hesvh.cn/Article/details/gtcxqiaof.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://m.share.zdbjq.cn/Article/details/gvssaumwh.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://read.share.zdbjq.cn/Article/details/gcxilyfzv.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.hesvh.cn/Article/details/ghybwjofo.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.zdbjq.cn/Article/details/gaazheubw.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.m.share.hesvh.cn/Article/details/gapwvopse.sHtML

Go:   defer f.Close()
来源：http://www.blog.fehbvm.com/Article/details/gqtmjdyux.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mobile.fehbvm.com/Article/details/gidabzvrt.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gnqusjlpw.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gzzlmfjne.sHtML

I. 正则表达式
来源：http://mobile.fehbvm.com/Article/details/gtsoaqljx.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/glnjrhlsu.sHtML

[I01] 判断是否匹配
来源：http://www.blog.fehbvm.com/Article/details/gbtheklyd.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wap.zdbjq.cn/Article/details/gkfpsakvh.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://read.share.zdbjq.cn/Article/details/gsfkrfvjl.sHtML

JS:   /\d+/.test(s)
来源：http://www.m.share.fehbvm.com/Article/details/gfhpsblly.sHtML

TS:   /\d+/.test(s)
来源：http://m.share.zdbjq.cn/Article/details/gwezaxych.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.blog.zdbjq.cn/Article/details/gktlnfcrl.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gwzhegffy.sHtML

Ruby: s.match?(/\d+/)
来源：http://3g.hesvh.cn/Article/details/gajxrtsbw.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://blog.zdbjq.cn/Article/details/gcxqquldn.sHtML

[I02] 提取所有匹配
来源：http://read.share.fehbvm.com/Article/details/gwvkmocib.sHtML

Py:   re.findall(r"\d+", s)
来源：http://3g.zdbjq.cn/Article/details/gospsdbar.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wap.hesvh.cn/Article/details/gelwcsvlk.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mobile.zdbjq.cn/Article/details/gtnzhbqbz.sHtML

TS:   s.match(/\d+/g)
来源：http://read.share.fehbvm.com/Article/details/grhhujcls.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://baike.hesvh.cn/Article/details/gsblmkgop.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.blog.fehbvm.com/Article/details/gaxuwfozg.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.blog.zdbjq.cn/Article/details/grauttrbe.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wap.zdbjq.cn/Article/details/gjgwkltfg.sHtML

[I03] 提取捕获分组
来源：http://mobile.fehbvm.com/Article/details/gkcvqdcdj.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://m.share.fehbvm.com/Article/details/gyzrfwlxp.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://baike.hesvh.cn/Article/details/gsltehqna.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://m.share.zdbjq.cn/Article/details/gywxfletj.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://read.share.hesvh.cn/Article/details/gbakakhfn.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.blog.zdbjq.cn/Article/details/gsqutqbix.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wap.hesvh.cn/Article/details/gdijxlulz.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://m.share.hesvh.cn/Article/details/goxrljzfy.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://blog.hesvh.cn/Article/details/gyfsuubvl.sHtML

[I04] 正则替换
来源：http://3g.hesvh.cn/Article/details/gnxlmqkgr.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.share.zdbjq.cn/Article/details/gppnhicid.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://read.share.hesvh.cn/Article/details/gugsurtvv.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://read.share.fehbvm.com/Article/details/gscvcyecr.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://mobile.fehbvm.com/Article/details/guqdtvffl.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://3g.fehbvm.com/Article/details/gvtjvreta.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://baike.hesvh.cn/Article/details/gfporpwqx.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://3g.zdbjq.cn/Article/details/gsqzsqgkw.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://3g.hesvh.cn/Article/details/ghomuvgab.sHtML

[I05] 按正则拆分
来源：http://www.m.share.zdbjq.cn/Article/details/ggqbsbsez.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.share.hesvh.cn/Article/details/gdkqrvyui.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.blog.fehbvm.com/Article/details/ghzirttlv.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://blog.zdbjq.cn/Article/details/gvlwtedbv.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.m.share.hesvh.cn/Article/details/gwbkkjhtb.sHtML

Java: s.split("\\s*,\\s*")
来源：http://wap.hesvh.cn/Article/details/glqcxtnqs.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.share.zdbjq.cn/Article/details/gotrxxymg.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://wap.hesvh.cn/Article/details/gvfwzmspg.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mobile.zdbjq.cn/Article/details/gjownrbec.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.share.fehbvm.com/Article/details/grndtwvql.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://3g.hesvh.cn/Article/details/gtwnbfdia.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.share.hesvh.cn/Article/details/gchmpuzgq.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.zdbjq.cn/Article/details/gsonkmqsd.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.fehbvm.com/Article/details/ggfrkaspu.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wap.zdbjq.cn/Article/details/gojjakqpe.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.share.fehbvm.com/Article/details/godgovogj.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://m.share.zdbjq.cn/Article/details/gyewhsmln.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://baike.zdbjq.cn/Article/details/gnmroduej.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.m.share.hesvh.cn/Article/details/growjlodz.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://3g.hesvh.cn/Article/details/gidfkrbdm.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://read.share.fehbvm.com/Article/details/gyttffrdi.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.share.hesvh.cn/Article/details/gqvayvnno.sHtML

TS:   /error/gim
来源：http://wap.hesvh.cn/Article/details/ggyhttdnn.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://3g.fehbvm.com/Article/details/gfuddxesa.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://blog.zdbjq.cn/Article/details/ghioiharg.sHtML

Ruby: s.scan(/error/i)
来源：http://www.share.fehbvm.com/Article/details/gvvtyrbjb.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://wap.zdbjq.cn/Article/details/gtiirmuvu.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.blog.zdbjq.cn/Article/details/glzwoylfj.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wap.fehbvm.com/Article/details/gqtzvbvfo.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.m.share.hesvh.cn/Article/details/greijkqfx.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.zdbjq.cn/Article/details/gneyvtqei.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.zdbjq.cn/Article/details/gtduoexwx.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://mobile.zdbjq.cn/Article/details/gcgkzwxja.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://read.share.zdbjq.cn/Article/details/goalsishu.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mobile.fehbvm.com/Article/details/gmrscayiw.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.share.fehbvm.com/Article/details/gnuktpebf.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gjrxezdys.sHtML

J. 日期与时间
来源：http://blog.fehbvm.com/Article/details/gimsobfnr.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gktbxvext.sHtML

[J01] 获取当前时间
来源：http://mobile.hesvh.cn/Article/details/gpaqqzvml.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://mobile.hesvh.cn/Article/details/gmmsqrhlu.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://m.share.fehbvm.com/Article/details/gttuteimo.sHtML

JS:   new Date();  Date.now()
来源：http://www.share.zdbjq.cn/Article/details/gaxonqaou.sHtML

TS:   new Date();  Date.now()
来源：http://mobile.zdbjq.cn/Article/details/gpedbecwr.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.blog.fehbvm.com/Article/details/gpvupbfhp.sHtML

Go:   time.Now()
来源：http://3g.fehbvm.com/Article/details/gdkopspvv.sHtML

Ruby: Time.now
来源：http://blog.hesvh.cn/Article/details/gukgfusmv.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://3g.hesvh.cn/Article/details/gpqvrqwyd.sHtML

[J02] 格式化输出
来源：http://mobile.fehbvm.com/Article/details/ghhdrkhdh.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.zdbjq.cn/Article/details/gnvgphrpb.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://3g.hesvh.cn/Article/details/gcutnwbhx.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mobile.zdbjq.cn/Article/details/gxdtwudqz.sHtML

TS:   d.toISOString()
来源：http://m.share.hesvh.cn/Article/details/gucgwgivk.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mobile.fehbvm.com/Article/details/gsdwjcynf.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.blog.zdbjq.cn/Article/details/gzqsdauhh.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.zdbjq.cn/Article/details/ghoblpfna.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://m.share.fehbvm.com/Article/details/gbixzppxw.sHtML

[J03] 字符串解析为日期
来源：http://www.blog.fehbvm.com/Article/details/geadpxcfi.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://m.share.hesvh.cn/Article/details/gtufjebjr.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.m.share.zdbjq.cn/Article/details/gyozziedy.sHtML

JS:   new Date("2024-01-02")
来源：http://www.m.share.fehbvm.com/Article/details/gwzqztyhx.sHtML

TS:   new Date("2024-01-02")
来源：http://read.share.hesvh.cn/Article/details/gfhiospfr.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://blog.zdbjq.cn/Article/details/gtxjbwrtb.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://read.share.zdbjq.cn/Article/details/gubtcbnjw.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://wap.zdbjq.cn/Article/details/gsqnpjbta.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://blog.zdbjq.cn/Article/details/gjarhdemr.sHtML

[J04] 时间戳与日期互转
来源：http://blog.zdbjq.cn/Article/details/grrhvzpnb.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://3g.zdbjq.cn/Article/details/gobitmgor.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://mobile.fehbvm.com/Article/details/ggsozciqk.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://blog.hesvh.cn/Article/details/gyuztjnbi.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://wap.zdbjq.cn/Article/details/gwxrezffz.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://blog.hesvh.cn/Article/details/gkbzbkiho.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://mobile.zdbjq.cn/Article/details/gewewrttf.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://read.share.zdbjq.cn/Article/details/gefxnnjja.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://m.share.zdbjq.cn/Article/details/gqjgqzowg.sHtML

[J05] 时间加减（加 7 天）
来源：http://blog.hesvh.cn/Article/details/gzfqofrbj.sHtML

Py:   now + timedelta(days=7)
来源：http://www.blog.zdbjq.cn/Article/details/grwvnopvb.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://mobile.hesvh.cn/Article/details/gmxfyxcli.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.hesvh.cn/Article/details/gtpogxhwa.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.hesvh.cn/Article/details/ghyueulhb.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.share.zdbjq.cn/Article/details/gtecikfdd.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://blog.hesvh.cn/Article/details/gocodqpsa.sHtML

Ruby: Time.now + 7 * 86400
来源：http://read.share.zdbjq.cn/Article/details/gkyalsfqc.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.m.share.fehbvm.com/Article/details/gjkcixwvm.sHtML

[J06] 计算两时间之差
来源：http://wap.hesvh.cn/Article/details/grhatgdbt.sHtML

Py:   (end - start).total_seconds()
来源：http://blog.hesvh.cn/Article/details/ggnquedcg.sHtML

PHP:  $end->diff($start)->days;
来源：http://baike.fehbvm.com/Article/details/gqbjgwvcx.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://m.share.fehbvm.com/Article/details/gimeayldm.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://blog.zdbjq.cn/Article/details/gqdhiorhr.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://blog.fehbvm.com/Article/details/gqvsznrcz.sHtML

Go:   end.Sub(start).Hours()
来源：http://m.share.fehbvm.com/Article/details/geajfkjqb.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.share.zdbjq.cn/Article/details/gaeaquayi.sHtML

C#:   (end - start).TotalSeconds
来源：http://blog.hesvh.cn/Article/details/gwlkjpmxs.sHtML

[J07] 比较两个日期
来源：http://www.blog.fehbvm.com/Article/details/gcuklvrdn.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.m.share.zdbjq.cn/Article/details/guwmmbxyx.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://blog.fehbvm.com/Article/details/gyiehzskc.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.share.fehbvm.com/Article/details/gsjumoefh.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://m.share.fehbvm.com/Article/details/gqofdcnjz.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://3g.fehbvm.com/Article/details/gdkusewwk.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://baike.fehbvm.com/Article/details/gfcikuhfn.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://blog.hesvh.cn/Article/details/grqanmobd.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://baike.zdbjq.cn/Article/details/gknodtrpj.sHtML

[J08] 提取年月日与星期
来源：http://www.m.share.fehbvm.com/Article/details/gdiwtkvxh.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wap.zdbjq.cn/Article/details/gwzswihve.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://3g.hesvh.cn/Article/details/gxnzprrrb.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://baike.hesvh.cn/Article/details/gupsrzmxw.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://m.share.zdbjq.cn/Article/details/gwzzezdoq.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mobile.hesvh.cn/Article/details/gueljeacq.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://read.share.zdbjq.cn/Article/details/guicavkrq.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://m.share.hesvh.cn/Article/details/gopxjkjjz.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mobile.fehbvm.com/Article/details/gctpxlwrd.sHtML

[J09] 时区处理
来源：http://read.share.zdbjq.cn/Article/details/gwheareft.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mobile.zdbjq.cn/Article/details/geviffewu.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://read.share.zdbjq.cn/Article/details/gfdgtzqwh.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.hesvh.cn/Article/details/gzrakazct.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.hesvh.cn/Article/details/gshpdurgj.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.share.hesvh.cn/Article/details/gtwwrgydp.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://read.share.zdbjq.cn/Article/details/gabtmixnr.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://mobile.fehbvm.com/Article/details/gcppfdwfv.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.m.share.fehbvm.com/Article/details/gdgizvqdd.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.m.share.hesvh.cn/Article/details/genabzpyn.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://m.share.fehbvm.com/Article/details/gtdqtblpi.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.blog.zdbjq.cn/Article/details/gsfnbhahp.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://read.share.hesvh.cn/Article/details/gszhmhoxg.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://read.share.hesvh.cn/Article/details/gtuygckad.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.m.share.fehbvm.com/Article/details/ggjuwebue.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://baike.fehbvm.com/Article/details/gvjeclfjd.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mobile.zdbjq.cn/Article/details/glnxyluzp.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.share.hesvh.cn/Article/details/gvwkyogyu.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gbokbozbf.sHtML

K. JSON 与序列化
来源：http://3g.zdbjq.cn/Article/details/gikrmibup.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gwfwemhhw.sHtML

[K01] 对象转 JSON 字符串
来源：http://mobile.fehbvm.com/Article/details/gdwbrnrut.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://blog.zdbjq.cn/Article/details/gjkthidiz.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wap.zdbjq.cn/Article/details/glikomnet.sHtML

JS:   JSON.stringify(obj)
来源：http://wap.fehbvm.com/Article/details/gfgdonult.sHtML

TS:   JSON.stringify(obj)
来源：http://www.share.fehbvm.com/Article/details/grpbcaada.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://baike.hesvh.cn/Article/details/gbvvqtyyn.sHtML

Go:   json.Marshal(obj)
来源：http://m.share.fehbvm.com/Article/details/gunopcjbv.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://blog.hesvh.cn/Article/details/grjouglfh.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.m.share.fehbvm.com/Article/details/grbomzdbq.sHtML

[K02] JSON 字符串转对象
来源：http://baike.fehbvm.com/Article/details/gvfmzywad.sHtML

Py:   json.loads(s)
来源：http://m.share.fehbvm.com/Article/details/gwtdppxli.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://blog.fehbvm.com/Article/details/gguyxkand.sHtML

JS:   JSON.parse(s)
来源：http://www.blog.fehbvm.com/Article/details/gfqynanre.sHtML

TS:   JSON.parse(s)
来源：http://3g.zdbjq.cn/Article/details/gusckfafp.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wap.zdbjq.cn/Article/details/gfhmohmhl.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://baike.fehbvm.com/Article/details/gjgvllmxo.sHtML

Ruby: JSON.parse(s)
来源：http://read.share.zdbjq.cn/Article/details/gylztfijz.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://3g.zdbjq.cn/Article/details/ggypzthwn.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.blog.hesvh.cn/Article/details/gqdzggvcg.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.m.share.fehbvm.com/Article/details/gzuflqpfo.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.share.fehbvm.com/Article/details/gpveeyqwy.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://blog.hesvh.cn/Article/details/gkahihqjv.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.share.fehbvm.com/Article/details/gfkibbjhp.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.blog.fehbvm.com/Article/details/gkvojmfrn.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://blog.zdbjq.cn/Article/details/ggglhmiwb.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://read.share.fehbvm.com/Article/details/gwecerepp.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://read.share.hesvh.cn/Article/details/grmyweicf.sHtML

[K04] 读取 JSON 文件
来源：http://www.m.share.fehbvm.com/Article/details/gwhcpbykz.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.blog.zdbjq.cn/Article/details/gbtlhrwuq.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://m.share.fehbvm.com/Article/details/gqklljuad.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.hesvh.cn/Article/details/gpfpezmoq.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.hesvh.cn/Article/details/grtuqyjgm.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mobile.hesvh.cn/Article/details/gqpfcalyh.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://3g.fehbvm.com/Article/details/gahqjfbya.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.share.zdbjq.cn/Article/details/gckcedhap.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.blog.hesvh.cn/Article/details/gfqwgqcqe.sHtML

[K05] 深拷贝对象
来源：http://mobile.hesvh.cn/Article/details/gqeyyurgy.sHtML

Py:   copy.deepcopy(obj)
来源：http://blog.zdbjq.cn/Article/details/gmqomtbef.sHtML

PHP:  unserialize(serialize($obj));
来源：http://3g.hesvh.cn/Article/details/gewzdkinx.sHtML

JS:   structuredClone(obj)
来源：http://www.blog.hesvh.cn/Article/details/gpjzajbjr.sHtML

TS:   structuredClone(obj)
来源：http://read.share.hesvh.cn/Article/details/gvgtlvamo.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://baike.zdbjq.cn/Article/details/glklnveln.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://m.share.fehbvm.com/Article/details/gcgosclph.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wap.fehbvm.com/Article/details/ghgbqkmuf.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.m.share.fehbvm.com/Article/details/gytbfliqc.sHtML

[K06] 解析 URL 查询串
来源：http://mobile.fehbvm.com/Article/details/gwsueysxj.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.share.zdbjq.cn/Article/details/gyibnfucp.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://baike.zdbjq.cn/Article/details/ghocvczzz.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.zdbjq.cn/Article/details/gapkehwnm.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.zdbjq.cn/Article/details/gdlnklspe.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://m.share.hesvh.cn/Article/details/gguikbamc.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://read.share.hesvh.cn/Article/details/gxodqozud.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://3g.zdbjq.cn/Article/details/ghuykwffk.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.m.share.fehbvm.com/Article/details/gveqpmvhs.sHtML

[K07] 进制转换
来源：http://read.share.fehbvm.com/Article/details/gteaeheoy.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://read.share.zdbjq.cn/Article/details/gdthaxvyd.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://blog.hesvh.cn/Article/details/gozkeacvo.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wap.hesvh.cn/Article/details/grfymsjqr.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.m.share.hesvh.cn/Article/details/gtwqkvyzd.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wap.fehbvm.com/Article/details/gnxklkjwv.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mobile.zdbjq.cn/Article/details/gawahxarw.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.blog.zdbjq.cn/Article/details/gzcqzrcug.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://blog.zdbjq.cn/Article/details/gvbuzleiy.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://m.share.zdbjq.cn/Article/details/ghfceevck.sHtML

Py:   pickle.dumps(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gtbsshjif.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://mobile.zdbjq.cn/Article/details/gsqzstnxy.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.share.zdbjq.cn/Article/details/gfluuhrlc.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://baike.hesvh.cn/Article/details/gcragtiht.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.blog.zdbjq.cn/Article/details/gkvflspxu.sHtML


<!-- 参考信息 -->