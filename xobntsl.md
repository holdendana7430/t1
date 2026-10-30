代发 wailian999

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://baike.fanxiaobao.xyz/Article/details/gyrzupqaf.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gucivqotj.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://wap.fanxiaobao.xyz/Article/details/gjcupuzvn.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjktptrxz.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.share.fanxiaobao.xyz/Article/details/gyenjhuky.sHtML

Ruby: rescue ArgumentError => e
来源：http://read.share.fanxiaobao.xyz/Article/details/gtmxinbgm.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://baike.fanxiaobao.xyz/Article/details/gqgbwsjxu.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.fanxiaobao.xyz/Article/details/giqwthmle.sHtML

Py:   value = d.get("k") or default
来源：http://m.share.fanxiaobao.xyz/Article/details/gqdleytra.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.blog.fanxiaobao.xyz/Article/details/glyheayxr.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://baike.fanxiaobao.xyz/Article/details/gewcuzxke.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.share.fanxiaobao.xyz/Article/details/gdpwbpgtr.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://m.share.fanxiaobao.xyz/Article/details/gbyzleeet.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://baike.fanxiaobao.xyz/Article/details/gfshmvgqp.sHtML

Ruby: d&.dig(:a, :b)
来源：http://blog.fanxiaobao.xyz/Article/details/gmxzeppvg.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwcslbtug.sHtML

[H07] 断言
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjyftsagi.sHtML

Py:   assert x > 0, "必须为正"
来源：http://m.share.fanxiaobao.xyz/Article/details/gihsgnnhm.sHtML

PHP:  assert($x > 0);
来源：http://blog.fanxiaobao.xyz/Article/details/gsnvricbo.sHtML

JS:   console.assert(x > 0);
来源：http://www.share.fanxiaobao.xyz/Article/details/gdozgoekv.sHtML

TS:   console.assert(x > 0);
来源：http://baike.fanxiaobao.xyz/Article/details/ghktnlstr.sHtML

Java: assert x > 0 : "必须为正";
来源：http://read.share.fanxiaobao.xyz/Article/details/guihulefn.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbdqsikmn.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grhkgyclw.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggxugxomh.sHtML

[H08] 获取错误信息与堆栈
来源：http://3g.fanxiaobao.xyz/Article/details/gdjvukwzz.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://mobile.fanxiaobao.xyz/Article/details/ghvawqgmn.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wap.fanxiaobao.xyz/Article/details/gvcsqtrtv.sHtML

JS:   e.message;  e.stack
来源：http://www.share.fanxiaobao.xyz/Article/details/gyriapwgw.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://m.share.fanxiaobao.xyz/Article/details/gwiuzssam.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://wap.fanxiaobao.xyz/Article/details/giesufess.sHtML

Go:   err.Error()
来源：http://wap.fanxiaobao.xyz/Article/details/gkjdakmrv.sHtML

Ruby: e.message;  e.backtrace
来源：http://baike.fanxiaobao.xyz/Article/details/ghlxzymug.sHtML

C#:   e.Message;  e.StackTrace
来源：http://m.share.fanxiaobao.xyz/Article/details/gpxanikmm.sHtML

[H09] 带错误码的异常
来源：http://read.share.fanxiaobao.xyz/Article/details/gifibgghd.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://baike.fanxiaobao.xyz/Article/details/gyejdqgwv.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://mobile.fanxiaobao.xyz/Article/details/guqygmxxo.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://m.share.fanxiaobao.xyz/Article/details/gwxnnfnev.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wap.fanxiaobao.xyz/Article/details/geuqdhvca.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wap.fanxiaobao.xyz/Article/details/gubctzqae.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mobile.fanxiaobao.xyz/Article/details/ggzfrrptj.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://m.share.fanxiaobao.xyz/Article/details/gycftqscu.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://blog.fanxiaobao.xyz/Article/details/gqppyjbyn.sHtML

[H10] 资源自动释放
来源：http://baike.fanxiaobao.xyz/Article/details/gmgugtxni.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://wap.fanxiaobao.xyz/Article/details/guygvlgjd.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://baike.fanxiaobao.xyz/Article/details/gmavdkymi.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.fanxiaobao.xyz/Article/details/gbaijbnwb.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.fanxiaobao.xyz/Article/details/gsfkdaicc.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjyecxfon.sHtML

Go:   defer f.Close()
来源：http://wap.fanxiaobao.xyz/Article/details/gvqfzfouq.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://baike.fanxiaobao.xyz/Article/details/gwlnqzuwj.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://3g.fanxiaobao.xyz/Article/details/gqkucrlqk.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gugjwtgbo.sHtML

I. 正则表达式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goksvorxm.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gknigwcfn.sHtML

[I01] 判断是否匹配
来源：http://read.share.fanxiaobao.xyz/Article/details/gfdrrksog.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://baike.fanxiaobao.xyz/Article/details/gaiiubuhb.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://m.share.fanxiaobao.xyz/Article/details/gbyjpbqnx.sHtML

JS:   /\d+/.test(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gzvvgdlog.sHtML

TS:   /\d+/.test(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/groscjlea.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://3g.fanxiaobao.xyz/Article/details/guactuhza.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wap.fanxiaobao.xyz/Article/details/gtcltpjxk.sHtML

Ruby: s.match?(/\d+/)
来源：http://m.share.fanxiaobao.xyz/Article/details/gwxqyyzdx.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://3g.fanxiaobao.xyz/Article/details/ghcvfsonl.sHtML

[I02] 提取所有匹配
来源：http://m.share.fanxiaobao.xyz/Article/details/gkkbomzcv.sHtML

Py:   re.findall(r"\d+", s)
来源：http://wap.fanxiaobao.xyz/Article/details/gyxjdvxdl.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://blog.fanxiaobao.xyz/Article/details/gayoaqykk.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wap.fanxiaobao.xyz/Article/details/gqtdeimjx.sHtML

TS:   s.match(/\d+/g)
来源：http://blog.fanxiaobao.xyz/Article/details/gnerlijkh.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://read.share.fanxiaobao.xyz/Article/details/gitairtng.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcxfjdxgn.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gctdkdktm.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://blog.fanxiaobao.xyz/Article/details/gikmdtwdu.sHtML

[I03] 提取捕获分组
来源：http://www.share.fanxiaobao.xyz/Article/details/gulxycscy.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gqqnnczvm.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mobile.fanxiaobao.xyz/Article/details/gimhtyrws.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.blog.fanxiaobao.xyz/Article/details/godkbrokf.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wap.fanxiaobao.xyz/Article/details/gvicmghqm.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://read.share.fanxiaobao.xyz/Article/details/gujcocgay.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.share.fanxiaobao.xyz/Article/details/gvieayzwf.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://blog.fanxiaobao.xyz/Article/details/gdwegmihm.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.share.fanxiaobao.xyz/Article/details/gxllnnjmy.sHtML

[I04] 正则替换
来源：http://wap.fanxiaobao.xyz/Article/details/gmclljwik.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gcezcyzla.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://3g.fanxiaobao.xyz/Article/details/gtkfbikuh.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.share.fanxiaobao.xyz/Article/details/gowaalnrb.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.share.fanxiaobao.xyz/Article/details/gdehzxikz.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.share.fanxiaobao.xyz/Article/details/gzccwftpo.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://3g.fanxiaobao.xyz/Article/details/gtrewxlbl.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://blog.fanxiaobao.xyz/Article/details/gsrdpzvmj.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.blog.fanxiaobao.xyz/Article/details/goidvprqm.sHtML

[I05] 按正则拆分
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfrghlerd.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gnjdyrpzp.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://blog.fanxiaobao.xyz/Article/details/gseaqgtkv.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://3g.fanxiaobao.xyz/Article/details/gjvwgcetl.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxlfnssec.sHtML

Java: s.split("\\s*,\\s*")
来源：http://blog.fanxiaobao.xyz/Article/details/grrtkqjlg.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://baike.fanxiaobao.xyz/Article/details/ganffveiu.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.share.fanxiaobao.xyz/Article/details/gzetuirwl.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://read.share.fanxiaobao.xyz/Article/details/gxuryxswp.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wap.fanxiaobao.xyz/Article/details/gujvziwep.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wap.fanxiaobao.xyz/Article/details/gnxvwevxe.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://m.share.fanxiaobao.xyz/Article/details/gnrpegcrv.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.fanxiaobao.xyz/Article/details/gvyncwgln.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdodzhihh.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjfwisjau.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://3g.fanxiaobao.xyz/Article/details/glpmqnzvz.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://m.share.fanxiaobao.xyz/Article/details/gersbiijr.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://blog.fanxiaobao.xyz/Article/details/ggqynoxro.sHtML

[I07] 忽略大小写与多行模式
来源：http://baike.fanxiaobao.xyz/Article/details/gnluugidm.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://m.share.fanxiaobao.xyz/Article/details/gnzaxzwbe.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mobile.fanxiaobao.xyz/Article/details/gtmravlky.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.share.fanxiaobao.xyz/Article/details/gajvjzqaf.sHtML

TS:   /error/gim
来源：http://blog.fanxiaobao.xyz/Article/details/gfhhohawj.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://baike.fanxiaobao.xyz/Article/details/gbmotybjo.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://read.share.fanxiaobao.xyz/Article/details/grmyutzwv.sHtML

Ruby: s.scan(/error/i)
来源：http://m.share.fanxiaobao.xyz/Article/details/gorrhmwlf.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://blog.fanxiaobao.xyz/Article/details/gsngqqsmz.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gawfnswwt.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mobile.fanxiaobao.xyz/Article/details/gasuqwhdo.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://blog.fanxiaobao.xyz/Article/details/grhnxtvnu.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.fanxiaobao.xyz/Article/details/gzbvdfmup.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzxbdynfg.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://wap.fanxiaobao.xyz/Article/details/gqnlcjakj.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gasyjfybp.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://3g.fanxiaobao.xyz/Article/details/gdfmojdvf.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://baike.fanxiaobao.xyz/Article/details/gxlfuoimn.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/ggcowqjcm.sHtML

J. 日期与时间
来源：http://www.share.fanxiaobao.xyz/Article/details/ggbqstqop.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/ghcvitqzm.sHtML

[J01] 获取当前时间
来源：http://www.share.fanxiaobao.xyz/Article/details/gdwfanuud.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://m.share.fanxiaobao.xyz/Article/details/gmlsfizba.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.share.fanxiaobao.xyz/Article/details/gvyzokgsd.sHtML

JS:   new Date();  Date.now()
来源：http://read.share.fanxiaobao.xyz/Article/details/gqxsegjam.sHtML

TS:   new Date();  Date.now()
来源：http://read.share.fanxiaobao.xyz/Article/details/gqfvjtaec.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://blog.fanxiaobao.xyz/Article/details/gizefabgt.sHtML

Go:   time.Now()
来源：http://m.share.fanxiaobao.xyz/Article/details/gqegqzajd.sHtML

Ruby: Time.now
来源：http://3g.fanxiaobao.xyz/Article/details/gifskwpym.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.share.fanxiaobao.xyz/Article/details/gfsmpzdxk.sHtML

[J02] 格式化输出
来源：http://wap.fanxiaobao.xyz/Article/details/gqvsjegsa.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.fanxiaobao.xyz/Article/details/gaybhffge.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://3g.fanxiaobao.xyz/Article/details/gqlzbtjau.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mobile.fanxiaobao.xyz/Article/details/gxlkxjjvi.sHtML

TS:   d.toISOString()
来源：http://read.share.fanxiaobao.xyz/Article/details/gffoykfes.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mobile.fanxiaobao.xyz/Article/details/gcxngceee.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://read.share.fanxiaobao.xyz/Article/details/ghkvpaytv.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.fanxiaobao.xyz/Article/details/grwoncgsh.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjzplmzst.sHtML

[J03] 字符串解析为日期
来源：http://wap.fanxiaobao.xyz/Article/details/gqcapaxcp.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://mobile.fanxiaobao.xyz/Article/details/gckdvniix.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://3g.fanxiaobao.xyz/Article/details/gdplcukdw.sHtML

JS:   new Date("2024-01-02")
来源：http://m.share.fanxiaobao.xyz/Article/details/ghnqqsnrg.sHtML

TS:   new Date("2024-01-02")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqemegqop.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://baike.fanxiaobao.xyz/Article/details/gbaqthpll.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://read.share.fanxiaobao.xyz/Article/details/gjnneljvy.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://m.share.fanxiaobao.xyz/Article/details/ggaximxdc.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://blog.fanxiaobao.xyz/Article/details/grzkvpbag.sHtML

[J04] 时间戳与日期互转
来源：http://m.share.fanxiaobao.xyz/Article/details/gpmezehsa.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://read.share.fanxiaobao.xyz/Article/details/guidfzgkc.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://mobile.fanxiaobao.xyz/Article/details/gmkfrfnjo.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwmggnihq.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://read.share.fanxiaobao.xyz/Article/details/gstvikbds.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://wap.fanxiaobao.xyz/Article/details/gziblfhuw.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://mobile.fanxiaobao.xyz/Article/details/gsbenyzaj.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://blog.fanxiaobao.xyz/Article/details/ghlvzscth.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://read.share.fanxiaobao.xyz/Article/details/gouwxwolh.sHtML

[J05] 时间加减（加 7 天）
来源：http://read.share.fanxiaobao.xyz/Article/details/gojnpunnm.sHtML

Py:   now + timedelta(days=7)
来源：http://wap.fanxiaobao.xyz/Article/details/gasooiwrz.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://read.share.fanxiaobao.xyz/Article/details/gjnoquauy.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.fanxiaobao.xyz/Article/details/gopnumhlq.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.fanxiaobao.xyz/Article/details/gcisgmkmj.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://mobile.fanxiaobao.xyz/Article/details/gevdtcnwn.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvsmujxit.sHtML

Ruby: Time.now + 7 * 86400
来源：http://m.share.fanxiaobao.xyz/Article/details/glairlnbk.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://wap.fanxiaobao.xyz/Article/details/gyqljyvdd.sHtML

[J06] 计算两时间之差
来源：http://m.share.fanxiaobao.xyz/Article/details/glvdazspo.sHtML

Py:   (end - start).total_seconds()
来源：http://m.share.fanxiaobao.xyz/Article/details/gxnylbosx.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.share.fanxiaobao.xyz/Article/details/gpbrkuaij.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://3g.fanxiaobao.xyz/Article/details/ghacryqiz.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://3g.fanxiaobao.xyz/Article/details/giakceniu.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://baike.fanxiaobao.xyz/Article/details/gfnvtcexy.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.share.fanxiaobao.xyz/Article/details/gsannaypp.sHtML

Ruby: end - start                 # 返回秒数
来源：http://baike.fanxiaobao.xyz/Article/details/gfihzrobq.sHtML

C#:   (end - start).TotalSeconds
来源：http://wap.fanxiaobao.xyz/Article/details/ghfmvbtjh.sHtML

[J07] 比较两个日期
来源：http://3g.fanxiaobao.xyz/Article/details/grafjnqcv.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://blog.fanxiaobao.xyz/Article/details/gypagdgqb.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.share.fanxiaobao.xyz/Article/details/gysgvcaiq.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://blog.fanxiaobao.xyz/Article/details/guhsjmzai.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.share.fanxiaobao.xyz/Article/details/grswvuasj.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gwotpdozm.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gvwhxgxzx.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://m.share.fanxiaobao.xyz/Article/details/grmqurnqv.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://3g.fanxiaobao.xyz/Article/details/gbmadfojn.sHtML

[J08] 提取年月日与星期
来源：http://m.share.fanxiaobao.xyz/Article/details/gwphrxfxo.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbnzzxzoz.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggszvppto.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grpbaqwyr.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mobile.fanxiaobao.xyz/Article/details/gflzpglzx.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gevyupshm.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://mobile.fanxiaobao.xyz/Article/details/gatzrrsyt.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://baike.fanxiaobao.xyz/Article/details/gbtneyyff.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://blog.fanxiaobao.xyz/Article/details/ghgdzyfmx.sHtML

[J09] 时区处理
来源：http://blog.fanxiaobao.xyz/Article/details/gpmcamjnh.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://blog.fanxiaobao.xyz/Article/details/garjplmnc.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://m.share.fanxiaobao.xyz/Article/details/gtrtjsdts.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.fanxiaobao.xyz/Article/details/goysbsdyt.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.fanxiaobao.xyz/Article/details/gdvnuvrpw.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mobile.fanxiaobao.xyz/Article/details/gswsllbmt.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://3g.fanxiaobao.xyz/Article/details/gjnjqbupo.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://blog.fanxiaobao.xyz/Article/details/gfhbxeiwh.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://3g.fanxiaobao.xyz/Article/details/gixlobftk.sHtML

[J10] 取今天 / 本月第一天
来源：http://baike.fanxiaobao.xyz/Article/details/gqtnblxxw.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gswzxxuwy.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://baike.fanxiaobao.xyz/Article/details/gvzrizsvi.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wap.fanxiaobao.xyz/Article/details/gxxpinwzi.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.blog.fanxiaobao.xyz/Article/details/guacsvlbm.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gpzdowghd.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://read.share.fanxiaobao.xyz/Article/details/gwnjqmppx.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://3g.fanxiaobao.xyz/Article/details/gylewyzyy.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://blog.fanxiaobao.xyz/Article/details/gdjptsbvo.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gcbhpowpy.sHtML

K. JSON 与序列化
来源：http://baike.fanxiaobao.xyz/Article/details/gtlodiekl.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gapxsxjzn.sHtML

[K01] 对象转 JSON 字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gtktnumvl.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://baike.fanxiaobao.xyz/Article/details/gssbuzumx.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mobile.fanxiaobao.xyz/Article/details/golkvicjz.sHtML

JS:   JSON.stringify(obj)
来源：http://read.share.fanxiaobao.xyz/Article/details/gazqhcnnf.sHtML

TS:   JSON.stringify(obj)
来源：http://wap.fanxiaobao.xyz/Article/details/ghwkaxlqi.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wap.fanxiaobao.xyz/Article/details/gvulrcdek.sHtML

Go:   json.Marshal(obj)
来源：http://mobile.fanxiaobao.xyz/Article/details/gxxyupydv.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gccqppgfm.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://blog.fanxiaobao.xyz/Article/details/gjodakozr.sHtML

[K02] JSON 字符串转对象
来源：http://mobile.fanxiaobao.xyz/Article/details/gfztqqjha.sHtML

Py:   json.loads(s)
来源：http://wap.fanxiaobao.xyz/Article/details/grkclylid.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://blog.fanxiaobao.xyz/Article/details/gpyivhlly.sHtML

JS:   JSON.parse(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gyewwxbqp.sHtML

TS:   JSON.parse(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gffpplhwe.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://baike.fanxiaobao.xyz/Article/details/gtnkhzxme.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.share.fanxiaobao.xyz/Article/details/gjecuizkg.sHtML

Ruby: JSON.parse(s)
来源：http://wap.fanxiaobao.xyz/Article/details/gweqzfgls.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gvfvzgubi.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://m.share.fanxiaobao.xyz/Article/details/gorpvezil.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbpdwofsp.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://m.share.fanxiaobao.xyz/Article/details/gypsugojf.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbhyeoady.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://3g.fanxiaobao.xyz/Article/details/gvojrjjhg.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://blog.fanxiaobao.xyz/Article/details/gzhboybfm.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mobile.fanxiaobao.xyz/Article/details/gcheijisy.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gueinatdn.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://3g.fanxiaobao.xyz/Article/details/gdrffrvtp.sHtML

[K04] 读取 JSON 文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gqdqgarla.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gspapirrn.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wap.fanxiaobao.xyz/Article/details/gjevobtte.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.fanxiaobao.xyz/Article/details/gonayvisx.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.fanxiaobao.xyz/Article/details/gofabrdmz.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://read.share.fanxiaobao.xyz/Article/details/gqxxyiwlr.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://read.share.fanxiaobao.xyz/Article/details/gtkeselia.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.share.fanxiaobao.xyz/Article/details/gprufaqfw.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpcibcgoj.sHtML

[K05] 深拷贝对象
来源：http://www.blog.fanxiaobao.xyz/Article/details/gngtpxxzl.sHtML

Py:   copy.deepcopy(obj)
来源：http://read.share.fanxiaobao.xyz/Article/details/gqqmlnfng.sHtML

PHP:  unserialize(serialize($obj));
来源：http://m.share.fanxiaobao.xyz/Article/details/grcrgkcdz.sHtML

JS:   structuredClone(obj)
来源：http://www.share.fanxiaobao.xyz/Article/details/ghmeooyqz.sHtML

TS:   structuredClone(obj)
来源：http://read.share.fanxiaobao.xyz/Article/details/grlqgglbh.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gidgirluc.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wap.fanxiaobao.xyz/Article/details/ghixcftbx.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://read.share.fanxiaobao.xyz/Article/details/gvbmdhrjh.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.share.fanxiaobao.xyz/Article/details/gnrskudfv.sHtML

[K06] 解析 URL 查询串
来源：http://wap.fanxiaobao.xyz/Article/details/gxedecsfk.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://m.share.fanxiaobao.xyz/Article/details/gozckciib.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://blog.fanxiaobao.xyz/Article/details/gaatqaxad.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvuvnbjlx.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.fanxiaobao.xyz/Article/details/gshvcilbe.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mobile.fanxiaobao.xyz/Article/details/gkbzkckxi.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://mobile.fanxiaobao.xyz/Article/details/ghpmdjphl.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mobile.fanxiaobao.xyz/Article/details/gcbdtbypl.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wap.fanxiaobao.xyz/Article/details/genoavqov.sHtML

[K07] 进制转换
来源：http://baike.fanxiaobao.xyz/Article/details/gqqxypenv.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://baike.fanxiaobao.xyz/Article/details/gipsftdad.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://3g.fanxiaobao.xyz/Article/details/gmqgeczou.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://baike.fanxiaobao.xyz/Article/details/gazdwnpzf.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://read.share.fanxiaobao.xyz/Article/details/gvndsujcw.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mobile.fanxiaobao.xyz/Article/details/ggoqsqneo.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://3g.fanxiaobao.xyz/Article/details/ghgveezvx.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://baike.fanxiaobao.xyz/Article/details/gvcqwgsqq.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://read.share.fanxiaobao.xyz/Article/details/gdmgilzmv.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://wap.fanxiaobao.xyz/Article/details/gaqnzwebb.sHtML

Py:   pickle.dumps(obj)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqdxnagez.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://m.share.fanxiaobao.xyz/Article/details/gaptfopkb.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://read.share.fanxiaobao.xyz/Article/details/gvnpdqnsk.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.share.fanxiaobao.xyz/Article/details/gbovcckwx.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbzgpczqi.sHtML

Go:   encoding/gob
来源：http://blog.fanxiaobao.xyz/Article/details/giotibdvl.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzqrjpgft.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://baike.fanxiaobao.xyz/Article/details/grrqsjlnt.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gipewbihy.sHtML

L. 网络请求
来源：http://mobile.fanxiaobao.xyz/Article/details/gzuczwvwo.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gigmcienf.sHtML

[L01] 发送 GET 请求
来源：http://read.share.fanxiaobao.xyz/Article/details/gmwaxlpzx.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://m.share.fanxiaobao.xyz/Article/details/gzzcnvkbs.sHtML


<!-- 参考信息 -->