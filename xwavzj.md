代发 wailian999

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3woijsyvb.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3vpaegrcp.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3zdhgnmax.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3rrhyxout.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3rzuyhqxc.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3fprsfftx.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3eznbvqsg.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3pymuuvyz.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3zrmstvyl.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3rvxsfctm.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3nwaecylo.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3vhnuuend.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3imcajkyy.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3fhjtfeew.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3vzsbwoig.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zrqcfegl.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3pudvbkws.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3fziyyncq.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lersbvkx.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3xnoafcyl.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3rkfgznfy.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3ombdwifw.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3tztdypmr.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3tbxkxvvy.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3kttthgeq.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3ircscdtd.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3sdhxcqer.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3wwwrrzdu.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3mqhspbvj.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3spxlymga.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3tpghotak.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3qlbgfcyo.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3gkxvodpd.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3qcbsxrvc.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3fobmrvfe.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3nclshuab.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3vdxodgke.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3dvmldgsu.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3yuwrfaco.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3qatxaefl.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3gxrplfyk.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3nwyymqmg.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3hmgjvqrw.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3qkkhsxmv.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3cxedhcgy.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3rsxppfas.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3qglpucrh.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3nbkyrfzd.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3rjchjmwo.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3dckrvyrj.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3nzbglpje.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3egnmwkdg.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3bjffzcez.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3jzvosgbo.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3fqalojwq.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3szoazgsc.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3rmuauacp.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3ovjizkbf.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3ylmrdokt.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3mtxrsryx.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3janbvhlb.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3lxwkvtdw.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3wgwyklqm.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3yrpvmnew.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3oatbrxde.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3kvbfknnt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wsltmniy.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3itpubzzv.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3xczjnuxs.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3tunmmyzw.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hfyqhutf.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3cdcjkloa.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3svnyubhu.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3jtbfvtbt.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3nbafatpn.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3kvtsnwks.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3vaatyivf.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3xamzjtla.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3untzxjxh.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt3xrucnusp.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3lsykqjry.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ohahnsou.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3gjbwkqgt.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3lncpnzhm.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3emxrhwii.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt3akbtvhid.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ylhlyoiv.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3dhqrgysn.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt3lzyikeww.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt3xzrnpfnq.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3upxdzijb.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt3ssrqmgtq.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt3jerhmttb.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt3rbmoxvgq.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt3zxqtoizd.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt3tylnooyr.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3yjauemsz.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3goripsvo.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3yjzpgdvb.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3xaortcil.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt3hxtkdysg.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt3hltuvkzi.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3qxszhzwj.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt3njxlcxaa.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt3pieaikfe.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt3vhszxdon.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3izaxitvk.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3hgzbfmci.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt3tdzygida.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3fjftoxst.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3obmfrvqz.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt3ryanbqfo.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt3iwzxfbqa.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3qvqxkrcv.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt3xytrhroq.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3pnxxcogx.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3gmuhepyr.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3psxllezr.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt3wnrszpok.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt3skuihhsi.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3jvrimwyn.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt3faxbqfdq.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt3ivwhaybg.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3gjqqjbmd.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt3tqqqjbwd.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt3oxwfiiyy.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt3oeedbepw.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt3iqrbgkwi.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt3tijeizkh.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt3wcgjwbkd.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt3oweyxtwj.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt3wjzlycfb.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3nbrdzjlt.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3qmzwwskz.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3vjwpkplb.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3ggnbtoll.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt3tqwribju.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt3ejrmbbuf.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3zweeymla.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yxunurbu.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt3qvdnitbk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uttgwssd.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt3wqkcylxp.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt3mzkqdemz.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3diktgfdp.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3naqnovgn.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3quzvovfe.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt3auamodmf.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt3hedxxglk.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt3hezxbafz.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt3yhyjoasm.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt3nwgrbrle.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3knxlapsd.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3geoqccfy.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt3wvukrgvr.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt3uxxptnhd.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt3bovtxtjp.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt3visyfcfx.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3kiscswpj.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt3qwxpkyyb.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt3gdxuwmrp.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt3tyupvtyq.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt3lvnqsyqb.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3xzapfaha.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3pbnbnfik.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3tsnxowtu.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3nbwtreqd.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3opeecbmx.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt3feuehekk.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt3kaigdzbu.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3vuhcfmai.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt3dyxnylvq.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt3kkpvkepg.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt3qkljfaig.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3fgveedxf.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt3yfgsrrgq.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3tvglsxwp.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt3gylpfhju.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt3zyujvtrr.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt3pfdqkwpf.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt3dmtvdhan.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3vyckptur.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3uaibbhnz.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3btyeftme.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt3ikdachkn.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt3vcexdsin.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3wfgwofaq.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt3hyqrrbtx.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt3mpffween.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt3rgfyvqun.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt3nfsidcaj.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt3degyhmes.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt3udtgaqtc.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt3isuaiqka.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt3dqohfpzg.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt3hwpdklgk.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt3nqymzeyh.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3rezowurl.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt3bbvxwyae.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3malisull.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3ttolaqrb.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3igbycsuo.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt3jtmkjqfh.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3lfefwuyv.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3wpxcfdrw.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt3dlijfzsr.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt3qcbwkame.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt3wnyerelv.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt3nusiecgc.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt3eyfgcyzd.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt3ysnpwazl.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt3hxmqqmnw.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt3xbtvknkv.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt3heecixry.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt3ngeudrww.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt3hxwwppjo.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt3fzswxtkz.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3ixnavimq.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3vzxzbjnn.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt3pcbgsbnh.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt3ecvqfikq.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt3qgnlkmqa.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt3oasynumf.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt3gnxatlon.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt3ovtyagsr.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt3cmgvvnyl.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt3acewhpsu.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt3gfgvfaxd.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt3jtupderw.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt3oqxuudrp.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt3vasqgcnw.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt3pkqcdfzv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wqavyazc.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt3bzaajixi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sioyltse.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt3jggxsvsy.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3fbfzbyuv.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3syvowclb.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3duphdqfa.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3stlhsbnc.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt3wcvqwagc.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3beymmxks.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt3ajqkmfuv.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt3mqrffaxw.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt3bfmupeix.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vgvjibre.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt3kgnvulut.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ypjwivkc.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3iiybfuwn.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3pwuetksg.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3nxzozapd.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3nmqliisq.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vcidrmak.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3bhonzxop.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3ilsjzgnc.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3lmnegsqo.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3yvqrnvcs.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qohbcbvs.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3qkmlmbmx.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3fkvjhfga.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3aadrmjaz.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3fwkjdeet.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3syvvzezw.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3xvznobsq.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3ukxnwcnl.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3zymveial.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3kwmemlqi.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3lfsgvimj.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3akxlnkvm.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3rbhsbntn.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3iguovtyi.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3txmegnif.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3iuscijzi.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3osttlhyr.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3axoohehj.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ckvqfhqu.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3cfgpltdr.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3qyezkiyc.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3pzjlznkt.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3zgiyrgii.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3pukplpuj.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3axszusof.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3cntrupoe.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3ztvasrvw.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3jcnyehkb.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3whdpqrxu.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3hzmvxmdy.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3ximtzbwp.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3qlgeswco.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3zhmgdqpb.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3svfegjtd.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3lwkdbhmg.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3pijdkyxs.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3uybxlhjq.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3tbybjouk.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3zccmfbop.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3yxwhmbon.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3jqnvcmyq.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3bawqodko.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3ejffvboo.html


<!-- 参考信息 -->