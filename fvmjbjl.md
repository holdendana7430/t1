代发 wailian999

C#:   throw new ArgumentException("错误信息");
来源：http://baike.fehbvm.com/Article/details/gskifrygm.sHtML

[H04] 自定义异常类型
来源：http://read.share.fehbvm.com/Article/details/gqrihblrp.sHtML

Py:   class MyError(Exception): pass
来源：http://blog.fehbvm.com/Article/details/guvbwmmao.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.hesvh.cn/Article/details/gbjmgfdpa.sHtML

JS:   class MyError extends Error {}
来源：http://3g.zdbjq.cn/Article/details/gfaffyttl.sHtML

TS:   class MyError extends Error {}
来源：http://www.blog.fehbvm.com/Article/details/gpxwsvwil.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.fehbvm.com/Article/details/gdskzgnin.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://3g.fehbvm.com/Article/details/goudthpkz.sHtML

Ruby: class MyError < StandardError; end
来源：http://m.share.zdbjq.cn/Article/details/gdxqklppn.sHtML

C#:   class MyException : Exception {}
来源：http://wap.fehbvm.com/Article/details/giokptvap.sHtML

[H05] 捕获特定类型
来源：http://blog.fehbvm.com/Article/details/gqejgzlgn.sHtML

Py:   except ValueError as e:
来源：http://3g.hesvh.cn/Article/details/gqpyghban.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://baike.hesvh.cn/Article/details/gfbwxouko.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.blog.hesvh.cn/Article/details/gqklnwdmr.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.m.share.hesvh.cn/Article/details/goyruemje.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://m.share.fehbvm.com/Article/details/gizkhjndt.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.blog.hesvh.cn/Article/details/ggrnubqdh.sHtML

Ruby: rescue ArgumentError => e
来源：http://3g.fehbvm.com/Article/details/gymdtwtbn.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mobile.fehbvm.com/Article/details/gswiqhisj.sHtML

[H06] 可选值 / 空值安全访问
来源：http://3g.hesvh.cn/Article/details/gfavslwma.sHtML

Py:   value = d.get("k") or default
来源：http://3g.hesvh.cn/Article/details/gpnazjnmy.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://baike.hesvh.cn/Article/details/geglmyjih.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://mobile.fehbvm.com/Article/details/gfubsmzzz.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://read.share.fehbvm.com/Article/details/gswvwpaah.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mobile.zdbjq.cn/Article/details/gzxkfqpsx.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.share.fehbvm.com/Article/details/giwjinhqs.sHtML

Ruby: d&.dig(:a, :b)
来源：http://read.share.fehbvm.com/Article/details/gcfjxnrlh.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.m.share.hesvh.cn/Article/details/ghctveosp.sHtML

[H07] 断言
来源：http://baike.fehbvm.com/Article/details/gpfyhccmq.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.m.share.hesvh.cn/Article/details/gorsangwm.sHtML

PHP:  assert($x > 0);
来源：http://baike.zdbjq.cn/Article/details/gjzhrkvsw.sHtML

JS:   console.assert(x > 0);
来源：http://mobile.zdbjq.cn/Article/details/grunubnhx.sHtML

TS:   console.assert(x > 0);
来源：http://www.m.share.zdbjq.cn/Article/details/ghiygzzgm.sHtML

Java: assert x > 0 : "必须为正";
来源：http://mobile.hesvh.cn/Article/details/grdbtdxje.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://blog.zdbjq.cn/Article/details/grkcorgss.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://wap.hesvh.cn/Article/details/gqgennext.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.share.zdbjq.cn/Article/details/gsvonsszf.sHtML

[H08] 获取错误信息与堆栈
来源：http://wap.fehbvm.com/Article/details/gpwdcvdfd.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://3g.zdbjq.cn/Article/details/gtkcnxmma.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://read.share.fehbvm.com/Article/details/gdaaviubq.sHtML

JS:   e.message;  e.stack
来源：http://baike.hesvh.cn/Article/details/genbccers.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://m.share.hesvh.cn/Article/details/gmhhnsunh.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://baike.hesvh.cn/Article/details/gelurnyyg.sHtML

Go:   err.Error()
来源：http://www.m.share.fehbvm.com/Article/details/gblykpeat.sHtML

Ruby: e.message;  e.backtrace
来源：http://baike.zdbjq.cn/Article/details/gvkpotfpw.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.blog.hesvh.cn/Article/details/gtyuamgww.sHtML

[H09] 带错误码的异常
来源：http://blog.hesvh.cn/Article/details/gfqvoqkyn.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.share.zdbjq.cn/Article/details/gzhksznpk.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.share.zdbjq.cn/Article/details/gulibrwia.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wap.hesvh.cn/Article/details/gilrhnrnm.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://read.share.zdbjq.cn/Article/details/gyxhiglpu.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://baike.fehbvm.com/Article/details/gelpaczfi.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.share.zdbjq.cn/Article/details/gdreeqwxz.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://3g.fehbvm.com/Article/details/glswahcyx.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://m.share.hesvh.cn/Article/details/gytslblwj.sHtML

[H10] 资源自动释放
来源：http://blog.fehbvm.com/Article/details/gexvghxyg.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.m.share.hesvh.cn/Article/details/gkuexykxs.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mobile.zdbjq.cn/Article/details/gewultgre.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.fehbvm.com/Article/details/gzybfqouw.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.zdbjq.cn/Article/details/geyggcrbi.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mobile.hesvh.cn/Article/details/guatlcfxw.sHtML

Go:   defer f.Close()
来源：http://baike.hesvh.cn/Article/details/gwjsmprlk.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://m.share.fehbvm.com/Article/details/gwnljruhu.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gnisenlmu.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gmjymgajx.sHtML

I. 正则表达式
来源：http://read.share.zdbjq.cn/Article/details/gqrmrbreb.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gphaiqqhc.sHtML

[I01] 判断是否匹配
来源：http://blog.zdbjq.cn/Article/details/gokljweas.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mobile.fehbvm.com/Article/details/gzlrokffc.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://wap.fehbvm.com/Article/details/grikzckfa.sHtML

JS:   /\d+/.test(s)
来源：http://www.share.zdbjq.cn/Article/details/ggpycbbso.sHtML

TS:   /\d+/.test(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gywwphwlz.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://blog.fehbvm.com/Article/details/gwzaprviw.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://3g.zdbjq.cn/Article/details/gkxemunem.sHtML

Ruby: s.match?(/\d+/)
来源：http://baike.fehbvm.com/Article/details/ghltribcy.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mobile.hesvh.cn/Article/details/grxifdeqq.sHtML

[I02] 提取所有匹配
来源：http://wap.zdbjq.cn/Article/details/gavsnsicp.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.m.share.fehbvm.com/Article/details/gvpiteuec.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://blog.fehbvm.com/Article/details/gjxllwlyp.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mobile.zdbjq.cn/Article/details/gklxzdkfd.sHtML

TS:   s.match(/\d+/g)
来源：http://www.share.fehbvm.com/Article/details/guljcoyud.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://baike.zdbjq.cn/Article/details/ghwgardlk.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://m.share.hesvh.cn/Article/details/gsybhbfrm.sHtML

Ruby: s.scan(/\d+/)
来源：http://wap.zdbjq.cn/Article/details/gbmpilnth.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://baike.hesvh.cn/Article/details/gjikatjuc.sHtML

[I03] 提取捕获分组
来源：http://read.share.fehbvm.com/Article/details/gqjucliif.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://m.share.zdbjq.cn/Article/details/gzorgvfsh.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://read.share.zdbjq.cn/Article/details/gqvwhmqrb.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.share.zdbjq.cn/Article/details/gxeneixiz.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.blog.hesvh.cn/Article/details/gyoeauvtm.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://mobile.zdbjq.cn/Article/details/gnguxrijv.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wap.zdbjq.cn/Article/details/gohukqtxw.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://3g.fehbvm.com/Article/details/gnnzypanx.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://3g.fehbvm.com/Article/details/gugaiwzhd.sHtML

[I04] 正则替换
来源：http://baike.fehbvm.com/Article/details/gihqloqvr.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.share.zdbjq.cn/Article/details/ghtmcynzn.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mobile.hesvh.cn/Article/details/gkrilfemv.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.hesvh.cn/Article/details/gigjhezyj.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://baike.zdbjq.cn/Article/details/gwnzyzhqr.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://mobile.hesvh.cn/Article/details/geshytjdu.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://read.share.hesvh.cn/Article/details/gibqqeoen.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://3g.zdbjq.cn/Article/details/gpvlcilmt.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mobile.fehbvm.com/Article/details/gsslwukjr.sHtML

[I05] 按正则拆分
来源：http://mobile.hesvh.cn/Article/details/goprppzee.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://3g.hesvh.cn/Article/details/gvulcpjwt.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.blog.zdbjq.cn/Article/details/guqjudxnv.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://m.share.fehbvm.com/Article/details/ggvhylizj.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://baike.fehbvm.com/Article/details/gtnocjrem.sHtML

Java: s.split("\\s*,\\s*")
来源：http://wap.fehbvm.com/Article/details/gzsnftcvr.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://m.share.fehbvm.com/Article/details/gsgikhuuy.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://mobile.zdbjq.cn/Article/details/gwinkacvx.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.share.fehbvm.com/Article/details/gyprhfjvd.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.blog.fehbvm.com/Article/details/gtjhjgyto.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://mobile.fehbvm.com/Article/details/geqpddvis.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://m.share.hesvh.cn/Article/details/gplicmbvh.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.fehbvm.com/Article/details/gdyjpmwrl.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.zdbjq.cn/Article/details/ggqouqrtw.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://baike.hesvh.cn/Article/details/gbyznwdli.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.blog.zdbjq.cn/Article/details/gmiebufud.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://mobile.hesvh.cn/Article/details/gguyrfuhi.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://read.share.zdbjq.cn/Article/details/gxkehrjxa.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.share.fehbvm.com/Article/details/grfxxhktm.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mobile.fehbvm.com/Article/details/gfpsskbqt.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://m.share.hesvh.cn/Article/details/gpyvvkdch.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://m.share.hesvh.cn/Article/details/gfnjnkdto.sHtML

TS:   /error/gim
来源：http://www.share.fehbvm.com/Article/details/ghqkbumlz.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://3g.fehbvm.com/Article/details/gqvgknxcw.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.share.hesvh.cn/Article/details/genghsqqy.sHtML

Ruby: s.scan(/error/i)
来源：http://www.m.share.zdbjq.cn/Article/details/gpowiuefe.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://wap.zdbjq.cn/Article/details/gkgcygbgf.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.blog.zdbjq.cn/Article/details/garjgpxdq.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://blog.zdbjq.cn/Article/details/gtslzvsup.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://3g.zdbjq.cn/Article/details/gmkvholoz.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.fehbvm.com/Article/details/gppqlmkhd.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.fehbvm.com/Article/details/gafkvtovr.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://read.share.zdbjq.cn/Article/details/guumyvrwk.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.m.share.hesvh.cn/Article/details/ghwnfegpx.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://blog.hesvh.cn/Article/details/gjxtrffub.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://baike.hesvh.cn/Article/details/glvzvaxsm.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gfcnssmns.sHtML

J. 日期与时间
来源：http://baike.hesvh.cn/Article/details/gfremovih.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gwohomwbd.sHtML

[J01] 获取当前时间
来源：http://wap.zdbjq.cn/Article/details/goutabzgj.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.blog.fehbvm.com/Article/details/grwvsqite.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://read.share.fehbvm.com/Article/details/gvxabtlth.sHtML

JS:   new Date();  Date.now()
来源：http://baike.zdbjq.cn/Article/details/gepmouqex.sHtML

TS:   new Date();  Date.now()
来源：http://blog.zdbjq.cn/Article/details/gwttxhgsn.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://blog.hesvh.cn/Article/details/gthcxjgbt.sHtML

Go:   time.Now()
来源：http://wap.hesvh.cn/Article/details/ghjrkrowf.sHtML

Ruby: Time.now
来源：http://read.share.fehbvm.com/Article/details/gopkfyqxd.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.m.share.zdbjq.cn/Article/details/givqlogug.sHtML

[J02] 格式化输出
来源：http://wap.zdbjq.cn/Article/details/gblmenjwg.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.zdbjq.cn/Article/details/gndkcsopv.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wap.fehbvm.com/Article/details/gbdsdacbr.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://3g.zdbjq.cn/Article/details/gvdycvlpt.sHtML

TS:   d.toISOString()
来源：http://baike.fehbvm.com/Article/details/gyncliqqh.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://m.share.hesvh.cn/Article/details/gdqvihzqk.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wap.hesvh.cn/Article/details/gawbrbhil.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.fehbvm.com/Article/details/gfvdlfeui.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://mobile.hesvh.cn/Article/details/gffkpboco.sHtML

[J03] 字符串解析为日期
来源：http://3g.fehbvm.com/Article/details/gkjprxxqu.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://read.share.hesvh.cn/Article/details/gofxquyxy.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://mobile.zdbjq.cn/Article/details/gheolacow.sHtML

JS:   new Date("2024-01-02")
来源：http://read.share.zdbjq.cn/Article/details/gqaudkobx.sHtML

TS:   new Date("2024-01-02")
来源：http://read.share.fehbvm.com/Article/details/gftslcknp.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://m.share.fehbvm.com/Article/details/gqkhicdxx.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://blog.zdbjq.cn/Article/details/gcvkseenf.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.m.share.zdbjq.cn/Article/details/gwzdqgqwd.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.blog.fehbvm.com/Article/details/glrfkfzup.sHtML

[J04] 时间戳与日期互转
来源：http://www.share.zdbjq.cn/Article/details/glqavutec.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wap.hesvh.cn/Article/details/grvecoyee.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.share.fehbvm.com/Article/details/gtmmkkmbt.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.blog.fehbvm.com/Article/details/gwnaxrxsg.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://mobile.hesvh.cn/Article/details/gbbitrclx.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://m.share.fehbvm.com/Article/details/gnvdnhheh.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wap.hesvh.cn/Article/details/gwzknhptg.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://baike.hesvh.cn/Article/details/gcjpekbmi.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://mobile.zdbjq.cn/Article/details/gmkxbungc.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.m.share.hesvh.cn/Article/details/gophjeofw.sHtML

Py:   now + timedelta(days=7)
来源：http://wap.hesvh.cn/Article/details/gjrtlpuhc.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.share.zdbjq.cn/Article/details/gfghxdzhw.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.fehbvm.com/Article/details/gtebwutuh.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.fehbvm.com/Article/details/gslaanauk.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://wap.fehbvm.com/Article/details/gwjqdkaev.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://m.share.fehbvm.com/Article/details/gmpuwjifd.sHtML

Ruby: Time.now + 7 * 86400
来源：http://mobile.zdbjq.cn/Article/details/gerekcehm.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://baike.zdbjq.cn/Article/details/grbtwtyct.sHtML

[J06] 计算两时间之差
来源：http://www.share.zdbjq.cn/Article/details/givdloxlf.sHtML

Py:   (end - start).total_seconds()
来源：http://www.m.share.hesvh.cn/Article/details/gviacbxjp.sHtML

PHP:  $end->diff($start)->days;
来源：http://wap.zdbjq.cn/Article/details/gtqghufgj.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://read.share.fehbvm.com/Article/details/gfwxketop.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://read.share.zdbjq.cn/Article/details/gwnfdakak.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://wap.zdbjq.cn/Article/details/glnigpymv.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.share.zdbjq.cn/Article/details/grkvhrpiq.sHtML

Ruby: end - start                 # 返回秒数
来源：http://read.share.fehbvm.com/Article/details/gxffikgef.sHtML

C#:   (end - start).TotalSeconds
来源：http://mobile.fehbvm.com/Article/details/gtnfcomkp.sHtML

[J07] 比较两个日期
来源：http://3g.fehbvm.com/Article/details/gqeyhnchc.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://read.share.hesvh.cn/Article/details/guftavunp.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://baike.hesvh.cn/Article/details/ggqhessha.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://read.share.hesvh.cn/Article/details/gfwadqavs.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://blog.zdbjq.cn/Article/details/gtgqfaqft.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.m.share.fehbvm.com/Article/details/gokpsmzlh.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.share.fehbvm.com/Article/details/gysmgvenr.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.blog.fehbvm.com/Article/details/gvkahfrgy.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://m.share.zdbjq.cn/Article/details/gbycndlli.sHtML

[J08] 提取年月日与星期
来源：http://baike.fehbvm.com/Article/details/gytjzfeon.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wap.zdbjq.cn/Article/details/gxlgtkzde.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://read.share.hesvh.cn/Article/details/gnkvivyff.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://blog.hesvh.cn/Article/details/gmrslytxa.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://read.share.hesvh.cn/Article/details/gaxeuqtxy.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://m.share.zdbjq.cn/Article/details/gsowanuow.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://blog.fehbvm.com/Article/details/gaifaibll.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mobile.hesvh.cn/Article/details/guixuwvwp.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://baike.fehbvm.com/Article/details/gaidwjvqg.sHtML

[J09] 时区处理
来源：http://baike.fehbvm.com/Article/details/giaebebxd.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://m.share.zdbjq.cn/Article/details/gpmwvufpm.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://baike.fehbvm.com/Article/details/gzpscbuzd.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.zdbjq.cn/Article/details/gjwbcppeq.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.zdbjq.cn/Article/details/ggwegpwia.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.share.hesvh.cn/Article/details/ghysgpcjo.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.blog.fehbvm.com/Article/details/gdrnzfclk.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://m.share.hesvh.cn/Article/details/gylobcyhs.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://blog.zdbjq.cn/Article/details/ghulvfxhg.sHtML

[J10] 取今天 / 本月第一天
来源：http://wap.zdbjq.cn/Article/details/gmtpqxdcm.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://mobile.hesvh.cn/Article/details/gpvvlsioa.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://baike.hesvh.cn/Article/details/gjrbminvr.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://baike.zdbjq.cn/Article/details/gtyrhzwei.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://read.share.fehbvm.com/Article/details/ggoqbzxci.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://baike.fehbvm.com/Article/details/gekgjqern.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.m.share.hesvh.cn/Article/details/gbtywvszr.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://blog.fehbvm.com/Article/details/gwzfzkkwq.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mobile.zdbjq.cn/Article/details/gprafqmgn.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gawsyzaph.sHtML

K. JSON 与序列化
来源：http://m.share.zdbjq.cn/Article/details/gxdtztdpm.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gacxkvmou.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.share.zdbjq.cn/Article/details/gcjtwdfgi.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://m.share.zdbjq.cn/Article/details/gtabrjyjg.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://3g.fehbvm.com/Article/details/gvgoebffe.sHtML

JS:   JSON.stringify(obj)
来源：http://baike.fehbvm.com/Article/details/gmhthacqh.sHtML

TS:   JSON.stringify(obj)
来源：http://m.share.fehbvm.com/Article/details/gaqfbikae.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.m.share.zdbjq.cn/Article/details/gzldlkrck.sHtML

Go:   json.Marshal(obj)
来源：http://blog.zdbjq.cn/Article/details/gssbbtmsv.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://blog.hesvh.cn/Article/details/geyjnldhb.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gpzovfokq.sHtML

[K02] JSON 字符串转对象
来源：http://blog.zdbjq.cn/Article/details/gfkkxmeef.sHtML

Py:   json.loads(s)
来源：http://www.share.hesvh.cn/Article/details/gmlvuvhjr.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wap.zdbjq.cn/Article/details/gkniytkos.sHtML

JS:   JSON.parse(s)
来源：http://wap.zdbjq.cn/Article/details/guccxlmmb.sHtML

TS:   JSON.parse(s)
来源：http://3g.fehbvm.com/Article/details/gehlgxvwt.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://m.share.hesvh.cn/Article/details/gnxdkgopl.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://blog.hesvh.cn/Article/details/gifwaxwnv.sHtML

Ruby: JSON.parse(s)
来源：http://baike.zdbjq.cn/Article/details/gpwsfkqoz.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://baike.zdbjq.cn/Article/details/gatckrpgo.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://read.share.hesvh.cn/Article/details/giuquqqqx.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://m.share.fehbvm.com/Article/details/gfyirxtyt.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://3g.zdbjq.cn/Article/details/ggcjetdya.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://baike.fehbvm.com/Article/details/gfhhzbnye.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://baike.fehbvm.com/Article/details/gifqinjxe.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gpqbbjlyt.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://baike.fehbvm.com/Article/details/gqbqwteik.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.blog.hesvh.cn/Article/details/gvjlfxzaa.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.blog.fehbvm.com/Article/details/grbnfgbkh.sHtML

[K04] 读取 JSON 文件
来源：http://blog.zdbjq.cn/Article/details/giiqcmpia.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://m.share.fehbvm.com/Article/details/gdndqiosi.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.share.fehbvm.com/Article/details/gfrewzkox.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.hesvh.cn/Article/details/gepagvkck.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.hesvh.cn/Article/details/gkvlgasmu.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.share.fehbvm.com/Article/details/gtgcqdsbx.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mobile.zdbjq.cn/Article/details/ghxzzntao.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.share.fehbvm.com/Article/details/gihqgodyi.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.m.share.fehbvm.com/Article/details/gclcjagcj.sHtML

[K05] 深拷贝对象
来源：http://3g.hesvh.cn/Article/details/gwewpqqxs.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gvwttiigx.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.share.hesvh.cn/Article/details/gkifvgpyl.sHtML

JS:   structuredClone(obj)
来源：http://www.share.fehbvm.com/Article/details/gmxipmzdi.sHtML

TS:   structuredClone(obj)
来源：http://www.share.zdbjq.cn/Article/details/gtgxnkjaz.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://m.share.fehbvm.com/Article/details/gybqogdeu.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.m.share.hesvh.cn/Article/details/gcxxcvjov.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mobile.fehbvm.com/Article/details/gknsesrtx.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://read.share.fehbvm.com/Article/details/gzveewolw.sHtML

[K06] 解析 URL 查询串
来源：http://blog.hesvh.cn/Article/details/gwfpkqani.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.share.fehbvm.com/Article/details/gdvxwyogc.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://blog.hesvh.cn/Article/details/gtcpingvl.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.zdbjq.cn/Article/details/gehlkyvbt.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.hesvh.cn/Article/details/gtekzdeyy.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wap.zdbjq.cn/Article/details/gjdivmyvz.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://mobile.zdbjq.cn/Article/details/gduahsvrl.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://blog.zdbjq.cn/Article/details/gjpatcfej.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://baike.fehbvm.com/Article/details/grhqybgon.sHtML

[K07] 进制转换
来源：http://m.share.fehbvm.com/Article/details/genbtutpb.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.blog.fehbvm.com/Article/details/gazcrfwoe.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mobile.zdbjq.cn/Article/details/ggersumnd.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.blog.hesvh.cn/Article/details/gujausaei.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://blog.zdbjq.cn/Article/details/godjdtbft.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.m.share.zdbjq.cn/Article/details/gyalxajhl.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://m.share.zdbjq.cn/Article/details/gibumkobq.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://read.share.zdbjq.cn/Article/details/gezfvvthj.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://blog.zdbjq.cn/Article/details/gbuppftnp.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.blog.zdbjq.cn/Article/details/gyobklljk.sHtML

Py:   pickle.dumps(obj)
来源：http://wap.hesvh.cn/Article/details/gbbfzdfhk.sHtML


<!-- 参考信息 -->