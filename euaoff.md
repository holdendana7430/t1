代发 wailian999

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2mfizumpf.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2iwgebfqi.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2gjsnhpkq.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2xmvmbuft.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2umcseiot.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2dicqvhvk.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2fvzdehnz.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2hlulohnh.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2dxkodniz.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2csnenvpe.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2pgumpkpa.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2bvoixeik.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2koqoruwl.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kgcrcqlp.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2iiachemg.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2wyqwfnfy.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2kmenkpbg.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2teveiljk.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ephglimf.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2poyvmcqz.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2ckvbpwpi.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2ssmphiut.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2ixniheso.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2beoxgrvt.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2kpjtqtaj.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2tlmdidsp.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2ojmqwifc.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2yvzcqamu.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2vxbpjtcj.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2ifstcffd.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2skoqbwvr.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2iiagskdj.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2nubuitxd.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2rlgvrcnk.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2mysyudpw.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2eyloteng.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2toljffwe.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2avdpsoib.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2kgmnybeu.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2iomidxzk.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2fhhfkgfe.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2aazkxzug.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2detomwcm.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2zlkbjdvs.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2zlikimcd.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2hwfiabai.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2gtvycufz.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2kjfhvttc.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2tupuguss.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2rsfswzwu.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2ojepytif.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2upiwzsma.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2pkonbofe.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2kccxjbuz.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2yzbogfmn.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2fvsltudm.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2gdswjhkw.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2npdjdlts.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2qvwhtukc.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2kyvxbsab.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2tdoaxsbb.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2yjoevcik.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2sliqgicf.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2rcskcojf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2euxqkznv.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2gcvuwomm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dwabqgzr.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2ixmtyfdf.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2yghxzscs.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2vtwwkiwj.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ztfrcjwz.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2kyzyalvp.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2gwqvktsl.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2iyvjvxbo.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2ptjwtazo.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2gditquqk.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2lgsbpdmo.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2hsjzetso.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2fbkkcese.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2uzlashwr.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2pgsqtsse.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2fshbjrsb.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2ozwqmyrr.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2emroptfs.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2yfilfafy.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2mxgcsjxs.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2sbzatxgc.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2vcuwllau.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2wmluiwxs.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2yxnvmgyc.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2gafitiwm.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2hipfpwcu.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2ngsbvqlf.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2ytlyjiqx.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2mglxlmjh.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2huiiarwz.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2zgmxsnxf.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2rvbfsgav.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2bykmooxi.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2kpdpphgk.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2qhhqzufy.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2keetxzrp.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2tmqxyfql.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt2xtlozwmp.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt2rknfkiuk.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt2jtbqcqeq.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2lwathxqn.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2wewqvtpu.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2ixmecfwg.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2ugtvxwxj.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2heiigihj.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt2wufpnxhd.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt2iqjiixzg.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2dqcofsom.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt2mrpeuqsr.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2jpsrrdxm.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2bogjiojq.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2ahntjpfq.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt2lwkwybth.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt2vwqgsjfi.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2roxzcbkp.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt2nkjeogne.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt2bufsdykg.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2gwjbnvew.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt2ujcidyts.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt2dkjmzque.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt2jhowgebk.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt2kzgbxrou.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt2fzqfpsrd.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt2hgxdkjgf.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt2wmntreik.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt2ekizebqd.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2unfmbusw.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2mjcjrpjz.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2tglvnulx.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2drqgrmyc.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt2actvtgkf.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt2ejiiqjtw.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2uybetxcz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rusqvgvc.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt2pvkauxoo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kimsgmlj.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2gmvphxoe.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt2lfdnkesm.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2ekyjheef.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2vcfvzcif.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2heoeyxkt.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt2vsohdumy.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt2iyvqsjxl.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt2uknotkid.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt2oymwexii.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt2lvnetjfm.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2xfjmoeuj.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2kdxewssv.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt2xwsswghn.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt2nmyjaahu.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt2cdcddldp.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2bpgfezfw.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2whsztawi.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt2gywqjkdp.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt2ihsnruug.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt2mgkcszyl.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt2covvrtwz.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2nismkbvr.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2trftwxjk.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2dohgimsg.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2chsowjqq.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2yjeokqly.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt2zgscwqoi.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt2qxyvszms.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2twxrlttc.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt2zrpttozk.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt2okfacxxl.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt2kxunfvph.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt2ywsyvfdo.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt2hbosuzbd.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt2vfhkznfi.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt2gyisshei.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt2sxnzvdok.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt2dgxstauj.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt2mmfkciwp.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2rkqxlzup.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2ahgadrnr.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt2whutwice.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt2jpmkqurh.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt2fwylwwug.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2tjfscjlc.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2soatkddj.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt2nfuzzmso.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt2uedntzcb.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt2itynwmnx.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt2uejasbcu.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt2xdgbktra.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt2zbwpznzw.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt2qyfdjzoh.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt2irnimcri.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt2vjgorewu.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2urhafbhj.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt2jpvejwxv.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2utavmywo.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2pgltcxll.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt2hsffndct.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2qsvpdsua.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2dxvgalku.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2ejtdqtyr.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt2efihhwvq.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt2jfddevzo.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt2htjstdnq.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt2buomjnbb.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt2ucypcwzz.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt2enktoqiq.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt2tenpdwqj.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt2viupcvzf.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt2nnjszvio.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt2tfbogdmx.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt2uhmxqhvx.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt2revdxflt.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2vapgxlts.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2oygfidme.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2vibzvind.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2mztpuwqs.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2ojypizfc.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt2jkcavuzn.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt2szmofpyc.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2txteeayr.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt2agezxrmk.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt2hzlapghe.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt2bavkhwmv.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2muerwyer.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt2lhyuiprl.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2qnakcrup.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2zlmzfuks.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jackvkls.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2uejdfzda.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pbjujdyc.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt2pqfsbrlj.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2itxcfzpu.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2cpzexrel.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2lakwgjob.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2cktgfkmw.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2vylwposp.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt2ogmujpdp.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2cebbkjkd.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2wtduqvxy.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2wslczonj.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jczxaeqn.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2vuwwncqt.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rhptwziv.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2epmzsgpa.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2qielgztk.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2yjhcthvj.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2pmaickuu.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ddsrtxzl.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2ylhtwrwe.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2htcztuaz.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2jqbpecxq.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2oemsugzm.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2wentmxzv.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2gqhpxnxm.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2ywtzgyjo.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2xpucmliw.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2lsrqecrs.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2jjqmbplh.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt2dyrcyzvj.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2mlnmdnls.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2evakgawk.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2uublfgbq.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2yqjdghiy.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2gzymjorc.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2jxskomdz.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2zwpjpwan.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2vuaxnypi.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2avtobdpv.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2nwzfucck.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2tpvinjhu.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2kukvnomu.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2tarszxpk.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2saorusni.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2zfofijup.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2gfesiery.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2vdofatxl.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2agcglaeu.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2perksnss.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2dtcyqkmp.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2vurrvlyo.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2bfcysqvd.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2xwknvpzr.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2cwzrreay.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2pjhpxyjq.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2iepnxfgj.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2itlqmfrj.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2wsopyezh.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2wztduluu.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2uenbjfat.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2lbputrps.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2lebnqkga.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2yktthvmx.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2htblshhd.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2wkseckqu.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2xzglvoah.html


<!-- 参考信息 -->