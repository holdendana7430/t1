代发 wailian999

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2icbpwkqc.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2erklwzku.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2wduuemlj.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2cfjqgcom.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2uhbkoflk.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2tnookkac.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2wlgqpxxf.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2mczjwaqk.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2tbuhluwh.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2xyihnhuh.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2cpmplbdn.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2axzcrwqn.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2hgkcqhsj.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2rquvalkm.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2bzqujstg.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2esvlyeyo.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2dgihnizl.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2vxvbbbcz.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2cphvazql.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2yikicpln.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2alnpfpvk.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qwahzvde.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fbvyhrzt.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wriagbtu.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2jrmcxroj.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2zxbqisdw.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2tctbpgql.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2cjsnjwlj.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2ijjnhakl.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2ngwqwgol.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2ilbdnsiu.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2hzbxzdcq.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2iulqcstx.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2cxfqboda.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2pbycawje.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2iooyawse.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2zfmbimme.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2rjdwohiy.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2nswddeif.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2mbgnrzll.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2wotvkuva.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2igqunnos.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2kjrsfkbp.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2fzxnbhfo.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2gqdtgsql.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2bgyiumyj.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2kbfyhmjo.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2kyqfnseo.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2ptdtbttq.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2fldffjqg.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2qqatdjze.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2ctrcsvox.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2ibvkaryw.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2bfjbxbtk.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2qchfhgce.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2xnsjptim.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2zcumdprz.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2mowzfyqi.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2dnxqchyq.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2drgvveit.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2mdhwlurz.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2xflnsjmm.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2ehgljawe.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2lycsnrzk.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2rzrppgvt.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2flaoxynn.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2sfkpcddx.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2qhwxeakr.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2aburfmdx.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2bycsmlkc.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2ofhphefb.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2xzpyjxqz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2abqkvozs.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2odkuxozg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mawsanxk.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2iplqxvew.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2bgmkqjqe.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2fykyqcgu.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vwywqwcv.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kjiafbjb.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2lslaoyic.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2huldufae.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2erzlvlvo.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2vaudxajs.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2pregqran.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2vyvhggot.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2igyyblql.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2wlqnwyyl.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2qxyddhiy.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2tmwopxpe.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2vpljwekm.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2izaesmyn.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2fpykzpnx.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2oemfzniv.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2kevslftg.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2ovfcqtyg.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2veqgdoyk.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2cbvzgklr.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2dqenaiui.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2oqikhmot.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2ccdzdzbz.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2yxfcmgvw.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2rycrmoiw.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2extvdura.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2bcvuomzg.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2jfekgvwq.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2cftefsxk.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2kxdponkc.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2xinccbat.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2ebhtuqim.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2gntbneiu.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt2kogwbnpg.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt2lmqjkwqr.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2zmziculm.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2yzuasywa.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2pxksjxww.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2ekvyriks.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2pnuswfyo.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2vpjviovg.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt2qmkixorz.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt2nxwvtsir.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2owprpvvf.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt2cvubiimp.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2aalbnnkv.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2vouecpwp.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2gwwnjuey.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt2fimtxmsw.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt2wbnvxbno.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2texwtyqj.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt2xgkhlygo.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt2vevffhzl.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2crpymolg.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt2mqtilttd.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt2tnouboiw.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt2vzhsqntz.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt2klhtdsrj.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt2gzehlcoj.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt2fqkxkapm.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt2gezrclvk.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt2eeczktsb.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2snnyjljm.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2zclvmedl.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2wmpqasor.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2fevhxwor.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt2fdjmfpua.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt2tnsnclqd.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2zsxgwxbo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sgfdtpgz.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt2esundihh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vadsavvb.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt2fdygzfrb.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt2dfxurgwx.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2muqixywh.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2sfxeofiy.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2ghakykya.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt2cepckrtb.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt2flphgipf.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt2hdapqmdc.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt2tsgxeamx.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2wvkmjyek.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2rlbqqhqg.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2efrtwedi.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt2qwbtsswj.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt2bqtcfdde.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt2auokdmok.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2fcyfzdif.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2jcjnmoen.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt2zekbnjpl.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt2jvuzsops.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt2tyflufby.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt2vbwxlvkj.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2dwprlcan.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2scccwwjh.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2qmyjewgh.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2tqqxujpb.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2cnpozhuv.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt2qtrbenow.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt2ghxvwfww.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt2ozjghtqv.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt2ndbswhra.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt2oicuivzn.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2iiexagkg.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt2ayfwbqlo.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt2ydkflnho.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt2rrxrxiqc.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt2jixoglhn.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt2ikqhiqvk.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt2zldrdrsg.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt2xkontofd.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2vjjwulku.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2rempzaio.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt2hzdpmsjj.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt2kbfsahhs.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt2hprpjhkh.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2cvsfwxir.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt2fmmtrecz.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt2skxzawtg.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt2cwkxbbsm.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt2aolhyqzc.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt2qrqoespu.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt2dcmlesls.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt2mnxkinos.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2puzeoont.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt2ckezotqs.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2khcftzgi.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2dnpsfxjc.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt2ttbajqpu.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2slxiltui.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2trubmxbe.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt2mwzvsxdj.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt2xnxghcsh.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2fwfyrudv.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2fooinbgp.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt2lluzgzhe.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt2gjgtvuot.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt2oxajlmuq.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt2hmbfzmqy.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt2gkrzspxq.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt2nsagruws.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt2khwlmpsx.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt2ezthavxk.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt2pzeypqjo.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt2mvglgibg.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt2laxrmkoe.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt2kzfghlcb.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2ecfilyqj.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2bjitubjv.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2twqwdkbb.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt2dwacesqx.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt2vyntmvuj.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt2ykjlpdoh.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt2umdsdnlr.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2mdulqntg.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt2zrymnxdq.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt2jexcekps.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2vhilipjc.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2zpmwzetl.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt2rgsfihxe.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2sawvdldl.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt2wsfazhyl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pkzgbfoe.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2tjsdvhlh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vobiziao.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ktmkoysd.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2elmrheuo.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2iuljjrkm.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2bbmezkke.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2pysyjmja.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2ggcfrmjv.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt2qeqizjua.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2phoapkmh.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2bkswbsrf.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt2wqdmkuum.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pyxdqbkj.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2jglwycdl.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2xxfzjrdi.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2idxtgfua.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2ypoleuem.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2iuffufig.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2ddchfhxa.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2otplrfcg.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2imdcrgrr.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2wdsfvpob.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2akbrwurh.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2sopkmsel.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2hronxvub.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2hlidjxky.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2skbwcsuw.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2pwwzarbu.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2mmqclemp.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2gzhyqxrv.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2bfjlxayo.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2ybrqtvqc.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2huxtttpy.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2tsjmbipm.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2plnrjrpc.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2ozyeluyh.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2jkzkjken.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2dbwufcfh.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2ypktqvmd.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2knnfehev.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2vfgztxfd.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2wztvrfxg.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2sgqqdvly.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2byltrpcn.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2gsctgjwh.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2mfwmvhdp.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2escwcpto.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2nsaarjvr.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2prgfnfuq.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2ubyszcnm.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2duiclwgz.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2gdsdeovl.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2sxxwyvis.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2yopyqlkh.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2xipihlgl.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2yutoinyt.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2ejfgjebz.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2bwcphufd.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2bullzncr.html


<!-- 参考信息 -->