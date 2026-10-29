代发 wailian999

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://baike.hesvh.cn/Article/details/gucsfevus.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.share.fehbvm.com/Article/details/geuovyont.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.blog.zdbjq.cn/Article/details/gtixspuxj.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.blog.fehbvm.com/Article/details/gsddyeegl.sHtML

[H07] 断言
来源：http://baike.fehbvm.com/Article/details/ggenzhppi.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.m.share.hesvh.cn/Article/details/gkylqethm.sHtML

PHP:  assert($x > 0);
来源：http://wap.fehbvm.com/Article/details/gaqwheiqe.sHtML

JS:   console.assert(x > 0);
来源：http://m.share.fehbvm.com/Article/details/gwzvrhdif.sHtML

TS:   console.assert(x > 0);
来源：http://wap.zdbjq.cn/Article/details/glggnivnj.sHtML

Java: assert x > 0 : "必须为正";
来源：http://wap.zdbjq.cn/Article/details/gddgcscpi.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://baike.zdbjq.cn/Article/details/gxqumborf.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.share.zdbjq.cn/Article/details/gtgcmyrzl.sHtML

C#:   Debug.Assert(x > 0);
来源：http://blog.fehbvm.com/Article/details/guunvclka.sHtML

[H08] 获取错误信息与堆栈
来源：http://blog.hesvh.cn/Article/details/gbytjxuhv.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://3g.hesvh.cn/Article/details/gbxfrrfpj.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.share.fehbvm.com/Article/details/gvgoanzly.sHtML

JS:   e.message;  e.stack
来源：http://baike.hesvh.cn/Article/details/gkuxuugzm.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.m.share.hesvh.cn/Article/details/grczbozmn.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://mobile.zdbjq.cn/Article/details/gfubidrfk.sHtML

Go:   err.Error()
来源：http://www.m.share.fehbvm.com/Article/details/gizklkdvh.sHtML

Ruby: e.message;  e.backtrace
来源：http://m.share.fehbvm.com/Article/details/gmarxldei.sHtML

C#:   e.Message;  e.StackTrace
来源：http://m.share.hesvh.cn/Article/details/gyewwhvhe.sHtML

[H09] 带错误码的异常
来源：http://read.share.hesvh.cn/Article/details/gjazdhubd.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.share.hesvh.cn/Article/details/gbbxlcgvc.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://mobile.zdbjq.cn/Article/details/goupvxahx.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://m.share.fehbvm.com/Article/details/gknhnexej.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.share.zdbjq.cn/Article/details/grftwvkjg.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mobile.fehbvm.com/Article/details/gjibqqghl.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://3g.zdbjq.cn/Article/details/gkevsgdgu.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://3g.zdbjq.cn/Article/details/ghlfrmvhe.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://baike.hesvh.cn/Article/details/gtyrtighw.sHtML

[H10] 资源自动释放
来源：http://wap.fehbvm.com/Article/details/gjjfsvspn.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.share.hesvh.cn/Article/details/gkqltptby.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.blog.hesvh.cn/Article/details/gsepwrvjj.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.fehbvm.com/Article/details/gyvdjweiq.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.zdbjq.cn/Article/details/gbqpvagsr.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://m.share.hesvh.cn/Article/details/gpgorzhrt.sHtML

Go:   defer f.Close()
来源：http://wap.hesvh.cn/Article/details/gfvsmoapg.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.share.hesvh.cn/Article/details/gulowdclt.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gqdchdjyu.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gcocoasra.sHtML

I. 正则表达式
来源：http://blog.fehbvm.com/Article/details/gdohkyjbg.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/grdegunyx.sHtML

[I01] 判断是否匹配
来源：http://3g.zdbjq.cn/Article/details/gyebxvdgf.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wap.fehbvm.com/Article/details/grlpplyel.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://3g.fehbvm.com/Article/details/goedrkahi.sHtML

JS:   /\d+/.test(s)
来源：http://blog.zdbjq.cn/Article/details/gaabbwqur.sHtML

TS:   /\d+/.test(s)
来源：http://mobile.fehbvm.com/Article/details/grenfeipg.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.share.zdbjq.cn/Article/details/ghrtaimjr.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mobile.hesvh.cn/Article/details/gowjlmpdt.sHtML

Ruby: s.match?(/\d+/)
来源：http://m.share.zdbjq.cn/Article/details/gaknavmry.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://m.share.zdbjq.cn/Article/details/guvjbeygd.sHtML

[I02] 提取所有匹配
来源：http://wap.fehbvm.com/Article/details/gadrpddgb.sHtML

Py:   re.findall(r"\d+", s)
来源：http://read.share.fehbvm.com/Article/details/gaczwncar.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://read.share.fehbvm.com/Article/details/gejhhbkcj.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.m.share.fehbvm.com/Article/details/gfdanqnqw.sHtML

TS:   s.match(/\d+/g)
来源：http://mobile.hesvh.cn/Article/details/gyedewktc.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://m.share.fehbvm.com/Article/details/gmsifupnl.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.blog.hesvh.cn/Article/details/gqpxiwaij.sHtML

Ruby: s.scan(/\d+/)
来源：http://3g.zdbjq.cn/Article/details/gukewvzqm.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.share.zdbjq.cn/Article/details/giadjgymu.sHtML

[I03] 提取捕获分组
来源：http://www.m.share.fehbvm.com/Article/details/gneusdedl.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://3g.zdbjq.cn/Article/details/gkrezrotj.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.share.hesvh.cn/Article/details/gfjfdupfj.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.m.share.hesvh.cn/Article/details/gqncvsdlm.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.m.share.fehbvm.com/Article/details/glppopvlm.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.blog.zdbjq.cn/Article/details/goaanvqos.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://baike.fehbvm.com/Article/details/gyvtnwayc.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://m.share.hesvh.cn/Article/details/gzjlkwery.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.share.fehbvm.com/Article/details/gebvmuahq.sHtML

[I04] 正则替换
来源：http://read.share.zdbjq.cn/Article/details/glhlvofwv.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://baike.fehbvm.com/Article/details/gghppiybb.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mobile.hesvh.cn/Article/details/gnllpwjik.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://wap.zdbjq.cn/Article/details/glpucxfwq.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://baike.hesvh.cn/Article/details/gdmbcvxuc.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://wap.fehbvm.com/Article/details/gtbinvmja.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://3g.hesvh.cn/Article/details/gvxprjder.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://wap.zdbjq.cn/Article/details/glnktospm.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.blog.fehbvm.com/Article/details/gdrszeoxy.sHtML

[I05] 按正则拆分
来源：http://mobile.fehbvm.com/Article/details/govzsdnra.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://mobile.hesvh.cn/Article/details/gzzetbkqu.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wap.hesvh.cn/Article/details/gxfwowblm.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.blog.hesvh.cn/Article/details/gocraowpx.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://read.share.hesvh.cn/Article/details/grpxwpsla.sHtML

Java: s.split("\\s*,\\s*")
来源：http://3g.fehbvm.com/Article/details/gkvybwvri.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://blog.zdbjq.cn/Article/details/gvzpizery.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://3g.hesvh.cn/Article/details/gaemowkdy.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://3g.fehbvm.com/Article/details/godwkawca.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://baike.zdbjq.cn/Article/details/gqfvdeidz.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.m.share.fehbvm.com/Article/details/gfurofxis.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.share.zdbjq.cn/Article/details/gxxcpdkel.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.zdbjq.cn/Article/details/ghdcuzyel.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.hesvh.cn/Article/details/gijanufsu.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.m.share.hesvh.cn/Article/details/ghsjlyosj.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.m.share.zdbjq.cn/Article/details/gzzapwfhs.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wap.zdbjq.cn/Article/details/gijxmomoz.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://blog.fehbvm.com/Article/details/glbnqtyxd.sHtML

[I07] 忽略大小写与多行模式
来源：http://read.share.fehbvm.com/Article/details/grybavhgj.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://read.share.fehbvm.com/Article/details/gnbbedzgx.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://3g.hesvh.cn/Article/details/ggzskevcq.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://read.share.fehbvm.com/Article/details/gvjkvscmf.sHtML

TS:   /error/gim
来源：http://3g.zdbjq.cn/Article/details/gnxltppto.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.share.hesvh.cn/Article/details/gtgivuhme.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://baike.zdbjq.cn/Article/details/gaxpbuncw.sHtML

Ruby: s.scan(/error/i)
来源：http://m.share.fehbvm.com/Article/details/ghzpgbwez.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://m.share.fehbvm.com/Article/details/gxttvpodi.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://m.share.hesvh.cn/Article/details/gtobzedon.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://read.share.zdbjq.cn/Article/details/gygsflzxz.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://baike.hesvh.cn/Article/details/gcnfjjbpq.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.zdbjq.cn/Article/details/gavbznpxd.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.hesvh.cn/Article/details/gsdxkghul.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://3g.zdbjq.cn/Article/details/gzyeqtcfw.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://blog.hesvh.cn/Article/details/gfqhgwjlf.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://blog.hesvh.cn/Article/details/gpzkwzclw.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.m.share.zdbjq.cn/Article/details/gycbfjfxa.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gcaetdszf.sHtML

J. 日期与时间
来源：http://m.share.zdbjq.cn/Article/details/gzqfnihpp.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gwbarbluu.sHtML

[J01] 获取当前时间
来源：http://baike.fehbvm.com/Article/details/gzbghytpj.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://m.share.zdbjq.cn/Article/details/goywlufeb.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://3g.zdbjq.cn/Article/details/gymzbhwnm.sHtML

JS:   new Date();  Date.now()
来源：http://www.share.fehbvm.com/Article/details/gaeyizqlg.sHtML

TS:   new Date();  Date.now()
来源：http://3g.hesvh.cn/Article/details/gmrrqghxr.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://blog.fehbvm.com/Article/details/gmdzbntrn.sHtML

Go:   time.Now()
来源：http://wap.zdbjq.cn/Article/details/gcvgslrob.sHtML

Ruby: Time.now
来源：http://baike.fehbvm.com/Article/details/gguhrljyw.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.m.share.zdbjq.cn/Article/details/gbhgrhojx.sHtML

[J02] 格式化输出
来源：http://wap.hesvh.cn/Article/details/gznkhddkh.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.zdbjq.cn/Article/details/gyxvikdwn.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mobile.hesvh.cn/Article/details/gmthkbjav.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://blog.zdbjq.cn/Article/details/ggrnfnvbz.sHtML

TS:   d.toISOString()
来源：http://read.share.zdbjq.cn/Article/details/gbjawnqla.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://3g.fehbvm.com/Article/details/gmdjboxpg.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wap.hesvh.cn/Article/details/gkfoyduiy.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.fehbvm.com/Article/details/gtkysveac.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://3g.hesvh.cn/Article/details/grkepeugc.sHtML

[J03] 字符串解析为日期
来源：http://www.share.zdbjq.cn/Article/details/gfkeznofe.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://3g.zdbjq.cn/Article/details/gtzcwtyvb.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.blog.hesvh.cn/Article/details/giizsphdw.sHtML

JS:   new Date("2024-01-02")
来源：http://www.share.hesvh.cn/Article/details/gcmjiqbxq.sHtML

TS:   new Date("2024-01-02")
来源：http://www.share.zdbjq.cn/Article/details/glcqnmtqp.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://m.share.fehbvm.com/Article/details/gxtbdakss.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://blog.fehbvm.com/Article/details/gncvpbrnw.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://baike.hesvh.cn/Article/details/gjnrbyyoj.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://read.share.zdbjq.cn/Article/details/geeqistye.sHtML

[J04] 时间戳与日期互转
来源：http://wap.hesvh.cn/Article/details/ggjjugkir.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://m.share.fehbvm.com/Article/details/gunnqvhkh.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://m.share.zdbjq.cn/Article/details/gttxamjyc.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://3g.fehbvm.com/Article/details/gwpxbbfoh.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://3g.fehbvm.com/Article/details/gmhvpzxpr.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://3g.zdbjq.cn/Article/details/gofhotejt.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://read.share.zdbjq.cn/Article/details/gruhofozy.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://read.share.fehbvm.com/Article/details/gcalosqpj.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://read.share.fehbvm.com/Article/details/gpojrclnz.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.share.zdbjq.cn/Article/details/gklzbggde.sHtML

Py:   now + timedelta(days=7)
来源：http://read.share.zdbjq.cn/Article/details/gaojetpfq.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://m.share.zdbjq.cn/Article/details/gwzktyzoc.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.zdbjq.cn/Article/details/gpcbjtyqo.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.fehbvm.com/Article/details/gxmdnzzaz.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://wap.fehbvm.com/Article/details/ghzqmkhus.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://wap.zdbjq.cn/Article/details/gzszzksqt.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.m.share.hesvh.cn/Article/details/gdmiztkgv.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.m.share.fehbvm.com/Article/details/gchjkguuv.sHtML

[J06] 计算两时间之差
来源：http://www.blog.fehbvm.com/Article/details/gzvjfqlry.sHtML

Py:   (end - start).total_seconds()
来源：http://www.m.share.hesvh.cn/Article/details/gktecgkty.sHtML

PHP:  $end->diff($start)->days;
来源：http://wap.zdbjq.cn/Article/details/goragygbx.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://3g.hesvh.cn/Article/details/gnwsomdzi.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.m.share.fehbvm.com/Article/details/garbjdvyo.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.share.zdbjq.cn/Article/details/gnlnqwmkl.sHtML

Go:   end.Sub(start).Hours()
来源：http://baike.hesvh.cn/Article/details/gtzslxewq.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.share.fehbvm.com/Article/details/gweybvgjm.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.m.share.hesvh.cn/Article/details/gljnofkcs.sHtML

[J07] 比较两个日期
来源：http://mobile.fehbvm.com/Article/details/gdztxckat.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://read.share.fehbvm.com/Article/details/gsmmzjjjp.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://3g.fehbvm.com/Article/details/gswzfelcf.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://mobile.fehbvm.com/Article/details/gbtmpegpq.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.fehbvm.com/Article/details/gtqgcuatr.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://blog.zdbjq.cn/Article/details/gwiojpmxl.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.share.fehbvm.com/Article/details/gseheozke.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://3g.hesvh.cn/Article/details/ghczxpqql.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://m.share.hesvh.cn/Article/details/glucmrgkl.sHtML

[J08] 提取年月日与星期
来源：http://www.share.hesvh.cn/Article/details/ggghmdbqx.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://baike.hesvh.cn/Article/details/gakhbuhgb.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://m.share.hesvh.cn/Article/details/gamjrewtx.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.m.share.hesvh.cn/Article/details/gkrhjsber.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.m.share.zdbjq.cn/Article/details/gupwjorqp.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://blog.zdbjq.cn/Article/details/grihqgyia.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://baike.hesvh.cn/Article/details/gvoebyakj.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://read.share.hesvh.cn/Article/details/gsjsxsexi.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://blog.fehbvm.com/Article/details/gzbdoljwl.sHtML

[J09] 时区处理
来源：http://read.share.fehbvm.com/Article/details/grhzytorg.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://read.share.hesvh.cn/Article/details/ghsgzfblm.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.m.share.zdbjq.cn/Article/details/gdqofktuf.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.zdbjq.cn/Article/details/gtyjaafmy.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.fehbvm.com/Article/details/gygrabcoz.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.m.share.fehbvm.com/Article/details/gkmyatduk.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://m.share.hesvh.cn/Article/details/ghoazcaav.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.blog.fehbvm.com/Article/details/gthkdobwm.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://blog.fehbvm.com/Article/details/ggsplckrc.sHtML

[J10] 取今天 / 本月第一天
来源：http://blog.hesvh.cn/Article/details/gdyossycv.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://read.share.zdbjq.cn/Article/details/gpnxewmhs.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wap.hesvh.cn/Article/details/gyvsgtijw.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.share.hesvh.cn/Article/details/gkxocvooh.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://read.share.fehbvm.com/Article/details/geibudrap.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.blog.hesvh.cn/Article/details/geozqojnd.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://m.share.fehbvm.com/Article/details/gzhlpohwi.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://baike.zdbjq.cn/Article/details/gsovzaogv.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://read.share.hesvh.cn/Article/details/geawitbfa.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gvcmxfhtk.sHtML

K. JSON 与序列化
来源：http://www.blog.fehbvm.com/Article/details/gtkbvfrlf.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gouwqzdhp.sHtML

[K01] 对象转 JSON 字符串
来源：http://blog.zdbjq.cn/Article/details/gatybrchv.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.share.zdbjq.cn/Article/details/gftcfycnt.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://m.share.zdbjq.cn/Article/details/goscvkjcg.sHtML

JS:   JSON.stringify(obj)
来源：http://3g.zdbjq.cn/Article/details/giqaytiif.sHtML

TS:   JSON.stringify(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gpqyumjyb.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mobile.zdbjq.cn/Article/details/gcfkcltmz.sHtML

Go:   json.Marshal(obj)
来源：http://3g.zdbjq.cn/Article/details/gkegcwxub.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://wap.hesvh.cn/Article/details/goofzobjt.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://read.share.fehbvm.com/Article/details/gxqnksahi.sHtML

[K02] JSON 字符串转对象
来源：http://read.share.zdbjq.cn/Article/details/gzwcpopjl.sHtML

Py:   json.loads(s)
来源：http://wap.hesvh.cn/Article/details/gomzljimy.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://3g.hesvh.cn/Article/details/gtlwwhodk.sHtML

JS:   JSON.parse(s)
来源：http://baike.hesvh.cn/Article/details/ghxnuhnyr.sHtML

TS:   JSON.parse(s)
来源：http://mobile.zdbjq.cn/Article/details/gfzgwzzsa.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mobile.fehbvm.com/Article/details/glnepnkay.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://baike.fehbvm.com/Article/details/gkoxlpmfg.sHtML

Ruby: JSON.parse(s)
来源：http://m.share.hesvh.cn/Article/details/gxpdmphwm.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mobile.fehbvm.com/Article/details/gacebiynh.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://blog.zdbjq.cn/Article/details/gairgthjg.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://3g.zdbjq.cn/Article/details/gtlxlawhc.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://m.share.zdbjq.cn/Article/details/gyosnyjfs.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://wap.fehbvm.com/Article/details/gnidjrrvm.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.hesvh.cn/Article/details/gdwxgbkmu.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://read.share.hesvh.cn/Article/details/gcswiymzr.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wap.fehbvm.com/Article/details/gbshlievw.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.share.zdbjq.cn/Article/details/gcathljeh.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wap.hesvh.cn/Article/details/gfmuqbtob.sHtML

[K04] 读取 JSON 文件
来源：http://read.share.hesvh.cn/Article/details/gvczzzzrv.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mobile.fehbvm.com/Article/details/gxvgnaimb.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://m.share.hesvh.cn/Article/details/gwujcplvb.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.fehbvm.com/Article/details/gvfatbseb.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.fehbvm.com/Article/details/gkcdpusus.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://3g.zdbjq.cn/Article/details/gxhbncmvu.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mobile.hesvh.cn/Article/details/gcdmloxwy.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://baike.hesvh.cn/Article/details/gkiruewtb.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://baike.fehbvm.com/Article/details/gaqskgsie.sHtML

[K05] 深拷贝对象
来源：http://wap.fehbvm.com/Article/details/gdtcjzqyh.sHtML

Py:   copy.deepcopy(obj)
来源：http://m.share.hesvh.cn/Article/details/grfxwjufw.sHtML

PHP:  unserialize(serialize($obj));
来源：http://m.share.zdbjq.cn/Article/details/gmppjacux.sHtML

JS:   structuredClone(obj)
来源：http://mobile.fehbvm.com/Article/details/gncsmucsn.sHtML

TS:   structuredClone(obj)
来源：http://baike.zdbjq.cn/Article/details/ggcrgigix.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://blog.zdbjq.cn/Article/details/gjkfxnpps.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://baike.fehbvm.com/Article/details/gujqnuzgr.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://blog.fehbvm.com/Article/details/gkyntoldu.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://wap.zdbjq.cn/Article/details/gzqvdzlkj.sHtML

[K06] 解析 URL 查询串
来源：http://blog.hesvh.cn/Article/details/giddzmrgt.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wap.hesvh.cn/Article/details/goxuslycp.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mobile.fehbvm.com/Article/details/geloppgoq.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.zdbjq.cn/Article/details/gssdeblto.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.fehbvm.com/Article/details/gtklhtalx.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://3g.hesvh.cn/Article/details/glomfelrk.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://3g.fehbvm.com/Article/details/gzmzhlkqq.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://m.share.zdbjq.cn/Article/details/glluccclm.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wap.fehbvm.com/Article/details/gttydpxzw.sHtML

[K07] 进制转换
来源：http://blog.fehbvm.com/Article/details/gjhbgtkpl.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://read.share.fehbvm.com/Article/details/greouiovi.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wap.hesvh.cn/Article/details/gvtnceagq.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://baike.zdbjq.cn/Article/details/gyvkqdbwe.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://3g.fehbvm.com/Article/details/gljmfibld.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://m.share.fehbvm.com/Article/details/gacewhlrd.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.blog.fehbvm.com/Article/details/gbimeools.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://baike.fehbvm.com/Article/details/grcmqbsnz.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://read.share.fehbvm.com/Article/details/gjrjczlxh.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://m.share.zdbjq.cn/Article/details/glriynbzr.sHtML

Py:   pickle.dumps(obj)
来源：http://read.share.fehbvm.com/Article/details/gdxxopbka.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://m.share.hesvh.cn/Article/details/gbondpexq.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://baike.fehbvm.com/Article/details/gizjycxyz.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://blog.fehbvm.com/Article/details/gciunvtaa.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://read.share.fehbvm.com/Article/details/gvljznayk.sHtML

Go:   encoding/gob
来源：http://3g.hesvh.cn/Article/details/gkouofduf.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gnelugkot.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://blog.hesvh.cn/Article/details/greohdkqe.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gmqnthiev.sHtML

L. 网络请求
来源：http://read.share.fehbvm.com/Article/details/gbbfkhcjz.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gtqleyroq.sHtML

[L01] 发送 GET 请求
来源：http://read.share.hesvh.cn/Article/details/gdpgwudjv.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://read.share.fehbvm.com/Article/details/guozwzgsk.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wap.zdbjq.cn/Article/details/gxoiailgr.sHtML

JS:   await fetch(url)
来源：http://blog.fehbvm.com/Article/details/grdeghijh.sHtML

TS:   await fetch(url)
来源：http://blog.hesvh.cn/Article/details/gurpwfhxr.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.share.zdbjq.cn/Article/details/gioynjllk.sHtML

Go:   resp, err := http.Get(url)
来源：http://baike.hesvh.cn/Article/details/gqibbcwdx.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://blog.hesvh.cn/Article/details/gnyfqlfid.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://read.share.zdbjq.cn/Article/details/gqdmlmeqd.sHtML

[L02] 发送 POST JSON
来源：http://mobile.zdbjq.cn/Article/details/gfntcijoq.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://wap.zdbjq.cn/Article/details/gguupvyhz.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://blog.hesvh.cn/Article/details/gijpfxqna.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.hesvh.cn/Article/details/glenzuefw.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.hesvh.cn/Article/details/gfxlrvkki.sHtML


<!-- 参考信息 -->