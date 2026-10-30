代发 wailian999

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnosvoyjw.sHtML

Ruby: rescue ArgumentError => e
来源：http://read.share.fanxiaobao.xyz/Article/details/guntxdeii.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjedpewam.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.m.share.fanxiaobao.xyz/Article/details/godevnqxr.sHtML

Py:   value = d.get("k") or default
来源：http://read.share.fanxiaobao.xyz/Article/details/gtduoomba.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnytnhhcf.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://read.share.fanxiaobao.xyz/Article/details/gaartdyku.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://3g.fanxiaobao.xyz/Article/details/glgcxfgvb.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwpilvryt.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://blog.fanxiaobao.xyz/Article/details/ggdnsqcin.sHtML

Ruby: d&.dig(:a, :b)
来源：http://m.share.fanxiaobao.xyz/Article/details/gkvvpaoxl.sHtML

C#:   obj?.A?.B ?? default
来源：http://m.share.fanxiaobao.xyz/Article/details/gyelvwqvh.sHtML

[H07] 断言
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnflvbiih.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkcdekwmi.sHtML

PHP:  assert($x > 0);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdmvvjmbz.sHtML

JS:   console.assert(x > 0);
来源：http://m.share.fanxiaobao.xyz/Article/details/grnereuaj.sHtML

TS:   console.assert(x > 0);
来源：http://blog.fanxiaobao.xyz/Article/details/gkuniexis.sHtML

Java: assert x > 0 : "必须为正";
来源：http://read.share.fanxiaobao.xyz/Article/details/gorexucrn.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://blog.fanxiaobao.xyz/Article/details/gridtbpds.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtxcchyfs.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.share.fanxiaobao.xyz/Article/details/gsgwnzsjb.sHtML

[H08] 获取错误信息与堆栈
来源：http://read.share.fanxiaobao.xyz/Article/details/goajkjqpm.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://read.share.fanxiaobao.xyz/Article/details/gkwusfzxw.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://baike.fanxiaobao.xyz/Article/details/gtbimhoxt.sHtML

JS:   e.message;  e.stack
来源：http://wap.fanxiaobao.xyz/Article/details/gusibkkzt.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://baike.fanxiaobao.xyz/Article/details/gommtlerf.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://read.share.fanxiaobao.xyz/Article/details/gzivnshwv.sHtML

Go:   err.Error()
来源：http://3g.fanxiaobao.xyz/Article/details/gqevollaa.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.blog.fanxiaobao.xyz/Article/details/geztpvhtk.sHtML

C#:   e.Message;  e.StackTrace
来源：http://read.share.fanxiaobao.xyz/Article/details/gxoemmnpk.sHtML

[H09] 带错误码的异常
来源：http://wap.fanxiaobao.xyz/Article/details/gctcuqbdz.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://read.share.fanxiaobao.xyz/Article/details/gvyljbyop.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://read.share.fanxiaobao.xyz/Article/details/gyllqvodl.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wap.fanxiaobao.xyz/Article/details/gqohjxrgf.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.share.fanxiaobao.xyz/Article/details/ggilofoho.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtebtjnwk.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wap.fanxiaobao.xyz/Article/details/gisjjprox.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzdoxfooh.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://read.share.fanxiaobao.xyz/Article/details/gpvydsjpj.sHtML

[H10] 资源自动释放
来源：http://m.share.fanxiaobao.xyz/Article/details/gqdocpdog.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://read.share.fanxiaobao.xyz/Article/details/goerkyumo.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gybubrbnt.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcppbrvxa.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glswefggt.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://m.share.fanxiaobao.xyz/Article/details/gckrzybla.sHtML

Go:   defer f.Close()
来源：http://www.blog.fanxiaobao.xyz/Article/details/glqinqzyh.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wap.fanxiaobao.xyz/Article/details/gjhdxgfkm.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://read.share.fanxiaobao.xyz/Article/details/gpjnresyf.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gskpradia.sHtML

I. 正则表达式
来源：http://3g.fanxiaobao.xyz/Article/details/gezvqrwam.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gweojmtnq.sHtML

[I01] 判断是否匹配
来源：http://blog.fanxiaobao.xyz/Article/details/ggqmiqfpa.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://baike.fanxiaobao.xyz/Article/details/gffdjbzhe.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://read.share.fanxiaobao.xyz/Article/details/giwiysfsi.sHtML

JS:   /\d+/.test(s)
来源：http://blog.fanxiaobao.xyz/Article/details/gxeascbxr.sHtML

TS:   /\d+/.test(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gweoiczkc.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mobile.fanxiaobao.xyz/Article/details/gfwziqiys.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gpcepwwes.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.share.fanxiaobao.xyz/Article/details/ghbtmvgoc.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mobile.fanxiaobao.xyz/Article/details/grjkdiynk.sHtML

[I02] 提取所有匹配
来源：http://3g.fanxiaobao.xyz/Article/details/gcrgmmmux.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gprajiimq.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://baike.fanxiaobao.xyz/Article/details/gypplamwl.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wap.fanxiaobao.xyz/Article/details/gdlgxjnmq.sHtML

TS:   s.match(/\d+/g)
来源：http://www.share.fanxiaobao.xyz/Article/details/gyrpyufpt.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.share.fanxiaobao.xyz/Article/details/gglovjsvt.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gkehnonjh.sHtML

Ruby: s.scan(/\d+/)
来源：http://mobile.fanxiaobao.xyz/Article/details/gnxwywpjj.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guocpfbtb.sHtML

[I03] 提取捕获分组
来源：http://www.blog.fanxiaobao.xyz/Article/details/gahkentql.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtushvaaf.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://read.share.fanxiaobao.xyz/Article/details/gffefzuic.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://baike.fanxiaobao.xyz/Article/details/gdyavxovq.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.blog.fanxiaobao.xyz/Article/details/glvybpdbt.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://mobile.fanxiaobao.xyz/Article/details/gstajvazu.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.share.fanxiaobao.xyz/Article/details/gutvxqrum.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wap.fanxiaobao.xyz/Article/details/gqtnvppsz.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wap.fanxiaobao.xyz/Article/details/gxwmotczw.sHtML

[I04] 正则替换
来源：http://wap.fanxiaobao.xyz/Article/details/gcxqrqdeg.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://baike.fanxiaobao.xyz/Article/details/gydaajhdg.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwlzksdmx.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxbpnolsx.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://mobile.fanxiaobao.xyz/Article/details/guhvxvuim.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://blog.fanxiaobao.xyz/Article/details/gvgrgezot.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gepkybvmc.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjfiwitnd.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://3g.fanxiaobao.xyz/Article/details/gsbmprwlu.sHtML

[I05] 按正则拆分
来源：http://3g.fanxiaobao.xyz/Article/details/gvqijzzzi.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://blog.fanxiaobao.xyz/Article/details/gqgzkkymw.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://blog.fanxiaobao.xyz/Article/details/glidvodwo.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.share.fanxiaobao.xyz/Article/details/guhfdamwb.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://wap.fanxiaobao.xyz/Article/details/gdbjkdopp.sHtML

Java: s.split("\\s*,\\s*")
来源：http://mobile.fanxiaobao.xyz/Article/details/gncxomtfx.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wap.fanxiaobao.xyz/Article/details/gohflbugo.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://wap.fanxiaobao.xyz/Article/details/gjuabosdc.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://read.share.fanxiaobao.xyz/Article/details/gnmyucjgu.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://m.share.fanxiaobao.xyz/Article/details/guxfxsple.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://blog.fanxiaobao.xyz/Article/details/gnwfztngl.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://blog.fanxiaobao.xyz/Article/details/gjawmqiqm.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmimcydvr.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.fanxiaobao.xyz/Article/details/gyeqwekbo.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://3g.fanxiaobao.xyz/Article/details/ggbdigodm.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcwsjwhgg.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wap.fanxiaobao.xyz/Article/details/grczzvyff.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://blog.fanxiaobao.xyz/Article/details/gstmvqakk.sHtML

[I07] 忽略大小写与多行模式
来源：http://m.share.fanxiaobao.xyz/Article/details/gherfvvjf.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.share.fanxiaobao.xyz/Article/details/gllvcqivf.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://baike.fanxiaobao.xyz/Article/details/gocasnmre.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://blog.fanxiaobao.xyz/Article/details/gknuoturl.sHtML

TS:   /error/gim
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmiffpvng.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mobile.fanxiaobao.xyz/Article/details/gweiqxtuw.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://blog.fanxiaobao.xyz/Article/details/gksicbgkw.sHtML

Ruby: s.scan(/error/i)
来源：http://www.share.fanxiaobao.xyz/Article/details/gkbdygjhi.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://blog.fanxiaobao.xyz/Article/details/gjldiupdb.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfngcmnsw.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://baike.fanxiaobao.xyz/Article/details/gwqynnykd.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://read.share.fanxiaobao.xyz/Article/details/gfxzqfxqs.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.fanxiaobao.xyz/Article/details/gbrhgvpvg.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.fanxiaobao.xyz/Article/details/gwfyvweoe.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://3g.fanxiaobao.xyz/Article/details/gkjxjxpcq.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wap.fanxiaobao.xyz/Article/details/ghdcuortz.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://m.share.fanxiaobao.xyz/Article/details/gflxozmck.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://blog.fanxiaobao.xyz/Article/details/gnnhbxxzv.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gduhvroxi.sHtML

J. 日期与时间
来源：http://blog.fanxiaobao.xyz/Article/details/gswtpxevu.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gtgmjlrga.sHtML

[J01] 获取当前时间
来源：http://3g.fanxiaobao.xyz/Article/details/gxucrddhu.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://3g.fanxiaobao.xyz/Article/details/glvrwyusg.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://blog.fanxiaobao.xyz/Article/details/gbxyqaslm.sHtML

JS:   new Date();  Date.now()
来源：http://m.share.fanxiaobao.xyz/Article/details/gridlhflu.sHtML

TS:   new Date();  Date.now()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjnpzcxpn.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://read.share.fanxiaobao.xyz/Article/details/gpnugkcod.sHtML

Go:   time.Now()
来源：http://3g.fanxiaobao.xyz/Article/details/gypsklwnz.sHtML

Ruby: Time.now
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gclnhgety.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdvutycvk.sHtML

[J02] 格式化输出
来源：http://3g.fanxiaobao.xyz/Article/details/gzxklfwzr.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.fanxiaobao.xyz/Article/details/gqvrwuudk.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvqokrdrw.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://blog.fanxiaobao.xyz/Article/details/gsfwmlyri.sHtML

TS:   d.toISOString()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqezkbmnb.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://baike.fanxiaobao.xyz/Article/details/gwoncgwuu.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsdergbpd.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.fanxiaobao.xyz/Article/details/gphfeytri.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.share.fanxiaobao.xyz/Article/details/gwzbrtdif.sHtML

[J03] 字符串解析为日期
来源：http://3g.fanxiaobao.xyz/Article/details/ggwmjtacp.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzhvvlhts.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://blog.fanxiaobao.xyz/Article/details/gpomgeowr.sHtML

JS:   new Date("2024-01-02")
来源：http://3g.fanxiaobao.xyz/Article/details/gejricqfq.sHtML

TS:   new Date("2024-01-02")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwbycdowg.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://blog.fanxiaobao.xyz/Article/details/gkzpuhnqg.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wap.fanxiaobao.xyz/Article/details/gzrbmqgyx.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://blog.fanxiaobao.xyz/Article/details/gvoxjzjgv.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://3g.fanxiaobao.xyz/Article/details/ggshrufiq.sHtML

[J04] 时间戳与日期互转
来源：http://3g.fanxiaobao.xyz/Article/details/gzgmaucmx.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://blog.fanxiaobao.xyz/Article/details/gnquutefg.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gropsanbu.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://3g.fanxiaobao.xyz/Article/details/gfvrtgugc.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://blog.fanxiaobao.xyz/Article/details/grasxsihs.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://wap.fanxiaobao.xyz/Article/details/gmydkrzhc.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://read.share.fanxiaobao.xyz/Article/details/gxaovylvm.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://m.share.fanxiaobao.xyz/Article/details/gdmqqzblp.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://mobile.fanxiaobao.xyz/Article/details/ggnsmzexq.sHtML

[J05] 时间加减（加 7 天）
来源：http://blog.fanxiaobao.xyz/Article/details/girxfynxd.sHtML

Py:   now + timedelta(days=7)
来源：http://blog.fanxiaobao.xyz/Article/details/gcjgtilmn.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqihurajv.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.fanxiaobao.xyz/Article/details/gpphjlhdz.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.fanxiaobao.xyz/Article/details/gcjwjkqiw.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://baike.fanxiaobao.xyz/Article/details/gvtdzfoep.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://3g.fanxiaobao.xyz/Article/details/gvyvztmrj.sHtML

Ruby: Time.now + 7 * 86400
来源：http://mobile.fanxiaobao.xyz/Article/details/gijdoutmy.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://baike.fanxiaobao.xyz/Article/details/ghzlohqnc.sHtML

[J06] 计算两时间之差
来源：http://www.share.fanxiaobao.xyz/Article/details/gviijwcum.sHtML

Py:   (end - start).total_seconds()
来源：http://blog.fanxiaobao.xyz/Article/details/gglhobped.sHtML

PHP:  $end->diff($start)->days;
来源：http://baike.fanxiaobao.xyz/Article/details/gndvpmrth.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://baike.fanxiaobao.xyz/Article/details/ghckcrbyv.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mobile.fanxiaobao.xyz/Article/details/geygyvulk.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://read.share.fanxiaobao.xyz/Article/details/gzpzvjajv.sHtML

Go:   end.Sub(start).Hours()
来源：http://blog.fanxiaobao.xyz/Article/details/glefgrvxy.sHtML

Ruby: end - start                 # 返回秒数
来源：http://read.share.fanxiaobao.xyz/Article/details/gbxlhnaee.sHtML

C#:   (end - start).TotalSeconds
来源：http://mobile.fanxiaobao.xyz/Article/details/gnaxfqdjl.sHtML

[J07] 比较两个日期
来源：http://wap.fanxiaobao.xyz/Article/details/gvynkorzu.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://baike.fanxiaobao.xyz/Article/details/gqciaiqov.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://mobile.fanxiaobao.xyz/Article/details/gkcoxxcxd.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://baike.fanxiaobao.xyz/Article/details/gkqrjjhez.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://3g.fanxiaobao.xyz/Article/details/gquwsujwa.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gltnnseif.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://3g.fanxiaobao.xyz/Article/details/gsfrdklhf.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.share.fanxiaobao.xyz/Article/details/gzzciyjpa.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxccrwqcb.sHtML

[J08] 提取年月日与星期
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjyxucfvp.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwuyqonkm.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://blog.fanxiaobao.xyz/Article/details/gkqwyhxjw.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://baike.fanxiaobao.xyz/Article/details/gkrtdqmkj.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mobile.fanxiaobao.xyz/Article/details/gvkmrubel.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gigzrpvvb.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://3g.fanxiaobao.xyz/Article/details/gprxxurhd.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://m.share.fanxiaobao.xyz/Article/details/grgthljin.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.share.fanxiaobao.xyz/Article/details/gxwbwvowr.sHtML

[J09] 时区处理
来源：http://www.blog.fanxiaobao.xyz/Article/details/gguigicju.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://baike.fanxiaobao.xyz/Article/details/ggzbeaixd.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsmhbnkwa.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.fanxiaobao.xyz/Article/details/graxeonjq.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.fanxiaobao.xyz/Article/details/gvapofwzs.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.share.fanxiaobao.xyz/Article/details/gzwpdbjuq.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://3g.fanxiaobao.xyz/Article/details/gsewyhalf.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.share.fanxiaobao.xyz/Article/details/gwdphgmxo.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://3g.fanxiaobao.xyz/Article/details/gobqxdxuy.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gurqwazzb.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gisgyzwnq.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://baike.fanxiaobao.xyz/Article/details/gmwwpgpyf.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpcypcqyi.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.share.fanxiaobao.xyz/Article/details/gzlzgbkpy.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://3g.fanxiaobao.xyz/Article/details/gmelzinde.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzuxsdzkd.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggaitgumk.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfepesgan.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfoggmwex.sHtML

K. JSON 与序列化
来源：http://blog.fanxiaobao.xyz/Article/details/goxhdsxea.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gelkmxvjq.sHtML

[K01] 对象转 JSON 字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gtkffacah.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://read.share.fanxiaobao.xyz/Article/details/gwfunqpwd.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://3g.fanxiaobao.xyz/Article/details/gqccktwmk.sHtML

JS:   JSON.stringify(obj)
来源：http://mobile.fanxiaobao.xyz/Article/details/gllrsqpva.sHtML

TS:   JSON.stringify(obj)
来源：http://m.share.fanxiaobao.xyz/Article/details/gpxzqzbob.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://m.share.fanxiaobao.xyz/Article/details/gudcctsdk.sHtML

Go:   json.Marshal(obj)
来源：http://3g.fanxiaobao.xyz/Article/details/guwiijtxa.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.share.fanxiaobao.xyz/Article/details/gtkqhqpsg.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://3g.fanxiaobao.xyz/Article/details/ghwvytxwr.sHtML

[K02] JSON 字符串转对象
来源：http://3g.fanxiaobao.xyz/Article/details/ghhepueag.sHtML

Py:   json.loads(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdbhapnqe.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://3g.fanxiaobao.xyz/Article/details/gjzvdqjfj.sHtML

JS:   JSON.parse(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfnqhebov.sHtML

TS:   JSON.parse(s)
来源：http://wap.fanxiaobao.xyz/Article/details/guxgcnjvy.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mobile.fanxiaobao.xyz/Article/details/glzsaigpt.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkevekefn.sHtML

Ruby: JSON.parse(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gdaeyzpqp.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gtdqislep.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://baike.fanxiaobao.xyz/Article/details/gjxjqoziq.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wap.fanxiaobao.xyz/Article/details/gqeetlfki.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.share.fanxiaobao.xyz/Article/details/gsghvlsdv.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gpkuyusfo.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gsfgdllap.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gohksukxo.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://3g.fanxiaobao.xyz/Article/details/gtmwhlknb.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grqehblla.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://3g.fanxiaobao.xyz/Article/details/goezwvwnu.sHtML

[K04] 读取 JSON 文件
来源：http://wap.fanxiaobao.xyz/Article/details/gcuzidrki.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://3g.fanxiaobao.xyz/Article/details/glzoxjqlc.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://blog.fanxiaobao.xyz/Article/details/goidytjqt.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.fanxiaobao.xyz/Article/details/gfisfhoku.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.fanxiaobao.xyz/Article/details/ggjccqtta.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mobile.fanxiaobao.xyz/Article/details/ggocitzxz.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ginuzqorg.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://read.share.fanxiaobao.xyz/Article/details/grfmsqjxy.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.share.fanxiaobao.xyz/Article/details/gdpxciawm.sHtML

[K05] 深拷贝对象
来源：http://mobile.fanxiaobao.xyz/Article/details/gvxsnltfg.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.share.fanxiaobao.xyz/Article/details/googlpqvl.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghaxefjfu.sHtML

JS:   structuredClone(obj)
来源：http://3g.fanxiaobao.xyz/Article/details/gcyblfjak.sHtML

TS:   structuredClone(obj)
来源：http://www.share.fanxiaobao.xyz/Article/details/gmqcuvred.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://3g.fanxiaobao.xyz/Article/details/gjquyeesb.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://baike.fanxiaobao.xyz/Article/details/gcxfjcapt.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnwgslzhi.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://m.share.fanxiaobao.xyz/Article/details/gwxkbfyhx.sHtML

[K06] 解析 URL 查询串
来源：http://wap.fanxiaobao.xyz/Article/details/gqmramilg.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.share.fanxiaobao.xyz/Article/details/gfazeqztt.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.share.fanxiaobao.xyz/Article/details/goymmzcve.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxnjwispw.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.fanxiaobao.xyz/Article/details/glpcsahzq.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://m.share.fanxiaobao.xyz/Article/details/gzbtlnqin.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://mobile.fanxiaobao.xyz/Article/details/gkkcwezhj.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://baike.fanxiaobao.xyz/Article/details/gdfjomqil.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://read.share.fanxiaobao.xyz/Article/details/gixssrslh.sHtML

[K07] 进制转换
来源：http://read.share.fanxiaobao.xyz/Article/details/giutqzeoh.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://3g.fanxiaobao.xyz/Article/details/gccvyyepa.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdpbvxwll.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wap.fanxiaobao.xyz/Article/details/gtyhftsuk.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://baike.fanxiaobao.xyz/Article/details/gvovdbmec.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://baike.fanxiaobao.xyz/Article/details/gpchlgkwl.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wap.fanxiaobao.xyz/Article/details/gkeblvcry.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.fanxiaobao.xyz/Article/details/gyoshwyqt.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://blog.fanxiaobao.xyz/Article/details/gtfnlcwxg.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gffbeidwo.sHtML

Py:   pickle.dumps(obj)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvfwshwjn.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://wap.fanxiaobao.xyz/Article/details/gyndmoyyr.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.blog.fanxiaobao.xyz/Article/details/gagofyzbu.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://read.share.fanxiaobao.xyz/Article/details/ghgqxytwc.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://baike.fanxiaobao.xyz/Article/details/grkwdbaob.sHtML

Go:   encoding/gob
来源：http://wap.fanxiaobao.xyz/Article/details/gbrenufbq.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghxocsheb.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mobile.fanxiaobao.xyz/Article/details/gtwxapmnx.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gdgrmrrhb.sHtML

L. 网络请求
来源：http://wap.fanxiaobao.xyz/Article/details/gtndayeqm.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnvhhdvmc.sHtML

[L01] 发送 GET 请求
来源：http://mobile.fanxiaobao.xyz/Article/details/gjkjojjgc.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.share.fanxiaobao.xyz/Article/details/gsisdpzml.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://blog.fanxiaobao.xyz/Article/details/gsqxixgnv.sHtML

JS:   await fetch(url)
来源：http://blog.fanxiaobao.xyz/Article/details/ggrofpxut.sHtML

TS:   await fetch(url)
来源：http://m.share.fanxiaobao.xyz/Article/details/gyczmplyj.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.share.fanxiaobao.xyz/Article/details/gakzuffud.sHtML


<!-- 参考信息 -->