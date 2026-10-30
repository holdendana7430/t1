代发 wailian999

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.share.zdbjq.cn/Article/details/gusbquwff.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://blog.zdbjq.cn/Article/details/gaosxckqp.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://m.share.fehbvm.com/Article/details/gnryqnewg.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://m.share.hesvh.cn/Article/details/gyfogdukl.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.share.fehbvm.com/Article/details/gkxdstcuc.sHtML

Ruby: rescue ArgumentError => e
来源：http://mobile.hesvh.cn/Article/details/gfpfipqhd.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.m.share.zdbjq.cn/Article/details/guuwquwyd.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.share.fehbvm.com/Article/details/gpsmzpnlc.sHtML

Py:   value = d.get("k") or default
来源：http://m.share.hesvh.cn/Article/details/gkgnwwcbc.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.m.share.fehbvm.com/Article/details/ginnjhysp.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://wap.hesvh.cn/Article/details/gthzzismy.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://baike.hesvh.cn/Article/details/gipfuphaq.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.m.share.zdbjq.cn/Article/details/gpebaxwie.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://blog.hesvh.cn/Article/details/gjaeftxno.sHtML

Ruby: d&.dig(:a, :b)
来源：http://mobile.fehbvm.com/Article/details/gjrkhdxts.sHtML

C#:   obj?.A?.B ?? default
来源：http://m.share.hesvh.cn/Article/details/gjohkcsdo.sHtML

[H07] 断言
来源：http://3g.zdbjq.cn/Article/details/gyjorkcdt.sHtML

Py:   assert x > 0, "必须为正"
来源：http://read.share.zdbjq.cn/Article/details/grgkdsvdy.sHtML

PHP:  assert($x > 0);
来源：http://read.share.hesvh.cn/Article/details/gprldcchh.sHtML

JS:   console.assert(x > 0);
来源：http://www.m.share.hesvh.cn/Article/details/ghcsyteis.sHtML

TS:   console.assert(x > 0);
来源：http://read.share.fehbvm.com/Article/details/gdwvnxljt.sHtML

Java: assert x > 0 : "必须为正";
来源：http://blog.hesvh.cn/Article/details/gdcmmdukk.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wap.zdbjq.cn/Article/details/gjgtwvfhn.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://m.share.zdbjq.cn/Article/details/gnsguwosh.sHtML

C#:   Debug.Assert(x > 0);
来源：http://baike.hesvh.cn/Article/details/gtnrzuaki.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.share.hesvh.cn/Article/details/gsduihksf.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://3g.fehbvm.com/Article/details/gbcfaiutu.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.share.zdbjq.cn/Article/details/gqyklbfqo.sHtML

JS:   e.message;  e.stack
来源：http://www.m.share.fehbvm.com/Article/details/gxqwttuay.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://3g.fehbvm.com/Article/details/gwunyfpjw.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://read.share.hesvh.cn/Article/details/gefcupcnw.sHtML

Go:   err.Error()
来源：http://m.share.fehbvm.com/Article/details/gokjtwdoh.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.share.hesvh.cn/Article/details/gqdqzqiai.sHtML

C#:   e.Message;  e.StackTrace
来源：http://baike.zdbjq.cn/Article/details/gpdxryjdi.sHtML

[H09] 带错误码的异常
来源：http://www.m.share.hesvh.cn/Article/details/ggdehiqbr.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://baike.hesvh.cn/Article/details/gakephbww.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://blog.fehbvm.com/Article/details/gmwsyjwyg.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://3g.zdbjq.cn/Article/details/gkcmwzjhu.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://baike.hesvh.cn/Article/details/grssmtqsv.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mobile.hesvh.cn/Article/details/gfdtywszw.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://3g.hesvh.cn/Article/details/gzpcsaqsl.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://3g.fehbvm.com/Article/details/gdquplxuq.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.m.share.zdbjq.cn/Article/details/gjczbaamo.sHtML

[H10] 资源自动释放
来源：http://m.share.fehbvm.com/Article/details/gsmubuine.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.m.share.hesvh.cn/Article/details/ghispjsmm.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://3g.hesvh.cn/Article/details/gbpqythik.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.hesvh.cn/Article/details/ghwoafafa.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.fehbvm.com/Article/details/gxngzsyps.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wap.hesvh.cn/Article/details/gdswnhiwa.sHtML

Go:   defer f.Close()
来源：http://read.share.fehbvm.com/Article/details/gyqdxyqra.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.m.share.fehbvm.com/Article/details/gfrfjhivt.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gkasodsqa.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gftfhuckb.sHtML

I. 正则表达式
来源：http://read.share.hesvh.cn/Article/details/ggxvhtmim.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gpyxzkrzg.sHtML

[I01] 判断是否匹配
来源：http://www.m.share.fehbvm.com/Article/details/gwoxeevkd.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://3g.hesvh.cn/Article/details/gyusyuggl.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://read.share.hesvh.cn/Article/details/ggensbwai.sHtML

JS:   /\d+/.test(s)
来源：http://baike.fehbvm.com/Article/details/gadveydyd.sHtML

TS:   /\d+/.test(s)
来源：http://3g.fehbvm.com/Article/details/gwxrmhifa.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wap.hesvh.cn/Article/details/gxhswvknd.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://read.share.fehbvm.com/Article/details/gtabafjns.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.m.share.fehbvm.com/Article/details/gxqqwknxi.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://blog.fehbvm.com/Article/details/gpvqlivku.sHtML

[I02] 提取所有匹配
来源：http://m.share.fehbvm.com/Article/details/gqomhjyhk.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.share.fehbvm.com/Article/details/glcxrbnaa.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.share.zdbjq.cn/Article/details/gbnxtzqiq.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://blog.zdbjq.cn/Article/details/gdfgzyxvj.sHtML

TS:   s.match(/\d+/g)
来源：http://blog.hesvh.cn/Article/details/gqlbgwbed.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://blog.hesvh.cn/Article/details/gqsfspmsr.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mobile.hesvh.cn/Article/details/gahtxgayr.sHtML

Ruby: s.scan(/\d+/)
来源：http://read.share.hesvh.cn/Article/details/grsxtktkq.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gzrodjiao.sHtML

[I03] 提取捕获分组
来源：http://www.blog.hesvh.cn/Article/details/gxmfsptme.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wap.fehbvm.com/Article/details/gmfqwkfvo.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://baike.fehbvm.com/Article/details/gezdpyycg.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wap.zdbjq.cn/Article/details/ghbsroxtz.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.share.fehbvm.com/Article/details/gafyonoek.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.m.share.zdbjq.cn/Article/details/gklrcqhwd.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.m.share.hesvh.cn/Article/details/grsftdrpa.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.blog.zdbjq.cn/Article/details/gfzfqyocg.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://read.share.hesvh.cn/Article/details/gbrzccwxc.sHtML

[I04] 正则替换
来源：http://www.share.fehbvm.com/Article/details/ggseacqgw.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://mobile.zdbjq.cn/Article/details/grmhkgwjn.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gfswfbgsx.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://baike.zdbjq.cn/Article/details/gsqjzsxwo.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://mobile.fehbvm.com/Article/details/gxsisweby.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://wap.zdbjq.cn/Article/details/gxvzmeatm.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://baike.zdbjq.cn/Article/details/gcsbhceyr.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://read.share.fehbvm.com/Article/details/gmmlfhgjo.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.blog.fehbvm.com/Article/details/ghuppimxu.sHtML

[I05] 按正则拆分
来源：http://m.share.zdbjq.cn/Article/details/ghpeuffla.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://baike.fehbvm.com/Article/details/gzhhsisdv.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://3g.hesvh.cn/Article/details/gsgvxzqgy.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.share.hesvh.cn/Article/details/gncntjxav.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://m.share.fehbvm.com/Article/details/gwzideyez.sHtML

Java: s.split("\\s*,\\s*")
来源：http://blog.zdbjq.cn/Article/details/gdueknfyw.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://baike.zdbjq.cn/Article/details/gzgbdfviy.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://wap.hesvh.cn/Article/details/gejklrgjc.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://read.share.fehbvm.com/Article/details/gkmfeschn.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://m.share.hesvh.cn/Article/details/gjkpybwem.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://m.share.hesvh.cn/Article/details/gxrttwnqk.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://mobile.hesvh.cn/Article/details/gzcsyecwg.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.hesvh.cn/Article/details/gpephzmim.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.zdbjq.cn/Article/details/gukdjbwvs.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.share.fehbvm.com/Article/details/gqilaykrj.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.m.share.zdbjq.cn/Article/details/gkczjvodj.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.share.fehbvm.com/Article/details/gchxblldp.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.share.fehbvm.com/Article/details/ghdhyqxim.sHtML

[I07] 忽略大小写与多行模式
来源：http://m.share.fehbvm.com/Article/details/gjhfdnlkg.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://m.share.fehbvm.com/Article/details/gqrwutacm.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mobile.hesvh.cn/Article/details/gjjcrkxey.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.blog.fehbvm.com/Article/details/gnmcxhrbw.sHtML

TS:   /error/gim
来源：http://mobile.fehbvm.com/Article/details/gfrnlfebe.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.blog.fehbvm.com/Article/details/glupfsgbq.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://read.share.hesvh.cn/Article/details/gmcpjnruk.sHtML

Ruby: s.scan(/error/i)
来源：http://m.share.zdbjq.cn/Article/details/gbbfkcaor.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.m.share.fehbvm.com/Article/details/guipohlne.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.share.hesvh.cn/Article/details/gckdrwqzm.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://3g.fehbvm.com/Article/details/gztbzhzys.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://read.share.zdbjq.cn/Article/details/gkyldjtbv.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.zdbjq.cn/Article/details/ghvlksjel.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.fehbvm.com/Article/details/gubdwzwnv.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.blog.zdbjq.cn/Article/details/guvevukhj.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://m.share.zdbjq.cn/Article/details/gcrpzsxui.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.share.hesvh.cn/Article/details/gjkvcgadm.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://read.share.hesvh.cn/Article/details/ggjuiuitm.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/ghaymgulm.sHtML

J. 日期与时间
来源：http://mobile.fehbvm.com/Article/details/gtcftbjig.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gzegbbemi.sHtML

[J01] 获取当前时间
来源：http://read.share.hesvh.cn/Article/details/gvwfrpkvb.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.m.share.hesvh.cn/Article/details/gujzjcpfc.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.blog.hesvh.cn/Article/details/gsdgmjjtj.sHtML

JS:   new Date();  Date.now()
来源：http://3g.zdbjq.cn/Article/details/gnvheekqo.sHtML

TS:   new Date();  Date.now()
来源：http://mobile.zdbjq.cn/Article/details/gnudobqrm.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://blog.fehbvm.com/Article/details/guqrboduu.sHtML

Go:   time.Now()
来源：http://m.share.hesvh.cn/Article/details/gmzdxqzru.sHtML

Ruby: Time.now
来源：http://3g.zdbjq.cn/Article/details/gtcrwdnle.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://3g.zdbjq.cn/Article/details/gtgqnwcoi.sHtML

[J02] 格式化输出
来源：http://wap.zdbjq.cn/Article/details/gouygmpov.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.hesvh.cn/Article/details/gsoubebkm.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://baike.fehbvm.com/Article/details/gjfjzcjrg.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.m.share.hesvh.cn/Article/details/gqqqrnopj.sHtML

TS:   d.toISOString()
来源：http://blog.fehbvm.com/Article/details/gytkkutba.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://wap.fehbvm.com/Article/details/gvluvmhkz.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.blog.zdbjq.cn/Article/details/gycovnbia.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.hesvh.cn/Article/details/gojchnfsp.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://mobile.zdbjq.cn/Article/details/gzyvrqwgk.sHtML

[J03] 字符串解析为日期
来源：http://3g.fehbvm.com/Article/details/gemqkgjzs.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://read.share.zdbjq.cn/Article/details/gmoynneaf.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://blog.fehbvm.com/Article/details/gnxjtoomb.sHtML

JS:   new Date("2024-01-02")
来源：http://baike.hesvh.cn/Article/details/gqbcekzdj.sHtML

TS:   new Date("2024-01-02")
来源：http://www.m.share.hesvh.cn/Article/details/gvgfxuaob.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.share.zdbjq.cn/Article/details/gfdlhexvc.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://blog.hesvh.cn/Article/details/gkbpgnekz.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://read.share.zdbjq.cn/Article/details/gxdtgjzza.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://m.share.fehbvm.com/Article/details/gkhcsyctl.sHtML

[J04] 时间戳与日期互转
来源：http://wap.hesvh.cn/Article/details/gitpihrik.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wap.hesvh.cn/Article/details/gmtmkqvde.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.share.hesvh.cn/Article/details/gemerdobo.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mobile.hesvh.cn/Article/details/gdwdveazi.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://baike.hesvh.cn/Article/details/gmtsooqkj.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.share.hesvh.cn/Article/details/gmubbobfd.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.blog.fehbvm.com/Article/details/gzokpixga.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wap.fehbvm.com/Article/details/gcpkcdgpc.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.m.share.hesvh.cn/Article/details/gxjpcfbyg.sHtML

[J05] 时间加减（加 7 天）
来源：http://m.share.zdbjq.cn/Article/details/gtfhhhosr.sHtML

Py:   now + timedelta(days=7)
来源：http://blog.hesvh.cn/Article/details/glxliwlxv.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.m.share.hesvh.cn/Article/details/gcjsvrzld.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.fehbvm.com/Article/details/gcsckuwfz.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.fehbvm.com/Article/details/gfbirlxqy.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://read.share.zdbjq.cn/Article/details/gdmnkauja.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://3g.fehbvm.com/Article/details/gsxzmwerm.sHtML

Ruby: Time.now + 7 * 86400
来源：http://3g.fehbvm.com/Article/details/gdumfegyv.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://mobile.hesvh.cn/Article/details/gmymbisxs.sHtML

[J06] 计算两时间之差
来源：http://m.share.fehbvm.com/Article/details/ggqwaaarx.sHtML

Py:   (end - start).total_seconds()
来源：http://www.share.fehbvm.com/Article/details/ghuldyatv.sHtML

PHP:  $end->diff($start)->days;
来源：http://3g.zdbjq.cn/Article/details/gcqgoxbxw.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wap.zdbjq.cn/Article/details/gdovzdplj.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.m.share.zdbjq.cn/Article/details/gexldjamg.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://3g.zdbjq.cn/Article/details/gcsbmwslu.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.blog.hesvh.cn/Article/details/gzjqqficq.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.share.fehbvm.com/Article/details/gwfeqomgr.sHtML

C#:   (end - start).TotalSeconds
来源：http://read.share.hesvh.cn/Article/details/gzehfkcci.sHtML

[J07] 比较两个日期
来源：http://mobile.zdbjq.cn/Article/details/guekikksw.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://mobile.fehbvm.com/Article/details/gtujdgrnh.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://m.share.zdbjq.cn/Article/details/gwbsvyxwv.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://baike.fehbvm.com/Article/details/gklbavocc.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://baike.fehbvm.com/Article/details/gcckiwxtz.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wap.zdbjq.cn/Article/details/gojupuxqe.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.share.zdbjq.cn/Article/details/gztyuyqah.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.blog.fehbvm.com/Article/details/gnnatcsje.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.m.share.hesvh.cn/Article/details/grrgeeivb.sHtML

[J08] 提取年月日与星期
来源：http://baike.zdbjq.cn/Article/details/gzowgkyss.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://3g.fehbvm.com/Article/details/gdeptowpu.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://3g.fehbvm.com/Article/details/gywfkjyej.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://baike.hesvh.cn/Article/details/gkxdmwbxe.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.m.share.hesvh.cn/Article/details/gmodboovz.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mobile.hesvh.cn/Article/details/gonqmwwcw.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.share.zdbjq.cn/Article/details/gssujqflf.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://blog.fehbvm.com/Article/details/gmeagjozz.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://m.share.fehbvm.com/Article/details/gedcgwyam.sHtML

[J09] 时区处理
来源：http://www.m.share.hesvh.cn/Article/details/gydyyqbyz.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.m.share.zdbjq.cn/Article/details/gvbbexxsm.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://baike.hesvh.cn/Article/details/gqaztemke.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.hesvh.cn/Article/details/ghjgkrawb.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.zdbjq.cn/Article/details/gemgcyqwj.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wap.hesvh.cn/Article/details/gkmgrlqvi.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://3g.hesvh.cn/Article/details/gtzeecpxn.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://baike.fehbvm.com/Article/details/guqgqghkj.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://m.share.fehbvm.com/Article/details/gdwukyiao.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.share.hesvh.cn/Article/details/gfgahwugs.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://baike.fehbvm.com/Article/details/gnzpofjtb.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://m.share.hesvh.cn/Article/details/gjzdtgfkt.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://m.share.fehbvm.com/Article/details/gkbeopisi.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://m.share.hesvh.cn/Article/details/gecxqnifg.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.blog.zdbjq.cn/Article/details/gxexruoto.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://read.share.fehbvm.com/Article/details/gwhapnxrc.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://baike.fehbvm.com/Article/details/gczlclrnr.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://blog.fehbvm.com/Article/details/geiubwxgv.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gdkdrrsqk.sHtML

K. JSON 与序列化
来源：http://blog.hesvh.cn/Article/details/guxujemop.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gorvzdiry.sHtML

[K01] 对象转 JSON 字符串
来源：http://m.share.fehbvm.com/Article/details/girffsvtl.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.share.fehbvm.com/Article/details/glokurttq.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://m.share.fehbvm.com/Article/details/gagheplqg.sHtML

JS:   JSON.stringify(obj)
来源：http://3g.zdbjq.cn/Article/details/gonsrrfex.sHtML

TS:   JSON.stringify(obj)
来源：http://www.share.zdbjq.cn/Article/details/gsljdfcpp.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mobile.fehbvm.com/Article/details/gikvvhweh.sHtML

Go:   json.Marshal(obj)
来源：http://read.share.fehbvm.com/Article/details/gxxgvdkva.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://read.share.fehbvm.com/Article/details/gxjpbxytp.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://3g.zdbjq.cn/Article/details/gchimszpx.sHtML

[K02] JSON 字符串转对象
来源：http://wap.zdbjq.cn/Article/details/gufktrevx.sHtML

Py:   json.loads(s)
来源：http://wap.fehbvm.com/Article/details/gsfdwjwdn.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://baike.hesvh.cn/Article/details/groiowuvv.sHtML

JS:   JSON.parse(s)
来源：http://www.blog.fehbvm.com/Article/details/gmbvimncg.sHtML

TS:   JSON.parse(s)
来源：http://read.share.hesvh.cn/Article/details/gjjbufotv.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.blog.fehbvm.com/Article/details/gayrgxuff.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://m.share.fehbvm.com/Article/details/gnekpebpb.sHtML

Ruby: JSON.parse(s)
来源：http://wap.fehbvm.com/Article/details/giydinmss.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wap.fehbvm.com/Article/details/gdchbluei.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://3g.fehbvm.com/Article/details/gjkwweqql.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://3g.hesvh.cn/Article/details/gedkzyvwj.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://blog.zdbjq.cn/Article/details/gnhfnuely.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.hesvh.cn/Article/details/gsuzuhmlt.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://m.share.hesvh.cn/Article/details/gyjbbjkva.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://3g.hesvh.cn/Article/details/gtwdakqzz.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://read.share.fehbvm.com/Article/details/gjcyqddjp.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://baike.hesvh.cn/Article/details/gdxdukrgn.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://blog.fehbvm.com/Article/details/gpwaowshq.sHtML

[K04] 读取 JSON 文件
来源：http://wap.hesvh.cn/Article/details/gcgcuohyp.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.blog.hesvh.cn/Article/details/grmzlwkgs.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://baike.zdbjq.cn/Article/details/gggybxcon.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.fehbvm.com/Article/details/gtmpvbfhy.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.fehbvm.com/Article/details/gyfbhnvzs.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://read.share.zdbjq.cn/Article/details/guftvvile.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://blog.hesvh.cn/Article/details/gjrzkwknj.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://read.share.fehbvm.com/Article/details/gdxybuasf.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://read.share.hesvh.cn/Article/details/grefzwzrv.sHtML

[K05] 深拷贝对象
来源：http://mobile.fehbvm.com/Article/details/gbciqucxw.sHtML

Py:   copy.deepcopy(obj)
来源：http://3g.fehbvm.com/Article/details/gcquxurwz.sHtML

PHP:  unserialize(serialize($obj));
来源：http://read.share.fehbvm.com/Article/details/giwjzlkww.sHtML

JS:   structuredClone(obj)
来源：http://read.share.zdbjq.cn/Article/details/gnnicyimx.sHtML

TS:   structuredClone(obj)
来源：http://wap.zdbjq.cn/Article/details/gajeobkht.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.share.fehbvm.com/Article/details/guluhsbgf.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://blog.zdbjq.cn/Article/details/gmosimuef.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mobile.fehbvm.com/Article/details/gnkywglur.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://blog.zdbjq.cn/Article/details/goctfnyed.sHtML

[K06] 解析 URL 查询串
来源：http://www.blog.hesvh.cn/Article/details/gbefggfmg.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wap.hesvh.cn/Article/details/gywcbcybr.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wap.zdbjq.cn/Article/details/gwnczkwic.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.zdbjq.cn/Article/details/guzpqgjcl.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.hesvh.cn/Article/details/gpbsgatvf.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://blog.zdbjq.cn/Article/details/gqcrhcria.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.m.share.hesvh.cn/Article/details/gqozkbwtz.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://baike.zdbjq.cn/Article/details/gjhfcgxut.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://baike.fehbvm.com/Article/details/gatvwbzdo.sHtML

[K07] 进制转换
来源：http://www.share.zdbjq.cn/Article/details/gkdnwxdee.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.blog.hesvh.cn/Article/details/gvmxjopng.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://blog.hesvh.cn/Article/details/gngnqmltu.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.m.share.hesvh.cn/Article/details/ggiipmiwy.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://m.share.zdbjq.cn/Article/details/grqhxxhrf.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://read.share.hesvh.cn/Article/details/gdwwadlvj.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://m.share.zdbjq.cn/Article/details/gdmtguwpf.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wap.zdbjq.cn/Article/details/grxsvnsbm.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.share.zdbjq.cn/Article/details/ghcqijvrp.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://baike.fehbvm.com/Article/details/gxvyoahxq.sHtML

Py:   pickle.dumps(obj)
来源：http://blog.fehbvm.com/Article/details/gjjhxcffu.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.blog.fehbvm.com/Article/details/gojkkstco.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://3g.hesvh.cn/Article/details/gigbrfxbv.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://wap.fehbvm.com/Article/details/glptcalyf.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.blog.fehbvm.com/Article/details/gncpkmvqh.sHtML

Go:   encoding/gob
来源：http://www.blog.hesvh.cn/Article/details/gxxlxjmbe.sHtML

Ruby: Marshal.dump(obj)
来源：http://mobile.fehbvm.com/Article/details/gaoydesst.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://m.share.fehbvm.com/Article/details/ghzlfivcu.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gvnnlwehs.sHtML

L. 网络请求
来源：http://baike.fehbvm.com/Article/details/gbcsockfg.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gnghhvjrh.sHtML

[L01] 发送 GET 请求
来源：http://www.blog.fehbvm.com/Article/details/gpwcyfzkd.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://read.share.zdbjq.cn/Article/details/gepokxtih.sHtML


<!-- 参考信息 -->