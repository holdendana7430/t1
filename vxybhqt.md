代发 wailian999

[H03] 主动抛出异常
来源：http://blog.hesvh.cn/Article/details/gnfscdmll.sHtML

Py:   raise ValueError("错误信息")
来源：http://read.share.hesvh.cn/Article/details/gugdvvjxm.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mobile.fehbvm.com/Article/details/grreifslb.sHtML

JS:   throw new Error("错误信息");
来源：http://www.m.share.zdbjq.cn/Article/details/guvvlsdfi.sHtML

TS:   throw new Error("错误信息");
来源：http://www.blog.fehbvm.com/Article/details/guicquygb.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.fehbvm.com/Article/details/gpfdpgsrc.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.m.share.fehbvm.com/Article/details/gggyxeuve.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://m.share.zdbjq.cn/Article/details/guuwzhkwn.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.m.share.fehbvm.com/Article/details/gbzraaypr.sHtML

[H04] 自定义异常类型
来源：http://m.share.zdbjq.cn/Article/details/gjerftxbt.sHtML

Py:   class MyError(Exception): pass
来源：http://3g.zdbjq.cn/Article/details/gbdjwtoth.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://blog.zdbjq.cn/Article/details/gzxcgxvqw.sHtML

JS:   class MyError extends Error {}
来源：http://mobile.fehbvm.com/Article/details/gzizeldan.sHtML

TS:   class MyError extends Error {}
来源：http://mobile.fehbvm.com/Article/details/grhtsyomv.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.blog.fehbvm.com/Article/details/gfokzaaho.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.share.fehbvm.com/Article/details/galzojlvy.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.share.zdbjq.cn/Article/details/grolvjzzj.sHtML

C#:   class MyException : Exception {}
来源：http://mobile.zdbjq.cn/Article/details/gdzzwclsv.sHtML

[H05] 捕获特定类型
来源：http://read.share.fehbvm.com/Article/details/gwjgxmvdt.sHtML

Py:   except ValueError as e:
来源：http://wap.hesvh.cn/Article/details/gsumtaclq.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://read.share.zdbjq.cn/Article/details/gnguifjqp.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://blog.zdbjq.cn/Article/details/gksqmbksg.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://wap.hesvh.cn/Article/details/gpjnlebqv.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://wap.zdbjq.cn/Article/details/goevzrvjp.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://read.share.zdbjq.cn/Article/details/gnllwwxjd.sHtML

Ruby: rescue ArgumentError => e
来源：http://blog.hesvh.cn/Article/details/gcntovgua.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wap.zdbjq.cn/Article/details/gxrzdgiqb.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.hesvh.cn/Article/details/gkhlohvla.sHtML

Py:   value = d.get("k") or default
来源：http://m.share.hesvh.cn/Article/details/gvdvshmhg.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://mobile.fehbvm.com/Article/details/ghvacxobb.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.hesvh.cn/Article/details/ggknypcfl.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://read.share.hesvh.cn/Article/details/gmfjnzlfl.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.share.hesvh.cn/Article/details/ghnledoyg.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.share.fehbvm.com/Article/details/gepzpjnqw.sHtML

Ruby: d&.dig(:a, :b)
来源：http://blog.fehbvm.com/Article/details/gdljomfll.sHtML

C#:   obj?.A?.B ?? default
来源：http://blog.fehbvm.com/Article/details/gorzgcqal.sHtML

[H07] 断言
来源：http://baike.fehbvm.com/Article/details/gflvjiyec.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.share.fehbvm.com/Article/details/gapdqxrxj.sHtML

PHP:  assert($x > 0);
来源：http://blog.fehbvm.com/Article/details/gxrbjlyxr.sHtML

JS:   console.assert(x > 0);
来源：http://mobile.zdbjq.cn/Article/details/gvtuycknd.sHtML

TS:   console.assert(x > 0);
来源：http://mobile.zdbjq.cn/Article/details/gdqhnszpc.sHtML

Java: assert x > 0 : "必须为正";
来源：http://wap.hesvh.cn/Article/details/gcxeoutsf.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.m.share.hesvh.cn/Article/details/gpxqfnegt.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://baike.zdbjq.cn/Article/details/gchvgjqbb.sHtML

C#:   Debug.Assert(x > 0);
来源：http://mobile.fehbvm.com/Article/details/gincnhrjd.sHtML

[H08] 获取错误信息与堆栈
来源：http://read.share.hesvh.cn/Article/details/gapzblngt.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.m.share.fehbvm.com/Article/details/gnunejixt.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.share.zdbjq.cn/Article/details/gilhzrysk.sHtML

JS:   e.message;  e.stack
来源：http://mobile.fehbvm.com/Article/details/ggmklguid.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://3g.zdbjq.cn/Article/details/gdvyvuvib.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.share.hesvh.cn/Article/details/gcfuzuxff.sHtML

Go:   err.Error()
来源：http://baike.hesvh.cn/Article/details/gqvnqqqko.sHtML

Ruby: e.message;  e.backtrace
来源：http://blog.hesvh.cn/Article/details/giipxcnux.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.share.zdbjq.cn/Article/details/gbgpoavgc.sHtML

[H09] 带错误码的异常
来源：http://mobile.fehbvm.com/Article/details/gxniyzfzr.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.share.zdbjq.cn/Article/details/gdzbbcvme.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.m.share.fehbvm.com/Article/details/gekkzyjak.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mobile.fehbvm.com/Article/details/gtpqtvosr.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://blog.hesvh.cn/Article/details/gsvqnycyw.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://blog.zdbjq.cn/Article/details/gqzttikbq.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://blog.hesvh.cn/Article/details/gpocdlmvs.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.m.share.fehbvm.com/Article/details/gxkcxwjct.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.m.share.zdbjq.cn/Article/details/gdzhizjzh.sHtML

[H10] 资源自动释放
来源：http://www.m.share.zdbjq.cn/Article/details/gymwkstgo.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://3g.zdbjq.cn/Article/details/gfrvicrhd.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.blog.hesvh.cn/Article/details/gfwckftgk.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.fehbvm.com/Article/details/gofradscp.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.zdbjq.cn/Article/details/ggzlzhyny.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://m.share.zdbjq.cn/Article/details/gwuvszdet.sHtML

Go:   defer f.Close()
来源：http://m.share.hesvh.cn/Article/details/gemklpzwh.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://3g.fehbvm.com/Article/details/gssqrslul.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gxuqxqxue.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gpuxbqoze.sHtML

I. 正则表达式
来源：http://blog.zdbjq.cn/Article/details/gejkwdjvj.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gvwhhxkni.sHtML

[I01] 判断是否匹配
来源：http://wap.hesvh.cn/Article/details/gxhjtdrwi.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://m.share.hesvh.cn/Article/details/gznoaimte.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://m.share.zdbjq.cn/Article/details/gdzeeilay.sHtML

JS:   /\d+/.test(s)
来源：http://read.share.zdbjq.cn/Article/details/ghnhjpkew.sHtML

TS:   /\d+/.test(s)
来源：http://3g.hesvh.cn/Article/details/gvcmupcrp.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://baike.zdbjq.cn/Article/details/gcqbgadjs.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mobile.fehbvm.com/Article/details/glaqhmqyv.sHtML

Ruby: s.match?(/\d+/)
来源：http://blog.zdbjq.cn/Article/details/gxhpsgads.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mobile.zdbjq.cn/Article/details/gezwpppxh.sHtML

[I02] 提取所有匹配
来源：http://baike.hesvh.cn/Article/details/gzlkmpnkd.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.blog.hesvh.cn/Article/details/gqictojqk.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.blog.fehbvm.com/Article/details/gcdbhkyrh.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wap.hesvh.cn/Article/details/goxygsujx.sHtML

TS:   s.match(/\d+/g)
来源：http://www.m.share.zdbjq.cn/Article/details/gfeqdqqcn.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gcptkosvi.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mobile.fehbvm.com/Article/details/gyfvsnpki.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.share.zdbjq.cn/Article/details/gslmsqfro.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mobile.hesvh.cn/Article/details/gpurpfwhn.sHtML

[I03] 提取捕获分组
来源：http://wap.zdbjq.cn/Article/details/gikcdsfii.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://blog.fehbvm.com/Article/details/gjlntwmzj.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wap.hesvh.cn/Article/details/ghbubrcav.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://read.share.hesvh.cn/Article/details/gtyxtglcq.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://3g.hesvh.cn/Article/details/gmppvuoht.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://read.share.fehbvm.com/Article/details/gmmakwqrx.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://read.share.hesvh.cn/Article/details/gfoxppmjt.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.share.fehbvm.com/Article/details/gvoyouozy.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.m.share.fehbvm.com/Article/details/gbadiegol.sHtML

[I04] 正则替换
来源：http://blog.fehbvm.com/Article/details/ghayzszqv.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.blog.hesvh.cn/Article/details/gmluvflud.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://blog.fehbvm.com/Article/details/gsoukgdii.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://baike.zdbjq.cn/Article/details/gfbsyfpyc.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://wap.fehbvm.com/Article/details/gebnmhczx.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.blog.hesvh.cn/Article/details/ghigonlte.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://read.share.zdbjq.cn/Article/details/godpuxdco.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://baike.zdbjq.cn/Article/details/goygadgji.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://3g.fehbvm.com/Article/details/guhioqssc.sHtML

[I05] 按正则拆分
来源：http://baike.fehbvm.com/Article/details/grihjrnmy.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.share.fehbvm.com/Article/details/gchjipdmp.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.blog.hesvh.cn/Article/details/gdyulswog.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://mobile.zdbjq.cn/Article/details/glgnhfper.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://mobile.hesvh.cn/Article/details/gbapwgrun.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.m.share.zdbjq.cn/Article/details/gpphozeqr.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.m.share.hesvh.cn/Article/details/gukqavyvw.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.share.zdbjq.cn/Article/details/grcgzkdok.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.share.hesvh.cn/Article/details/gfwsvfoew.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.blog.fehbvm.com/Article/details/gznovtfjm.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wap.fehbvm.com/Article/details/gwxiqlbxz.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://3g.zdbjq.cn/Article/details/gogtpzjpq.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.fehbvm.com/Article/details/gejffuoms.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.zdbjq.cn/Article/details/gxiyppqqh.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://baike.zdbjq.cn/Article/details/gocwlpetw.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://m.share.hesvh.cn/Article/details/gvmnrjkwa.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.blog.fehbvm.com/Article/details/gdgwbgwgi.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://read.share.zdbjq.cn/Article/details/gavpxchoi.sHtML

[I07] 忽略大小写与多行模式
来源：http://read.share.zdbjq.cn/Article/details/gfdjyustu.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wap.fehbvm.com/Article/details/guzbqrrhm.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://blog.hesvh.cn/Article/details/gjmzzkjtp.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.share.fehbvm.com/Article/details/gzoillmjd.sHtML

TS:   /error/gim
来源：http://3g.fehbvm.com/Article/details/gjezucupd.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://3g.fehbvm.com/Article/details/gdtedzapv.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.share.hesvh.cn/Article/details/goastlwlh.sHtML

Ruby: s.scan(/error/i)
来源：http://blog.hesvh.cn/Article/details/gaersikhk.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://baike.fehbvm.com/Article/details/gxwljoodw.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://3g.fehbvm.com/Article/details/geaqgnwid.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://baike.fehbvm.com/Article/details/gdnebrosg.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.m.share.zdbjq.cn/Article/details/gqauopwfa.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.fehbvm.com/Article/details/gbxwpqllq.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.fehbvm.com/Article/details/gobtxmtca.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://wap.hesvh.cn/Article/details/ggxpljsnz.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://blog.fehbvm.com/Article/details/gpttmners.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.blog.fehbvm.com/Article/details/gnzvymmzo.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://blog.zdbjq.cn/Article/details/gssmzibft.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gipfbkhah.sHtML

J. 日期与时间
来源：http://3g.fehbvm.com/Article/details/gxubuxflr.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/ggwazijva.sHtML

[J01] 获取当前时间
来源：http://www.share.fehbvm.com/Article/details/gbihfvxoc.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://baike.hesvh.cn/Article/details/gurrytzlc.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://baike.hesvh.cn/Article/details/gxzelegxb.sHtML

JS:   new Date();  Date.now()
来源：http://read.share.zdbjq.cn/Article/details/goqsnskwo.sHtML

TS:   new Date();  Date.now()
来源：http://wap.zdbjq.cn/Article/details/gzgqktjdy.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://m.share.zdbjq.cn/Article/details/gjumxcjmo.sHtML

Go:   time.Now()
来源：http://blog.fehbvm.com/Article/details/gnudqhoow.sHtML

Ruby: Time.now
来源：http://mobile.fehbvm.com/Article/details/gmpcorsiv.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://mobile.fehbvm.com/Article/details/ghcrlhyrk.sHtML

[J02] 格式化输出
来源：http://m.share.zdbjq.cn/Article/details/gnnwgkygb.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.hesvh.cn/Article/details/gbusdqtcc.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wap.hesvh.cn/Article/details/gvmjimjdr.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.m.share.hesvh.cn/Article/details/gquplgjhq.sHtML

TS:   d.toISOString()
来源：http://3g.hesvh.cn/Article/details/gqcybhgrb.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.m.share.fehbvm.com/Article/details/gbmtrdlyv.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://blog.hesvh.cn/Article/details/gyynydpoi.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.fehbvm.com/Article/details/gyebedzcp.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://3g.zdbjq.cn/Article/details/gpyiiuluq.sHtML

[J03] 字符串解析为日期
来源：http://www.blog.fehbvm.com/Article/details/gpvzvmavt.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://3g.fehbvm.com/Article/details/gsfzhoooh.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://3g.fehbvm.com/Article/details/gzairpxyg.sHtML

JS:   new Date("2024-01-02")
来源：http://blog.zdbjq.cn/Article/details/gdyhsmtcd.sHtML

TS:   new Date("2024-01-02")
来源：http://blog.zdbjq.cn/Article/details/gyyynlqna.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://blog.fehbvm.com/Article/details/gajdinzgx.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://read.share.fehbvm.com/Article/details/gfsyvxueh.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://wap.zdbjq.cn/Article/details/gkeqzipll.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://read.share.fehbvm.com/Article/details/gcreqgrcz.sHtML

[J04] 时间戳与日期互转
来源：http://read.share.zdbjq.cn/Article/details/gldzkedmr.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.share.hesvh.cn/Article/details/gntlirruz.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wap.hesvh.cn/Article/details/gprmhvzkd.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://baike.fehbvm.com/Article/details/gksvxojuy.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://3g.fehbvm.com/Article/details/giheqjmlw.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.share.hesvh.cn/Article/details/ggvkjjufj.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://read.share.zdbjq.cn/Article/details/gsvvcxwjp.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://blog.fehbvm.com/Article/details/gmgulxtrg.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://m.share.fehbvm.com/Article/details/ghccyjjji.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.share.zdbjq.cn/Article/details/gtkicfjrw.sHtML

Py:   now + timedelta(days=7)
来源：http://3g.fehbvm.com/Article/details/grhfrkxft.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://m.share.hesvh.cn/Article/details/gwlbisftf.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.fehbvm.com/Article/details/gchnhjsih.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.hesvh.cn/Article/details/gujpzbpvs.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://3g.hesvh.cn/Article/details/gicdezttl.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://m.share.fehbvm.com/Article/details/guukcityo.sHtML

Ruby: Time.now + 7 * 86400
来源：http://3g.hesvh.cn/Article/details/gsxoirujl.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.m.share.hesvh.cn/Article/details/gkyshfzcs.sHtML

[J06] 计算两时间之差
来源：http://baike.zdbjq.cn/Article/details/gkjlkmomd.sHtML

Py:   (end - start).total_seconds()
来源：http://www.blog.zdbjq.cn/Article/details/gmouoytko.sHtML

PHP:  $end->diff($start)->days;
来源：http://m.share.zdbjq.cn/Article/details/gqejbugwr.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.m.share.hesvh.cn/Article/details/gqlcnahbm.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://read.share.zdbjq.cn/Article/details/glhxausjq.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.share.hesvh.cn/Article/details/gfrnhfnyn.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.m.share.hesvh.cn/Article/details/gydbpxkls.sHtML

Ruby: end - start                 # 返回秒数
来源：http://wap.fehbvm.com/Article/details/gckqpjlcr.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.blog.hesvh.cn/Article/details/gwpekplfa.sHtML

[J07] 比较两个日期
来源：http://m.share.fehbvm.com/Article/details/gikgbmcro.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://m.share.zdbjq.cn/Article/details/gyqiseatq.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://read.share.fehbvm.com/Article/details/gwssphhas.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://mobile.hesvh.cn/Article/details/gppcbtfbq.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://read.share.zdbjq.cn/Article/details/gfcbbfbhy.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://read.share.zdbjq.cn/Article/details/gsjlasvqn.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://blog.hesvh.cn/Article/details/gudusxtwe.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.blog.hesvh.cn/Article/details/gxoxnkxbx.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.share.zdbjq.cn/Article/details/gwnexlhyr.sHtML

[J08] 提取年月日与星期
来源：http://m.share.hesvh.cn/Article/details/galmcsong.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://m.share.fehbvm.com/Article/details/gvcljdoxl.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://m.share.zdbjq.cn/Article/details/gfpnednqi.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wap.zdbjq.cn/Article/details/gzxkgbmuz.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://3g.zdbjq.cn/Article/details/gmgoecfpb.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wap.hesvh.cn/Article/details/gglsuoful.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.share.hesvh.cn/Article/details/ghnjtizdv.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://3g.fehbvm.com/Article/details/gcyqwnivg.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.blog.zdbjq.cn/Article/details/ggcpwabcx.sHtML

[J09] 时区处理
来源：http://read.share.fehbvm.com/Article/details/galrnmiyd.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wap.zdbjq.cn/Article/details/gfhpygbin.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://3g.zdbjq.cn/Article/details/gorjgfnox.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.hesvh.cn/Article/details/gpodxfnjx.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.zdbjq.cn/Article/details/gnywjywlm.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mobile.fehbvm.com/Article/details/gtoehnsza.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://read.share.zdbjq.cn/Article/details/geemdgbkp.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://blog.fehbvm.com/Article/details/gtlszzslu.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://m.share.fehbvm.com/Article/details/gshfuzyzx.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.blog.fehbvm.com/Article/details/gzzudfndi.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.m.share.hesvh.cn/Article/details/gdbzbytph.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mobile.hesvh.cn/Article/details/gzvhhzymd.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mobile.zdbjq.cn/Article/details/gtyrkiwvk.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://blog.fehbvm.com/Article/details/gftyqgpeu.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://blog.fehbvm.com/Article/details/gosxsqcrg.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.blog.fehbvm.com/Article/details/ghalxewyi.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://m.share.fehbvm.com/Article/details/ghrbtbnlt.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://m.share.zdbjq.cn/Article/details/gfsmdxswn.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gidwxmgur.sHtML

K. JSON 与序列化
来源：http://read.share.fehbvm.com/Article/details/grclolvwz.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/golmnctvk.sHtML

[K01] 对象转 JSON 字符串
来源：http://baike.fehbvm.com/Article/details/gtjkmswnu.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.blog.zdbjq.cn/Article/details/gthpqhcgv.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://blog.hesvh.cn/Article/details/ghqtyqglo.sHtML

JS:   JSON.stringify(obj)
来源：http://3g.fehbvm.com/Article/details/ggwlxpirv.sHtML

TS:   JSON.stringify(obj)
来源：http://baike.zdbjq.cn/Article/details/gcdkmvvln.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.m.share.fehbvm.com/Article/details/ghttsfrtg.sHtML

Go:   json.Marshal(obj)
来源：http://mobile.fehbvm.com/Article/details/gadcwhtpq.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://m.share.hesvh.cn/Article/details/guuhnkkct.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://blog.fehbvm.com/Article/details/gpipiobbw.sHtML

[K02] JSON 字符串转对象
来源：http://m.share.hesvh.cn/Article/details/gtphbufdo.sHtML

Py:   json.loads(s)
来源：http://www.m.share.fehbvm.com/Article/details/gvjccikha.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://blog.hesvh.cn/Article/details/ghsknfkqi.sHtML

JS:   JSON.parse(s)
来源：http://3g.fehbvm.com/Article/details/gbdinkftm.sHtML

TS:   JSON.parse(s)
来源：http://baike.fehbvm.com/Article/details/gkjlnhzgg.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://m.share.zdbjq.cn/Article/details/gbueacflz.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://blog.zdbjq.cn/Article/details/gpydddxsi.sHtML

Ruby: JSON.parse(s)
来源：http://mobile.hesvh.cn/Article/details/gqpakdyfd.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wap.zdbjq.cn/Article/details/gcgqzqsio.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://m.share.hesvh.cn/Article/details/gqsqncfwv.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.share.fehbvm.com/Article/details/gymuqpbnf.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.hesvh.cn/Article/details/gflczrsry.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://3g.hesvh.cn/Article/details/gucgzvxje.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://baike.zdbjq.cn/Article/details/gyxrzciza.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://read.share.hesvh.cn/Article/details/gbcqklvbq.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://3g.zdbjq.cn/Article/details/ggcbgtbpx.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.share.hesvh.cn/Article/details/gqpxpjtbx.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://m.share.fehbvm.com/Article/details/gniixcnle.sHtML

[K04] 读取 JSON 文件
来源：http://mobile.hesvh.cn/Article/details/gdheaioxz.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.share.fehbvm.com/Article/details/grgkwlobw.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.share.hesvh.cn/Article/details/gokjgrkai.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.fehbvm.com/Article/details/gbofymkvp.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.fehbvm.com/Article/details/gzwwutpzz.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.m.share.hesvh.cn/Article/details/gqrfxebdh.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wap.zdbjq.cn/Article/details/gipmwinrd.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://read.share.zdbjq.cn/Article/details/gdxvopetr.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.share.fehbvm.com/Article/details/grgaryteq.sHtML

[K05] 深拷贝对象
来源：http://baike.fehbvm.com/Article/details/gquuubheb.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.share.hesvh.cn/Article/details/gabqfwxia.sHtML

PHP:  unserialize(serialize($obj));
来源：http://m.share.fehbvm.com/Article/details/gcdzkqkip.sHtML

JS:   structuredClone(obj)
来源：http://blog.hesvh.cn/Article/details/gxjkugzlo.sHtML

TS:   structuredClone(obj)
来源：http://blog.zdbjq.cn/Article/details/gnrabunxh.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://baike.zdbjq.cn/Article/details/gvxlusfbc.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://read.share.fehbvm.com/Article/details/gdqrjgqju.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.blog.zdbjq.cn/Article/details/gpfpdrogt.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://3g.fehbvm.com/Article/details/gnbfolkxq.sHtML

[K06] 解析 URL 查询串
来源：http://www.m.share.hesvh.cn/Article/details/gmmsimbsm.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://blog.fehbvm.com/Article/details/guqaiaivz.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://m.share.fehbvm.com/Article/details/gloadenll.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.fehbvm.com/Article/details/ghzfcsvnl.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.hesvh.cn/Article/details/gdukkzxfa.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://3g.fehbvm.com/Article/details/gplgqgjin.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://baike.hesvh.cn/Article/details/glhzshvfh.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wap.zdbjq.cn/Article/details/gomduhibi.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://m.share.hesvh.cn/Article/details/gwxgexmtc.sHtML

[K07] 进制转换
来源：http://wap.zdbjq.cn/Article/details/gldosyfcx.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.m.share.zdbjq.cn/Article/details/grjjgzrje.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://read.share.zdbjq.cn/Article/details/gbodlzsaj.sHtML


<!-- 参考信息 -->