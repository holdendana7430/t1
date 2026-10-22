代发 wailian999

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2jcraqiqx.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2egyrssmk.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2eduxjjgb.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2yrzykbim.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2hsduwdnf.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2djiwokhg.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2tkecclnv.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2tcngwmew.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2swcecrnh.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2aftkqsgc.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2idmpxqdi.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2obvtekgy.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2esuxxdfo.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2anzuqjss.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jvtqltcy.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qwxiuosc.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2aczbkymn.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2ipqvqgij.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2widzjoxu.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2fiiuxbbx.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2pgsjbuco.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2tvxueiqq.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2ylvdfjpp.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2padpmgpy.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2vebonhou.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2nlegfxgw.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2gcjsrfpx.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2tmkgcaok.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2irxodgrh.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2xtyusgcm.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ooubigry.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2weudseuj.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2tnwnvown.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2hoctocqp.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2oflwxhcs.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2eqmetiur.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2zflrgyrh.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2wychyemh.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2ppvsftoo.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2inffdbch.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2dydirgos.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2jktmjwkr.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2lkjnmozr.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2lcqbhhti.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2zhidalps.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2uvenmhrt.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2iyhzbvux.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2tylhpnlh.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2yyhgaesu.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2iwrgfhtj.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2mbcfhjwf.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2weenhlgz.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2uogmyjzy.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2fuwzafks.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2qboaufkd.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2iicaisab.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2kxcapnsv.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2ddeiqalq.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2tdxvyjvo.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2qmfpqbif.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2dqpzoidp.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2plnravon.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2upscjqsk.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ehadxapm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gvxxzdpo.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2ivwsdqki.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rxhwpnzn.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2exqdohni.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2tsvucsny.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2mdhidqff.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mhnhzarm.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2jyopunmf.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2pgkswytz.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2sickvyee.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2gtybwmvq.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2wvmnsxgn.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2axprdlyr.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2tycrznhw.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2lhohuthg.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2hkulaoys.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2uomhzjva.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2sutnmqli.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2tzteikxu.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2vcfyxoew.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2ulxpustt.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2gkvaivcp.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2hgctsxeo.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2vzzonzzc.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2uxptoegb.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2ynbujzta.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2kpygxfxz.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2lmeqchaa.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2xxmonroy.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2ebuxcmjm.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2fgaooedx.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2dwuxgbty.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2gkbmmkmu.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2bjxphajz.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2potaqvoa.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2agvfskyz.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2qjcjnshh.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2juabscza.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2agmgxpyh.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt2bscjfvpk.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt2pkrwkooy.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2xefwnjol.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2slcsqktt.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2tyfvtrrs.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2voftreyc.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2kvhdkqld.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2cqvawyvl.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt2biqypfdk.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt2gskxomnt.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2pokpbyez.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt2kcyhstyu.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2hgftjjii.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2baxmrfsh.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2ufaqgncs.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt2olqbbdwn.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt2gkqnsjcy.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2mrjncucx.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt2crsbdfbp.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt2focptluy.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2usmhmtpn.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt2svwgrfhp.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt2pqlheeym.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt2fywlwdrq.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt2kjvyxpsl.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt2westhvtz.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt2afdekjfl.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt2ymtuptyc.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt2tynqtsrk.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2ljvohwhr.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2iqipujdz.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2kxyigxqv.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2njmvlzvw.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt2vcrtorme.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt2hrurvhyg.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2rqmyylvg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hxitbnsw.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt2kmkzhqkl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ohlcpioa.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt2rursszkj.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt2rsocbawq.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2zqulgqru.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2xhfysonb.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2nwrxccdp.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt2xabtglou.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt2gsbmyjcl.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt2rhbkdwsa.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt2uyduwcou.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2lrsavbeq.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2xjirvfkn.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2mtnujigl.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt2frpfdjfu.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt2tjiioytz.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt2soafjcxb.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt2tlohlkiw.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2ojhmcouq.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt2opsjdcha.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt2zhgshfzy.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt2vdntwbij.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt2awdwsuco.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2wastjnif.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2aazphzli.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2ewswcaew.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2ohjynvzr.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2feqoieix.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt2bdtnjsep.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt2evurykwe.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2ppdddtgh.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt2vsavdasg.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2qptedhbp.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt2ostvgmjp.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt2qvqzmrif.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt2coygxrns.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2pmrpzqsr.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2fkrmheoo.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt2vsvvtzyc.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt2lsghdgkh.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt2ekdzjkhr.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2tlpqtneq.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2gstmhbfi.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2vqncolzh.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt2ursijtjc.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt2txldfkgi.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2vcjpwjwo.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt2svptyqtr.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt2zhqheoky.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt2hzsurehq.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt2bqlqsowa.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt2ytnlowsy.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt2wtsrmvrt.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt2isuayjjs.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2vuaqwauz.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt2ovpssbqe.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2unjwkddl.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2isjizgci.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt2xxyqsofs.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2pbjjnjad.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2aplwzdow.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2azptmaot.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt2gfkuacqv.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2eqrpikdy.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2moopnujf.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt2ktbxdvtp.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt2lktvolzs.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt2vajdxmst.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt2bfwunpfb.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt2koaccuwf.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt2sobpdugy.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt2umaihbrx.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt2ybvyqyyj.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt2wycmlzaw.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt2llfimwre.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2tmucmyii.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt2gcdjefqw.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2vhmyhfzn.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2evxexpug.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2uhmyghiv.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2hubfyixa.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2zgyxovug.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt2brjcpijq.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt2aburfvoz.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt2ncxctqdx.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt2pyrhdmur.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt2gyaihecm.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt2wgiufoad.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2axtebsgm.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt2npffbopc.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt2nbkamrbh.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2zngtjavu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tpvfprdi.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2kzwsommx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2anczkpxv.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt2ofevfkvu.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2yuckdkht.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2zrwmwnjv.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2fqpfwhfz.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2omgyaogf.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2jjdokpgg.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt2dabdqcsp.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2kamhzzbt.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2naazqzqd.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt2hlzktnjq.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt2lgojevlq.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2cmvpubux.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2acpfxdfj.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2mxcempjc.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2jvypdymx.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2hvmdquau.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2rsfpropo.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt2htnikkys.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2cgwcwpmf.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2gvmpfbgz.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2qozjqqgv.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ryynrzvh.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ssxtroui.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2nvdpvdsf.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2nnskfdsi.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2babqryfr.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2ttborgvz.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2syjurgim.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt2nugzmsiz.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2fsqkwqkm.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2aomsvesr.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2wvknxsoa.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2caznsfya.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2hnfjzffn.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2oanmenxc.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2nxodxbbw.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2gudqgnmk.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2jnbdrtda.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2nvvoxczo.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2bwflzxuz.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2jcrurqls.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2rtntnavx.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2tgsqcrlz.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2bhcujjbn.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2gnwpfakv.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2ikkurxez.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2cchengyk.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2bwumpdzk.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2maotpcxh.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2jmcrrdyi.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2tuxllfbu.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2okosrrsh.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2iubahbmt.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2qotojxim.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2vubsdvbf.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2vsjtatrf.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2ejhybpxy.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2zgrvrxes.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2ifmhltcm.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2eqkrydcx.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2vadauqxb.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2ssprkzrl.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2fgfpxjbu.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2gwrurrjy.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2blhgruap.html


<!-- 参考信息 -->