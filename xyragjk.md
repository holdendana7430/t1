代发 wailian999

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.share.fanxiaobao.xyz/Article/details/gclarkzes.sHtML

Ruby: rescue ArgumentError => e
来源：http://m.share.fanxiaobao.xyz/Article/details/gdmshzdvi.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyblpwflr.sHtML

[H06] 可选值 / 空值安全访问
来源：http://baike.fanxiaobao.xyz/Article/details/gqzjxfdtl.sHtML

Py:   value = d.get("k") or default
来源：http://m.share.fanxiaobao.xyz/Article/details/guommqmqv.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.fanxiaobao.xyz/Article/details/gzwkzjfab.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkpkqmqqf.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://blog.fanxiaobao.xyz/Article/details/gssmypfsa.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://m.share.fanxiaobao.xyz/Article/details/gwqacxalp.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.share.fanxiaobao.xyz/Article/details/goyhbwcno.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyxaynwvq.sHtML

C#:   obj?.A?.B ?? default
来源：http://wap.fanxiaobao.xyz/Article/details/gnmbwkidm.sHtML

[H07] 断言
来源：http://www.share.fanxiaobao.xyz/Article/details/grnkybmew.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.share.fanxiaobao.xyz/Article/details/gnzyuzpyp.sHtML

PHP:  assert($x > 0);
来源：http://wap.fanxiaobao.xyz/Article/details/gnnqienao.sHtML

JS:   console.assert(x > 0);
来源：http://www.share.fanxiaobao.xyz/Article/details/gooeqqxka.sHtML

TS:   console.assert(x > 0);
来源：http://3g.fanxiaobao.xyz/Article/details/gxudusfsq.sHtML

Java: assert x > 0 : "必须为正";
来源：http://read.share.fanxiaobao.xyz/Article/details/gvfklmyea.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvofrmejx.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://read.share.fanxiaobao.xyz/Article/details/gamaoxoyz.sHtML

C#:   Debug.Assert(x > 0);
来源：http://3g.fanxiaobao.xyz/Article/details/gormkyoqc.sHtML

[H08] 获取错误信息与堆栈
来源：http://3g.fanxiaobao.xyz/Article/details/gzxqtedsm.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://3g.fanxiaobao.xyz/Article/details/gsnburijy.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wap.fanxiaobao.xyz/Article/details/glyassfrw.sHtML

JS:   e.message;  e.stack
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfpxdhylf.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://baike.fanxiaobao.xyz/Article/details/gjzvzgsst.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://3g.fanxiaobao.xyz/Article/details/grwgkucsj.sHtML

Go:   err.Error()
来源：http://baike.fanxiaobao.xyz/Article/details/gikglnpqi.sHtML

Ruby: e.message;  e.backtrace
来源：http://blog.fanxiaobao.xyz/Article/details/gzulqkmls.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkqsdgqqv.sHtML

[H09] 带错误码的异常
来源：http://wap.fanxiaobao.xyz/Article/details/gqozcsuar.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://read.share.fanxiaobao.xyz/Article/details/gjwwogkeu.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvgfbhjwa.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://3g.fanxiaobao.xyz/Article/details/gheiddoij.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://3g.fanxiaobao.xyz/Article/details/gdvjixqkr.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://baike.fanxiaobao.xyz/Article/details/gcwivciwi.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://blog.fanxiaobao.xyz/Article/details/ghwolbseo.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.share.fanxiaobao.xyz/Article/details/gwcearxbe.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://3g.fanxiaobao.xyz/Article/details/gxacccrqj.sHtML

[H10] 资源自动释放
来源：http://baike.fanxiaobao.xyz/Article/details/gyizhofix.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://wap.fanxiaobao.xyz/Article/details/gnsfbjgir.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.share.fanxiaobao.xyz/Article/details/gwymbogoo.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.fanxiaobao.xyz/Article/details/greimgndm.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.fanxiaobao.xyz/Article/details/govkacyjo.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mobile.fanxiaobao.xyz/Article/details/gjodrzrvm.sHtML

Go:   defer f.Close()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjzdlrytw.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://blog.fanxiaobao.xyz/Article/details/gifxhgevp.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mobile.fanxiaobao.xyz/Article/details/glvuabnri.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gvpdivynd.sHtML

I. 正则表达式
来源：http://baike.fanxiaobao.xyz/Article/details/gbgipjkop.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gofhyqtgo.sHtML

[I01] 判断是否匹配
来源：http://m.share.fanxiaobao.xyz/Article/details/gfxkizlrp.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gyaykbhie.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.share.fanxiaobao.xyz/Article/details/gujvmqotd.sHtML

JS:   /\d+/.test(s)
来源：http://baike.fanxiaobao.xyz/Article/details/gqwleygij.sHtML

TS:   /\d+/.test(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gkefbtmqw.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://m.share.fanxiaobao.xyz/Article/details/gycdjovbs.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://3g.fanxiaobao.xyz/Article/details/gknrlmcug.sHtML

Ruby: s.match?(/\d+/)
来源：http://m.share.fanxiaobao.xyz/Article/details/gbtdmxkej.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://m.share.fanxiaobao.xyz/Article/details/gvohnvcok.sHtML

[I02] 提取所有匹配
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdnqudkjg.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzzbkkooc.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://read.share.fanxiaobao.xyz/Article/details/gwtxgoedl.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://3g.fanxiaobao.xyz/Article/details/gzdwoaymw.sHtML

TS:   s.match(/\d+/g)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gujswsrcz.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://read.share.fanxiaobao.xyz/Article/details/gplolvisy.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gpmvoedxv.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.share.fanxiaobao.xyz/Article/details/gbwouwojn.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtjtklcgz.sHtML

[I03] 提取捕获分组
来源：http://blog.fanxiaobao.xyz/Article/details/gfbjnoubj.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gfttzflyc.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mobile.fanxiaobao.xyz/Article/details/gtfxmoysi.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://3g.fanxiaobao.xyz/Article/details/gmonxebpk.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://m.share.fanxiaobao.xyz/Article/details/ghlnioyas.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://3g.fanxiaobao.xyz/Article/details/gaewzsgcx.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://read.share.fanxiaobao.xyz/Article/details/gtnsenahk.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://blog.fanxiaobao.xyz/Article/details/gnnocbqqt.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://baike.fanxiaobao.xyz/Article/details/gcbpuxlhe.sHtML

[I04] 正则替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gosmxxtjd.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://baike.fanxiaobao.xyz/Article/details/gybytcpdf.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://baike.fanxiaobao.xyz/Article/details/gvdelgdux.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.share.fanxiaobao.xyz/Article/details/gwfudqadv.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.share.fanxiaobao.xyz/Article/details/ghtdvivtt.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://m.share.fanxiaobao.xyz/Article/details/gmpqdzgch.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfmvuvxwa.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://blog.fanxiaobao.xyz/Article/details/ghcpncdfz.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://read.share.fanxiaobao.xyz/Article/details/gecgdwzod.sHtML

[I05] 按正则拆分
来源：http://read.share.fanxiaobao.xyz/Article/details/gewchplvd.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://wap.fanxiaobao.xyz/Article/details/gaykdcbaf.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://baike.fanxiaobao.xyz/Article/details/genbqbyce.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjrsqscnf.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://3g.fanxiaobao.xyz/Article/details/gqixlfydc.sHtML

Java: s.split("\\s*,\\s*")
来源：http://blog.fanxiaobao.xyz/Article/details/gymntaucc.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gztilfrpi.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://3g.fanxiaobao.xyz/Article/details/gbmhezzjj.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.share.fanxiaobao.xyz/Article/details/gpjjvchjm.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gopvztfje.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://3g.fanxiaobao.xyz/Article/details/gktbgaeuc.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcxcoywvi.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gahwcgwxw.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmodqieys.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://m.share.fanxiaobao.xyz/Article/details/gztgkflvz.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmaklpmxr.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wap.fanxiaobao.xyz/Article/details/grzdjvebu.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://blog.fanxiaobao.xyz/Article/details/gsnnzijvc.sHtML

[I07] 忽略大小写与多行模式
来源：http://baike.fanxiaobao.xyz/Article/details/gxqctkolv.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://baike.fanxiaobao.xyz/Article/details/glujgugio.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mobile.fanxiaobao.xyz/Article/details/gmsidmrtj.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://3g.fanxiaobao.xyz/Article/details/gwocabkys.sHtML

TS:   /error/gim
来源：http://wap.fanxiaobao.xyz/Article/details/gkhuamdac.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnbqkhbio.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://3g.fanxiaobao.xyz/Article/details/gujgreopr.sHtML

Ruby: s.scan(/error/i)
来源：http://3g.fanxiaobao.xyz/Article/details/gnczdcmfk.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://read.share.fanxiaobao.xyz/Article/details/gungigmyr.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyfeespaj.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://blog.fanxiaobao.xyz/Article/details/gpvccxyuh.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvaclletp.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.fanxiaobao.xyz/Article/details/gnvastmwu.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.fanxiaobao.xyz/Article/details/gsvilaoke.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gngrkmazp.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.share.fanxiaobao.xyz/Article/details/glpiollfs.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://baike.fanxiaobao.xyz/Article/details/gmqigevry.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsadgfyqp.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gbvqthtqv.sHtML

J. 日期与时间
来源：http://m.share.fanxiaobao.xyz/Article/details/gqmdjazmj.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gubpgfswu.sHtML

[J01] 获取当前时间
来源：http://wap.fanxiaobao.xyz/Article/details/gbuhfikxl.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://mobile.fanxiaobao.xyz/Article/details/gxzbhfjmz.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.share.fanxiaobao.xyz/Article/details/gljcsmtce.sHtML

JS:   new Date();  Date.now()
来源：http://m.share.fanxiaobao.xyz/Article/details/gfaxcwyve.sHtML

TS:   new Date();  Date.now()
来源：http://wap.fanxiaobao.xyz/Article/details/gyjyorehm.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gujzlsmzk.sHtML

Go:   time.Now()
来源：http://baike.fanxiaobao.xyz/Article/details/gjjajslpu.sHtML

Ruby: Time.now
来源：http://blog.fanxiaobao.xyz/Article/details/grbufbpkz.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkkypuktf.sHtML

[J02] 格式化输出
来源：http://baike.fanxiaobao.xyz/Article/details/gftjcpljj.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.fanxiaobao.xyz/Article/details/gxwkpohey.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wap.fanxiaobao.xyz/Article/details/goygzipid.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mobile.fanxiaobao.xyz/Article/details/gtzqdrmfr.sHtML

TS:   d.toISOString()
来源：http://baike.fanxiaobao.xyz/Article/details/gpogygsgs.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geexiyotl.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://3g.fanxiaobao.xyz/Article/details/gvejovgcs.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.fanxiaobao.xyz/Article/details/gqnmseprz.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://blog.fanxiaobao.xyz/Article/details/gsvfffkxk.sHtML

[J03] 字符串解析为日期
来源：http://wap.fanxiaobao.xyz/Article/details/gdsyhwbhl.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.share.fanxiaobao.xyz/Article/details/gwvpnbgos.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://baike.fanxiaobao.xyz/Article/details/ghglnnwxy.sHtML

JS:   new Date("2024-01-02")
来源：http://blog.fanxiaobao.xyz/Article/details/gbrhwipfc.sHtML

TS:   new Date("2024-01-02")
来源：http://blog.fanxiaobao.xyz/Article/details/ggtitztef.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.share.fanxiaobao.xyz/Article/details/ggbpaenxq.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://m.share.fanxiaobao.xyz/Article/details/gxzrwfsbq.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://blog.fanxiaobao.xyz/Article/details/gdwgjifzs.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://read.share.fanxiaobao.xyz/Article/details/gymagnrfb.sHtML

[J04] 时间戳与日期互转
来源：http://blog.fanxiaobao.xyz/Article/details/gfjccctso.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gquxppfyk.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://m.share.fanxiaobao.xyz/Article/details/gftvpmqms.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://blog.fanxiaobao.xyz/Article/details/gnzxukvlg.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://read.share.fanxiaobao.xyz/Article/details/gpvugmqmi.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gejgbdovn.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.blog.fanxiaobao.xyz/Article/details/geuwfmmhg.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://m.share.fanxiaobao.xyz/Article/details/gfobzasdn.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://read.share.fanxiaobao.xyz/Article/details/ghnfdokzz.sHtML

[J05] 时间加减（加 7 天）
来源：http://mobile.fanxiaobao.xyz/Article/details/gtqedwrnf.sHtML

Py:   now + timedelta(days=7)
来源：http://3g.fanxiaobao.xyz/Article/details/gklsjkuro.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://3g.fanxiaobao.xyz/Article/details/gkcqkasaa.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.fanxiaobao.xyz/Article/details/gbdudjrqc.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.fanxiaobao.xyz/Article/details/gwslooblk.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://wap.fanxiaobao.xyz/Article/details/grhormrbq.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://baike.fanxiaobao.xyz/Article/details/gnroeyfli.sHtML

Ruby: Time.now + 7 * 86400
来源：http://3g.fanxiaobao.xyz/Article/details/ggtuqdxtn.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://wap.fanxiaobao.xyz/Article/details/gmpefffpb.sHtML

[J06] 计算两时间之差
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grbetzrap.sHtML

Py:   (end - start).total_seconds()
来源：http://read.share.fanxiaobao.xyz/Article/details/ggmkycrqs.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.share.fanxiaobao.xyz/Article/details/gqtedbqcu.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wap.fanxiaobao.xyz/Article/details/gvgmvykuz.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mobile.fanxiaobao.xyz/Article/details/gowrkhmfq.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://3g.fanxiaobao.xyz/Article/details/gquoophjv.sHtML

Go:   end.Sub(start).Hours()
来源：http://wap.fanxiaobao.xyz/Article/details/gxuekgukt.sHtML

Ruby: end - start                 # 返回秒数
来源：http://mobile.fanxiaobao.xyz/Article/details/gjiynijwt.sHtML

C#:   (end - start).TotalSeconds
来源：http://blog.fanxiaobao.xyz/Article/details/gmjbbspff.sHtML

[J07] 比较两个日期
来源：http://3g.fanxiaobao.xyz/Article/details/gxflnayuu.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://wap.fanxiaobao.xyz/Article/details/gmhwvjwgl.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwhxxmdrb.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://baike.fanxiaobao.xyz/Article/details/gcnhonvqe.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://3g.fanxiaobao.xyz/Article/details/ggawjudbb.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://read.share.fanxiaobao.xyz/Article/details/glmtmoybe.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://read.share.fanxiaobao.xyz/Article/details/ggbykkysp.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://baike.fanxiaobao.xyz/Article/details/gbmonlron.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzwelntaq.sHtML

[J08] 提取年月日与星期
来源：http://baike.fanxiaobao.xyz/Article/details/gacpretxm.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.share.fanxiaobao.xyz/Article/details/giupbudds.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://baike.fanxiaobao.xyz/Article/details/gwarnncwk.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://read.share.fanxiaobao.xyz/Article/details/gbychqcmx.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://m.share.fanxiaobao.xyz/Article/details/giciasokh.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.share.fanxiaobao.xyz/Article/details/gjazyebeu.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://blog.fanxiaobao.xyz/Article/details/gcftfnewt.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://3g.fanxiaobao.xyz/Article/details/gamkggfxg.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://blog.fanxiaobao.xyz/Article/details/gckavxaej.sHtML

[J09] 时区处理
来源：http://wap.fanxiaobao.xyz/Article/details/gzcrkjsqs.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcweuzjoq.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.share.fanxiaobao.xyz/Article/details/gvzycxlhg.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzkumhduz.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.fanxiaobao.xyz/Article/details/gipjhtoib.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://3g.fanxiaobao.xyz/Article/details/gaporkdbi.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mobile.fanxiaobao.xyz/Article/details/gbonvgpax.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://read.share.fanxiaobao.xyz/Article/details/gmltrqsbq.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmmxdpjlh.sHtML

[J10] 取今天 / 本月第一天
来源：http://wap.fanxiaobao.xyz/Article/details/gnprteziq.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://wap.fanxiaobao.xyz/Article/details/gkriyrwtk.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.share.fanxiaobao.xyz/Article/details/gudrzbdtk.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gwwynlshb.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://blog.fanxiaobao.xyz/Article/details/gbhrtpnbn.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gxjfjuvkh.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://read.share.fanxiaobao.xyz/Article/details/gsfyvfudf.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://read.share.fanxiaobao.xyz/Article/details/gcrqibhhj.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gymjwrzjj.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gcjfqvitq.sHtML

K. JSON 与序列化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goqcencjs.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gglcpwavo.sHtML

[K01] 对象转 JSON 字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gggkumrnf.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://m.share.fanxiaobao.xyz/Article/details/gpmnhplju.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gympedumk.sHtML

JS:   JSON.stringify(obj)
来源：http://3g.fanxiaobao.xyz/Article/details/gicoatwdn.sHtML

TS:   JSON.stringify(obj)
来源：http://m.share.fanxiaobao.xyz/Article/details/gljvzrabw.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://read.share.fanxiaobao.xyz/Article/details/gukpjfdjp.sHtML

Go:   json.Marshal(obj)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbfoddeeo.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://3g.fanxiaobao.xyz/Article/details/giimpvufy.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://m.share.fanxiaobao.xyz/Article/details/geqktadmh.sHtML

[K02] JSON 字符串转对象
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvylgzhkk.sHtML

Py:   json.loads(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gikhpvkce.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wap.fanxiaobao.xyz/Article/details/gathfqpdj.sHtML

JS:   JSON.parse(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gtjejpwms.sHtML

TS:   JSON.parse(s)
来源：http://3g.fanxiaobao.xyz/Article/details/giebsscvg.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://read.share.fanxiaobao.xyz/Article/details/gyprxendd.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://wap.fanxiaobao.xyz/Article/details/gzkmzbuwf.sHtML

Ruby: JSON.parse(s)
来源：http://baike.fanxiaobao.xyz/Article/details/guimywgkd.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gyspldsks.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://wap.fanxiaobao.xyz/Article/details/gxfubksud.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggkbookga.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://read.share.fanxiaobao.xyz/Article/details/gabdbrerh.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkbhnwjhq.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gndsowctm.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://m.share.fanxiaobao.xyz/Article/details/ghoienycp.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wap.fanxiaobao.xyz/Article/details/garpslhuj.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://read.share.fanxiaobao.xyz/Article/details/gkmfzwjqx.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://read.share.fanxiaobao.xyz/Article/details/glgirhbxu.sHtML

[K04] 读取 JSON 文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkbbostae.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtcfnfini.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://blog.fanxiaobao.xyz/Article/details/gfqlvqquq.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.fanxiaobao.xyz/Article/details/gocdcwozv.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.fanxiaobao.xyz/Article/details/gjubmjfhu.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mobile.fanxiaobao.xyz/Article/details/gduwqzril.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.share.fanxiaobao.xyz/Article/details/gyrulqufh.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://3g.fanxiaobao.xyz/Article/details/gutlqqqaj.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://baike.fanxiaobao.xyz/Article/details/gkmnqdnen.sHtML

[K05] 深拷贝对象
来源：http://baike.fanxiaobao.xyz/Article/details/gtjwizxch.sHtML

Py:   copy.deepcopy(obj)
来源：http://wap.fanxiaobao.xyz/Article/details/gtspjptpl.sHtML

PHP:  unserialize(serialize($obj));
来源：http://blog.fanxiaobao.xyz/Article/details/ghbltqurd.sHtML

JS:   structuredClone(obj)
来源：http://m.share.fanxiaobao.xyz/Article/details/giwdpcxlh.sHtML

TS:   structuredClone(obj)
来源：http://blog.fanxiaobao.xyz/Article/details/ghaapvtwz.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://m.share.fanxiaobao.xyz/Article/details/gvthtezav.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://read.share.fanxiaobao.xyz/Article/details/gmmxudxuj.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.share.fanxiaobao.xyz/Article/details/gkdfgnciv.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzcdqcouq.sHtML

[K06] 解析 URL 查询串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gujcdxcqh.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://m.share.fanxiaobao.xyz/Article/details/gkhoasfgx.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://3g.fanxiaobao.xyz/Article/details/gyzrfswty.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gharotcnl.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.fanxiaobao.xyz/Article/details/grvjvinsl.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://blog.fanxiaobao.xyz/Article/details/gamgjceuv.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://blog.fanxiaobao.xyz/Article/details/gdnqoceiq.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wap.fanxiaobao.xyz/Article/details/gkuzkqzyn.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://baike.fanxiaobao.xyz/Article/details/gjkuyrnyl.sHtML

[K07] 进制转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gpkwbhqao.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://3g.fanxiaobao.xyz/Article/details/gyxgxjxyk.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://read.share.fanxiaobao.xyz/Article/details/goksxywmg.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://blog.fanxiaobao.xyz/Article/details/gajsyixdn.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grxckubxf.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.share.fanxiaobao.xyz/Article/details/gfaqayplu.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://blog.fanxiaobao.xyz/Article/details/gmhkwnbxk.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mobile.fanxiaobao.xyz/Article/details/gukllbdey.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.share.fanxiaobao.xyz/Article/details/guwlztnin.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://mobile.fanxiaobao.xyz/Article/details/gqilbudgl.sHtML

Py:   pickle.dumps(obj)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gixwoihip.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://baike.fanxiaobao.xyz/Article/details/gpyxvihdb.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyjrzfcpw.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://read.share.fanxiaobao.xyz/Article/details/grnrljixy.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://m.share.fanxiaobao.xyz/Article/details/gurvczknr.sHtML

Go:   encoding/gob
来源：http://3g.fanxiaobao.xyz/Article/details/gigbyawkx.sHtML

Ruby: Marshal.dump(obj)
来源：http://mobile.fanxiaobao.xyz/Article/details/gduaywkcj.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://m.share.fanxiaobao.xyz/Article/details/grubflcbo.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gkrllqnwz.sHtML

L. 网络请求
来源：http://www.share.fanxiaobao.xyz/Article/details/gafpfnswf.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/grbyiebhp.sHtML

[L01] 发送 GET 请求
来源：http://wap.fanxiaobao.xyz/Article/details/gdkeczzqu.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mobile.fanxiaobao.xyz/Article/details/gkfabkjfc.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mobile.fanxiaobao.xyz/Article/details/guigfwcnm.sHtML

JS:   await fetch(url)
来源：http://baike.fanxiaobao.xyz/Article/details/gsxuyteeg.sHtML

TS:   await fetch(url)
来源：http://blog.fanxiaobao.xyz/Article/details/gdosqvpmm.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://read.share.fanxiaobao.xyz/Article/details/guupurilu.sHtML


<!-- 参考信息 -->