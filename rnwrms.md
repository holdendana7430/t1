代发 wailian999

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2suubvqro.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2clscfjra.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2pinxvxqa.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2yekymebb.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2ndgbkmqg.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2bzvvbbqr.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2nrxfsfyi.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2gwtjflhu.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2wlmqtice.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2bzcderzr.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2dlzpqqjq.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2azfvuutv.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2tifnenaz.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2vonaaweq.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2tgilagkn.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2pfiaqlaj.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2zxksjmoa.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2ccznhzlm.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2oonsmdvr.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2emslewle.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2gvjlewya.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2yfnocujt.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2ceuwqwly.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2hvocwllx.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2cqtblhnh.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2szyxuvjx.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2duqbcbhw.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2gwvsroyt.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2smditkzu.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jevnobfb.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qfmrprky.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2xrkrbafy.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2fyrsutgy.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2jnzafrdx.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2oqxozydp.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2cqdjejdb.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2bzeqcgns.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2cmeuohqb.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2uxauaicz.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2uxhdjhot.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2mvmkxgys.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2itqetogm.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2gtbsnbjr.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2iqbeojrm.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2tkegcepa.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2cnjytgyc.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2vqibmrak.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2gkqajruk.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2onezkojk.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2opxzxzdr.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2eorurfkn.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2phigvqsa.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2rlbjdwsf.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2gfleqlom.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2eqdpzkmu.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2iqnqnmwe.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2bbhtznuz.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2kybhchjc.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2ruakcyxa.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2azoxbmdu.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2tnjtgmhr.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2kqiqxgct.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2zucbbonp.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2crlcqoxw.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2muxfumdh.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2apekimtk.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2yletgjwp.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2avnbezpj.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2hgrftcrw.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2qbetqabf.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2qxomrsmc.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2ldewylkp.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2zopriimc.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2xutpqcnx.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2cuxailjl.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2tnlxztgu.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2fsryyxkz.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2ovqzatis.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2sobucxel.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2lpfwcurk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sfcbmksf.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2ryzglvwk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2duthmctu.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ymfuyjfw.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2rovvqeix.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2kupqmmey.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2ngmegrul.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2izmjavbm.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2sejamifg.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jloxzfam.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2yaqytykh.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2qncdhgan.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2mpmobmce.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2ylrrvtne.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2nbdrelsd.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2sgyoblrs.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2rzjtbqot.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2nvyxzgdu.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2mqfgrkjf.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2jdurekxt.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2jxfkhbnl.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2eqmqzhrp.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2tlqrgkxk.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2sijwtzri.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2ulpomcay.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2izrlyuxb.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2fvhzbyry.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2zeuodyno.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2apnmnpdl.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2alefoadq.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2zqskxaku.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2zzqnuzww.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2helwgcyj.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2yhaowsiq.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2evqgwwxu.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2wgezltkt.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2mjmrafbm.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2ubkpkvda.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2knewwmos.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt2ufaqzxdl.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt2ygnaglqh.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt2dfbuaviu.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2lmldhkkx.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2ygdqtuwe.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2qmwedxve.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2qqjkbxkn.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2ywnzlwla.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2kmetxwfe.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt2urxmvbgu.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2zrisnoss.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt2hqithcbr.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2xfrtsjqk.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2vyxbxdfw.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2ksowdocz.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt2ontrwmbt.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt2ztielhbz.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2ojvufmgd.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt2pexkbklm.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt2gxswqtkj.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2ecmgbvbn.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt2lnzgquva.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt2ueujmjaz.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt2vqsogljm.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt2qbtivhvt.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt2btdzukja.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt2lkjlhqqz.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt2mlgquokm.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt2wtuyfwah.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2zwxcncwj.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2ezsppvae.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2twqwjecl.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2fywimawg.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt2itrastgo.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt2gqboyoov.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2xjjdtkfq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xemeyevb.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt2byycsayd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hjnkgfok.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2vpqcgrrq.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt2fsnxdvje.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2nncxxaxv.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2mzvodyie.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2pgxogywq.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt2etriigdr.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt2suadujmk.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt2oikdpxcq.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt2btqcxfns.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt2jipzlhky.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2ggegakcf.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2bmqtjzqk.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt2ddyqgjvw.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt2qscyzbty.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt2zjjubmhz.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt2wiaigwvk.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2wyfimvbh.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt2axwurpmc.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt2fhkixgix.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt2lsrrvwuc.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt2hvoergct.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2djgihmjk.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2otueetnv.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2yherqfpv.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2otmemmbw.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2nvyrmdes.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt2ffttcwzi.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt2ceaozdci.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt2qoibuaqw.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt2mjtrotrl.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt2mejwufpw.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2ymevscda.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2eemzzcvv.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt2fgtzfesl.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2vogquany.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2lolemnwm.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt2slwecuus.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt2saepfdgo.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt2hnvbexyf.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2mnpgprwd.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2hkqjldir.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt2gqtcdvno.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt2tpxunvgf.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt2busilokq.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt2ydbnjzrw.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt2jcjjtonf.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt2uwmlupsl.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt2boneyyrz.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt2kltxfhgo.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt2okngcnyg.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt2uomymmvx.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt2nhcuubvc.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2txsaokxh.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt2ovzqquop.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2uafdcwlw.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2rkkcxfpv.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt2yofyxcrb.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2eqvjcfed.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2ctkunzcd.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt2djmhbbkl.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt2yywingnu.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2wnukenfa.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2gydwdinp.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt2owxpgedf.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt2bgeubbtn.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt2fljceppw.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt2kknebnab.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt2hxwrpzmz.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt2ycchgqkt.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt2akwaeapt.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt2pwsuitfm.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt2ryegblsm.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt2plyiurjh.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2oaxazaaq.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt2mxoadwsr.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2eozqweta.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2ollfgfny.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2comjtjac.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2sgqqowda.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2dxwhqsam.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt2cfksmcnb.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt2gkrhxkun.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2bfjmczxg.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt2xhxmdrwy.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2nuyxvfsu.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2zydncevb.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2zyfqgoir.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt2sxdjczpw.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt2baqsormk.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt2fpcwguqk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cocswnjb.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2vaguprwi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2idztfjit.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2lgcyuxcz.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2ovfjspna.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2iuiyknes.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2vmqviysc.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2jnhsjkxo.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2ntllhobn.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt2evktgguz.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2lolqvssf.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2nfpnqgep.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt2sdoaktkm.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt2puthvzgp.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2aaaagqsl.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xhvtxvzd.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2vqhdrdgc.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2alaypmpa.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2flrteiuw.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2iggppbda.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2uoopdvrk.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2gghexvsn.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2nzxtefsj.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2csmojmpr.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xvchgnld.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2vjnreflt.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2fylcpwds.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2gqngwfbr.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2qjqvcqws.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2sabhytmf.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2bijuduyv.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt2vtllgtbs.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2qlburzbe.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2rscpbffe.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2vszuphqt.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2ffmysvru.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2mkhhlslb.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2vvjexzrr.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2gncdpsyi.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2euhpxsyu.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2socdkocw.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2ubzmjqbc.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ypzkequd.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2npxandtf.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2yenjyfes.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2piarxlrp.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2cnhuwagw.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2sylzhoys.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2zvcqdmue.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2prhtcqbz.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2phqxurzy.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2wczurjph.html


<!-- 参考信息 -->