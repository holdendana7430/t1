代发 wailian999

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3rovxuzwc.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3hejfxabe.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fiytnbux.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3ldurwvle.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3aenzstfd.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3qtydjavi.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3elnfvyiq.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3wpdfmgmt.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3yjegwpug.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3rbwzcgsv.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3adtqzfls.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3lefwiytx.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3adlnvixf.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3wgelvadi.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3esmxfyds.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3qlxnfiin.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3yaxdzdcf.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3bztzvuvg.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3dfwvpjth.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3gflousgw.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3zylcjfot.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3luixyybx.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3vkwmvwhj.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3pdmsgwsz.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3ftvbaqqt.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3nutvdwlo.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3gnrqfoqv.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3qrucdvjw.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3roladeqy.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3aeeoawgf.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3dlnisooh.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3hsetvieh.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3gofkmsth.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3hxohxtje.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3ttvjywht.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3vcufcsen.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3xsqlqumn.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3otoiobpu.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3brccxowx.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3njtveind.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3bjkamvus.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3wktnquyl.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3nqqamdha.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3bimqpxgh.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3qcluxmyu.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3sgkbmuzg.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3lglxzkor.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3recaskwl.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3ifjoomcy.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3rnipinoc.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3barixijz.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3lwsgizxu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rjggdvij.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3zhuoaydh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ljhznevz.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3snkzndry.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3qujcqxzo.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3txpwrfcy.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3xdfsstzn.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3lamrjuzv.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3vglewhem.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3iqrwjzbm.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3uuazwwta.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3weylrnwj.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3lkubfrss.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3uoqyopzq.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt3gbgcynzi.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt3fdaxvmob.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3vcbubodl.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt3kbuxquaj.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3oscqxgxc.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3dwhgkuoj.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3hqaehljw.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt3itnxtyrp.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt3ylrremcv.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3rafxyzyc.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3iseepabx.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt3zwoxtoej.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3eqfrbfcj.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt3xsjtonyc.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt3hbgqmxij.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt3fujhhpzk.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt3ofwxzgdf.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt3evbqbnsc.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3tripxgmq.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3skpyvnlj.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3wmivtzvg.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3lyswvegj.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt3hrldvrif.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt3moskpmvy.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3zwxrojpo.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt3jyrbwlte.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt3xogvzrxd.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt3wzvpelyh.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3fddwbjuz.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3bzgtqlrt.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt3gbexrjwh.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3qmnbdwru.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3wscymbuf.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt3hntbknct.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt3jswdydyy.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3gmeqramc.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt3vmdbcfvz.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3duhevbvj.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3sdfabesq.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3sshbesym.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt3pikwituc.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt3gxcpffly.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3xxlivisi.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt3gtsnzpnc.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt3ecmdjenk.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3mbsdwojj.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt3gvphbbnb.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt3pcwkzeva.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt3bmfkcnwe.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt3jyjlnbfx.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt3jlkhavjm.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt3uvlajqnd.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt3iurdeavl.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt3gjgtdrty.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3ifzqeuzt.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3zrazxsln.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3aavarhgy.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3lgvnidak.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt3dlrenyau.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt3qbagtikz.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3rgviefxf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fjfphqxk.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt3hkycapjg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3luadhpkw.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3julnztht.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt3lodgaoba.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3pdfrwhez.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3hglrimlv.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3tqiephvt.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt3foyocgnl.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt3wgatttjn.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt3qphncara.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt3ymwzolld.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt3kmfxmkpn.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3rbpzoxtv.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3yqzkawzy.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt3xqkosizn.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt3qlxgmedp.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt3nuzwnruy.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt3vphftmdv.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3hmuytqex.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt3osgqvhod.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt3hirrhany.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt3bylioirl.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt3jeixercv.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3cjvynrqo.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3ufkintym.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3mkhzkqpg.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3zlrngorm.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3kmbarzos.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt3ryicbwrk.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt3zyhzvteg.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt3izmsuxjn.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt3fzlafbvr.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt3orvmzmxu.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3qirsumwi.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt3cjkqnqtv.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt3fqjjpjiz.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt3ljhvtdjs.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3vpyiatjg.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt3lxsbhodf.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt3iwhlcjpf.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt3jhfpzhoz.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3vihnampo.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3uiskhihm.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt3ekaybemv.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt3vyvwvjlr.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt3vrihlcrh.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt3lrortyun.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt3dtrfqvya.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt3olqijqki.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt3aenuqexm.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt3pavliiej.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt3ylsqxpel.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt3eckjcxwz.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt3muwdgqpf.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt3zubdniae.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt3vubdczke.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt3uujjweeu.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3xuscaped.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt3mioehxmo.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3aamuhwcl.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3wqyvfijw.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3eeqyxzsr.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt3kmimpzjx.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3oeultyzh.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3beegubnd.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt3lltcaota.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt3suxhorta.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt3wvikholg.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt3ewmloqbk.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt3jhlxmbhc.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt3fnljhiqd.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt3yfceyxef.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt3sxpbfyqx.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt3sdizwpyz.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt3bljfztwa.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt3qglnicgl.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt3rmcgfbws.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3qtlibapv.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3fptjzduu.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt3zvspdjtv.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt3huhmvmsa.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt3aqabzizy.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt3xtbneawv.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt3kgtkuuep.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt3cnfeahbt.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt3tszroufw.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt3uixclhnr.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt3rrwmnxrk.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt3gvhscwsz.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt3yrwmceyd.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt3oqmveiya.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt3hjzlddxd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dhycypde.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt3bphfmrat.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kssfptbc.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt3xvbofvoc.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3qszjlkuf.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3snjlspdc.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3eyckqfkw.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ymkbkwma.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt3epfbvhlg.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3oybfcfzo.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt3ydaiehmr.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3oxomcgqe.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3ewtyrhjc.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt3djndckva.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt3aplxspqn.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3etuwnlkz.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3blflakpt.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3huaxtlmv.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3ukqdvstg.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rrdyuxch.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3mzabrqkv.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3lgmqnmco.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3gsmbtbjt.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3odptgecf.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3fhfmwjmy.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3sqqfothn.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3tapakypw.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3xwahbvfx.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3vfpzfxzi.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3vunnupmg.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3nsmmanwr.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3jkvxwcwj.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3lxqplqaa.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3iaptintp.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3fejuvudn.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3gxtypqku.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3jcvmrhum.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3khizrizm.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3ulzcgfnz.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3muaqgcja.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3drhzohci.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3hxqsahmv.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3afcosnlq.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3juzqbcwg.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3zzpuofih.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3jfwzihgw.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3dotltmqg.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3qrcdcefs.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3zugcrqdo.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3avuujtkl.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3vycqxqmh.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3xeuqrdtk.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3jhdztyto.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3bxtpiukx.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3cdlsckgz.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3cxxqznzd.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3sntofemw.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3pinnvwfw.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3bxvfynpo.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3svcgbygi.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3mcuolftx.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3hxsbdujj.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3yizryoth.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3qbgsbmzx.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3dwirhkoa.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3bmdikdnl.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3ktnzgome.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3vhzmcvij.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3axxyigji.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3kgjkuoyy.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3ajafjhks.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3thocjzvf.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3crsireqj.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3ovxdhxpk.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3oxgbbvtp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qekhnddd.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3ygffsznk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zcrfrxlw.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3skhfvftq.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3fwzkkela.html


<!-- 参考信息 -->