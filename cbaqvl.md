代发 wailian999

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2igsmxoid.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2rynmsfci.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2tfjphkym.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2zmdvvdnu.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2cxhztuip.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2kvlobiuy.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2dkfgxpfg.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2tlzajidl.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2muvrsgqc.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2uoddgtou.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2gjqqfsdq.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2emybrmks.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2ffmzdeng.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2wzmuyzog.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2ihkyutiz.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2htepgocw.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2tlrleblg.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2mqjopssg.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2oxeymyva.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2evanuygh.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2bgsygqev.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ycwmswtm.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vionqudw.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2djunxxbu.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2uthcpfwh.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2hcjwctjc.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tmqwcjcv.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2gpswiyai.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2wvfgryru.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2cutknewo.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2wbnsqlze.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2ptqpicgm.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2deypqubh.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2cizvtnfc.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2ypbklqon.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2vqdevtwe.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2iufiwels.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2yjszwudg.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2xoajfkna.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2xavqhkhp.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2uggbckhx.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2lurhamtt.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2sdoflwou.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2ogopcvth.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2uhpnbtga.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2yncclxtq.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2pjtxsdqy.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2iyfqgidm.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2rrudjldv.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2wumwlxqc.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2spqbdvli.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2uweqtonm.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2fvxxfhlg.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2emfvzcvp.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2thuvgpux.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2lahpjkep.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2jxgujawc.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2eqjyfyyb.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2jepropmq.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2pmmviuwt.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2lrstydmn.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2yblnuejp.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2rftvrehf.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2uejsiwqi.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2srrsscdw.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2ghcdhjdh.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2obgvtbca.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2nzgjizzm.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2dlnzzgoo.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2rlommphl.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2dfxkhjcv.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2gvqbzkvd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zppxkekr.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2msjbnaww.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hcsmhtob.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2wukprbhj.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2nrnlagxb.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2xsixqfwo.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2lwevzrve.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2yxqfnjqu.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2swluwbes.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2pvtvbnqs.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2jdajflby.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2itzimcxp.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ojxsbfyu.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2aydvegbk.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2wibohdzs.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2proimknt.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2dqwfoxbd.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2rjwnfbqq.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2lhplxrhy.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2hhamqrib.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2idvkfgrs.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2bcsicadh.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2fnomukmw.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2rlejpyux.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2jyvldqns.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2riiidgbj.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2owewdqbv.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2jckdytjc.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2crdkuccu.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2idevxbfq.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2oeltuiek.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2kmreesbz.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2fhbvldpt.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2fzllswav.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2dbulozqc.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2uyprfflt.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2jitqcywz.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2wqxptxts.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2ewkqnhpp.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt2dtvmqgzc.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt2bpsipnoe.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt2wpaegqfu.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2hfvfnxmh.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2gerxqmun.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2zpiunpil.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2pjjxzvzq.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2qbehkvsb.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt2gcrmatrd.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt2xhmwsqzl.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2rrnmjbzh.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt2jhsizudf.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2efjcifde.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2dlmwuxok.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2mplaldcs.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt2ykrogxns.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt2msdiqybj.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2mufmgpqz.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt2jfsdjgxr.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt2vwmxvjpd.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2xbbcezdk.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt2shkzhtph.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt2rizkzulf.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt2bdkhcejq.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt2wipdylol.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt2dsndjmic.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt2vkqcvyca.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt2frijmxtu.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt2toymfrgg.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2pebvxvex.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2cmuduokv.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2eazzxjaa.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2bmpcxcyv.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt2urbmzdbq.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt2uwfpdelo.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2dzvxihnh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kzgiqoew.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt2qynwczht.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rvpilebk.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2zinfyxcy.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt2uvrdzpbn.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2vauqvmqg.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2ztpgqwgi.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2xeiykotc.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt2fcttahpc.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt2ewmhwgyg.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt2fvftxcix.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt2bswzkfga.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt2ijxvmnka.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2bhsmcceo.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2bbrmhuot.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt2zmmlgdgc.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt2qmndynow.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt2somgqtit.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt2rdkgsgpy.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2zthpphkr.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt2auytolum.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt2cpxbnsks.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt2rzmchary.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt2efkdwukm.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2ofupsuoa.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2eytsnexu.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2fpoguxgw.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2dvfjysgn.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2telqpunl.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt2imccrfgn.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt2ylkoehgk.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt2ocvbpxnt.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt2msnskasn.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2uaocyzbh.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2leisalra.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2xelfqbfp.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2dvyrtpgh.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2smzjlxpl.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt2khtqolyh.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt2rqjyqbtj.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt2ljazifjw.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt2cqjazwhw.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2wgmkjvbw.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2hkermvzi.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt2mufeiaes.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt2gnsrfyla.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt2okwojcgx.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt2cpgcpxij.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2ukfsuqof.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt2upwzkgqc.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt2zuxpmbpe.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt2avlqgxrv.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt2xphklwig.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt2hsfwpgtf.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt2ebykxpsh.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt2xoxjflfx.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt2mlcjbqhb.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2tiwhmyds.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2gqaeahrp.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt2rvzqmxuy.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2kwbobdmp.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2poblonjd.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt2vmklcydj.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt2ldhoxxyo.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2gutnhhgl.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2ycrawgus.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt2ghalkwye.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt2lqlbnkdu.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt2gsngzuov.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt2brqqiral.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt2iaoasqsa.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt2odecgfze.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt2tybrdycv.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt2oigcjmjh.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt2lrgewkqb.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt2djewwoyl.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2vhrgwoba.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt2kahqlpsc.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2tobbkuna.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2guwqjryc.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt2kyqnrsev.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2qrqaxcna.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2lttpkfdc.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt2yavwizlh.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt2qfjrmnjk.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt2hgkwrnqs.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt2grfbzaka.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt2jhfknknl.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt2fraaomnw.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2pdnphldk.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt2mlnojkcq.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2srmhicua.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2pbxjimlw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wkrawqin.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt2wykidqrt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ojbqhhwf.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2hunvqqtn.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2kmisqgxc.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2pquecjdp.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2typduvdh.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2fswohqop.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2dktwzmpu.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt2zjtfdkuq.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2bycgtphn.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2xacostqr.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt2ykmujrnj.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2hczonslu.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2azpqhfza.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ltbuvbxk.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2yzerxhev.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2inyxckit.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2tapwpcau.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2stqrzqjt.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2ridjxyoy.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2dryyhuvx.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2jitfxpxi.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2hebuossq.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2ckckrrmf.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2xaaibadu.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2wmdomzvg.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2qffelpff.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2samosote.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2tjoaobon.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2uptrzfqh.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2zrucogkr.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2knevhzzr.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2adztzeyd.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2rysekerj.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2aexnywss.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2dnphjkos.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2ushbxuqe.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2zahznfbl.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2jlmtbvxi.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2gnxaayhu.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2dkyrassu.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2zfpateyn.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2rmoawtwt.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2gynhuvzo.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2xwuxqbhh.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2rqnjozqu.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2ejoyxkcb.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2ybyhqank.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2gvganzhb.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2vubhdhig.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2cywkrdkj.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2gcapdgjl.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2cokdvcwd.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2oywaihbo.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2nwwtxdpi.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2vssfhewt.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2heusiior.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2mpvaixfy.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2dnbjjpxs.html


<!-- 参考信息 -->