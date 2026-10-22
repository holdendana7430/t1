代发 wailian999

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2vymfhwdz.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2wpoeqhkk.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2vgixddto.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2rsudpwyv.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2rvovsysl.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2oyqlcmdy.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2aoybbevg.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2biujrvmp.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2xtsqdmis.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2iqjqvluu.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2twhxyeht.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2xtshfurz.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2hxkzdjfm.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2jehtsvqq.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2hnizxylc.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2qqiyewbm.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2efhkwlvi.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2hzvujwwk.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2yhoynbsp.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2fwertish.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2lmfqlevd.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2wusezffq.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2tgtywpex.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2jpaevbsx.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2kamthjpw.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2happalhe.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2hhgpaurp.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2bawxqfwf.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2wealfdao.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2qgzxdzak.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2pvaeuvhb.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2cyrlgjek.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2bhyuvrpd.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2cfrknrue.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2dqwmtqpb.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2frysdmsa.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2rpuarahr.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2jpzzmaqd.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2yhmqmpjf.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2upfdruqp.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2zulpsvii.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2akrltiyq.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2apvcovgb.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2vbghjiew.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2yghxfrwv.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2tdddnzyk.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2uxzcbbmd.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2scdbagbj.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2lwefjmka.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2buriwbku.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2aigmgtmy.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2ipxnwzsq.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2linrxppc.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2upvbcwjt.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2pnmlumkk.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2oekksvel.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2whtqfpzr.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2dukdwqte.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gnzwwziv.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2skdohciw.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2xsoegzfg.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2ibfyfoke.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2gtfmwlbn.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2pgrtepic.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2hyttbfbo.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hzlxzroe.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2fxcwibdd.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2uisqomlr.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2dwftsppa.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2ohrppsxh.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2kvvxpjud.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2yekmkobq.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2qmarjfqw.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2wcifaygh.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2qfqgjjwf.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2fcktlrmo.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2wfblasae.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2dfxibcsr.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2khjembwp.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2idzpgovx.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2cmptyxwd.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2efurgioq.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2pwzlxocz.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2apwibsay.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2eaxuldyx.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2zeebjrve.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2aiemlmug.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2lgbyvwkt.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2lluodrqd.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2xunairev.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2annuvqwh.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2azkdrnlu.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2cvwytoso.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2vcbowzor.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2jrysgnsm.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt2evzeriiq.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt2jzpatpgk.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2chzboqpw.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2cdqoeaym.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2werqnisn.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2cxulnclj.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2cpztszkb.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2tiyrcnga.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt2bgqbnjmk.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt2dfayxaou.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2sjcspnyc.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt2oyjoqjqa.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2euekfcfn.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2qghezexi.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2bviuappe.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt2gcofzrhh.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt2odrznezu.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2chclkbbn.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt2bypiqbtg.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt2sfupaasz.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2tktuxjnl.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt2enlkxucf.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt2jbuqvmyb.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt2phlkipyp.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt2icebomgr.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt2tikjejhc.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt2odjokyrq.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt2izzzihjc.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt2aioxbbcc.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2wghgvuli.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2sihaxcup.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2ymfyqkfa.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2zghbilyj.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt2cwiqgpxm.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt2wnvzabyj.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2cklcbmph.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jarrbedu.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt2qqdazyxo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ggyxerla.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2nphbjzyh.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt2uxjnlisu.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2mmpcjjaq.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2bdmapqps.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2xhprljpq.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt2vgdbwmyi.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt2yuegwjjk.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt2mqgrtsuw.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt2scurxucv.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt2hclqjgft.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2fblsvmos.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2ohrsucir.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt2zkgfuhwv.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt2mjnemgca.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt2emznodfq.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt2vurfdtod.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2lbqvkxvp.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt2kdojeafm.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt2ioajfvcv.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt2fhzbevrv.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt2joymbqms.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2vtsyaqlv.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2expjkvpr.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2yrrjwdah.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2xqkzuydh.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2tagrdzks.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt2screxwix.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt2ebybyyel.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt2afvktfjs.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt2hfqwfnul.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2dqragopi.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2kikornln.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2rdbwfbab.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2gtbtuhhz.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2tjyiimtr.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt2rnaqxjpb.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt2fregwppm.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt2tmqyeokq.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt2xpjwenpv.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2sdmdnuoj.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2jamnortz.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2rouojbbs.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt2wadhglvy.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt2ouslubmp.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt2vdredazt.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt2tqetpetn.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt2gzmckgjq.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt2emcibqnj.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt2vjczpurk.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt2rsltbbdu.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt2ryezpzyt.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt2higdjxds.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2czrcltfc.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt2gfozqrwu.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt2jpwwhnch.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2zfsuocwq.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt2trkuznlq.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2nexknfjb.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2ykdpsdkg.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2kwjdxehb.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt2bbsaabrz.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2rxsreabz.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2qwonsvzb.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt2hiixfhqv.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt2jiquyuml.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt2tqhfnxcy.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt2wdcnggjh.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt2axpmdkdj.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt2oghswjne.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt2jeqnjbhd.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt2xczarujy.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt2ehfagabs.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt2yfrmhiwx.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2qyhqdtcw.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt2itkbmidq.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2qibgxjuq.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2fklncubp.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt2zstqhrbo.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2fucndvbu.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2dwlthfya.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt2jixkqhuo.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt2apzosipj.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2vowlrehc.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt2vhodtjtq.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt2prcnggvz.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2cplzdmjf.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2rkalcqlx.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt2rewohtve.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2rhdwsgex.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt2prlujpns.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2weypnten.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt2bzhbnngp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gvyahqjh.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt2hktgvxmv.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2nzhabhqu.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2lyzweahe.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2xfysjhir.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2mbombdww.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt2shaupred.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt2hdzoyupa.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2peflcaid.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2zvftxwob.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2zdecfeyg.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2flgrjohe.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2kvlqqkqx.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2brfjozll.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2htcawuvv.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2zyrgzkya.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2ysoawfzt.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2kfvnttkm.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt2aojsnpop.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2pjqfxtvg.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2sjsjtevk.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2eocpzowp.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2brptgxng.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2qmeqofow.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2fvyeheqy.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2dvetyfnx.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2qlblyinz.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2cptlpwpu.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2iqfjqgkg.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt2sbycayxv.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2hqiiwyzq.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2xoxrmmae.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2gjyloyvl.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2yyywvlmo.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2pfgxlssa.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2tonjzpkh.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2zupprdkf.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2tropgpus.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2iwhuvhdb.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2cfgmvrhe.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2fexfkroa.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2vgxronel.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2jqpqgtbf.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2quverdnh.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2nroczazq.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2ccpcvlpa.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2amhtindk.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2czpvvjgn.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2ilauwfgy.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2qwrxacmo.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2nstysyws.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2elqrsckv.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2evafjcuy.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2ptrsmtfw.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2wfasqovd.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2sdxjqtkd.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2nauecpbg.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2idaokolt.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2ectayktw.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2qdqrildy.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2hdazdloa.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2mjcjbfrd.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2qggtinxq.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2xwvhffhf.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2ocmgqucg.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2uvoqomue.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2zdpserdh.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2rqiupbuw.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2vjuilmwm.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2unszvzvh.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2wecjkgup.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2tnqndlai.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2gomplxvv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vatclndn.html


<!-- 参考信息 -->