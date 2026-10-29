代发 wailian999

C#:   throw new ArgumentException("错误信息");
来源：http://wap.zdbjq.cn/Article/details/gijiybqvq.sHtML

[H04] 自定义异常类型
来源：http://3g.fehbvm.com/Article/details/gskrvvtaq.sHtML

Py:   class MyError(Exception): pass
来源：http://blog.hesvh.cn/Article/details/gnzkdhltp.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://m.share.hesvh.cn/Article/details/grrpejnex.sHtML

JS:   class MyError extends Error {}
来源：http://baike.fehbvm.com/Article/details/gxmittjnj.sHtML

TS:   class MyError extends Error {}
来源：http://read.share.zdbjq.cn/Article/details/gcixmyzlm.sHtML

Java: class MyException extends RuntimeException {}
来源：http://baike.hesvh.cn/Article/details/gnckdmlkt.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.share.fehbvm.com/Article/details/glaxhihsw.sHtML

Ruby: class MyError < StandardError; end
来源：http://read.share.hesvh.cn/Article/details/gieshnnqe.sHtML

C#:   class MyException : Exception {}
来源：http://www.m.share.fehbvm.com/Article/details/grmymhdoy.sHtML

[H05] 捕获特定类型
来源：http://3g.fehbvm.com/Article/details/gtkxpxdiw.sHtML

Py:   except ValueError as e:
来源：http://www.share.fehbvm.com/Article/details/gzmobofxq.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.m.share.hesvh.cn/Article/details/gccrqdgju.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://m.share.hesvh.cn/Article/details/gwtjedxqv.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://mobile.fehbvm.com/Article/details/gqlwekrjo.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://m.share.fehbvm.com/Article/details/giejzhlfg.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://3g.hesvh.cn/Article/details/gmykhhhfq.sHtML

Ruby: rescue ArgumentError => e
来源：http://m.share.hesvh.cn/Article/details/gdfudqmpv.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wap.hesvh.cn/Article/details/gdnbfdqye.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.m.share.fehbvm.com/Article/details/ghzsssiua.sHtML

Py:   value = d.get("k") or default
来源：http://mobile.fehbvm.com/Article/details/gadsdjqzb.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.blog.fehbvm.com/Article/details/grvagtffx.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://blog.zdbjq.cn/Article/details/ggjlbvdjx.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://mobile.fehbvm.com/Article/details/gdjbrxbus.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://read.share.zdbjq.cn/Article/details/gtoxalflj.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://m.share.hesvh.cn/Article/details/gjghbcucy.sHtML

Ruby: d&.dig(:a, :b)
来源：http://3g.fehbvm.com/Article/details/godqlzkot.sHtML

C#:   obj?.A?.B ?? default
来源：http://blog.zdbjq.cn/Article/details/gicgzbpll.sHtML

[H07] 断言
来源：http://3g.hesvh.cn/Article/details/gzptmpjio.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.m.share.zdbjq.cn/Article/details/gewgnjgyt.sHtML

PHP:  assert($x > 0);
来源：http://www.blog.fehbvm.com/Article/details/gypmtzkgv.sHtML

JS:   console.assert(x > 0);
来源：http://m.share.hesvh.cn/Article/details/gknhrnpno.sHtML

TS:   console.assert(x > 0);
来源：http://3g.hesvh.cn/Article/details/gewfqwetu.sHtML

Java: assert x > 0 : "必须为正";
来源：http://baike.hesvh.cn/Article/details/gdpnurafm.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.share.hesvh.cn/Article/details/gvpymorgr.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://3g.fehbvm.com/Article/details/ggxoqkcae.sHtML

C#:   Debug.Assert(x > 0);
来源：http://mobile.hesvh.cn/Article/details/gqfyygret.sHtML

[H08] 获取错误信息与堆栈
来源：http://baike.fehbvm.com/Article/details/gcergiatu.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://wap.hesvh.cn/Article/details/gxlatewsw.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.blog.zdbjq.cn/Article/details/gdwqlzalf.sHtML

JS:   e.message;  e.stack
来源：http://m.share.zdbjq.cn/Article/details/gsethaqsp.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://3g.hesvh.cn/Article/details/gkymrunbf.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.m.share.fehbvm.com/Article/details/gfwbmbpnu.sHtML

Go:   err.Error()
来源：http://mobile.zdbjq.cn/Article/details/gggflnpux.sHtML

Ruby: e.message;  e.backtrace
来源：http://wap.hesvh.cn/Article/details/gkoqdkuqv.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.share.zdbjq.cn/Article/details/gjcvvnodj.sHtML

[H09] 带错误码的异常
来源：http://baike.fehbvm.com/Article/details/gntyhesvj.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.share.fehbvm.com/Article/details/gjbelepag.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://blog.hesvh.cn/Article/details/gpaapuviw.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://3g.zdbjq.cn/Article/details/gxytcffrm.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://blog.fehbvm.com/Article/details/gfsaazaxo.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mobile.fehbvm.com/Article/details/geaqplcnf.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.blog.fehbvm.com/Article/details/gfsbjsfem.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.blog.fehbvm.com/Article/details/gnuqkuyhc.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://wap.zdbjq.cn/Article/details/gdcghmttx.sHtML

[H10] 资源自动释放
来源：http://3g.fehbvm.com/Article/details/gfajzamdr.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.m.share.hesvh.cn/Article/details/gpnfttpjh.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://blog.hesvh.cn/Article/details/geckockti.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.fehbvm.com/Article/details/gspiytgut.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.zdbjq.cn/Article/details/guflanvqi.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.share.fehbvm.com/Article/details/gpdobcurm.sHtML

Go:   defer f.Close()
来源：http://www.m.share.fehbvm.com/Article/details/gihiaxguo.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://blog.hesvh.cn/Article/details/gsisilspc.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://blog.hesvh.cn/Article/details/gxlcsrezp.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gezbbruzg.sHtML

I. 正则表达式
来源：http://wap.fehbvm.com/Article/details/ganblzcoc.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gjlqcifzu.sHtML

[I01] 判断是否匹配
来源：http://m.share.hesvh.cn/Article/details/gbifdkefp.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.blog.hesvh.cn/Article/details/gynxyystj.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://blog.fehbvm.com/Article/details/gkaiajgjq.sHtML

JS:   /\d+/.test(s)
来源：http://www.blog.hesvh.cn/Article/details/gjvieplgt.sHtML

TS:   /\d+/.test(s)
来源：http://mobile.zdbjq.cn/Article/details/ggaohzbio.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wap.hesvh.cn/Article/details/gukgqtzxd.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://blog.hesvh.cn/Article/details/gxmvxabyn.sHtML

Ruby: s.match?(/\d+/)
来源：http://blog.hesvh.cn/Article/details/gdsbgptsu.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.share.hesvh.cn/Article/details/ggbuxmkjm.sHtML

[I02] 提取所有匹配
来源：http://read.share.fehbvm.com/Article/details/glfycpdtk.sHtML

Py:   re.findall(r"\d+", s)
来源：http://blog.fehbvm.com/Article/details/gwowpndjj.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.share.hesvh.cn/Article/details/ghgensddm.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://m.share.fehbvm.com/Article/details/gteisjasc.sHtML

TS:   s.match(/\d+/g)
来源：http://www.share.zdbjq.cn/Article/details/glpsmdhdd.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mobile.hesvh.cn/Article/details/gphclndvn.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.share.fehbvm.com/Article/details/gbenrhpxt.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.share.fehbvm.com/Article/details/gbgflkadd.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.blog.fehbvm.com/Article/details/gvtdiewmp.sHtML

[I03] 提取捕获分组
来源：http://mobile.hesvh.cn/Article/details/gbeljgdru.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wap.zdbjq.cn/Article/details/gsunmqxbp.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://m.share.hesvh.cn/Article/details/gvlppofaf.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://m.share.zdbjq.cn/Article/details/gjvurdowc.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://read.share.fehbvm.com/Article/details/gchzwyflt.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.share.zdbjq.cn/Article/details/ganvymqnk.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.blog.zdbjq.cn/Article/details/gkgcjytcd.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.blog.fehbvm.com/Article/details/gdnvtdciw.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://m.share.fehbvm.com/Article/details/gewyyikdf.sHtML

[I04] 正则替换
来源：http://baike.fehbvm.com/Article/details/gcgvqbcvs.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://baike.zdbjq.cn/Article/details/gufelzlms.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.share.hesvh.cn/Article/details/gmcenlcmc.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://blog.zdbjq.cn/Article/details/gnktofgdh.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://m.share.fehbvm.com/Article/details/gzehjcyol.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://mobile.zdbjq.cn/Article/details/gkzqhxbjl.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://baike.hesvh.cn/Article/details/gepytkywj.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://mobile.zdbjq.cn/Article/details/gxohhcgzm.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mobile.hesvh.cn/Article/details/guyecjkzt.sHtML

[I05] 按正则拆分
来源：http://read.share.fehbvm.com/Article/details/gxsoupdid.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.share.fehbvm.com/Article/details/gvfifphzy.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://blog.fehbvm.com/Article/details/gwmjyjxlz.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://baike.fehbvm.com/Article/details/gpfumhmwp.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://blog.fehbvm.com/Article/details/grzikjere.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.m.share.fehbvm.com/Article/details/ghtgykuti.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://m.share.hesvh.cn/Article/details/gktxbgfkx.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.share.fehbvm.com/Article/details/gsicmeotv.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.blog.fehbvm.com/Article/details/giorxsxxi.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wap.hesvh.cn/Article/details/gafagbtnh.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://blog.zdbjq.cn/Article/details/grxgpunng.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://3g.hesvh.cn/Article/details/gvpfrnrwg.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.hesvh.cn/Article/details/ghcbevtcu.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.hesvh.cn/Article/details/gbcigsogn.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.m.share.fehbvm.com/Article/details/gqmelroff.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://m.share.fehbvm.com/Article/details/gswmbersj.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://mobile.hesvh.cn/Article/details/gjzzmvxnp.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.blog.zdbjq.cn/Article/details/gmalbsnmn.sHtML

[I07] 忽略大小写与多行模式
来源：http://wap.hesvh.cn/Article/details/guhcsyvae.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wap.zdbjq.cn/Article/details/glrzlgvje.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://3g.fehbvm.com/Article/details/gshjjmfgw.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wap.zdbjq.cn/Article/details/gtgtgxgfk.sHtML

TS:   /error/gim
来源：http://www.share.fehbvm.com/Article/details/gamjumkwn.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://read.share.zdbjq.cn/Article/details/gkgyqxnss.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.blog.hesvh.cn/Article/details/gxjwjrgvr.sHtML

Ruby: s.scan(/error/i)
来源：http://3g.hesvh.cn/Article/details/gvacchman.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://blog.fehbvm.com/Article/details/gjypiavsr.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://wap.hesvh.cn/Article/details/gquzhxbem.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.m.share.zdbjq.cn/Article/details/gmadpctzb.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.blog.hesvh.cn/Article/details/gwozchwmd.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.fehbvm.com/Article/details/gvraxgzgz.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.fehbvm.com/Article/details/gzhiadcfm.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.blog.zdbjq.cn/Article/details/gdaifczhl.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.blog.hesvh.cn/Article/details/gsxfgbxjw.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://baike.zdbjq.cn/Article/details/gbdraoyju.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.blog.hesvh.cn/Article/details/gxhynvfmj.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gpfogvckt.sHtML

J. 日期与时间
来源：http://blog.hesvh.cn/Article/details/ghpizkfhr.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gtnyxlcci.sHtML

[J01] 获取当前时间
来源：http://www.m.share.fehbvm.com/Article/details/gcnxtplod.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.blog.fehbvm.com/Article/details/gbroqpjal.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.blog.fehbvm.com/Article/details/gysqrfolc.sHtML

JS:   new Date();  Date.now()
来源：http://baike.fehbvm.com/Article/details/gtzpisssq.sHtML

TS:   new Date();  Date.now()
来源：http://www.share.hesvh.cn/Article/details/gwntbchia.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://baike.fehbvm.com/Article/details/gfcugzbsm.sHtML

Go:   time.Now()
来源：http://baike.zdbjq.cn/Article/details/gfpeudxky.sHtML

Ruby: Time.now
来源：http://www.m.share.zdbjq.cn/Article/details/gacwkdtve.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.blog.hesvh.cn/Article/details/goimpsqhp.sHtML

[J02] 格式化输出
来源：http://mobile.zdbjq.cn/Article/details/gpwqucbhg.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.zdbjq.cn/Article/details/gegolrvmk.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://m.share.fehbvm.com/Article/details/gbcdrweyw.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://read.share.fehbvm.com/Article/details/geanxxyuf.sHtML

TS:   d.toISOString()
来源：http://www.blog.hesvh.cn/Article/details/gfepbcqut.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.blog.hesvh.cn/Article/details/gvrnxlpuo.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://3g.zdbjq.cn/Article/details/gyeqnvwva.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.hesvh.cn/Article/details/gcpplfuky.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.m.share.zdbjq.cn/Article/details/gackdwhnn.sHtML

[J03] 字符串解析为日期
来源：http://blog.zdbjq.cn/Article/details/gxnnxmiid.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://baike.zdbjq.cn/Article/details/gpjgalllg.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.blog.fehbvm.com/Article/details/grnkzairx.sHtML

JS:   new Date("2024-01-02")
来源：http://3g.zdbjq.cn/Article/details/gbpgvzzfa.sHtML

TS:   new Date("2024-01-02")
来源：http://wap.fehbvm.com/Article/details/gsptvaryu.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://m.share.fehbvm.com/Article/details/gnxvswlhm.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.m.share.hesvh.cn/Article/details/gplwhzdun.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.share.hesvh.cn/Article/details/gluhgtiso.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://3g.hesvh.cn/Article/details/gpxkpphnh.sHtML

[J04] 时间戳与日期互转
来源：http://www.blog.fehbvm.com/Article/details/geawmrrjh.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.m.share.zdbjq.cn/Article/details/ggrzutege.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wap.hesvh.cn/Article/details/gshfqbdvq.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://3g.hesvh.cn/Article/details/gqfuyovgb.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://wap.fehbvm.com/Article/details/gjfhhbdhj.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://read.share.fehbvm.com/Article/details/gyhacxkjl.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://m.share.hesvh.cn/Article/details/gdhpemqyu.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wap.fehbvm.com/Article/details/gdcebnlgd.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.share.hesvh.cn/Article/details/giapcvimt.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.blog.fehbvm.com/Article/details/ghercyxsm.sHtML

Py:   now + timedelta(days=7)
来源：http://m.share.zdbjq.cn/Article/details/gzendgvah.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://mobile.fehbvm.com/Article/details/gspbpmjaa.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.zdbjq.cn/Article/details/gtprhfqec.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.hesvh.cn/Article/details/gofrvjunz.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.m.share.zdbjq.cn/Article/details/gpnaghfca.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.blog.fehbvm.com/Article/details/gosmmtqvk.sHtML

Ruby: Time.now + 7 * 86400
来源：http://wap.zdbjq.cn/Article/details/guuhxnrir.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://3g.zdbjq.cn/Article/details/glnzyjsoo.sHtML

[J06] 计算两时间之差
来源：http://www.m.share.hesvh.cn/Article/details/gcunxauvr.sHtML

Py:   (end - start).total_seconds()
来源：http://read.share.zdbjq.cn/Article/details/grufswfde.sHtML

PHP:  $end->diff($start)->days;
来源：http://read.share.fehbvm.com/Article/details/gjtbuvdzn.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://read.share.zdbjq.cn/Article/details/gpgirunxm.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.m.share.hesvh.cn/Article/details/gueukfnez.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.m.share.zdbjq.cn/Article/details/gdpfbmrso.sHtML

Go:   end.Sub(start).Hours()
来源：http://mobile.fehbvm.com/Article/details/ghmiywazx.sHtML

Ruby: end - start                 # 返回秒数
来源：http://3g.hesvh.cn/Article/details/ggbdamjuo.sHtML

C#:   (end - start).TotalSeconds
来源：http://mobile.zdbjq.cn/Article/details/giznejzsx.sHtML

[J07] 比较两个日期
来源：http://mobile.zdbjq.cn/Article/details/gsbwdgneh.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://wap.fehbvm.com/Article/details/gdpsrwqdn.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://3g.hesvh.cn/Article/details/gbhggqxct.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.blog.fehbvm.com/Article/details/gpzfbztyq.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://blog.fehbvm.com/Article/details/goofxshzr.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://m.share.hesvh.cn/Article/details/gxjwnopmj.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.m.share.fehbvm.com/Article/details/gbouamrgi.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://mobile.hesvh.cn/Article/details/gkpdbypvs.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://wap.fehbvm.com/Article/details/glbdptogc.sHtML

[J08] 提取年月日与星期
来源：http://m.share.zdbjq.cn/Article/details/gngsgfiel.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://3g.fehbvm.com/Article/details/gqiojhwsg.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mobile.hesvh.cn/Article/details/gylkzbvbv.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wap.fehbvm.com/Article/details/guukxiira.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://wap.fehbvm.com/Article/details/ghnpzvswn.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.m.share.fehbvm.com/Article/details/gvzqhrkoq.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.share.fehbvm.com/Article/details/gtrgwarsl.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mobile.zdbjq.cn/Article/details/geutasuaq.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://read.share.zdbjq.cn/Article/details/gwuhjugvc.sHtML

[J09] 时区处理
来源：http://www.blog.fehbvm.com/Article/details/gjpepdxpc.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mobile.hesvh.cn/Article/details/gohtflfqq.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.blog.fehbvm.com/Article/details/gexqpmspj.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.hesvh.cn/Article/details/gbdlepasp.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.hesvh.cn/Article/details/gmzguokcn.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.share.hesvh.cn/Article/details/gysuooojv.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://baike.hesvh.cn/Article/details/gpcejbgwx.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://blog.fehbvm.com/Article/details/gflkiycgc.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://baike.zdbjq.cn/Article/details/givkldjpj.sHtML

[J10] 取今天 / 本月第一天
来源：http://wap.zdbjq.cn/Article/details/gpxcktfgf.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.share.fehbvm.com/Article/details/gpvozbhju.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mobile.hesvh.cn/Article/details/gtbcxpndv.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.share.zdbjq.cn/Article/details/geptoxknh.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://baike.zdbjq.cn/Article/details/gkmluhztp.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://blog.zdbjq.cn/Article/details/ggwcjiomi.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://m.share.fehbvm.com/Article/details/gdfolvvmf.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wap.zdbjq.cn/Article/details/gcfhvtkpv.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://m.share.fehbvm.com/Article/details/gbewvvsex.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/ghocpeyvq.sHtML

K. JSON 与序列化
来源：http://www.m.share.hesvh.cn/Article/details/gcoinwyli.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/geczgrmdb.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gxhjvvguy.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.m.share.fehbvm.com/Article/details/gjoeonkuu.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.fehbvm.com/Article/details/gnwwxbxpu.sHtML

JS:   JSON.stringify(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/geweiouvk.sHtML

TS:   JSON.stringify(obj)
来源：http://3g.hesvh.cn/Article/details/grcvdzggx.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.share.fehbvm.com/Article/details/gksqoyaib.sHtML

Go:   json.Marshal(obj)
来源：http://3g.zdbjq.cn/Article/details/gnobsfnap.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://blog.hesvh.cn/Article/details/glboqimwy.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gubfjmteh.sHtML

[K02] JSON 字符串转对象
来源：http://www.share.zdbjq.cn/Article/details/gjryrijkv.sHtML

Py:   json.loads(s)
来源：http://mobile.fehbvm.com/Article/details/gjoaleuze.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://read.share.hesvh.cn/Article/details/ghnuuywwe.sHtML

JS:   JSON.parse(s)
来源：http://www.blog.zdbjq.cn/Article/details/gqhjrsigh.sHtML

TS:   JSON.parse(s)
来源：http://www.blog.fehbvm.com/Article/details/gxytdxhbu.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://3g.zdbjq.cn/Article/details/gdygywjby.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://wap.fehbvm.com/Article/details/gbocggquk.sHtML

Ruby: JSON.parse(s)
来源：http://3g.zdbjq.cn/Article/details/gkvihrdez.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mobile.zdbjq.cn/Article/details/gbyjvyngv.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.share.fehbvm.com/Article/details/gbwdykknl.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://baike.zdbjq.cn/Article/details/ghybsflzo.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://baike.hesvh.cn/Article/details/gmlaylgoj.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://blog.hesvh.cn/Article/details/gkafueuvt.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.fehbvm.com/Article/details/gxamzyqky.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://3g.fehbvm.com/Article/details/goqxhlvcy.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://m.share.hesvh.cn/Article/details/gbveuvwdh.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://read.share.fehbvm.com/Article/details/genispmzc.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://3g.zdbjq.cn/Article/details/gepbezzby.sHtML

[K04] 读取 JSON 文件
来源：http://blog.zdbjq.cn/Article/details/geqkuaiwc.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.share.fehbvm.com/Article/details/gjlpkxafe.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://read.share.zdbjq.cn/Article/details/ghzrkageu.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.hesvh.cn/Article/details/gwuhzqgwc.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.zdbjq.cn/Article/details/gbdifgsjl.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.share.fehbvm.com/Article/details/gtuzazqfm.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.blog.hesvh.cn/Article/details/gxzsdblgd.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://mobile.fehbvm.com/Article/details/gwpddjhmh.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://3g.fehbvm.com/Article/details/gdpbjlvkw.sHtML

[K05] 深拷贝对象
来源：http://baike.hesvh.cn/Article/details/gpckcbiwk.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gmpegspkt.sHtML

PHP:  unserialize(serialize($obj));
来源：http://m.share.zdbjq.cn/Article/details/ghkjddcuz.sHtML

JS:   structuredClone(obj)
来源：http://baike.fehbvm.com/Article/details/gosyauxds.sHtML

TS:   structuredClone(obj)
来源：http://read.share.hesvh.cn/Article/details/gxklmpenx.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://m.share.zdbjq.cn/Article/details/gtrjlewtk.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.share.hesvh.cn/Article/details/gpbqbcrkj.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.m.share.hesvh.cn/Article/details/gsagmqied.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://read.share.zdbjq.cn/Article/details/gcnwlsgyx.sHtML

[K06] 解析 URL 查询串
来源：http://blog.fehbvm.com/Article/details/ggronsfch.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://m.share.fehbvm.com/Article/details/gflvauffp.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://baike.hesvh.cn/Article/details/ghdjtvuby.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.fehbvm.com/Article/details/gkawkvjaf.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.fehbvm.com/Article/details/gwblpqccn.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://m.share.hesvh.cn/Article/details/gorntkxif.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://m.share.hesvh.cn/Article/details/ggqvijrbl.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wap.hesvh.cn/Article/details/grycvzbqd.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.blog.hesvh.cn/Article/details/gjapwfhty.sHtML

[K07] 进制转换
来源：http://read.share.zdbjq.cn/Article/details/gvacmaybc.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.blog.fehbvm.com/Article/details/gtewzgoyl.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wap.hesvh.cn/Article/details/glpvfimjq.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.m.share.fehbvm.com/Article/details/gkxgupzww.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mobile.zdbjq.cn/Article/details/gtdyzeiyb.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mobile.fehbvm.com/Article/details/gfvraqglz.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.m.share.zdbjq.cn/Article/details/ghhbqqvgf.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mobile.zdbjq.cn/Article/details/gvtfpdnpj.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wap.fehbvm.com/Article/details/glarkveip.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://m.share.zdbjq.cn/Article/details/gummvjaxy.sHtML

Py:   pickle.dumps(obj)
来源：http://baike.zdbjq.cn/Article/details/gwaglplgy.sHtML


<!-- 参考信息 -->