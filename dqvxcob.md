代发 wailian999

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://baike.fanxiaobao.xyz/Article/details/gxactgdld.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://baike.fanxiaobao.xyz/Article/details/guboeznnc.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://3g.fanxiaobao.xyz/Article/details/gvjxszpft.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gpojgurjr.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://read.share.fanxiaobao.xyz/Article/details/gbhzbwocq.sHtML

Ruby: rescue ArgumentError => e
来源：http://blog.fanxiaobao.xyz/Article/details/gswhfmhzf.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtpqypvhf.sHtML

[H06] 可选值 / 空值安全访问
来源：http://blog.fanxiaobao.xyz/Article/details/gluzfogni.sHtML

Py:   value = d.get("k") or default
来源：http://mobile.fanxiaobao.xyz/Article/details/ghsublnmo.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.fanxiaobao.xyz/Article/details/gndwrjnbv.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://blog.fanxiaobao.xyz/Article/details/gowrwxydl.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://mobile.fanxiaobao.xyz/Article/details/gtgagebhw.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwjohuenk.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://3g.fanxiaobao.xyz/Article/details/gmxgycdxf.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.share.fanxiaobao.xyz/Article/details/gvfnjuwpn.sHtML

C#:   obj?.A?.B ?? default
来源：http://3g.fanxiaobao.xyz/Article/details/gghhqaffi.sHtML

[H07] 断言
来源：http://www.share.fanxiaobao.xyz/Article/details/gslcfjqej.sHtML

Py:   assert x > 0, "必须为正"
来源：http://mobile.fanxiaobao.xyz/Article/details/gofuhelto.sHtML

PHP:  assert($x > 0);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gurbuarwu.sHtML

JS:   console.assert(x > 0);
来源：http://baike.fanxiaobao.xyz/Article/details/gtmnkdxqy.sHtML

TS:   console.assert(x > 0);
来源：http://blog.fanxiaobao.xyz/Article/details/gsvesrljy.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzlsccpeg.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.share.fanxiaobao.xyz/Article/details/gvyvfvvlz.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://mobile.fanxiaobao.xyz/Article/details/gldpzfxkw.sHtML

C#:   Debug.Assert(x > 0);
来源：http://m.share.fanxiaobao.xyz/Article/details/gsxvlekdc.sHtML

[H08] 获取错误信息与堆栈
来源：http://blog.fanxiaobao.xyz/Article/details/gaxcldpwj.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://baike.fanxiaobao.xyz/Article/details/gizpchqha.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.share.fanxiaobao.xyz/Article/details/gitluvmmk.sHtML

JS:   e.message;  e.stack
来源：http://blog.fanxiaobao.xyz/Article/details/gppdpjadx.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gazhxhlch.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://read.share.fanxiaobao.xyz/Article/details/garnyqgks.sHtML

Go:   err.Error()
来源：http://wap.fanxiaobao.xyz/Article/details/gmvcueoqr.sHtML

Ruby: e.message;  e.backtrace
来源：http://mobile.fanxiaobao.xyz/Article/details/gtyqpoqtq.sHtML

C#:   e.Message;  e.StackTrace
来源：http://mobile.fanxiaobao.xyz/Article/details/gmuksepir.sHtML

[H09] 带错误码的异常
来源：http://baike.fanxiaobao.xyz/Article/details/gqlurkyry.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfdfhegij.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://read.share.fanxiaobao.xyz/Article/details/gxeqbamln.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnczjcjqf.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.share.fanxiaobao.xyz/Article/details/gqnuqvnjx.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://blog.fanxiaobao.xyz/Article/details/gjykezavw.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://read.share.fanxiaobao.xyz/Article/details/gpjuwdjrr.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://baike.fanxiaobao.xyz/Article/details/gkwjghwmv.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://baike.fanxiaobao.xyz/Article/details/goxrvelym.sHtML

[H10] 资源自动释放
来源：http://read.share.fanxiaobao.xyz/Article/details/gyfvjajaf.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://blog.fanxiaobao.xyz/Article/details/gywagxvac.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wap.fanxiaobao.xyz/Article/details/gzmzbmkxv.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.fanxiaobao.xyz/Article/details/gitqhddkw.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.fanxiaobao.xyz/Article/details/gfmzvtyac.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnjyioalh.sHtML

Go:   defer f.Close()
来源：http://www.share.fanxiaobao.xyz/Article/details/guqtkludb.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mobile.fanxiaobao.xyz/Article/details/gkmvjxgnc.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wap.fanxiaobao.xyz/Article/details/gnekxteci.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gjjuvlhgg.sHtML

I. 正则表达式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvmyynupf.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gnzjxbdtx.sHtML

[I01] 判断是否匹配
来源：http://blog.fanxiaobao.xyz/Article/details/gtjomyqwx.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gduqubffo.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjrlefqzb.sHtML

JS:   /\d+/.test(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbdvydtyv.sHtML

TS:   /\d+/.test(s)
来源：http://blog.fanxiaobao.xyz/Article/details/gbpdurdyf.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://read.share.fanxiaobao.xyz/Article/details/gcipcutdm.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wap.fanxiaobao.xyz/Article/details/gptiyqlzb.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gskmwgivl.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbkewqgxs.sHtML

[I02] 提取所有匹配
来源：http://baike.fanxiaobao.xyz/Article/details/gfggvpbpn.sHtML

Py:   re.findall(r"\d+", s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gzjxmmiyx.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wap.fanxiaobao.xyz/Article/details/gzveggucp.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://read.share.fanxiaobao.xyz/Article/details/gmzzrxmfe.sHtML

TS:   s.match(/\d+/g)
来源：http://blog.fanxiaobao.xyz/Article/details/gkbnocifr.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://read.share.fanxiaobao.xyz/Article/details/glibgztyy.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdrmrsrwo.sHtML

Ruby: s.scan(/\d+/)
来源：http://baike.fanxiaobao.xyz/Article/details/gfgizftcv.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.share.fanxiaobao.xyz/Article/details/gntlnduqz.sHtML

[I03] 提取捕获分组
来源：http://mobile.fanxiaobao.xyz/Article/details/gbgtuvdtt.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://baike.fanxiaobao.xyz/Article/details/gxtvbcehb.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://baike.fanxiaobao.xyz/Article/details/gyhlqpsdt.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wap.fanxiaobao.xyz/Article/details/gkdzzaqum.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wap.fanxiaobao.xyz/Article/details/gaojbzicm.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://baike.fanxiaobao.xyz/Article/details/gtkbjszod.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://baike.fanxiaobao.xyz/Article/details/gcaewnwou.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://blog.fanxiaobao.xyz/Article/details/gbmphwrst.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://blog.fanxiaobao.xyz/Article/details/glcqxnbnv.sHtML

[I04] 正则替换
来源：http://3g.fanxiaobao.xyz/Article/details/gbwfqryeb.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gvlxustgm.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://baike.fanxiaobao.xyz/Article/details/gqwsdcala.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://read.share.fanxiaobao.xyz/Article/details/gtliumvzn.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://m.share.fanxiaobao.xyz/Article/details/gvmgqlyia.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://read.share.fanxiaobao.xyz/Article/details/gxbulppjg.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://read.share.fanxiaobao.xyz/Article/details/gosusnetv.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://read.share.fanxiaobao.xyz/Article/details/gsymmtpgo.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mobile.fanxiaobao.xyz/Article/details/giqcdpcqx.sHtML

[I05] 按正则拆分
来源：http://baike.fanxiaobao.xyz/Article/details/giwpxgyrx.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://wap.fanxiaobao.xyz/Article/details/geohukiza.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mobile.fanxiaobao.xyz/Article/details/gdvloacjg.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goqsozfpu.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gklnqrrau.sHtML

Java: s.split("\\s*,\\s*")
来源：http://wap.fanxiaobao.xyz/Article/details/gzxtgjkxh.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://mobile.fanxiaobao.xyz/Article/details/ggcfkyxhs.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://3g.fanxiaobao.xyz/Article/details/gxlvkvhin.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://baike.fanxiaobao.xyz/Article/details/gfwmrfhei.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://baike.fanxiaobao.xyz/Article/details/gpvcioyxv.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gruzowmrt.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wap.fanxiaobao.xyz/Article/details/ggndbrfrq.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsrycktxw.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.fanxiaobao.xyz/Article/details/gbrvwzovm.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://blog.fanxiaobao.xyz/Article/details/gltzyuqhz.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://3g.fanxiaobao.xyz/Article/details/glyejowbu.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqiluiaem.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://3g.fanxiaobao.xyz/Article/details/gegjwjsci.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.blog.fanxiaobao.xyz/Article/details/glcusxzvq.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mobile.fanxiaobao.xyz/Article/details/gzvfvcajr.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://blog.fanxiaobao.xyz/Article/details/gvcwsyshe.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gstgnqvuk.sHtML

TS:   /error/gim
来源：http://mobile.fanxiaobao.xyz/Article/details/gxfqtsfyg.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wap.fanxiaobao.xyz/Article/details/gwiyfiqev.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wap.fanxiaobao.xyz/Article/details/gpfwmcqjc.sHtML

Ruby: s.scan(/error/i)
来源：http://baike.fanxiaobao.xyz/Article/details/gkxjuhykn.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mobile.fanxiaobao.xyz/Article/details/gvzzorimb.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://wap.fanxiaobao.xyz/Article/details/gxzmsuoil.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.share.fanxiaobao.xyz/Article/details/ggsuygjkq.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://baike.fanxiaobao.xyz/Article/details/gymkgvrpt.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.fanxiaobao.xyz/Article/details/gtspppgzn.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.fanxiaobao.xyz/Article/details/gbjynoqxo.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpzihdlwi.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.share.fanxiaobao.xyz/Article/details/gdkkbbysm.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://m.share.fanxiaobao.xyz/Article/details/gaodhezaz.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://baike.fanxiaobao.xyz/Article/details/gvgawbgwl.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gzsqtotdo.sHtML

J. 日期与时间
来源：http://www.share.fanxiaobao.xyz/Article/details/giogfhkrq.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/grxueyopa.sHtML

[J01] 获取当前时间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzmdzymqq.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://wap.fanxiaobao.xyz/Article/details/goxrbxzva.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdfvaayez.sHtML

JS:   new Date();  Date.now()
来源：http://3g.fanxiaobao.xyz/Article/details/gicxkopmj.sHtML

TS:   new Date();  Date.now()
来源：http://blog.fanxiaobao.xyz/Article/details/grcewqzuo.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://baike.fanxiaobao.xyz/Article/details/gobxtnaiy.sHtML

Go:   time.Now()
来源：http://baike.fanxiaobao.xyz/Article/details/ghcmhatvs.sHtML

Ruby: Time.now
来源：http://www.share.fanxiaobao.xyz/Article/details/girekbitc.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://m.share.fanxiaobao.xyz/Article/details/gueniqebl.sHtML

[J02] 格式化输出
来源：http://read.share.fanxiaobao.xyz/Article/details/gazhmviel.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gojozuudl.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wap.fanxiaobao.xyz/Article/details/gdgptvpwk.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.share.fanxiaobao.xyz/Article/details/galrpmdhb.sHtML

TS:   d.toISOString()
来源：http://wap.fanxiaobao.xyz/Article/details/gsdsvpwbs.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.blog.fanxiaobao.xyz/Article/details/glawbekfx.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://3g.fanxiaobao.xyz/Article/details/gwnsojpaa.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.fanxiaobao.xyz/Article/details/grlmavwbb.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdahpvvjz.sHtML

[J03] 字符串解析为日期
来源：http://mobile.fanxiaobao.xyz/Article/details/gfzohdpin.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://blog.fanxiaobao.xyz/Article/details/gkzraeerb.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.blog.fanxiaobao.xyz/Article/details/goswxsedw.sHtML

JS:   new Date("2024-01-02")
来源：http://m.share.fanxiaobao.xyz/Article/details/gmfmhfqyf.sHtML

TS:   new Date("2024-01-02")
来源：http://blog.fanxiaobao.xyz/Article/details/gqfmcqstt.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grcvaxpwz.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://3g.fanxiaobao.xyz/Article/details/gihziudci.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://read.share.fanxiaobao.xyz/Article/details/gnqoqosdw.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://baike.fanxiaobao.xyz/Article/details/gnrdveinw.sHtML

[J04] 时间戳与日期互转
来源：http://baike.fanxiaobao.xyz/Article/details/guvnzlwlk.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gskldmezx.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://blog.fanxiaobao.xyz/Article/details/gkmcfuibv.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gszamcpvp.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guhgmbtnt.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://blog.fanxiaobao.xyz/Article/details/gxphoowrq.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://3g.fanxiaobao.xyz/Article/details/gocodzyku.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.share.fanxiaobao.xyz/Article/details/gpxhxljzo.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyjmpzqwz.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcosggtpm.sHtML

Py:   now + timedelta(days=7)
来源：http://wap.fanxiaobao.xyz/Article/details/gahnxalxm.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://m.share.fanxiaobao.xyz/Article/details/guvkljuuk.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.fanxiaobao.xyz/Article/details/gyglprmtl.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.fanxiaobao.xyz/Article/details/ghfdcdwby.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://3g.fanxiaobao.xyz/Article/details/gzneflenc.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://wap.fanxiaobao.xyz/Article/details/gdtybqmml.sHtML

Ruby: Time.now + 7 * 86400
来源：http://baike.fanxiaobao.xyz/Article/details/gjgvlairm.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://3g.fanxiaobao.xyz/Article/details/geiurerwt.sHtML

[J06] 计算两时间之差
来源：http://m.share.fanxiaobao.xyz/Article/details/gjfkmnoyl.sHtML

Py:   (end - start).total_seconds()
来源：http://blog.fanxiaobao.xyz/Article/details/gnsguimfh.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghfsaxkxi.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://read.share.fanxiaobao.xyz/Article/details/gqicvggxf.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wap.fanxiaobao.xyz/Article/details/gmuhsvlam.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://3g.fanxiaobao.xyz/Article/details/grymaiaku.sHtML

Go:   end.Sub(start).Hours()
来源：http://baike.fanxiaobao.xyz/Article/details/gaxzfyppy.sHtML

Ruby: end - start                 # 返回秒数
来源：http://mobile.fanxiaobao.xyz/Article/details/gwolnakqk.sHtML

C#:   (end - start).TotalSeconds
来源：http://wap.fanxiaobao.xyz/Article/details/gpxjoytac.sHtML

[J07] 比较两个日期
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtfpebxaz.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://3g.fanxiaobao.xyz/Article/details/gxownddca.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.share.fanxiaobao.xyz/Article/details/gmqsjtwlw.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://3g.fanxiaobao.xyz/Article/details/gelzazvhx.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gotvsgfka.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gcqhftogf.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geqhamelv.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://m.share.fanxiaobao.xyz/Article/details/gshvylbgv.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://baike.fanxiaobao.xyz/Article/details/gjgmxpkau.sHtML

[J08] 提取年月日与星期
来源：http://wap.fanxiaobao.xyz/Article/details/gkdavjort.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.share.fanxiaobao.xyz/Article/details/gjdhiwkgx.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wap.fanxiaobao.xyz/Article/details/gdotgsyff.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://baike.fanxiaobao.xyz/Article/details/gtahhmrqm.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://read.share.fanxiaobao.xyz/Article/details/gxwgcfmsl.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.share.fanxiaobao.xyz/Article/details/gbvrlxtyh.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geitkbnhn.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://baike.fanxiaobao.xyz/Article/details/gewtpsnvl.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://blog.fanxiaobao.xyz/Article/details/gnyvjknqz.sHtML

[J09] 时区处理
来源：http://www.share.fanxiaobao.xyz/Article/details/gslwzvqee.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://baike.fanxiaobao.xyz/Article/details/gsrecbqux.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.share.fanxiaobao.xyz/Article/details/gtttagjxt.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.fanxiaobao.xyz/Article/details/gptktmqwg.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.fanxiaobao.xyz/Article/details/gsadbkury.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://baike.fanxiaobao.xyz/Article/details/gxcmodzlb.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://read.share.fanxiaobao.xyz/Article/details/ggfmsvlom.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://blog.fanxiaobao.xyz/Article/details/glqgjlltm.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://m.share.fanxiaobao.xyz/Article/details/gpsgtcdzw.sHtML

[J10] 取今天 / 本月第一天
来源：http://3g.fanxiaobao.xyz/Article/details/gscmoxhjy.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://wap.fanxiaobao.xyz/Article/details/gtgikrsor.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://baike.fanxiaobao.xyz/Article/details/gywwqwllx.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gogctzriq.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wap.fanxiaobao.xyz/Article/details/gosfggibv.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gexfymamk.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtrpucmnc.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gohxqqgsp.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gobzgxocy.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/ghhvyvdkw.sHtML

K. JSON 与序列化
来源：http://read.share.fanxiaobao.xyz/Article/details/gkmqdbpgd.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/giqtsaiuy.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gazennbqx.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wap.fanxiaobao.xyz/Article/details/getvtsime.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://baike.fanxiaobao.xyz/Article/details/gmqflfldv.sHtML

JS:   JSON.stringify(obj)
来源：http://www.share.fanxiaobao.xyz/Article/details/ggrjwktgl.sHtML

TS:   JSON.stringify(obj)
来源：http://www.blog.fanxiaobao.xyz/Article/details/getuduawh.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mobile.fanxiaobao.xyz/Article/details/gejvnqzps.sHtML

Go:   json.Marshal(obj)
来源：http://m.share.fanxiaobao.xyz/Article/details/gshsukhzj.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://mobile.fanxiaobao.xyz/Article/details/grumucsyf.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://3g.fanxiaobao.xyz/Article/details/gmkntsuwa.sHtML

[K02] JSON 字符串转对象
来源：http://wap.fanxiaobao.xyz/Article/details/gwqlzznub.sHtML

Py:   json.loads(s)
来源：http://blog.fanxiaobao.xyz/Article/details/gryeminfw.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://m.share.fanxiaobao.xyz/Article/details/gkdewyttp.sHtML

JS:   JSON.parse(s)
来源：http://blog.fanxiaobao.xyz/Article/details/gtwfzqicr.sHtML

TS:   JSON.parse(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbbbdigrv.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.share.fanxiaobao.xyz/Article/details/gvwqqieof.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://mobile.fanxiaobao.xyz/Article/details/glucdexzg.sHtML

Ruby: JSON.parse(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/ggfnibnav.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gqhmakewn.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.share.fanxiaobao.xyz/Article/details/gjlzmhzad.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://blog.fanxiaobao.xyz/Article/details/galnecglw.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mobile.fanxiaobao.xyz/Article/details/gmjiezsyd.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gijemygse.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://baike.fanxiaobao.xyz/Article/details/gylscdxxj.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://blog.fanxiaobao.xyz/Article/details/gqfxhwbgm.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://3g.fanxiaobao.xyz/Article/details/gaizhixom.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.share.fanxiaobao.xyz/Article/details/gpsaeinqi.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxmxupfpt.sHtML

[K04] 读取 JSON 文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/guydvrxwv.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://m.share.fanxiaobao.xyz/Article/details/gwmhfiiin.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mobile.fanxiaobao.xyz/Article/details/gvpkuxozd.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.fanxiaobao.xyz/Article/details/gkdmninzk.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.fanxiaobao.xyz/Article/details/gcwtkcalu.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wap.fanxiaobao.xyz/Article/details/girttvxnz.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://baike.fanxiaobao.xyz/Article/details/gskfqekyl.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gymiyadiw.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mobile.fanxiaobao.xyz/Article/details/gfztonero.sHtML

[K05] 深拷贝对象
来源：http://3g.fanxiaobao.xyz/Article/details/gwkgfyitj.sHtML

Py:   copy.deepcopy(obj)
来源：http://mobile.fanxiaobao.xyz/Article/details/gtsyyyrxy.sHtML

PHP:  unserialize(serialize($obj));
来源：http://wap.fanxiaobao.xyz/Article/details/gqsruublu.sHtML

JS:   structuredClone(obj)
来源：http://www.share.fanxiaobao.xyz/Article/details/gnnymekpc.sHtML

TS:   structuredClone(obj)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gedfuibkf.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://3g.fanxiaobao.xyz/Article/details/gtdspnaqw.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wap.fanxiaobao.xyz/Article/details/gzyrpujqv.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wap.fanxiaobao.xyz/Article/details/gmdfzzgji.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsxongeew.sHtML

[K06] 解析 URL 查询串
来源：http://baike.fanxiaobao.xyz/Article/details/gemknqbsu.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.share.fanxiaobao.xyz/Article/details/gtxslfqyu.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://m.share.fanxiaobao.xyz/Article/details/gfogyhlyu.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.fanxiaobao.xyz/Article/details/gjasvxubd.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.fanxiaobao.xyz/Article/details/gavywovqv.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.share.fanxiaobao.xyz/Article/details/gkcfquhuq.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://3g.fanxiaobao.xyz/Article/details/ghwjvnult.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://m.share.fanxiaobao.xyz/Article/details/gvqhebndm.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.blog.fanxiaobao.xyz/Article/details/grvcahkrr.sHtML

[K07] 进制转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gredzyyoq.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wap.fanxiaobao.xyz/Article/details/gmewxkclk.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcrvvqafd.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://m.share.fanxiaobao.xyz/Article/details/gatyflion.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://read.share.fanxiaobao.xyz/Article/details/gbhijiqey.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://baike.fanxiaobao.xyz/Article/details/gyxqprvyq.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://3g.fanxiaobao.xyz/Article/details/gcedzwfew.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://baike.fanxiaobao.xyz/Article/details/gfypibwti.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://blog.fanxiaobao.xyz/Article/details/gddgasomp.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://mobile.fanxiaobao.xyz/Article/details/gpgvtwxgb.sHtML

Py:   pickle.dumps(obj)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gywhmhhdx.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://baike.fanxiaobao.xyz/Article/details/ghgrxxbcx.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://wap.fanxiaobao.xyz/Article/details/giflgmzmk.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://read.share.fanxiaobao.xyz/Article/details/gnbmmxuxr.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdoewytfd.sHtML

Go:   encoding/gob
来源：http://blog.fanxiaobao.xyz/Article/details/ghzjzyzjh.sHtML

Ruby: Marshal.dump(obj)
来源：http://baike.fanxiaobao.xyz/Article/details/glmjbmsaj.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wap.fanxiaobao.xyz/Article/details/gjndxberz.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gcjprylet.sHtML

L. 网络请求
来源：http://3g.fanxiaobao.xyz/Article/details/gscfwzdvm.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gjrkozqth.sHtML

[L01] 发送 GET 请求
来源：http://wap.fanxiaobao.xyz/Article/details/gsgrlikjc.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://blog.fanxiaobao.xyz/Article/details/gsfyhbmjs.sHtML


<!-- 参考信息 -->