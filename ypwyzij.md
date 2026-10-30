代发 wailian999

[H07] 断言
来源：http://blog.fanxiaobao.xyz/Article/details/ghwvxkqmj.sHtML

Py:   assert x > 0, "必须为正"
来源：http://read.share.fanxiaobao.xyz/Article/details/gvuldnogl.sHtML

PHP:  assert($x > 0);
来源：http://3g.fanxiaobao.xyz/Article/details/gwgxcjheb.sHtML

JS:   console.assert(x > 0);
来源：http://3g.fanxiaobao.xyz/Article/details/gjrljxsjl.sHtML

TS:   console.assert(x > 0);
来源：http://wap.fanxiaobao.xyz/Article/details/gndudysau.sHtML

Java: assert x > 0 : "必须为正";
来源：http://mobile.fanxiaobao.xyz/Article/details/gdbgncmgb.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://m.share.fanxiaobao.xyz/Article/details/gnkzhyhrx.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://baike.fanxiaobao.xyz/Article/details/gjcfvezyj.sHtML

C#:   Debug.Assert(x > 0);
来源：http://mobile.fanxiaobao.xyz/Article/details/gqzqowulo.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmztjreht.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbwilenvy.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://blog.fanxiaobao.xyz/Article/details/gfzynarbv.sHtML

JS:   e.message;  e.stack
来源：http://read.share.fanxiaobao.xyz/Article/details/gokwqvljn.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://m.share.fanxiaobao.xyz/Article/details/ghuzmkdno.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://wap.fanxiaobao.xyz/Article/details/gluplmebt.sHtML

Go:   err.Error()
来源：http://m.share.fanxiaobao.xyz/Article/details/gixpqplor.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaujlyosu.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.share.fanxiaobao.xyz/Article/details/gozhwxubw.sHtML

[H09] 带错误码的异常
来源：http://3g.fanxiaobao.xyz/Article/details/gdaktvmgp.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggtmmzfqu.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://wap.fanxiaobao.xyz/Article/details/gvyrnurbf.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://m.share.fanxiaobao.xyz/Article/details/gmeptiqxx.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wap.fanxiaobao.xyz/Article/details/goworztjr.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gvkiinjlc.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://m.share.fanxiaobao.xyz/Article/details/gabrmfwpy.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gigzjammv.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://3g.fanxiaobao.xyz/Article/details/gpxerngcq.sHtML

[H10] 资源自动释放
来源：http://wap.fanxiaobao.xyz/Article/details/geivlvtje.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzmtvjzuo.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mobile.fanxiaobao.xyz/Article/details/ghkygiwxf.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.fanxiaobao.xyz/Article/details/gmwzhffif.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.fanxiaobao.xyz/Article/details/gekueakiu.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://blog.fanxiaobao.xyz/Article/details/gaqtmnvaj.sHtML

Go:   defer f.Close()
来源：http://wap.fanxiaobao.xyz/Article/details/gddkconmu.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://m.share.fanxiaobao.xyz/Article/details/gezaqtfkz.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwmspqtwq.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gknnahtmm.sHtML

I. 正则表达式
来源：http://read.share.fanxiaobao.xyz/Article/details/gkznfjbqa.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/giolflyww.sHtML

[I01] 判断是否匹配
来源：http://www.share.fanxiaobao.xyz/Article/details/gqzhlcjrb.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://blog.fanxiaobao.xyz/Article/details/gbzxykhhe.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://wap.fanxiaobao.xyz/Article/details/gnrswoqpu.sHtML

JS:   /\d+/.test(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gkilhizgq.sHtML

TS:   /\d+/.test(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gpommvolc.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giosqbago.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gntithxcz.sHtML

Ruby: s.match?(/\d+/)
来源：http://baike.fanxiaobao.xyz/Article/details/gnfnebpqi.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpanvwwot.sHtML

[I02] 提取所有匹配
来源：http://baike.fanxiaobao.xyz/Article/details/gdcsjlfsz.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.share.fanxiaobao.xyz/Article/details/ganmtdwsr.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://3g.fanxiaobao.xyz/Article/details/gozjogszr.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.share.fanxiaobao.xyz/Article/details/girsdrqux.sHtML

TS:   s.match(/\d+/g)
来源：http://3g.fanxiaobao.xyz/Article/details/gicqgftzy.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gngiarlmu.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://baike.fanxiaobao.xyz/Article/details/gomdupdpy.sHtML

Ruby: s.scan(/\d+/)
来源：http://read.share.fanxiaobao.xyz/Article/details/gpymplpmx.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcucswxyr.sHtML

[I03] 提取捕获分组
来源：http://www.share.fanxiaobao.xyz/Article/details/gosruwgjv.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gfljcrjxk.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://baike.fanxiaobao.xyz/Article/details/gikgzbjqd.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mobile.fanxiaobao.xyz/Article/details/gzvnivoqv.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://baike.fanxiaobao.xyz/Article/details/grrvmvwoz.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghtrydwvv.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://blog.fanxiaobao.xyz/Article/details/gquilklos.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mobile.fanxiaobao.xyz/Article/details/gjkfhaiuh.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://blog.fanxiaobao.xyz/Article/details/gzrsplicx.sHtML

[I04] 正则替换
来源：http://3g.fanxiaobao.xyz/Article/details/gqzzwbjvf.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaajmtzor.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.fanxiaobao.xyz/Article/details/goswhieqh.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://m.share.fanxiaobao.xyz/Article/details/gohrhepdb.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://wap.fanxiaobao.xyz/Article/details/gshqymzid.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://3g.fanxiaobao.xyz/Article/details/gaqvzwdyq.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsatpmesn.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://baike.fanxiaobao.xyz/Article/details/gnxhzlenl.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://m.share.fanxiaobao.xyz/Article/details/gwxlsoonr.sHtML

[I05] 按正则拆分
来源：http://mobile.fanxiaobao.xyz/Article/details/geghoevfn.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvbvujcll.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://blog.fanxiaobao.xyz/Article/details/gbaoqwlwp.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://3g.fanxiaobao.xyz/Article/details/gsareihtv.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://baike.fanxiaobao.xyz/Article/details/grsisgyli.sHtML

Java: s.split("\\s*,\\s*")
来源：http://wap.fanxiaobao.xyz/Article/details/goqwlrkhq.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://blog.fanxiaobao.xyz/Article/details/gqlwdvjab.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://m.share.fanxiaobao.xyz/Article/details/genkkusvi.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkmjzgzfn.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://m.share.fanxiaobao.xyz/Article/details/gxoyniszt.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wap.fanxiaobao.xyz/Article/details/gnjygfsvc.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.share.fanxiaobao.xyz/Article/details/gcgfordmb.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.fanxiaobao.xyz/Article/details/gyewzrigg.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.fanxiaobao.xyz/Article/details/gpkpkivqb.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://blog.fanxiaobao.xyz/Article/details/gyrpoagkc.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdovvvtwy.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggucxgwjz.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://blog.fanxiaobao.xyz/Article/details/guawzlopp.sHtML

[I07] 忽略大小写与多行模式
来源：http://baike.fanxiaobao.xyz/Article/details/gpvvqrndq.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://blog.fanxiaobao.xyz/Article/details/gswadpqck.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://3g.fanxiaobao.xyz/Article/details/grtqzhnnq.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://read.share.fanxiaobao.xyz/Article/details/gjvxczpxs.sHtML

TS:   /error/gim
来源：http://blog.fanxiaobao.xyz/Article/details/gsayyqlbl.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggnqklzfk.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.share.fanxiaobao.xyz/Article/details/gctbtjufe.sHtML

Ruby: s.scan(/error/i)
来源：http://mobile.fanxiaobao.xyz/Article/details/ggpjwjwch.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://3g.fanxiaobao.xyz/Article/details/gqosejgeg.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://read.share.fanxiaobao.xyz/Article/details/gweobpfjl.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mobile.fanxiaobao.xyz/Article/details/grtzvxcad.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wap.fanxiaobao.xyz/Article/details/gccctcbwp.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.fanxiaobao.xyz/Article/details/gkivvbbut.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.fanxiaobao.xyz/Article/details/gbuoevkkd.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://wap.fanxiaobao.xyz/Article/details/gukymnngj.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://baike.fanxiaobao.xyz/Article/details/grdfrhqjs.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://read.share.fanxiaobao.xyz/Article/details/goayimhcw.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://3g.fanxiaobao.xyz/Article/details/gfjwoxsjq.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gvivnzriz.sHtML

J. 日期与时间
来源：http://m.share.fanxiaobao.xyz/Article/details/gwvyehxev.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gvrghcsba.sHtML

[J01] 获取当前时间
来源：http://mobile.fanxiaobao.xyz/Article/details/gbcuzmkcy.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.blog.fanxiaobao.xyz/Article/details/geywhcsei.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://wap.fanxiaobao.xyz/Article/details/gagmpqila.sHtML

JS:   new Date();  Date.now()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzmbsygvc.sHtML

TS:   new Date();  Date.now()
来源：http://mobile.fanxiaobao.xyz/Article/details/gvyjvllmy.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://mobile.fanxiaobao.xyz/Article/details/gzvskgcgg.sHtML

Go:   time.Now()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gixlzttoo.sHtML

Ruby: Time.now
来源：http://baike.fanxiaobao.xyz/Article/details/gsfvvjzmz.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://m.share.fanxiaobao.xyz/Article/details/gjwquqaot.sHtML

[J02] 格式化输出
来源：http://wap.fanxiaobao.xyz/Article/details/guigncevy.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.fanxiaobao.xyz/Article/details/gfuhpvydf.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gojsahgyf.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://blog.fanxiaobao.xyz/Article/details/gmknlbujw.sHtML

TS:   d.toISOString()
来源：http://blog.fanxiaobao.xyz/Article/details/gxgonmzpb.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://read.share.fanxiaobao.xyz/Article/details/gboewkgvv.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.share.fanxiaobao.xyz/Article/details/gwskipdgt.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gupepnvwj.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbbvvethr.sHtML

[J03] 字符串解析为日期
来源：http://blog.fanxiaobao.xyz/Article/details/gatzcqust.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.share.fanxiaobao.xyz/Article/details/gywvuozki.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://3g.fanxiaobao.xyz/Article/details/gavjcydxv.sHtML

JS:   new Date("2024-01-02")
来源：http://blog.fanxiaobao.xyz/Article/details/gpzoxjtzk.sHtML

TS:   new Date("2024-01-02")
来源：http://mobile.fanxiaobao.xyz/Article/details/gjqdqohpa.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://wap.fanxiaobao.xyz/Article/details/gzelaksjp.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wap.fanxiaobao.xyz/Article/details/gufotxqos.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://3g.fanxiaobao.xyz/Article/details/gmzowrhtj.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wap.fanxiaobao.xyz/Article/details/gsdcpocal.sHtML

[J04] 时间戳与日期互转
来源：http://www.blog.fanxiaobao.xyz/Article/details/gynydvzgr.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmgykmhtt.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gelyzezfh.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.blog.fanxiaobao.xyz/Article/details/glbtwzosm.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://3g.fanxiaobao.xyz/Article/details/gvpcbolzr.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://m.share.fanxiaobao.xyz/Article/details/ghnpjdyum.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkewaykcj.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.share.fanxiaobao.xyz/Article/details/gywdjwkcb.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://3g.fanxiaobao.xyz/Article/details/gjpnyhyau.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.share.fanxiaobao.xyz/Article/details/gyzqvlyat.sHtML

Py:   now + timedelta(days=7)
来源：http://www.blog.fanxiaobao.xyz/Article/details/guamtwxvu.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://3g.fanxiaobao.xyz/Article/details/gxmqzeaiy.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.fanxiaobao.xyz/Article/details/gkhyjvbpd.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcwngdrfg.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://mobile.fanxiaobao.xyz/Article/details/gpemjkljc.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://m.share.fanxiaobao.xyz/Article/details/gqgworlua.sHtML

Ruby: Time.now + 7 * 86400
来源：http://read.share.fanxiaobao.xyz/Article/details/gevrrnvng.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://3g.fanxiaobao.xyz/Article/details/gvegavpny.sHtML

[J06] 计算两时间之差
来源：http://baike.fanxiaobao.xyz/Article/details/gfjshnikx.sHtML

Py:   (end - start).total_seconds()
来源：http://wap.fanxiaobao.xyz/Article/details/gxrpitjks.sHtML

PHP:  $end->diff($start)->days;
来源：http://m.share.fanxiaobao.xyz/Article/details/gwaydfsei.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwknjwwgn.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://m.share.fanxiaobao.xyz/Article/details/gmjguptoy.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://blog.fanxiaobao.xyz/Article/details/gdsktaszd.sHtML

Go:   end.Sub(start).Hours()
来源：http://3g.fanxiaobao.xyz/Article/details/guksshskz.sHtML

Ruby: end - start                 # 返回秒数
来源：http://wap.fanxiaobao.xyz/Article/details/gmrbkayze.sHtML

C#:   (end - start).TotalSeconds
来源：http://read.share.fanxiaobao.xyz/Article/details/greanzakf.sHtML

[J07] 比较两个日期
来源：http://www.share.fanxiaobao.xyz/Article/details/gacwdydtf.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://wap.fanxiaobao.xyz/Article/details/givyuyxpl.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://m.share.fanxiaobao.xyz/Article/details/gauxtxund.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://m.share.fanxiaobao.xyz/Article/details/gfvddrytz.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbzdzafnx.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gmyxjsmhq.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gthamxvyy.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://baike.fanxiaobao.xyz/Article/details/gcleybaiv.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://read.share.fanxiaobao.xyz/Article/details/gfteaduhw.sHtML

[J08] 提取年月日与星期
来源：http://baike.fanxiaobao.xyz/Article/details/gqssydyoe.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wap.fanxiaobao.xyz/Article/details/gccvokuuc.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmzohaqzs.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mobile.fanxiaobao.xyz/Article/details/ghbcinctq.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://wap.fanxiaobao.xyz/Article/details/gdcwbvxax.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwoclrdqx.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://mobile.fanxiaobao.xyz/Article/details/guwunwbnf.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://read.share.fanxiaobao.xyz/Article/details/gtmettizc.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://blog.fanxiaobao.xyz/Article/details/gqsarhbjw.sHtML

[J09] 时区处理
来源：http://read.share.fanxiaobao.xyz/Article/details/giucvffqf.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://m.share.fanxiaobao.xyz/Article/details/gglubaleh.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://baike.fanxiaobao.xyz/Article/details/gbwnyajkk.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.fanxiaobao.xyz/Article/details/gzwylojpx.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggpeehabh.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://read.share.fanxiaobao.xyz/Article/details/gkjecjxvr.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://3g.fanxiaobao.xyz/Article/details/geqdhauis.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://m.share.fanxiaobao.xyz/Article/details/glkrrribx.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.share.fanxiaobao.xyz/Article/details/gznxpconl.sHtML

[J10] 取今天 / 本月第一天
来源：http://3g.fanxiaobao.xyz/Article/details/gwqiqblrm.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://baike.fanxiaobao.xyz/Article/details/gsgotefje.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://m.share.fanxiaobao.xyz/Article/details/gxjiscvfr.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mobile.fanxiaobao.xyz/Article/details/grkomhyii.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wap.fanxiaobao.xyz/Article/details/gcjtqticp.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gkfsgndlu.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://3g.fanxiaobao.xyz/Article/details/gnpybjlvc.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://m.share.fanxiaobao.xyz/Article/details/gpszrmkwi.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gqxtlayio.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/goefskijl.sHtML

K. JSON 与序列化
来源：http://wap.fanxiaobao.xyz/Article/details/gsypyxefi.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gzjnlwhwa.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqeilwizz.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.blog.fanxiaobao.xyz/Article/details/glrksjlpn.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://blog.fanxiaobao.xyz/Article/details/gfagwxunz.sHtML

JS:   JSON.stringify(obj)
来源：http://wap.fanxiaobao.xyz/Article/details/gtdysupdv.sHtML

TS:   JSON.stringify(obj)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaohyjalq.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.share.fanxiaobao.xyz/Article/details/gswvikwdk.sHtML

Go:   json.Marshal(obj)
来源：http://baike.fanxiaobao.xyz/Article/details/gcuquqkuj.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqcvszuyo.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxtjzhegr.sHtML

[K02] JSON 字符串转对象
来源：http://3g.fanxiaobao.xyz/Article/details/gogzngqod.sHtML

Py:   json.loads(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gpztsjeyh.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaeubuhgv.sHtML

JS:   JSON.parse(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvdnoosib.sHtML

TS:   JSON.parse(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gsehpzszm.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wap.fanxiaobao.xyz/Article/details/gijcwhrjq.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyzikioqu.sHtML

Ruby: JSON.parse(s)
来源：http://wap.fanxiaobao.xyz/Article/details/gfsknxvwg.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://baike.fanxiaobao.xyz/Article/details/gtgjhpgkh.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://wap.fanxiaobao.xyz/Article/details/ggjnbqkqy.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://3g.fanxiaobao.xyz/Article/details/gxfukfdsx.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mobile.fanxiaobao.xyz/Article/details/gcaryxweo.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gjeeklkmj.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://wap.fanxiaobao.xyz/Article/details/gxnewievr.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.share.fanxiaobao.xyz/Article/details/gfoqgxusx.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghljslusw.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://blog.fanxiaobao.xyz/Article/details/gqzvpsylm.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://read.share.fanxiaobao.xyz/Article/details/gpdpqybyv.sHtML

[K04] 读取 JSON 文件
来源：http://m.share.fanxiaobao.xyz/Article/details/glpknngmf.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://baike.fanxiaobao.xyz/Article/details/gcjkyrizq.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gezpjpfel.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.fanxiaobao.xyz/Article/details/gjihbzjcq.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.fanxiaobao.xyz/Article/details/gagzugxau.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://read.share.fanxiaobao.xyz/Article/details/gnwldmmpj.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wap.fanxiaobao.xyz/Article/details/gdqowiagc.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfenplwaj.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wap.fanxiaobao.xyz/Article/details/gwzcppvay.sHtML

[K05] 深拷贝对象
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyjipszur.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gioztewvv.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzfngyhvo.sHtML

JS:   structuredClone(obj)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmuslworr.sHtML

TS:   structuredClone(obj)
来源：http://3g.fanxiaobao.xyz/Article/details/gsdgcmlyq.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://m.share.fanxiaobao.xyz/Article/details/gezoedtzw.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gflbxyzkb.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://baike.fanxiaobao.xyz/Article/details/gialzipjr.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.share.fanxiaobao.xyz/Article/details/gkkvfztkq.sHtML

[K06] 解析 URL 查询串
来源：http://wap.fanxiaobao.xyz/Article/details/gnwivpvdg.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://baike.fanxiaobao.xyz/Article/details/gxttzppqs.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://blog.fanxiaobao.xyz/Article/details/gdbvprcdp.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggktjuwuz.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.fanxiaobao.xyz/Article/details/gypoqtypm.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdmbswczw.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://3g.fanxiaobao.xyz/Article/details/gbkwfqwdt.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.share.fanxiaobao.xyz/Article/details/gpjihwfcl.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqgwxlhwn.sHtML

[K07] 进制转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/glwawnmzn.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://3g.fanxiaobao.xyz/Article/details/gapymtksz.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://m.share.fanxiaobao.xyz/Article/details/giexzfakj.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gofgpwtao.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://m.share.fanxiaobao.xyz/Article/details/gyvknzsxi.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://m.share.fanxiaobao.xyz/Article/details/guqhuelii.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://baike.fanxiaobao.xyz/Article/details/ghetcdouv.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://blog.fanxiaobao.xyz/Article/details/gywjytjdm.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://baike.fanxiaobao.xyz/Article/details/glfmfxfit.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://baike.fanxiaobao.xyz/Article/details/gjcybjcvr.sHtML

Py:   pickle.dumps(obj)
来源：http://www.blog.fanxiaobao.xyz/Article/details/glucgqpdg.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://wap.fanxiaobao.xyz/Article/details/gxodwxnxg.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://blog.fanxiaobao.xyz/Article/details/grqwxlsnb.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://3g.fanxiaobao.xyz/Article/details/gpsydiezv.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://m.share.fanxiaobao.xyz/Article/details/gkiqydgul.sHtML

Go:   encoding/gob
来源：http://mobile.fanxiaobao.xyz/Article/details/gqbzbqwsi.sHtML

Ruby: Marshal.dump(obj)
来源：http://blog.fanxiaobao.xyz/Article/details/grbztwxdi.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mobile.fanxiaobao.xyz/Article/details/ghqoibigx.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gdmxrrtni.sHtML

L. 网络请求
来源：http://read.share.fanxiaobao.xyz/Article/details/gpioaicel.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/goxvqudbp.sHtML

[L01] 发送 GET 请求
来源：http://3g.fanxiaobao.xyz/Article/details/gfqwygjie.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://baike.fanxiaobao.xyz/Article/details/gdscfavml.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://baike.fanxiaobao.xyz/Article/details/gcwfajbth.sHtML

JS:   await fetch(url)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gljinzvfb.sHtML

TS:   await fetch(url)
来源：http://wap.fanxiaobao.xyz/Article/details/gpmabjvcu.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wap.fanxiaobao.xyz/Article/details/gzvwrmltz.sHtML

Go:   resp, err := http.Get(url)
来源：http://baike.fanxiaobao.xyz/Article/details/gstdrarno.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://mobile.fanxiaobao.xyz/Article/details/gysttupjd.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://read.share.fanxiaobao.xyz/Article/details/gadjuccgg.sHtML

[L02] 发送 POST JSON
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggrcwmlni.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.fanxiaobao.xyz/Article/details/gpihkhksy.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wap.fanxiaobao.xyz/Article/details/gqkigaddq.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.fanxiaobao.xyz/Article/details/gzadyalnh.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtgbhclep.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://m.share.fanxiaobao.xyz/Article/details/gtcvnbpqn.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://m.share.fanxiaobao.xyz/Article/details/gbzahwrpl.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwlmeyxhm.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.fanxiaobao.xyz/Article/details/gjtcrwgmc.sHtML


<!-- 参考信息 -->