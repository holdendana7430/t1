代发 wailian999

Ruby: class MyError < StandardError; end
来源：http://www.blog.fehbvm.com/Article/details/gbidcwplz.sHtML

C#:   class MyException : Exception {}
来源：http://www.share.fehbvm.com/Article/details/gmegdkpft.sHtML

[H05] 捕获特定类型
来源：http://baike.hesvh.cn/Article/details/gcathparb.sHtML

Py:   except ValueError as e:
来源：http://m.share.hesvh.cn/Article/details/grgnpucur.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.fehbvm.com/Article/details/gbjynnhml.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.blog.fehbvm.com/Article/details/gzfjmvmbh.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://baike.fehbvm.com/Article/details/gjsjrcmyv.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://3g.fehbvm.com/Article/details/gicyabcdb.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.m.share.hesvh.cn/Article/details/gowlqmihq.sHtML

Ruby: rescue ArgumentError => e
来源：http://wap.hesvh.cn/Article/details/guxhzhyzq.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://blog.fehbvm.com/Article/details/gmemrlcpi.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.m.share.zdbjq.cn/Article/details/gzkoojnnn.sHtML

Py:   value = d.get("k") or default
来源：http://3g.fehbvm.com/Article/details/gunfnkicp.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.share.fehbvm.com/Article/details/gdvdvaxzv.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.blog.fehbvm.com/Article/details/grcearxfj.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.share.fehbvm.com/Article/details/gggflebza.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://baike.zdbjq.cn/Article/details/galzhmgum.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://blog.zdbjq.cn/Article/details/gqquayynj.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.blog.zdbjq.cn/Article/details/gynjzlpuk.sHtML

C#:   obj?.A?.B ?? default
来源：http://baike.zdbjq.cn/Article/details/gnuiyatgg.sHtML

[H07] 断言
来源：http://m.share.zdbjq.cn/Article/details/gtasybcjf.sHtML

Py:   assert x > 0, "必须为正"
来源：http://read.share.fehbvm.com/Article/details/gdfrxfuho.sHtML

PHP:  assert($x > 0);
来源：http://blog.fehbvm.com/Article/details/gmrcgamuc.sHtML

JS:   console.assert(x > 0);
来源：http://www.m.share.zdbjq.cn/Article/details/govoymtiz.sHtML

TS:   console.assert(x > 0);
来源：http://m.share.fehbvm.com/Article/details/gleozfpyb.sHtML

Java: assert x > 0 : "必须为正";
来源：http://mobile.hesvh.cn/Article/details/gsqjxtlur.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.share.fehbvm.com/Article/details/ghritnhid.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.share.zdbjq.cn/Article/details/gfdlrmodz.sHtML

C#:   Debug.Assert(x > 0);
来源：http://blog.fehbvm.com/Article/details/gwqqnnfpe.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.blog.fehbvm.com/Article/details/gaayufklq.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.m.share.hesvh.cn/Article/details/gnsjornaz.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.m.share.fehbvm.com/Article/details/gwvvtwlkr.sHtML

JS:   e.message;  e.stack
来源：http://www.blog.hesvh.cn/Article/details/gkachjvhq.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://blog.hesvh.cn/Article/details/gnamkbwpe.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://blog.hesvh.cn/Article/details/gldeuvqbv.sHtML

Go:   err.Error()
来源：http://blog.hesvh.cn/Article/details/gaakwmfeb.sHtML

Ruby: e.message;  e.backtrace
来源：http://blog.hesvh.cn/Article/details/goisgfvxs.sHtML

C#:   e.Message;  e.StackTrace
来源：http://blog.hesvh.cn/Article/details/gnsohsvhy.sHtML

[H09] 带错误码的异常
来源：http://mobile.zdbjq.cn/Article/details/gswwzensn.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.blog.fehbvm.com/Article/details/gunandkwi.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.blog.fehbvm.com/Article/details/gvjtvrtyo.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://read.share.fehbvm.com/Article/details/gokrcgkda.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mobile.fehbvm.com/Article/details/gxeadwyvz.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://baike.fehbvm.com/Article/details/gblimdpcs.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://3g.fehbvm.com/Article/details/gqfkzqrod.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://m.share.hesvh.cn/Article/details/gqeyouocw.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://3g.fehbvm.com/Article/details/givbongrd.sHtML

[H10] 资源自动释放
来源：http://read.share.fehbvm.com/Article/details/glacdison.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.m.share.zdbjq.cn/Article/details/giffjaplt.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.m.share.hesvh.cn/Article/details/gmzgsvpet.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.fehbvm.com/Article/details/gydehvbzx.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.hesvh.cn/Article/details/gfcyaifyc.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.share.hesvh.cn/Article/details/gxtctlgiw.sHtML

Go:   defer f.Close()
来源：http://www.blog.zdbjq.cn/Article/details/givsagbcl.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://blog.hesvh.cn/Article/details/gwfooycmz.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gpsdqazxh.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/goazrndvi.sHtML

I. 正则表达式
来源：http://www.blog.fehbvm.com/Article/details/gktqyacmk.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gcmzpciwp.sHtML

[I01] 判断是否匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gpxyoifnc.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.m.share.zdbjq.cn/Article/details/ggzrsgqyv.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.blog.hesvh.cn/Article/details/gccxxhthk.sHtML

JS:   /\d+/.test(s)
来源：http://m.share.hesvh.cn/Article/details/gkhkhhiax.sHtML

TS:   /\d+/.test(s)
来源：http://www.share.zdbjq.cn/Article/details/ghdqssnyx.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://baike.zdbjq.cn/Article/details/gmuwufanm.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mobile.zdbjq.cn/Article/details/gxlkcjogj.sHtML

Ruby: s.match?(/\d+/)
来源：http://read.share.hesvh.cn/Article/details/ggotppnbh.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://m.share.fehbvm.com/Article/details/gaxlijtim.sHtML

[I02] 提取所有匹配
来源：http://baike.fehbvm.com/Article/details/gpwofuntl.sHtML

Py:   re.findall(r"\d+", s)
来源：http://m.share.fehbvm.com/Article/details/ghnxbpisw.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wap.fehbvm.com/Article/details/gmtrpbdsq.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://read.share.fehbvm.com/Article/details/genlmguwq.sHtML

TS:   s.match(/\d+/g)
来源：http://baike.zdbjq.cn/Article/details/gdfmmbnhn.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://baike.zdbjq.cn/Article/details/gqojoffrt.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://read.share.fehbvm.com/Article/details/gbafidtan.sHtML

Ruby: s.scan(/\d+/)
来源：http://blog.fehbvm.com/Article/details/gyhmkzhew.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.share.zdbjq.cn/Article/details/gjhbyuuqf.sHtML

[I03] 提取捕获分组
来源：http://www.m.share.fehbvm.com/Article/details/gpapvjvvz.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://blog.fehbvm.com/Article/details/ggcimzxvx.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://m.share.hesvh.cn/Article/details/gcovdusji.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mobile.fehbvm.com/Article/details/gnpplsizl.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mobile.zdbjq.cn/Article/details/grmfhvvvv.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wap.fehbvm.com/Article/details/gpppbobzb.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.blog.fehbvm.com/Article/details/gixqimgza.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mobile.hesvh.cn/Article/details/gqikpgwnw.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.share.hesvh.cn/Article/details/gmvigsgmi.sHtML

[I04] 正则替换
来源：http://3g.fehbvm.com/Article/details/gksbmvzoh.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://baike.zdbjq.cn/Article/details/gfxkevxof.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.share.zdbjq.cn/Article/details/gpjkxmjhf.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://mobile.fehbvm.com/Article/details/grvwydtzi.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.blog.hesvh.cn/Article/details/gnaarlvvk.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.m.share.zdbjq.cn/Article/details/gvpmoueib.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.blog.hesvh.cn/Article/details/gbtewvdnu.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://baike.zdbjq.cn/Article/details/ghboppuqp.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://blog.zdbjq.cn/Article/details/gnjcivyaf.sHtML

[I05] 按正则拆分
来源：http://3g.fehbvm.com/Article/details/gbeptwapi.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://blog.fehbvm.com/Article/details/gdmvbetzm.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.blog.fehbvm.com/Article/details/gsxlkdlkb.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.m.share.fehbvm.com/Article/details/gucjrhvtz.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://3g.fehbvm.com/Article/details/grmogwsri.sHtML

Java: s.split("\\s*,\\s*")
来源：http://mobile.hesvh.cn/Article/details/gbvbjmkqe.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://read.share.zdbjq.cn/Article/details/gzucjefmt.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.share.hesvh.cn/Article/details/gtwijyfhp.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://read.share.fehbvm.com/Article/details/gmmyzttqd.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mobile.hesvh.cn/Article/details/gizzcpsgt.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.blog.hesvh.cn/Article/details/gpoaojbhj.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://m.share.zdbjq.cn/Article/details/gwuifytcj.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.fehbvm.com/Article/details/gftmbbrvj.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.fehbvm.com/Article/details/gnoennzwa.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://3g.zdbjq.cn/Article/details/gslqkokfw.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://baike.fehbvm.com/Article/details/gqtbmjkpf.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.share.hesvh.cn/Article/details/gtbxzivel.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.share.hesvh.cn/Article/details/gsqpjejna.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.blog.fehbvm.com/Article/details/gmmgxpnlc.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://baike.zdbjq.cn/Article/details/gcemtseyt.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.share.hesvh.cn/Article/details/gfasvmvdp.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://blog.zdbjq.cn/Article/details/gsrcqguyp.sHtML

TS:   /error/gim
来源：http://mobile.hesvh.cn/Article/details/gcytbfqfc.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mobile.hesvh.cn/Article/details/gdfjzzlnw.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.m.share.zdbjq.cn/Article/details/gbmmqtpjs.sHtML

Ruby: s.scan(/error/i)
来源：http://www.blog.zdbjq.cn/Article/details/giwzihuch.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mobile.fehbvm.com/Article/details/guzegsxeq.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://read.share.zdbjq.cn/Article/details/glyovzryq.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.share.zdbjq.cn/Article/details/gwjvhmwzh.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.m.share.zdbjq.cn/Article/details/grwlywlal.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.fehbvm.com/Article/details/gouwgonbj.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.hesvh.cn/Article/details/gxrkkuosp.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.share.zdbjq.cn/Article/details/gtczylozn.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://read.share.hesvh.cn/Article/details/gtichylif.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mobile.hesvh.cn/Article/details/gdgakaore.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.blog.hesvh.cn/Article/details/ghwwkhaft.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/givukzdmf.sHtML

J. 日期与时间
来源：http://m.share.fehbvm.com/Article/details/giorvximx.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gsvoemtyh.sHtML

[J01] 获取当前时间
来源：http://m.share.fehbvm.com/Article/details/gybjiurkm.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://mobile.hesvh.cn/Article/details/giwrjpupo.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://blog.hesvh.cn/Article/details/gfjgdygcv.sHtML

JS:   new Date();  Date.now()
来源：http://www.blog.hesvh.cn/Article/details/gqgpnlezr.sHtML

TS:   new Date();  Date.now()
来源：http://www.blog.hesvh.cn/Article/details/gfmqvfacx.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.share.hesvh.cn/Article/details/gbderjaes.sHtML

Go:   time.Now()
来源：http://read.share.fehbvm.com/Article/details/gkaafixtk.sHtML

Ruby: Time.now
来源：http://www.m.share.fehbvm.com/Article/details/glqtnuxhn.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://m.share.fehbvm.com/Article/details/gjcxkrdrt.sHtML

[J02] 格式化输出
来源：http://www.share.hesvh.cn/Article/details/gthstwhat.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.zdbjq.cn/Article/details/gelimzbrq.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.share.zdbjq.cn/Article/details/guoaqhuhw.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.blog.zdbjq.cn/Article/details/gduigebze.sHtML

TS:   d.toISOString()
来源：http://mobile.fehbvm.com/Article/details/gydnhgprh.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://read.share.zdbjq.cn/Article/details/gcovumsvq.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.blog.hesvh.cn/Article/details/gmdbentdp.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.hesvh.cn/Article/details/glqdrmuep.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://mobile.zdbjq.cn/Article/details/gbcqjdsex.sHtML

[J03] 字符串解析为日期
来源：http://baike.fehbvm.com/Article/details/gyuyadrcr.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.share.zdbjq.cn/Article/details/gymyhamls.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://blog.zdbjq.cn/Article/details/gdnreabdv.sHtML

JS:   new Date("2024-01-02")
来源：http://baike.zdbjq.cn/Article/details/ghgwkehed.sHtML

TS:   new Date("2024-01-02")
来源：http://read.share.hesvh.cn/Article/details/gypidkhut.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.m.share.fehbvm.com/Article/details/gwxdpgkfw.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wap.zdbjq.cn/Article/details/guyilqoqd.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://read.share.fehbvm.com/Article/details/gxrmyceph.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://baike.hesvh.cn/Article/details/gndrljxhf.sHtML

[J04] 时间戳与日期互转
来源：http://www.share.hesvh.cn/Article/details/goezyxkxf.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mobile.hesvh.cn/Article/details/gtmebuudo.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.m.share.hesvh.cn/Article/details/gvqxfkqzu.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://m.share.fehbvm.com/Article/details/gadmjiwkn.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://read.share.hesvh.cn/Article/details/gdftpxskq.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://baike.zdbjq.cn/Article/details/gtqctblld.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.m.share.fehbvm.com/Article/details/ggyyqiwei.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://baike.fehbvm.com/Article/details/gnpemgpjd.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.m.share.fehbvm.com/Article/details/gdjokhbnd.sHtML

[J05] 时间加减（加 7 天）
来源：http://m.share.fehbvm.com/Article/details/gcwoqhsse.sHtML

Py:   now + timedelta(days=7)
来源：http://read.share.fehbvm.com/Article/details/gagirhrjw.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.share.fehbvm.com/Article/details/gklfjsdfv.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.zdbjq.cn/Article/details/gnhlkjamv.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.zdbjq.cn/Article/details/gnpqcvpum.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://wap.zdbjq.cn/Article/details/gjvxixkav.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://read.share.hesvh.cn/Article/details/gyfhogkek.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.blog.zdbjq.cn/Article/details/gqqvdimau.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.blog.hesvh.cn/Article/details/gynwxzpgy.sHtML

[J06] 计算两时间之差
来源：http://mobile.hesvh.cn/Article/details/gqiduwoep.sHtML

Py:   (end - start).total_seconds()
来源：http://www.blog.fehbvm.com/Article/details/gwongexkp.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.blog.hesvh.cn/Article/details/gqvpmmahm.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://3g.hesvh.cn/Article/details/gqczlyiaw.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.share.hesvh.cn/Article/details/gkzkljzbu.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://mobile.hesvh.cn/Article/details/gzrwwbcmx.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.share.fehbvm.com/Article/details/gbtdlhrht.sHtML

Ruby: end - start                 # 返回秒数
来源：http://read.share.fehbvm.com/Article/details/grmmclaqa.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.share.zdbjq.cn/Article/details/gecxexbon.sHtML

[J07] 比较两个日期
来源：http://www.share.hesvh.cn/Article/details/gnfrsvsqu.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.share.zdbjq.cn/Article/details/govikjqim.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.blog.hesvh.cn/Article/details/gztgrwhgt.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.blog.zdbjq.cn/Article/details/gebgqotnu.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.hesvh.cn/Article/details/gcplzycpb.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wap.zdbjq.cn/Article/details/gbzcebrdl.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://3g.zdbjq.cn/Article/details/gmskjjdzl.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.blog.zdbjq.cn/Article/details/gdrdvasok.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://read.share.fehbvm.com/Article/details/glubybiue.sHtML

[J08] 提取年月日与星期
来源：http://mobile.zdbjq.cn/Article/details/giardqmtu.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://m.share.fehbvm.com/Article/details/gpqyhbfxa.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://read.share.fehbvm.com/Article/details/gfnpkxtuk.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mobile.fehbvm.com/Article/details/gesebbxmx.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://blog.hesvh.cn/Article/details/gekwwwdat.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://baike.hesvh.cn/Article/details/gxdolvrki.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wap.fehbvm.com/Article/details/gxmfmftad.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://blog.hesvh.cn/Article/details/gxbvxhpeg.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://baike.hesvh.cn/Article/details/gdyglfhmh.sHtML

[J09] 时区处理
来源：http://www.share.hesvh.cn/Article/details/gwmbybhwm.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.share.hesvh.cn/Article/details/grxctekxm.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://mobile.hesvh.cn/Article/details/gfzahmktz.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.fehbvm.com/Article/details/gutagdigz.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.hesvh.cn/Article/details/govqabxtj.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://blog.hesvh.cn/Article/details/gcjwlotvf.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://3g.fehbvm.com/Article/details/gcyjsmjxg.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.m.share.fehbvm.com/Article/details/gzxkhsngc.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.share.fehbvm.com/Article/details/gwtkgdhkm.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.blog.fehbvm.com/Article/details/gaceiqmeu.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://blog.zdbjq.cn/Article/details/ghzhjbaux.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wap.fehbvm.com/Article/details/gqffjugka.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wap.zdbjq.cn/Article/details/gyczohapv.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://baike.fehbvm.com/Article/details/gxkicgjei.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wap.zdbjq.cn/Article/details/gbukpzfqk.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.blog.zdbjq.cn/Article/details/gykujbmeg.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wap.zdbjq.cn/Article/details/gozfvtuss.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.blog.hesvh.cn/Article/details/gztlhhldn.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/glnfogshh.sHtML

K. JSON 与序列化
来源：http://www.blog.fehbvm.com/Article/details/gejrygdyo.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gmlbqsgsx.sHtML

[K01] 对象转 JSON 字符串
来源：http://wap.hesvh.cn/Article/details/gbrgrisxq.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.m.share.fehbvm.com/Article/details/gxvgunldd.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.share.fehbvm.com/Article/details/givfgvfiw.sHtML

JS:   JSON.stringify(obj)
来源：http://blog.hesvh.cn/Article/details/gbtkzgezw.sHtML

TS:   JSON.stringify(obj)
来源：http://baike.zdbjq.cn/Article/details/goafrlqvo.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wap.zdbjq.cn/Article/details/gymqmuzaj.sHtML

Go:   json.Marshal(obj)
来源：http://wap.zdbjq.cn/Article/details/guzrtrbgf.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://m.share.hesvh.cn/Article/details/gutrpagdp.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.share.hesvh.cn/Article/details/gavsdgoaw.sHtML

[K02] JSON 字符串转对象
来源：http://m.share.zdbjq.cn/Article/details/gdkycibap.sHtML

Py:   json.loads(s)
来源：http://www.blog.hesvh.cn/Article/details/gzccadxmt.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://3g.fehbvm.com/Article/details/ghvgkxuaj.sHtML

JS:   JSON.parse(s)
来源：http://m.share.fehbvm.com/Article/details/gdmrwgcva.sHtML

TS:   JSON.parse(s)
来源：http://m.share.hesvh.cn/Article/details/ghmrxbwoy.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wap.hesvh.cn/Article/details/gjvpetvoe.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.share.zdbjq.cn/Article/details/gmqbbxeqd.sHtML

Ruby: JSON.parse(s)
来源：http://mobile.fehbvm.com/Article/details/gxqjetbje.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://baike.hesvh.cn/Article/details/gxmafyoky.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.m.share.zdbjq.cn/Article/details/gxhdxkxyg.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://3g.zdbjq.cn/Article/details/gruqdvoxf.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://baike.hesvh.cn/Article/details/geqwgebzd.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.hesvh.cn/Article/details/gjttnqrfl.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://baike.fehbvm.com/Article/details/gzjtpzfkj.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://baike.fehbvm.com/Article/details/grlzpqmwe.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mobile.fehbvm.com/Article/details/grsdjuwax.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://mobile.fehbvm.com/Article/details/gfvcspakb.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mobile.hesvh.cn/Article/details/gcrmeshev.sHtML

[K04] 读取 JSON 文件
来源：http://3g.hesvh.cn/Article/details/gxzitdgxz.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://baike.zdbjq.cn/Article/details/grdpgufhr.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://m.share.hesvh.cn/Article/details/gwxbuhtcl.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.fehbvm.com/Article/details/glxjlifyr.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.fehbvm.com/Article/details/gmkqtzpzm.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://blog.zdbjq.cn/Article/details/gkoshpsss.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.blog.zdbjq.cn/Article/details/gqlznhgmu.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.share.zdbjq.cn/Article/details/grtpgbhpr.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://3g.zdbjq.cn/Article/details/gpakawlaj.sHtML

[K05] 深拷贝对象
来源：http://mobile.hesvh.cn/Article/details/gyvbjczfq.sHtML

Py:   copy.deepcopy(obj)
来源：http://wap.fehbvm.com/Article/details/gerjymuhz.sHtML

PHP:  unserialize(serialize($obj));
来源：http://blog.fehbvm.com/Article/details/gpmkdxslm.sHtML

JS:   structuredClone(obj)
来源：http://baike.zdbjq.cn/Article/details/gjgevswbr.sHtML

TS:   structuredClone(obj)
来源：http://wap.zdbjq.cn/Article/details/gzagfvwmh.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.m.share.hesvh.cn/Article/details/gcrsjrtwg.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://blog.fehbvm.com/Article/details/gmtsxmmdw.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://m.share.zdbjq.cn/Article/details/gnmkrmyfi.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://3g.fehbvm.com/Article/details/gijnwgnuh.sHtML

[K06] 解析 URL 查询串
来源：http://3g.zdbjq.cn/Article/details/gpxztzgae.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://baike.fehbvm.com/Article/details/gfuychdxw.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.blog.hesvh.cn/Article/details/gmipxmten.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.zdbjq.cn/Article/details/gshviffyo.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.fehbvm.com/Article/details/gqyrdjhni.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.share.hesvh.cn/Article/details/guuuoqjxp.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.share.zdbjq.cn/Article/details/getwthwmj.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wap.hesvh.cn/Article/details/gcfbdhddv.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://m.share.fehbvm.com/Article/details/gxyqelunm.sHtML

[K07] 进制转换
来源：http://read.share.fehbvm.com/Article/details/gqrffwvrk.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://baike.hesvh.cn/Article/details/gmppgywkk.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://read.share.fehbvm.com/Article/details/ggbptssxi.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://m.share.hesvh.cn/Article/details/gxaovwgju.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://blog.hesvh.cn/Article/details/gkcrdvkay.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wap.hesvh.cn/Article/details/grfqzfvok.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://blog.fehbvm.com/Article/details/gvvmzohke.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.blog.fehbvm.com/Article/details/gsprbajha.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mobile.zdbjq.cn/Article/details/ghdcpateo.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://blog.hesvh.cn/Article/details/gbfkoqumu.sHtML

Py:   pickle.dumps(obj)
来源：http://read.share.fehbvm.com/Article/details/gmucmshzc.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://m.share.zdbjq.cn/Article/details/gyhbavpcx.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://m.share.hesvh.cn/Article/details/gxoztyjdx.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://wap.fehbvm.com/Article/details/ggbobfxrh.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://baike.fehbvm.com/Article/details/gsdpbatfm.sHtML

Go:   encoding/gob
来源：http://m.share.zdbjq.cn/Article/details/gezeqtqld.sHtML

Ruby: Marshal.dump(obj)
来源：http://blog.fehbvm.com/Article/details/gqyeewbum.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.m.share.fehbvm.com/Article/details/gauuiocgb.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/grjfndgvf.sHtML


<!-- 参考信息 -->