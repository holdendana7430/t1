代发 wailian999

JS:   class MyError extends Error {}
来源：http://3g.fanxiaobao.xyz/Article/details/gikvkrpum.sHtML

TS:   class MyError extends Error {}
来源：http://blog.fanxiaobao.xyz/Article/details/gdfrqxuri.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghexqjvsc.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goutjxcto.sHtML

Ruby: class MyError < StandardError; end
来源：http://m.share.fanxiaobao.xyz/Article/details/gabjwsvwu.sHtML

C#:   class MyException : Exception {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/guxocrqrh.sHtML

[H05] 捕获特定类型
来源：http://m.share.fanxiaobao.xyz/Article/details/ghmlfizuz.sHtML

Py:   except ValueError as e:
来源：http://baike.fanxiaobao.xyz/Article/details/gntadsctc.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://read.share.fanxiaobao.xyz/Article/details/ggkuawiey.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjtizcawu.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://3g.fanxiaobao.xyz/Article/details/gcrqmqxsc.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gbpgcylag.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://3g.fanxiaobao.xyz/Article/details/gqzgpczio.sHtML

Ruby: rescue ArgumentError => e
来源：http://read.share.fanxiaobao.xyz/Article/details/gkizqjjkv.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://3g.fanxiaobao.xyz/Article/details/guhjvkrzo.sHtML

[H06] 可选值 / 空值安全访问
来源：http://blog.fanxiaobao.xyz/Article/details/gldcjzoes.sHtML

Py:   value = d.get("k") or default
来源：http://baike.fanxiaobao.xyz/Article/details/grnnarwxp.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://mobile.fanxiaobao.xyz/Article/details/gbtibkscv.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghaowvzhn.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://baike.fanxiaobao.xyz/Article/details/gfirpwqyr.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wap.fanxiaobao.xyz/Article/details/gvdamxpsu.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://m.share.fanxiaobao.xyz/Article/details/gyfgbqndc.sHtML

Ruby: d&.dig(:a, :b)
来源：http://baike.fanxiaobao.xyz/Article/details/guumstplr.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.share.fanxiaobao.xyz/Article/details/gfavegkbm.sHtML

[H07] 断言
来源：http://3g.fanxiaobao.xyz/Article/details/gqmayebqv.sHtML

Py:   assert x > 0, "必须为正"
来源：http://read.share.fanxiaobao.xyz/Article/details/gsvsceypq.sHtML

PHP:  assert($x > 0);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtytsmzgv.sHtML

JS:   console.assert(x > 0);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkwhubsbv.sHtML

TS:   console.assert(x > 0);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsuwpmvsn.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfiiretvd.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wap.fanxiaobao.xyz/Article/details/gcdpjcpcw.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://blog.fanxiaobao.xyz/Article/details/gkiasczhy.sHtML

C#:   Debug.Assert(x > 0);
来源：http://mobile.fanxiaobao.xyz/Article/details/gdyjbrimn.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxclzkogf.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://wap.fanxiaobao.xyz/Article/details/gznrimzuk.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://m.share.fanxiaobao.xyz/Article/details/gbinrlwrr.sHtML

JS:   e.message;  e.stack
来源：http://3g.fanxiaobao.xyz/Article/details/givtcwdpf.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://m.share.fanxiaobao.xyz/Article/details/ggmaqdoqh.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://blog.fanxiaobao.xyz/Article/details/gwebzrutj.sHtML

Go:   err.Error()
来源：http://wap.fanxiaobao.xyz/Article/details/gngpyzugr.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghabffwfa.sHtML

C#:   e.Message;  e.StackTrace
来源：http://wap.fanxiaobao.xyz/Article/details/gigqhkvsf.sHtML

[H09] 带错误码的异常
来源：http://3g.fanxiaobao.xyz/Article/details/gaqlfurmm.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://m.share.fanxiaobao.xyz/Article/details/gwmsezfiy.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.share.fanxiaobao.xyz/Article/details/gwcijwozm.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://blog.fanxiaobao.xyz/Article/details/gvhygjdnw.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://3g.fanxiaobao.xyz/Article/details/gyelxlavk.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://blog.fanxiaobao.xyz/Article/details/grlbrxkpf.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guwhxkgux.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://blog.fanxiaobao.xyz/Article/details/gravxpcme.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfrpewcvh.sHtML

[H10] 资源自动释放
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjxvkqckt.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://baike.fanxiaobao.xyz/Article/details/gngoeldml.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://baike.fanxiaobao.xyz/Article/details/ggrrqaixs.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.fanxiaobao.xyz/Article/details/gnregvysh.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwyjqjoqz.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://3g.fanxiaobao.xyz/Article/details/gnupnqtoe.sHtML

Go:   defer f.Close()
来源：http://blog.fanxiaobao.xyz/Article/details/gjbsbaznq.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://blog.fanxiaobao.xyz/Article/details/gbgmqhepo.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://blog.fanxiaobao.xyz/Article/details/gcuvsqdkg.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gcmwevztd.sHtML

I. 正则表达式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gycyadvdm.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gbvcaafgr.sHtML

[I01] 判断是否匹配
来源：http://m.share.fanxiaobao.xyz/Article/details/geajsknbo.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://read.share.fanxiaobao.xyz/Article/details/ghowjnoeg.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://mobile.fanxiaobao.xyz/Article/details/glycajmnf.sHtML

JS:   /\d+/.test(s)
来源：http://baike.fanxiaobao.xyz/Article/details/gomqjlhnd.sHtML

TS:   /\d+/.test(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gkedkpnnl.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxorbcuut.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyyhwfqih.sHtML

Ruby: s.match?(/\d+/)
来源：http://m.share.fanxiaobao.xyz/Article/details/gsohsdrms.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://m.share.fanxiaobao.xyz/Article/details/grzwgtvkt.sHtML

[I02] 提取所有匹配
来源：http://www.share.fanxiaobao.xyz/Article/details/gjuarkpah.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gekdplyoc.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://3g.fanxiaobao.xyz/Article/details/gfvjnwzyg.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.share.fanxiaobao.xyz/Article/details/gigrzxbfz.sHtML

TS:   s.match(/\d+/g)
来源：http://wap.fanxiaobao.xyz/Article/details/gfmfurbsj.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://baike.fanxiaobao.xyz/Article/details/goxutgpdi.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.share.fanxiaobao.xyz/Article/details/giecsfnfw.sHtML

Ruby: s.scan(/\d+/)
来源：http://read.share.fanxiaobao.xyz/Article/details/goxzbcnlr.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://read.share.fanxiaobao.xyz/Article/details/gtgdjlpok.sHtML

[I03] 提取捕获分组
来源：http://m.share.fanxiaobao.xyz/Article/details/gkzdmeqcx.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://3g.fanxiaobao.xyz/Article/details/gxbspekow.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://blog.fanxiaobao.xyz/Article/details/glhdjpqse.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://read.share.fanxiaobao.xyz/Article/details/ghuemqyic.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mobile.fanxiaobao.xyz/Article/details/gfqctyrjv.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://read.share.fanxiaobao.xyz/Article/details/gnadayctk.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://read.share.fanxiaobao.xyz/Article/details/gphvpoxft.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wap.fanxiaobao.xyz/Article/details/gjshduxuv.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wap.fanxiaobao.xyz/Article/details/grqwvgetk.sHtML

[I04] 正则替换
来源：http://www.share.fanxiaobao.xyz/Article/details/giznrogrx.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gheyociyr.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.share.fanxiaobao.xyz/Article/details/gdytdgtqx.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://wap.fanxiaobao.xyz/Article/details/ggcyjfmte.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://3g.fanxiaobao.xyz/Article/details/gdrtcedyz.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://baike.fanxiaobao.xyz/Article/details/ghpmeezpk.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://blog.fanxiaobao.xyz/Article/details/gbsoybsks.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gylkntwbm.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.share.fanxiaobao.xyz/Article/details/guczhdmac.sHtML

[I05] 按正则拆分
来源：http://3g.fanxiaobao.xyz/Article/details/gdtfpzlut.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://wap.fanxiaobao.xyz/Article/details/gjeorsmoy.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://3g.fanxiaobao.xyz/Article/details/gtzppqbmg.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://3g.fanxiaobao.xyz/Article/details/gqbelteso.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gehcpbayj.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.share.fanxiaobao.xyz/Article/details/gyskldnhv.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gvgujlfjw.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.share.fanxiaobao.xyz/Article/details/gxstnuvfd.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mobile.fanxiaobao.xyz/Article/details/gtubqnwea.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://3g.fanxiaobao.xyz/Article/details/gthnyoobm.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://m.share.fanxiaobao.xyz/Article/details/gjmfjizbl.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wap.fanxiaobao.xyz/Article/details/gnwprrdbf.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.fanxiaobao.xyz/Article/details/growzrkwe.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.fanxiaobao.xyz/Article/details/gnbleceuh.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://baike.fanxiaobao.xyz/Article/details/gezlpfzyt.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://blog.fanxiaobao.xyz/Article/details/gtjqhoegx.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glheatnyy.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbnjvqvra.sHtML

[I07] 忽略大小写与多行模式
来源：http://baike.fanxiaobao.xyz/Article/details/gshpesein.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mobile.fanxiaobao.xyz/Article/details/gfbdcewdc.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mobile.fanxiaobao.xyz/Article/details/gzwepqspt.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkpyfvgkk.sHtML

TS:   /error/gim
来源：http://wap.fanxiaobao.xyz/Article/details/geyzorszq.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wap.fanxiaobao.xyz/Article/details/gctzoinkf.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://3g.fanxiaobao.xyz/Article/details/grfnxpkpt.sHtML

Ruby: s.scan(/error/i)
来源：http://read.share.fanxiaobao.xyz/Article/details/gtrkfvlfy.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.share.fanxiaobao.xyz/Article/details/ggvzszxzj.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://baike.fanxiaobao.xyz/Article/details/gwzvzqugp.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://blog.fanxiaobao.xyz/Article/details/gwfptwspg.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mobile.fanxiaobao.xyz/Article/details/gczrfxhsu.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.fanxiaobao.xyz/Article/details/grlrhpzbl.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.fanxiaobao.xyz/Article/details/gxgqdyoih.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://m.share.fanxiaobao.xyz/Article/details/gxypplepy.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://3g.fanxiaobao.xyz/Article/details/gjrzsreed.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://3g.fanxiaobao.xyz/Article/details/ggnfhjfjp.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gywoadkok.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/giomtefcj.sHtML

J. 日期与时间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gucovuepo.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gebtxbhzx.sHtML

[J01] 获取当前时间
来源：http://read.share.fanxiaobao.xyz/Article/details/gpxvtvuwh.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://mobile.fanxiaobao.xyz/Article/details/gkmtfrwgo.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://baike.fanxiaobao.xyz/Article/details/gxzeqzhqx.sHtML

JS:   new Date();  Date.now()
来源：http://www.share.fanxiaobao.xyz/Article/details/gqaploqss.sHtML

TS:   new Date();  Date.now()
来源：http://read.share.fanxiaobao.xyz/Article/details/gfeagpthb.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://3g.fanxiaobao.xyz/Article/details/gtrpeisjt.sHtML

Go:   time.Now()
来源：http://read.share.fanxiaobao.xyz/Article/details/gqhvporum.sHtML

Ruby: Time.now
来源：http://mobile.fanxiaobao.xyz/Article/details/geotwkthc.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wap.fanxiaobao.xyz/Article/details/gfxrsumki.sHtML

[J02] 格式化输出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gugabfmgy.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.fanxiaobao.xyz/Article/details/gqzblmbcx.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnhmhjhmd.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wap.fanxiaobao.xyz/Article/details/gkanhaohw.sHtML

TS:   d.toISOString()
来源：http://mobile.fanxiaobao.xyz/Article/details/ggcjfrlad.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://m.share.fanxiaobao.xyz/Article/details/gpqijjyey.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://read.share.fanxiaobao.xyz/Article/details/gqloczcru.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.fanxiaobao.xyz/Article/details/gtifvnqla.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://mobile.fanxiaobao.xyz/Article/details/gftcyvwdm.sHtML

[J03] 字符串解析为日期
来源：http://www.share.fanxiaobao.xyz/Article/details/gfbeddfis.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://read.share.fanxiaobao.xyz/Article/details/gyjemwuci.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://m.share.fanxiaobao.xyz/Article/details/gsgjzjfdx.sHtML

JS:   new Date("2024-01-02")
来源：http://3g.fanxiaobao.xyz/Article/details/gqzaqruer.sHtML

TS:   new Date("2024-01-02")
来源：http://www.share.fanxiaobao.xyz/Article/details/gdrvwlzlm.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwotvinta.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://read.share.fanxiaobao.xyz/Article/details/glsajbepq.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxkfugwwf.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://baike.fanxiaobao.xyz/Article/details/glmcfnokz.sHtML

[J04] 时间戳与日期互转
来源：http://3g.fanxiaobao.xyz/Article/details/gzkgdledn.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://3g.fanxiaobao.xyz/Article/details/gapxytgmc.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjjnctnwt.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://baike.fanxiaobao.xyz/Article/details/gfxvizkur.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghmgkycqm.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.share.fanxiaobao.xyz/Article/details/griczwccv.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://3g.fanxiaobao.xyz/Article/details/giujrcwmb.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjsylzmdz.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqvtbisfg.sHtML

[J05] 时间加减（加 7 天）
来源：http://read.share.fanxiaobao.xyz/Article/details/gmstqkazf.sHtML

Py:   now + timedelta(days=7)
来源：http://blog.fanxiaobao.xyz/Article/details/gdwosednm.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://3g.fanxiaobao.xyz/Article/details/goioqvhww.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.fanxiaobao.xyz/Article/details/gljlplddj.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.fanxiaobao.xyz/Article/details/gaebvimfh.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkgodwdxp.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://m.share.fanxiaobao.xyz/Article/details/gsdmlpach.sHtML

Ruby: Time.now + 7 * 86400
来源：http://3g.fanxiaobao.xyz/Article/details/gbqycnemy.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://baike.fanxiaobao.xyz/Article/details/gyeklmtbu.sHtML

[J06] 计算两时间之差
来源：http://3g.fanxiaobao.xyz/Article/details/gqllphgrw.sHtML

Py:   (end - start).total_seconds()
来源：http://blog.fanxiaobao.xyz/Article/details/gbbepbsnx.sHtML

PHP:  $end->diff($start)->days;
来源：http://m.share.fanxiaobao.xyz/Article/details/gckykxudg.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wap.fanxiaobao.xyz/Article/details/gtbidetgt.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wap.fanxiaobao.xyz/Article/details/gppuoduww.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gidvqtgse.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.share.fanxiaobao.xyz/Article/details/gzcbgkebp.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gacytobjn.sHtML

C#:   (end - start).TotalSeconds
来源：http://mobile.fanxiaobao.xyz/Article/details/giijqtsqp.sHtML

[J07] 比较两个日期
来源：http://blog.fanxiaobao.xyz/Article/details/gebaeweom.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://wap.fanxiaobao.xyz/Article/details/gfuelztdf.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.share.fanxiaobao.xyz/Article/details/gfztaiyvg.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://m.share.fanxiaobao.xyz/Article/details/gmryzsrkl.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://baike.fanxiaobao.xyz/Article/details/gqwjknsup.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://blog.fanxiaobao.xyz/Article/details/gogdaajgp.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gmuogfjdq.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://blog.fanxiaobao.xyz/Article/details/gcicwyjhk.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://baike.fanxiaobao.xyz/Article/details/gkfagytwv.sHtML

[J08] 提取年月日与星期
来源：http://m.share.fanxiaobao.xyz/Article/details/gmhgamkek.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://blog.fanxiaobao.xyz/Article/details/gihrrwlkh.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://m.share.fanxiaobao.xyz/Article/details/gtlttjwxf.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjbgdwbqn.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmludpvkh.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.share.fanxiaobao.xyz/Article/details/gobomhoar.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://baike.fanxiaobao.xyz/Article/details/galvjanoa.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://read.share.fanxiaobao.xyz/Article/details/gryllwixm.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://3g.fanxiaobao.xyz/Article/details/gvsrsgtav.sHtML

[J09] 时区处理
来源：http://blog.fanxiaobao.xyz/Article/details/gdcvumpbe.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wap.fanxiaobao.xyz/Article/details/gnguwmqzd.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://m.share.fanxiaobao.xyz/Article/details/ghwnafonb.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnkbjpqme.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.fanxiaobao.xyz/Article/details/geblvywey.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://baike.fanxiaobao.xyz/Article/details/ghnhkdiwa.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.share.fanxiaobao.xyz/Article/details/gyhrgdoax.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://wap.fanxiaobao.xyz/Article/details/gktpnkzlt.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://3g.fanxiaobao.xyz/Article/details/gcdmcqrly.sHtML

[J10] 取今天 / 本月第一天
来源：http://3g.fanxiaobao.xyz/Article/details/gutokvarg.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gifwwmqri.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.share.fanxiaobao.xyz/Article/details/gdxkbqyek.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://baike.fanxiaobao.xyz/Article/details/gbkxrfdjk.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.share.fanxiaobao.xyz/Article/details/ggkjfpkok.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gfvmoaptx.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://read.share.fanxiaobao.xyz/Article/details/gjdlklotg.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://baike.fanxiaobao.xyz/Article/details/gxjsenpvf.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gppuzsxki.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfdzjixtn.sHtML

K. JSON 与序列化
来源：http://mobile.fanxiaobao.xyz/Article/details/gqeuejhpl.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gadspfvbq.sHtML

[K01] 对象转 JSON 字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gwfdmkyyi.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://blog.fanxiaobao.xyz/Article/details/ghvqqblyx.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://blog.fanxiaobao.xyz/Article/details/gazhaafvc.sHtML

JS:   JSON.stringify(obj)
来源：http://www.share.fanxiaobao.xyz/Article/details/gexieigft.sHtML

TS:   JSON.stringify(obj)
来源：http://www.share.fanxiaobao.xyz/Article/details/ghmduypck.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.share.fanxiaobao.xyz/Article/details/gvjwtuqwc.sHtML

Go:   json.Marshal(obj)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjwykokvx.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://baike.fanxiaobao.xyz/Article/details/gaudkhalt.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gltczgifu.sHtML

[K02] JSON 字符串转对象
来源：http://mobile.fanxiaobao.xyz/Article/details/gpvoezktf.sHtML

Py:   json.loads(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/geblymduo.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gljdfyjlm.sHtML

JS:   JSON.parse(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gahcuwghh.sHtML

TS:   JSON.parse(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gvrspkxzw.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcmsizkdg.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://blog.fanxiaobao.xyz/Article/details/giokuqqkm.sHtML

Ruby: JSON.parse(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gminsuhsv.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/grfefzeme.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghofyeesh.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.share.fanxiaobao.xyz/Article/details/gqnccypll.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://read.share.fanxiaobao.xyz/Article/details/glqifrgjp.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://blog.fanxiaobao.xyz/Article/details/ggbccdizk.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyawlkkrr.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://blog.fanxiaobao.xyz/Article/details/ggmxaistx.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://3g.fanxiaobao.xyz/Article/details/gfxauezuc.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggozzubqg.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://m.share.fanxiaobao.xyz/Article/details/gyviqwcpp.sHtML

[K04] 读取 JSON 文件
来源：http://3g.fanxiaobao.xyz/Article/details/gkuvytnmg.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wap.fanxiaobao.xyz/Article/details/gcnslnvhl.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsafbnmwj.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.fanxiaobao.xyz/Article/details/gzlwghpwk.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.fanxiaobao.xyz/Article/details/gsbaozqzh.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwptxxvrl.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://m.share.fanxiaobao.xyz/Article/details/gkzcoradt.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://3g.fanxiaobao.xyz/Article/details/grqrftfdq.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mobile.fanxiaobao.xyz/Article/details/gaxbmnbya.sHtML

[K05] 深拷贝对象
来源：http://mobile.fanxiaobao.xyz/Article/details/gixjqmspz.sHtML

Py:   copy.deepcopy(obj)
来源：http://mobile.fanxiaobao.xyz/Article/details/gqjvrapoa.sHtML

PHP:  unserialize(serialize($obj));
来源：http://mobile.fanxiaobao.xyz/Article/details/gnhwnunzh.sHtML

JS:   structuredClone(obj)
来源：http://mobile.fanxiaobao.xyz/Article/details/gxrqrcocn.sHtML

TS:   structuredClone(obj)
来源：http://www.share.fanxiaobao.xyz/Article/details/grimbekdp.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://mobile.fanxiaobao.xyz/Article/details/givdehqgi.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wap.fanxiaobao.xyz/Article/details/glengjocm.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkngmsaaj.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://3g.fanxiaobao.xyz/Article/details/gbsuxqhqp.sHtML

[K06] 解析 URL 查询串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gosxdmjmq.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmuqyoqkt.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://read.share.fanxiaobao.xyz/Article/details/gsonvpkds.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.fanxiaobao.xyz/Article/details/gomiycbjg.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.fanxiaobao.xyz/Article/details/ghuudnkkd.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://blog.fanxiaobao.xyz/Article/details/ghuawzqfy.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gngqxlrty.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://m.share.fanxiaobao.xyz/Article/details/gvschuakj.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://baike.fanxiaobao.xyz/Article/details/glhsgyzkr.sHtML

[K07] 进制转换
来源：http://blog.fanxiaobao.xyz/Article/details/gnmrfbcuu.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzhuoqfja.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://3g.fanxiaobao.xyz/Article/details/gyssfjfpt.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mobile.fanxiaobao.xyz/Article/details/ggqznuwvm.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mobile.fanxiaobao.xyz/Article/details/gsbqavmsg.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mobile.fanxiaobao.xyz/Article/details/gorxsjpal.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfmklbqcd.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdsodqtli.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://3g.fanxiaobao.xyz/Article/details/gzlsadzfg.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://m.share.fanxiaobao.xyz/Article/details/gdlctwvee.sHtML

Py:   pickle.dumps(obj)
来源：http://wap.fanxiaobao.xyz/Article/details/gwffvbjhd.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://blog.fanxiaobao.xyz/Article/details/gfbbesxjo.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://baike.fanxiaobao.xyz/Article/details/gbeghlvas.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giekfdtik.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://3g.fanxiaobao.xyz/Article/details/gkvxhcvpo.sHtML


<!-- 参考信息 -->