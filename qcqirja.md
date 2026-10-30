代发 wailian999

[H03] 主动抛出异常
来源：http://baike.hesvh.cn/Article/details/gjtkygndl.sHtML

Py:   raise ValueError("错误信息")
来源：http://baike.zdbjq.cn/Article/details/godoghqtk.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.hesvh.cn/Article/details/gsivorscj.sHtML

JS:   throw new Error("错误信息");
来源：http://wap.fehbvm.com/Article/details/gqliicmeb.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.hesvh.cn/Article/details/gqqmdrfmw.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://m.share.zdbjq.cn/Article/details/ggcrkvnkk.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://3g.hesvh.cn/Article/details/gksjjmddm.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://mobile.hesvh.cn/Article/details/ghofpjebw.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://blog.fehbvm.com/Article/details/gykuvlntn.sHtML

[H04] 自定义异常类型
来源：http://www.blog.fehbvm.com/Article/details/gpmoiywiz.sHtML

Py:   class MyError(Exception): pass
来源：http://baike.fehbvm.com/Article/details/grsvgzglo.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://m.share.fehbvm.com/Article/details/gzwknkvoj.sHtML

JS:   class MyError extends Error {}
来源：http://3g.fehbvm.com/Article/details/gwtthoaub.sHtML

TS:   class MyError extends Error {}
来源：http://m.share.fehbvm.com/Article/details/glbpuqasa.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.share.fehbvm.com/Article/details/gghiciodg.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.blog.hesvh.cn/Article/details/gsfiwnqdv.sHtML

Ruby: class MyError < StandardError; end
来源：http://3g.fehbvm.com/Article/details/gfnwcoldm.sHtML

C#:   class MyException : Exception {}
来源：http://baike.fehbvm.com/Article/details/gnwtubkbd.sHtML

[H05] 捕获特定类型
来源：http://wap.hesvh.cn/Article/details/gvbcbxiuh.sHtML

Py:   except ValueError as e:
来源：http://blog.zdbjq.cn/Article/details/ghmtfcrbe.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.blog.fehbvm.com/Article/details/ghrinpcds.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://baike.zdbjq.cn/Article/details/gdbpldysz.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://mobile.zdbjq.cn/Article/details/gppctanbl.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://m.share.hesvh.cn/Article/details/gvrfoyfvg.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://m.share.zdbjq.cn/Article/details/giymwxmax.sHtML

Ruby: rescue ArgumentError => e
来源：http://blog.hesvh.cn/Article/details/gfkhkwyuc.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.share.hesvh.cn/Article/details/gswddgtrn.sHtML

[H06] 可选值 / 空值安全访问
来源：http://blog.zdbjq.cn/Article/details/gvkyqjeek.sHtML

Py:   value = d.get("k") or default
来源：http://m.share.fehbvm.com/Article/details/glhkkwljb.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://m.share.zdbjq.cn/Article/details/gfubxpigx.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://read.share.fehbvm.com/Article/details/ggcffjoac.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://m.share.fehbvm.com/Article/details/gjcjssoam.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://3g.fehbvm.com/Article/details/gimmfmnzj.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.m.share.hesvh.cn/Article/details/gevxuwsbg.sHtML

Ruby: d&.dig(:a, :b)
来源：http://m.share.zdbjq.cn/Article/details/gdotrazej.sHtML

C#:   obj?.A?.B ?? default
来源：http://wap.fehbvm.com/Article/details/gdzunlnja.sHtML

[H07] 断言
来源：http://www.share.hesvh.cn/Article/details/gsqmkeybg.sHtML

Py:   assert x > 0, "必须为正"
来源：http://blog.zdbjq.cn/Article/details/goohvnaho.sHtML

PHP:  assert($x > 0);
来源：http://wap.hesvh.cn/Article/details/gjyfijuxm.sHtML

JS:   console.assert(x > 0);
来源：http://www.share.hesvh.cn/Article/details/gjolxhnym.sHtML

TS:   console.assert(x > 0);
来源：http://blog.zdbjq.cn/Article/details/gayroetuh.sHtML

Java: assert x > 0 : "必须为正";
来源：http://baike.fehbvm.com/Article/details/gyvjpqzdm.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.blog.zdbjq.cn/Article/details/ghstpmaov.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.share.fehbvm.com/Article/details/gcxhlxogq.sHtML

C#:   Debug.Assert(x > 0);
来源：http://read.share.hesvh.cn/Article/details/gehytqnkg.sHtML

[H08] 获取错误信息与堆栈
来源：http://m.share.zdbjq.cn/Article/details/gqixcbgbz.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://baike.hesvh.cn/Article/details/gmeuaznxh.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.share.zdbjq.cn/Article/details/gfwgylmeg.sHtML

JS:   e.message;  e.stack
来源：http://www.m.share.fehbvm.com/Article/details/gwgvnwrnn.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://mobile.fehbvm.com/Article/details/ghvwnuzyy.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://m.share.zdbjq.cn/Article/details/giznoyaah.sHtML

Go:   err.Error()
来源：http://baike.hesvh.cn/Article/details/gouifikkt.sHtML

Ruby: e.message;  e.backtrace
来源：http://3g.fehbvm.com/Article/details/gxsouuedu.sHtML

C#:   e.Message;  e.StackTrace
来源：http://wap.fehbvm.com/Article/details/gdxcpuvlt.sHtML

[H09] 带错误码的异常
来源：http://mobile.hesvh.cn/Article/details/ggmochuwt.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.share.hesvh.cn/Article/details/gnyfimxey.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://blog.zdbjq.cn/Article/details/gmutsegrr.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://3g.zdbjq.cn/Article/details/gjfmuljyy.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mobile.fehbvm.com/Article/details/gwqhqcrjq.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.m.share.fehbvm.com/Article/details/gyfbnbhav.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mobile.hesvh.cn/Article/details/gnexhzsza.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://wap.fehbvm.com/Article/details/gudjntnrq.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.blog.fehbvm.com/Article/details/gnkkewaak.sHtML

[H10] 资源自动释放
来源：http://wap.hesvh.cn/Article/details/girjcxpin.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://mobile.hesvh.cn/Article/details/gzeuylimg.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://baike.fehbvm.com/Article/details/gcsvutisq.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.fehbvm.com/Article/details/grkkadhkg.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.fehbvm.com/Article/details/gvlunyctj.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://baike.hesvh.cn/Article/details/gmylqvrar.sHtML

Go:   defer f.Close()
来源：http://mobile.fehbvm.com/Article/details/gqfpurfdv.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://3g.hesvh.cn/Article/details/gkoxvrhdp.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://3g.fehbvm.com/Article/details/gfqyfjbyj.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gkavnqtor.sHtML

I. 正则表达式
来源：http://www.m.share.hesvh.cn/Article/details/gmxqqyeyx.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gkupfvlln.sHtML

[I01] 判断是否匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gaejyqmax.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://blog.hesvh.cn/Article/details/gsmbfgjsg.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.share.zdbjq.cn/Article/details/gnobgpfhe.sHtML

JS:   /\d+/.test(s)
来源：http://www.m.share.hesvh.cn/Article/details/gswydwfyf.sHtML

TS:   /\d+/.test(s)
来源：http://m.share.fehbvm.com/Article/details/gspyvthju.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://m.share.fehbvm.com/Article/details/gydhopzru.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mobile.zdbjq.cn/Article/details/gjqykiudv.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.share.fehbvm.com/Article/details/gczxcissx.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://3g.hesvh.cn/Article/details/gdzozsmui.sHtML

[I02] 提取所有匹配
来源：http://www.share.zdbjq.cn/Article/details/ggamhylfh.sHtML

Py:   re.findall(r"\d+", s)
来源：http://read.share.fehbvm.com/Article/details/gslvfuvlj.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://m.share.hesvh.cn/Article/details/gfheieojp.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wap.zdbjq.cn/Article/details/ggsvqpzjf.sHtML

TS:   s.match(/\d+/g)
来源：http://blog.hesvh.cn/Article/details/ghdtuqbtq.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mobile.fehbvm.com/Article/details/gevwhwcyp.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wap.hesvh.cn/Article/details/ghsjaelur.sHtML

Ruby: s.scan(/\d+/)
来源：http://3g.hesvh.cn/Article/details/glogdxgui.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wap.fehbvm.com/Article/details/gfpzlbvgo.sHtML

[I03] 提取捕获分组
来源：http://mobile.fehbvm.com/Article/details/guxdnwbxx.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://baike.zdbjq.cn/Article/details/galsidfhr.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://read.share.zdbjq.cn/Article/details/gmrkvfmxn.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wap.zdbjq.cn/Article/details/gwzepvbuk.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.share.zdbjq.cn/Article/details/gzwgusiaw.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.blog.fehbvm.com/Article/details/gkdjivrcr.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wap.fehbvm.com/Article/details/gnkhadiav.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://baike.hesvh.cn/Article/details/glmqywprf.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.share.hesvh.cn/Article/details/gxandaheu.sHtML

[I04] 正则替换
来源：http://3g.hesvh.cn/Article/details/gzaghbnqx.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://m.share.zdbjq.cn/Article/details/gtnyfaheq.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gfdwtznbh.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://wap.fehbvm.com/Article/details/gcjppsrvv.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://baike.hesvh.cn/Article/details/gbgsmhckj.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://baike.fehbvm.com/Article/details/gmgmeqlda.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.blog.zdbjq.cn/Article/details/ggtoiypkx.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.share.fehbvm.com/Article/details/glxnonzpv.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://blog.hesvh.cn/Article/details/gxdgtikwg.sHtML

[I05] 按正则拆分
来源：http://m.share.zdbjq.cn/Article/details/goijpgegz.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://m.share.hesvh.cn/Article/details/gxhooxufr.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://3g.fehbvm.com/Article/details/gguojwtas.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.m.share.fehbvm.com/Article/details/gsnpyhtjj.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://3g.fehbvm.com/Article/details/gkxxslouc.sHtML

Java: s.split("\\s*,\\s*")
来源：http://mobile.zdbjq.cn/Article/details/ggoyxmppi.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://baike.fehbvm.com/Article/details/gsyobqbig.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.share.hesvh.cn/Article/details/gckzruhne.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://baike.zdbjq.cn/Article/details/gnohitcfg.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wap.hesvh.cn/Article/details/gsrxzhnfx.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://m.share.zdbjq.cn/Article/details/gyxzmvedr.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.m.share.zdbjq.cn/Article/details/gfuukvzpr.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.hesvh.cn/Article/details/gklkjycif.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.zdbjq.cn/Article/details/gcqmfssie.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://3g.fehbvm.com/Article/details/gborcuzwy.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.blog.zdbjq.cn/Article/details/ggznqqoel.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.share.hesvh.cn/Article/details/goensmvff.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://3g.fehbvm.com/Article/details/gacqwdlkf.sHtML

[I07] 忽略大小写与多行模式
来源：http://blog.hesvh.cn/Article/details/gauphdtbr.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.m.share.zdbjq.cn/Article/details/ggknwbapd.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://read.share.hesvh.cn/Article/details/gprmpingu.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wap.hesvh.cn/Article/details/gbpopgdtn.sHtML

TS:   /error/gim
来源：http://baike.fehbvm.com/Article/details/gasregxbq.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://baike.zdbjq.cn/Article/details/gkmjvdgtc.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.share.zdbjq.cn/Article/details/gxpxarszt.sHtML

Ruby: s.scan(/error/i)
来源：http://www.share.zdbjq.cn/Article/details/guhumioza.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.share.hesvh.cn/Article/details/gsvryeieu.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://baike.fehbvm.com/Article/details/gtnbdelra.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wap.zdbjq.cn/Article/details/gqljfjkem.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.share.zdbjq.cn/Article/details/gadfcvyai.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.zdbjq.cn/Article/details/gpkltvebf.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.fehbvm.com/Article/details/gaytnicvm.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://mobile.zdbjq.cn/Article/details/gjbxpklcj.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wap.fehbvm.com/Article/details/gkldbabyz.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://baike.fehbvm.com/Article/details/gvfcwjhup.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://m.share.zdbjq.cn/Article/details/gbbotujsw.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/goeqhvawd.sHtML

J. 日期与时间
来源：http://baike.hesvh.cn/Article/details/gknoebtzv.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/ggorjjrhs.sHtML

[J01] 获取当前时间
来源：http://mobile.zdbjq.cn/Article/details/gghiemdwc.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://blog.fehbvm.com/Article/details/gwxlirtcd.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://read.share.hesvh.cn/Article/details/gjkswjhkk.sHtML

JS:   new Date();  Date.now()
来源：http://m.share.hesvh.cn/Article/details/gygklkxqa.sHtML

TS:   new Date();  Date.now()
来源：http://blog.fehbvm.com/Article/details/gruiomzdk.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://3g.fehbvm.com/Article/details/glehhhmkt.sHtML

Go:   time.Now()
来源：http://baike.hesvh.cn/Article/details/gltoykgby.sHtML

Ruby: Time.now
来源：http://www.share.hesvh.cn/Article/details/gczpwjtrx.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wap.hesvh.cn/Article/details/gjympgifd.sHtML

[J02] 格式化输出
来源：http://read.share.zdbjq.cn/Article/details/gioneiwut.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.fehbvm.com/Article/details/gdarnqdwj.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.share.hesvh.cn/Article/details/gnshpjzio.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.share.zdbjq.cn/Article/details/gcqihclak.sHtML

TS:   d.toISOString()
来源：http://m.share.fehbvm.com/Article/details/gfzlwsuoh.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.share.zdbjq.cn/Article/details/guqgdvpso.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://m.share.hesvh.cn/Article/details/gxolnobim.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.hesvh.cn/Article/details/gnidgdjuy.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wap.zdbjq.cn/Article/details/gjqwjbuyz.sHtML

[J03] 字符串解析为日期
来源：http://www.share.zdbjq.cn/Article/details/gblyvwuyn.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://read.share.hesvh.cn/Article/details/gmsvgkbpe.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://3g.hesvh.cn/Article/details/gjfvdhzik.sHtML

JS:   new Date("2024-01-02")
来源：http://www.blog.hesvh.cn/Article/details/giyizrdxq.sHtML

TS:   new Date("2024-01-02")
来源：http://3g.zdbjq.cn/Article/details/gxmnedjpb.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.blog.zdbjq.cn/Article/details/ghuqoxhwx.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://m.share.zdbjq.cn/Article/details/gddhkccix.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://wap.fehbvm.com/Article/details/gjiivpkao.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mobile.hesvh.cn/Article/details/gbglyedlq.sHtML

[J04] 时间戳与日期互转
来源：http://www.blog.fehbvm.com/Article/details/gyqojiuvy.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.share.hesvh.cn/Article/details/gjmxuzsvd.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://baike.hesvh.cn/Article/details/gkqbilugj.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://blog.hesvh.cn/Article/details/ghlnxrzhn.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://baike.hesvh.cn/Article/details/gwrdwulqo.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.share.fehbvm.com/Article/details/ghmcvnjph.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.blog.zdbjq.cn/Article/details/guulpeyub.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.blog.zdbjq.cn/Article/details/ggbjdxjjm.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wap.fehbvm.com/Article/details/ggbkrlrre.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.m.share.fehbvm.com/Article/details/gzjxmcnam.sHtML

Py:   now + timedelta(days=7)
来源：http://blog.zdbjq.cn/Article/details/gtmrdwnhb.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://3g.fehbvm.com/Article/details/grhdczbph.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.zdbjq.cn/Article/details/gdbpsfddc.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.fehbvm.com/Article/details/gdpeuxhhw.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://read.share.hesvh.cn/Article/details/gucjzcxht.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://blog.hesvh.cn/Article/details/gqcxkocqe.sHtML

Ruby: Time.now + 7 * 86400
来源：http://baike.hesvh.cn/Article/details/gahstadvs.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.share.hesvh.cn/Article/details/ggoutscee.sHtML

[J06] 计算两时间之差
来源：http://m.share.fehbvm.com/Article/details/gytyedctz.sHtML

Py:   (end - start).total_seconds()
来源：http://www.blog.zdbjq.cn/Article/details/gzfcodpst.sHtML

PHP:  $end->diff($start)->days;
来源：http://3g.zdbjq.cn/Article/details/gbadypsyw.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://m.share.fehbvm.com/Article/details/gafvsikhu.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wap.zdbjq.cn/Article/details/gbvplbaiw.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://m.share.hesvh.cn/Article/details/gfpslxfuw.sHtML

Go:   end.Sub(start).Hours()
来源：http://wap.zdbjq.cn/Article/details/gthbixvly.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.m.share.fehbvm.com/Article/details/gehqsrvkh.sHtML

C#:   (end - start).TotalSeconds
来源：http://baike.fehbvm.com/Article/details/grjqmyaws.sHtML

[J07] 比较两个日期
来源：http://www.m.share.zdbjq.cn/Article/details/gtmytmxpn.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://baike.fehbvm.com/Article/details/gfcmzxbkc.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://baike.hesvh.cn/Article/details/gtwiagnzy.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://mobile.fehbvm.com/Article/details/gxrhbrmtb.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://mobile.zdbjq.cn/Article/details/ggzvzunpe.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://3g.zdbjq.cn/Article/details/gnecrytml.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.m.share.hesvh.cn/Article/details/gthrwxbrc.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://baike.zdbjq.cn/Article/details/gciffrrnn.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://baike.fehbvm.com/Article/details/gdzowpwey.sHtML

[J08] 提取年月日与星期
来源：http://3g.fehbvm.com/Article/details/gedxpwoqh.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://m.share.hesvh.cn/Article/details/ganvjvadk.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://m.share.zdbjq.cn/Article/details/gpxeqkmfn.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://m.share.zdbjq.cn/Article/details/gluirxrjf.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.blog.zdbjq.cn/Article/details/gjhfxztiw.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://3g.hesvh.cn/Article/details/gyjplpwmo.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://read.share.fehbvm.com/Article/details/gehlcaazh.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wap.hesvh.cn/Article/details/gaqhftoua.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wap.fehbvm.com/Article/details/guvoiqslc.sHtML

[J09] 时区处理
来源：http://blog.hesvh.cn/Article/details/gkgwlihzy.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.blog.zdbjq.cn/Article/details/glcmesaqk.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wap.zdbjq.cn/Article/details/glngcerkq.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.hesvh.cn/Article/details/gygvmowxz.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.fehbvm.com/Article/details/gdadgoght.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://blog.hesvh.cn/Article/details/gxtytgjeq.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.blog.zdbjq.cn/Article/details/gewmjpsly.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://mobile.fehbvm.com/Article/details/gtbwncikv.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://3g.hesvh.cn/Article/details/gaupbgmgg.sHtML

[J10] 取今天 / 本月第一天
来源：http://wap.zdbjq.cn/Article/details/gnllimfaw.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.share.zdbjq.cn/Article/details/gsgxpavgq.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://3g.hesvh.cn/Article/details/gxwjzkqom.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://3g.hesvh.cn/Article/details/guytjrqga.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.share.fehbvm.com/Article/details/gwlmmuyjm.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.m.share.hesvh.cn/Article/details/gvcfbtpcu.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://read.share.fehbvm.com/Article/details/gartekvud.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://baike.fehbvm.com/Article/details/gbxlzqsiq.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://read.share.fehbvm.com/Article/details/gkrkisied.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gpwwxhgsy.sHtML

K. JSON 与序列化
来源：http://m.share.fehbvm.com/Article/details/gaadiidef.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gpiypjfgc.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.blog.hesvh.cn/Article/details/gjxuzbmxk.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://baike.zdbjq.cn/Article/details/gmivfhcps.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://read.share.zdbjq.cn/Article/details/gwxqgrary.sHtML

JS:   JSON.stringify(obj)
来源：http://mobile.fehbvm.com/Article/details/gmkwanrul.sHtML

TS:   JSON.stringify(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gzpgysvsc.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://3g.fehbvm.com/Article/details/glslovymh.sHtML

Go:   json.Marshal(obj)
来源：http://blog.fehbvm.com/Article/details/gqckdpoky.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://m.share.fehbvm.com/Article/details/geyqofsem.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gdlhfhwho.sHtML

[K02] JSON 字符串转对象
来源：http://m.share.hesvh.cn/Article/details/gcvidengq.sHtML

Py:   json.loads(s)
来源：http://wap.fehbvm.com/Article/details/gmcdbjvtu.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://3g.zdbjq.cn/Article/details/grkkqxrsh.sHtML

JS:   JSON.parse(s)
来源：http://baike.hesvh.cn/Article/details/gmapqvgio.sHtML

TS:   JSON.parse(s)
来源：http://www.share.hesvh.cn/Article/details/gvaxpsbkd.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mobile.fehbvm.com/Article/details/ghmzpgzdt.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://m.share.hesvh.cn/Article/details/goubekyej.sHtML

Ruby: JSON.parse(s)
来源：http://m.share.fehbvm.com/Article/details/gojdltsno.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gmpfrlkcr.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.blog.hesvh.cn/Article/details/gzwfwddsd.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://baike.fehbvm.com/Article/details/grrdszwnl.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.share.hesvh.cn/Article/details/gnixdojxv.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://m.share.hesvh.cn/Article/details/gwsbfhsgt.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://wap.zdbjq.cn/Article/details/gihodhvlc.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://m.share.hesvh.cn/Article/details/ggqcelzrv.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.blog.hesvh.cn/Article/details/gadxwvuqw.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gixbrbhfh.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://m.share.zdbjq.cn/Article/details/gkolitwfe.sHtML

[K04] 读取 JSON 文件
来源：http://m.share.fehbvm.com/Article/details/gtbtedxhb.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://3g.zdbjq.cn/Article/details/gqrwqzagh.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wap.fehbvm.com/Article/details/gysnkxors.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.zdbjq.cn/Article/details/gszpqwpkv.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.zdbjq.cn/Article/details/gedocgpuy.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.share.hesvh.cn/Article/details/gkcmzaudo.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.m.share.hesvh.cn/Article/details/goezbtclo.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://read.share.fehbvm.com/Article/details/gbeidqbmb.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.blog.fehbvm.com/Article/details/gpvkilhev.sHtML

[K05] 深拷贝对象
来源：http://baike.hesvh.cn/Article/details/gdccmxiog.sHtML

Py:   copy.deepcopy(obj)
来源：http://baike.zdbjq.cn/Article/details/gwkpknmfv.sHtML

PHP:  unserialize(serialize($obj));
来源：http://3g.hesvh.cn/Article/details/gmaqxhahw.sHtML

JS:   structuredClone(obj)
来源：http://read.share.fehbvm.com/Article/details/gdkrfbrgo.sHtML

TS:   structuredClone(obj)
来源：http://m.share.zdbjq.cn/Article/details/gtmukeoxk.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.blog.hesvh.cn/Article/details/gxffewbvd.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://read.share.zdbjq.cn/Article/details/gjtsojzxt.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://baike.zdbjq.cn/Article/details/grxyrvexj.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://blog.hesvh.cn/Article/details/gcmzmhxtl.sHtML

[K06] 解析 URL 查询串
来源：http://www.m.share.zdbjq.cn/Article/details/gzyozqmem.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://baike.hesvh.cn/Article/details/gixgvjsek.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.m.share.zdbjq.cn/Article/details/grjqckifb.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.fehbvm.com/Article/details/gxblahvfy.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.hesvh.cn/Article/details/gxzkpiuoo.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://3g.zdbjq.cn/Article/details/gpxwracmt.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.share.fehbvm.com/Article/details/gchprfbej.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://blog.fehbvm.com/Article/details/gqjzeylrl.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mobile.zdbjq.cn/Article/details/gafahinbt.sHtML

[K07] 进制转换
来源：http://www.share.zdbjq.cn/Article/details/gvcwfghqr.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://baike.zdbjq.cn/Article/details/gwlxzqvkz.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://read.share.fehbvm.com/Article/details/gxvanqogf.sHtML


<!-- 参考信息 -->