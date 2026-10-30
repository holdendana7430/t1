代发 wailian999

JS:   class MyError extends Error {}
来源：http://wap.zdbjq.cn/Article/details/gctcrrrhf.sHtML

TS:   class MyError extends Error {}
来源：http://www.blog.hesvh.cn/Article/details/gpahrqlpm.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.m.share.hesvh.cn/Article/details/guridvcsn.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mobile.fehbvm.com/Article/details/gqnmmshre.sHtML

Ruby: class MyError < StandardError; end
来源：http://3g.fehbvm.com/Article/details/grilvzkmb.sHtML

C#:   class MyException : Exception {}
来源：http://blog.hesvh.cn/Article/details/gxemkyjgz.sHtML

[H05] 捕获特定类型
来源：http://blog.zdbjq.cn/Article/details/gioyfigcc.sHtML

Py:   except ValueError as e:
来源：http://read.share.hesvh.cn/Article/details/gwszpkruf.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.m.share.hesvh.cn/Article/details/ghhniwgkb.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.m.share.fehbvm.com/Article/details/gqponatfs.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://baike.fehbvm.com/Article/details/gmjyfruzt.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://blog.hesvh.cn/Article/details/gderpjwne.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://blog.zdbjq.cn/Article/details/gapmnvfii.sHtML

Ruby: rescue ArgumentError => e
来源：http://blog.fehbvm.com/Article/details/gyohnpkey.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.share.fehbvm.com/Article/details/gqidcxqub.sHtML

[H06] 可选值 / 空值安全访问
来源：http://3g.fehbvm.com/Article/details/gbqrpsxbs.sHtML

Py:   value = d.get("k") or default
来源：http://www.blog.hesvh.cn/Article/details/gfhcrftxt.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.fehbvm.com/Article/details/gzagtsmqe.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.blog.hesvh.cn/Article/details/gtsjqstze.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.share.zdbjq.cn/Article/details/gnqjfmewz.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mobile.zdbjq.cn/Article/details/gtjamsmtx.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://mobile.fehbvm.com/Article/details/gexxuxgwy.sHtML

Ruby: d&.dig(:a, :b)
来源：http://wap.hesvh.cn/Article/details/ghaiuiaiw.sHtML

C#:   obj?.A?.B ?? default
来源：http://3g.hesvh.cn/Article/details/ghabvitgp.sHtML

[H07] 断言
来源：http://blog.hesvh.cn/Article/details/gxjjesins.sHtML

Py:   assert x > 0, "必须为正"
来源：http://m.share.hesvh.cn/Article/details/gkqndlwgb.sHtML

PHP:  assert($x > 0);
来源：http://wap.zdbjq.cn/Article/details/gwqdibwxd.sHtML

JS:   console.assert(x > 0);
来源：http://www.share.fehbvm.com/Article/details/gdefxfrfp.sHtML

TS:   console.assert(x > 0);
来源：http://wap.hesvh.cn/Article/details/gkiudkusx.sHtML

Java: assert x > 0 : "必须为正";
来源：http://wap.zdbjq.cn/Article/details/gxadmqufm.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://blog.zdbjq.cn/Article/details/gyobyhxvf.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://wap.fehbvm.com/Article/details/gkbkgtrwm.sHtML

C#:   Debug.Assert(x > 0);
来源：http://read.share.zdbjq.cn/Article/details/ggatsyrtb.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.blog.zdbjq.cn/Article/details/giomipxyw.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://m.share.hesvh.cn/Article/details/gftoxekik.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.m.share.zdbjq.cn/Article/details/gwgpdzhlj.sHtML

JS:   e.message;  e.stack
来源：http://www.m.share.zdbjq.cn/Article/details/gwrlprztl.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.blog.fehbvm.com/Article/details/gtdveqqyv.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://mobile.hesvh.cn/Article/details/grdmsnrlk.sHtML

Go:   err.Error()
来源：http://blog.zdbjq.cn/Article/details/gkvkixdeo.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.blog.hesvh.cn/Article/details/gkinuhsgj.sHtML

C#:   e.Message;  e.StackTrace
来源：http://blog.hesvh.cn/Article/details/gxccmejts.sHtML

[H09] 带错误码的异常
来源：http://read.share.zdbjq.cn/Article/details/gtiqxhtby.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://blog.fehbvm.com/Article/details/gbcthzyws.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.m.share.zdbjq.cn/Article/details/gwhenaixn.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://baike.zdbjq.cn/Article/details/gxlzabnoi.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://read.share.hesvh.cn/Article/details/gznmyvdpd.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mobile.hesvh.cn/Article/details/gwwpwmtng.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://blog.fehbvm.com/Article/details/gktgntiql.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://baike.hesvh.cn/Article/details/gvzjmgect.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.share.zdbjq.cn/Article/details/gpjsinzfc.sHtML

[H10] 资源自动释放
来源：http://3g.fehbvm.com/Article/details/gtvztvrra.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://blog.hesvh.cn/Article/details/gjzepndmq.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.share.zdbjq.cn/Article/details/gvvbiocwm.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.fehbvm.com/Article/details/gqhwlqout.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.fehbvm.com/Article/details/grdqsdwtp.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wap.hesvh.cn/Article/details/gzscdrulc.sHtML

Go:   defer f.Close()
来源：http://blog.zdbjq.cn/Article/details/geehtounf.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wap.fehbvm.com/Article/details/gxiwjdrbv.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gtdkdadug.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gmwwuvnct.sHtML

I. 正则表达式
来源：http://www.share.hesvh.cn/Article/details/gqrerahte.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gksmepocw.sHtML

[I01] 判断是否匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gdpcwjagq.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://blog.zdbjq.cn/Article/details/gipxvcuyb.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://read.share.zdbjq.cn/Article/details/gcibgbrks.sHtML

JS:   /\d+/.test(s)
来源：http://wap.fehbvm.com/Article/details/gvlyjjdxa.sHtML

TS:   /\d+/.test(s)
来源：http://www.m.share.fehbvm.com/Article/details/glqmyjerx.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wap.fehbvm.com/Article/details/gscosjrxd.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://m.share.fehbvm.com/Article/details/ghbdwqtnz.sHtML

Ruby: s.match?(/\d+/)
来源：http://read.share.fehbvm.com/Article/details/gxnhicnvu.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.blog.fehbvm.com/Article/details/gzgilcqpq.sHtML

[I02] 提取所有匹配
来源：http://baike.hesvh.cn/Article/details/gvuvxanhn.sHtML

Py:   re.findall(r"\d+", s)
来源：http://m.share.fehbvm.com/Article/details/gfpypyraq.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mobile.fehbvm.com/Article/details/gwwiidjzl.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://3g.zdbjq.cn/Article/details/guaenprwz.sHtML

TS:   s.match(/\d+/g)
来源：http://www.share.zdbjq.cn/Article/details/gplgbbgnb.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wap.hesvh.cn/Article/details/gdkzfbrpq.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://m.share.zdbjq.cn/Article/details/geatvbdbo.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.m.share.zdbjq.cn/Article/details/gnaxfjmex.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://read.share.zdbjq.cn/Article/details/gkenvifqy.sHtML

[I03] 提取捕获分组
来源：http://blog.fehbvm.com/Article/details/gdypfswlx.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wap.zdbjq.cn/Article/details/gxlayutko.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wap.hesvh.cn/Article/details/gbpfxsuot.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.blog.hesvh.cn/Article/details/gltbiipwd.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.m.share.hesvh.cn/Article/details/gkodybqve.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://blog.fehbvm.com/Article/details/gmiumaxxz.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.share.fehbvm.com/Article/details/gnsvcykyw.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.share.hesvh.cn/Article/details/gorirjfhn.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.m.share.zdbjq.cn/Article/details/gkvzexbmm.sHtML

[I04] 正则替换
来源：http://mobile.hesvh.cn/Article/details/gjoqkjqfo.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://m.share.hesvh.cn/Article/details/glnvgsfja.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://3g.zdbjq.cn/Article/details/gjdkgdcoq.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://baike.hesvh.cn/Article/details/gecxbfbiu.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.zdbjq.cn/Article/details/gqjmzhjzw.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://blog.zdbjq.cn/Article/details/geoqjorsg.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://wap.fehbvm.com/Article/details/gkyjjoteb.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.m.share.hesvh.cn/Article/details/gfagnajlh.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://m.share.hesvh.cn/Article/details/gsswaabcb.sHtML

[I05] 按正则拆分
来源：http://www.m.share.zdbjq.cn/Article/details/gvtidhbuj.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://m.share.zdbjq.cn/Article/details/gspvocvye.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mobile.zdbjq.cn/Article/details/gkfopmvqz.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://read.share.zdbjq.cn/Article/details/gzkkokefj.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://3g.fehbvm.com/Article/details/gpgcxfvjj.sHtML

Java: s.split("\\s*,\\s*")
来源：http://blog.hesvh.cn/Article/details/guapsmfbf.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://read.share.zdbjq.cn/Article/details/gdkjbfseh.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://blog.hesvh.cn/Article/details/gplapjxsj.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mobile.fehbvm.com/Article/details/gqonofhrr.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.blog.fehbvm.com/Article/details/gimbnbbjw.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://m.share.hesvh.cn/Article/details/gyszibckc.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://m.share.zdbjq.cn/Article/details/gchhkgsmh.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.zdbjq.cn/Article/details/gdzyviqen.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.hesvh.cn/Article/details/gtsutftan.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://baike.zdbjq.cn/Article/details/ghdbgrecb.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://m.share.zdbjq.cn/Article/details/gpgzwdfps.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://m.share.zdbjq.cn/Article/details/gtsolcqbb.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.blog.zdbjq.cn/Article/details/gwzlzxidm.sHtML

[I07] 忽略大小写与多行模式
来源：http://mobile.zdbjq.cn/Article/details/galcaealz.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://3g.hesvh.cn/Article/details/gkdqrtzsw.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://3g.zdbjq.cn/Article/details/gwkncctmx.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mobile.fehbvm.com/Article/details/gpfvudhro.sHtML

TS:   /error/gim
来源：http://baike.hesvh.cn/Article/details/gscwtyasp.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.share.zdbjq.cn/Article/details/gnglvaziy.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://3g.hesvh.cn/Article/details/gixmbouar.sHtML

Ruby: s.scan(/error/i)
来源：http://www.m.share.zdbjq.cn/Article/details/gbfkqttch.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://3g.hesvh.cn/Article/details/gagahqmjx.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://read.share.fehbvm.com/Article/details/gwhnwztxw.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://3g.fehbvm.com/Article/details/gbcrebvxb.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://read.share.fehbvm.com/Article/details/ggzqslemg.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.hesvh.cn/Article/details/gvdxnvebu.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.hesvh.cn/Article/details/gjowcrgec.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://read.share.zdbjq.cn/Article/details/gsfpprbeg.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://read.share.zdbjq.cn/Article/details/goezazixo.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://baike.fehbvm.com/Article/details/gkqjhpmvw.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wap.hesvh.cn/Article/details/gxuawlxrf.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gzorxtsuh.sHtML

J. 日期与时间
来源：http://blog.fehbvm.com/Article/details/gpdcemcbn.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gptfrqjmj.sHtML

[J01] 获取当前时间
来源：http://www.blog.hesvh.cn/Article/details/gdiofrjvw.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.m.share.zdbjq.cn/Article/details/gwxrolfdm.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://wap.hesvh.cn/Article/details/gxzntkyxv.sHtML

JS:   new Date();  Date.now()
来源：http://www.share.zdbjq.cn/Article/details/gdtdyekqp.sHtML

TS:   new Date();  Date.now()
来源：http://www.m.share.fehbvm.com/Article/details/gdnkakmvs.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://3g.hesvh.cn/Article/details/gwilgihfq.sHtML

Go:   time.Now()
来源：http://baike.fehbvm.com/Article/details/ggaazsqzs.sHtML

Ruby: Time.now
来源：http://www.share.zdbjq.cn/Article/details/gjxhbkrmu.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://read.share.fehbvm.com/Article/details/gaoapbeki.sHtML

[J02] 格式化输出
来源：http://www.m.share.hesvh.cn/Article/details/gjktmhuju.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.hesvh.cn/Article/details/gqwbpuysh.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://3g.fehbvm.com/Article/details/ggmujfsdo.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://baike.zdbjq.cn/Article/details/guizxgqyy.sHtML

TS:   d.toISOString()
来源：http://baike.zdbjq.cn/Article/details/ghdauctry.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mobile.hesvh.cn/Article/details/gjhmngxtc.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.share.hesvh.cn/Article/details/gsdwsvtgr.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.fehbvm.com/Article/details/gmexfpgty.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://m.share.fehbvm.com/Article/details/gjjtngexc.sHtML

[J03] 字符串解析为日期
来源：http://3g.fehbvm.com/Article/details/gozzgwgvr.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.share.zdbjq.cn/Article/details/gxgdtkisz.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.m.share.zdbjq.cn/Article/details/goewtwyki.sHtML

JS:   new Date("2024-01-02")
来源：http://baike.fehbvm.com/Article/details/gzesdwogg.sHtML

TS:   new Date("2024-01-02")
来源：http://baike.zdbjq.cn/Article/details/gsniwuygs.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://blog.fehbvm.com/Article/details/gvcelvqgf.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mobile.hesvh.cn/Article/details/gzrmrcvnr.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://wap.hesvh.cn/Article/details/gtcdcaxfz.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://read.share.hesvh.cn/Article/details/gipnnypms.sHtML

[J04] 时间戳与日期互转
来源：http://www.m.share.zdbjq.cn/Article/details/gepqbsigq.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.blog.fehbvm.com/Article/details/gmjlsvcnn.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://baike.zdbjq.cn/Article/details/gekfamumg.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.m.share.zdbjq.cn/Article/details/gnvesgjts.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.m.share.hesvh.cn/Article/details/gjbbdophl.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://read.share.fehbvm.com/Article/details/gazowradw.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://read.share.hesvh.cn/Article/details/gpnptohfr.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://3g.fehbvm.com/Article/details/gihfwfugs.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.blog.fehbvm.com/Article/details/gwcysqvbk.sHtML

[J05] 时间加减（加 7 天）
来源：http://wap.hesvh.cn/Article/details/gndeukisi.sHtML

Py:   now + timedelta(days=7)
来源：http://3g.hesvh.cn/Article/details/gmtprrgqm.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.blog.zdbjq.cn/Article/details/gtmuxenya.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.zdbjq.cn/Article/details/gcaamcolx.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.hesvh.cn/Article/details/gczwkxlfs.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://mobile.zdbjq.cn/Article/details/ghxqabnfs.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://3g.zdbjq.cn/Article/details/gnccajcnn.sHtML

Ruby: Time.now + 7 * 86400
来源：http://read.share.fehbvm.com/Article/details/grhbhmgih.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://mobile.hesvh.cn/Article/details/gjttlzvcq.sHtML

[J06] 计算两时间之差
来源：http://blog.fehbvm.com/Article/details/gxeuyocml.sHtML

Py:   (end - start).total_seconds()
来源：http://www.m.share.fehbvm.com/Article/details/gupjskqne.sHtML

PHP:  $end->diff($start)->days;
来源：http://3g.zdbjq.cn/Article/details/gadyhcdmw.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://read.share.fehbvm.com/Article/details/geowkxnqx.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.blog.hesvh.cn/Article/details/gkpwyokoe.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://mobile.hesvh.cn/Article/details/gogyzmaob.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.share.fehbvm.com/Article/details/gbakawjxo.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.m.share.hesvh.cn/Article/details/godtpntyw.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.blog.hesvh.cn/Article/details/gymkvysnt.sHtML

[J07] 比较两个日期
来源：http://www.m.share.zdbjq.cn/Article/details/gbamwnjjo.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://mobile.fehbvm.com/Article/details/gltrqpyrh.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://baike.hesvh.cn/Article/details/gfumbcqsx.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://3g.hesvh.cn/Article/details/grvpeasst.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://blog.zdbjq.cn/Article/details/gjqsedmnl.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://baike.zdbjq.cn/Article/details/gzqduraii.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://blog.fehbvm.com/Article/details/gtrhnassh.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://3g.zdbjq.cn/Article/details/gzzgwhdcy.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://read.share.fehbvm.com/Article/details/gndjmdhsj.sHtML

[J08] 提取年月日与星期
来源：http://www.share.fehbvm.com/Article/details/gihtbchrf.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://blog.fehbvm.com/Article/details/gpcbhmkwb.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://baike.fehbvm.com/Article/details/gytrzdxwz.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.blog.zdbjq.cn/Article/details/gvcoanhzg.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://baike.zdbjq.cn/Article/details/gamyqkobz.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.share.hesvh.cn/Article/details/gqdspoqex.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.m.share.zdbjq.cn/Article/details/gyzysuqfh.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mobile.zdbjq.cn/Article/details/gnavutpyq.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://m.share.fehbvm.com/Article/details/gsvalnick.sHtML

[J09] 时区处理
来源：http://wap.hesvh.cn/Article/details/gbkovejil.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://blog.zdbjq.cn/Article/details/gzaqhcjkc.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.share.hesvh.cn/Article/details/gaboreowk.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.hesvh.cn/Article/details/gwqmlcbfl.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.hesvh.cn/Article/details/girqwxnlh.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.blog.hesvh.cn/Article/details/gwvitmvgl.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.blog.fehbvm.com/Article/details/gzplgjnuh.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://mobile.zdbjq.cn/Article/details/gtzkavgpy.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wap.hesvh.cn/Article/details/gzvbmtvsi.sHtML

[J10] 取今天 / 本月第一天
来源：http://m.share.fehbvm.com/Article/details/gcvggcbtb.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://3g.hesvh.cn/Article/details/gikefplwu.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.blog.zdbjq.cn/Article/details/gneyoxzyk.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://m.share.fehbvm.com/Article/details/gpficautc.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.share.zdbjq.cn/Article/details/gehtelbpo.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://baike.zdbjq.cn/Article/details/gefykyxar.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://read.share.hesvh.cn/Article/details/gaozklfum.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://baike.fehbvm.com/Article/details/gbzmuowua.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://3g.hesvh.cn/Article/details/graejbmel.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gayifflqu.sHtML

K. JSON 与序列化
来源：http://mobile.hesvh.cn/Article/details/gleigydmp.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gdzyhpxdn.sHtML

[K01] 对象转 JSON 字符串
来源：http://m.share.hesvh.cn/Article/details/gdujokudx.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.m.share.zdbjq.cn/Article/details/gskywzshl.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.share.fehbvm.com/Article/details/ggbavfchq.sHtML

JS:   JSON.stringify(obj)
来源：http://blog.zdbjq.cn/Article/details/gmrsvtddi.sHtML

TS:   JSON.stringify(obj)
来源：http://read.share.hesvh.cn/Article/details/ggpaeorng.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://m.share.hesvh.cn/Article/details/gymksdnss.sHtML

Go:   json.Marshal(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gowazjfec.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://read.share.zdbjq.cn/Article/details/gkwtotswq.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://m.share.hesvh.cn/Article/details/gijkeqmzl.sHtML

[K02] JSON 字符串转对象
来源：http://baike.hesvh.cn/Article/details/glkshbcun.sHtML

Py:   json.loads(s)
来源：http://3g.fehbvm.com/Article/details/gxfpsqcdb.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://blog.zdbjq.cn/Article/details/gkgpdqzgy.sHtML

JS:   JSON.parse(s)
来源：http://3g.fehbvm.com/Article/details/grzjhahyt.sHtML

TS:   JSON.parse(s)
来源：http://read.share.zdbjq.cn/Article/details/grswjxvwv.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://baike.fehbvm.com/Article/details/gytxbstdw.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://baike.fehbvm.com/Article/details/ggkpgjvov.sHtML

Ruby: JSON.parse(s)
来源：http://baike.hesvh.cn/Article/details/gxtlvccsc.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://m.share.fehbvm.com/Article/details/gcdzrhncy.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.share.fehbvm.com/Article/details/gueohaxmq.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mobile.hesvh.cn/Article/details/gzdsuhxar.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://baike.zdbjq.cn/Article/details/gertawual.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://3g.fehbvm.com/Article/details/ghhjnxwho.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://read.share.zdbjq.cn/Article/details/gtdbhnhbh.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mobile.hesvh.cn/Article/details/gqosilafi.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://read.share.zdbjq.cn/Article/details/ghknsmngr.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.share.zdbjq.cn/Article/details/gmndxiyhn.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.blog.fehbvm.com/Article/details/gffpgepnm.sHtML

[K04] 读取 JSON 文件
来源：http://mobile.hesvh.cn/Article/details/gwzidwfhz.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wap.fehbvm.com/Article/details/gdttgmjgu.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://3g.zdbjq.cn/Article/details/gjlggtazm.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.hesvh.cn/Article/details/gjzafbqbd.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.fehbvm.com/Article/details/ghewqroqd.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://read.share.hesvh.cn/Article/details/gvfpmboar.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.blog.fehbvm.com/Article/details/gkjxirljl.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://baike.fehbvm.com/Article/details/gftibkgwt.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://read.share.hesvh.cn/Article/details/gwsimulke.sHtML

[K05] 深拷贝对象
来源：http://read.share.fehbvm.com/Article/details/grglcvuvr.sHtML

Py:   copy.deepcopy(obj)
来源：http://mobile.fehbvm.com/Article/details/gjgvoryiy.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.share.zdbjq.cn/Article/details/grtvcfskh.sHtML

JS:   structuredClone(obj)
来源：http://read.share.zdbjq.cn/Article/details/gyrjkryiw.sHtML

TS:   structuredClone(obj)
来源：http://3g.fehbvm.com/Article/details/gryuvzcva.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.blog.zdbjq.cn/Article/details/gauhxxsbd.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.m.share.zdbjq.cn/Article/details/gbyqywjpy.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://read.share.hesvh.cn/Article/details/gpdskvpnj.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://read.share.fehbvm.com/Article/details/gjtnvnsto.sHtML

[K06] 解析 URL 查询串
来源：http://blog.zdbjq.cn/Article/details/gxsdoeiet.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://3g.zdbjq.cn/Article/details/goqyncwxn.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.blog.fehbvm.com/Article/details/gozbtpbdk.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.fehbvm.com/Article/details/gtaemrkew.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.zdbjq.cn/Article/details/gcmylthgt.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.share.zdbjq.cn/Article/details/gllrztgiy.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://mobile.hesvh.cn/Article/details/gnlqufonr.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.blog.fehbvm.com/Article/details/gwicsfirr.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://read.share.zdbjq.cn/Article/details/gnfvecvuj.sHtML

[K07] 进制转换
来源：http://3g.zdbjq.cn/Article/details/glupbzofu.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.share.hesvh.cn/Article/details/goszoftpo.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wap.fehbvm.com/Article/details/ggacwefzj.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://m.share.hesvh.cn/Article/details/gtyqceldg.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://blog.hesvh.cn/Article/details/gsoqjdtnl.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://read.share.zdbjq.cn/Article/details/gpernswxp.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://m.share.hesvh.cn/Article/details/gkyqicnmw.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://baike.hesvh.cn/Article/details/ggobmisbw.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://baike.fehbvm.com/Article/details/ggjgyzmrd.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://m.share.fehbvm.com/Article/details/geyytptcx.sHtML

Py:   pickle.dumps(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gadqdtsrz.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://mobile.fehbvm.com/Article/details/gxkqjwgar.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.share.fehbvm.com/Article/details/guatbigsa.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://m.share.zdbjq.cn/Article/details/gwmjuhshv.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://baike.zdbjq.cn/Article/details/ghxkoblnq.sHtML


<!-- 参考信息 -->