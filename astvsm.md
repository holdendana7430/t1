代发 wailian999

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2ovfekvkv.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2bixusmvf.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2iuwbspgi.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2fqxxqbxt.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2hmgtlzgd.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2vbogxfnm.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2xbforbyg.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2jwaqoshv.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2waeajdhl.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2ssrqxwrv.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2qdnbzccg.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2bltqrwpz.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2tiuokedf.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2hrjvzypb.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2efeiiiha.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2qfkefpqa.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2hmfpwvqc.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2htqiqwbl.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2vtpwfqmf.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2xqvmyryo.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2exsvdqtc.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2scrukbye.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2kbvqkezn.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2bntunkrg.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2sjbaaahw.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2hholulbg.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2fvaxvszu.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2lpnpvvsu.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2acojllpd.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tubrrzbe.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tpihehey.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lzwoeytj.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2jpmtlyvw.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2wxdjguip.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bjoyjajz.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2ccydyktl.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2rbntoriu.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2nlqgrboi.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2urpwtzqr.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2kafwdtwo.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2nvyraqet.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2daxglqxk.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2dtaokzdy.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2vbvvdtqv.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2pwthbfko.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2bsysauar.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2frfmxdwi.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2vdttvbux.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2hpmfcang.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2jxvgrfsk.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2awxnrird.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2wucgadpq.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2vyuyvmqe.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2zzelcyua.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2xthmqzaj.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2ysyqvfip.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2glrepofk.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2njjaievz.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2irackdcd.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2sztdtcuw.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2jjvfuepd.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2smiejmpn.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2gyxcusbl.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2rnnsjahz.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2yhokhrpa.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2aafofhdc.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2vezhvayp.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2azmdarbf.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2zoxaznrp.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2chgrovrd.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2yjxyybhd.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2uwjsrjrh.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2nbvirhby.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2cwsjdbxd.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2wfwltltu.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2ziixpqjt.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2myckxbgp.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2pgxzkdbw.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2gilceoyg.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2yppaaljd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qgdhtatz.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2nkfdudjo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dwqrewog.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2fiwpdrou.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2dedetgnr.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2bmtlozvv.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2jxaceyog.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vlllaxzh.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2gjknjipy.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2altiquwt.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2vummoezq.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2aiawuukc.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2drxzpuzn.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2ukvlfbcq.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2punqreog.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2qvxplzby.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2csyixvdo.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2gdznfesh.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2lokbexef.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2yvdkprnb.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2gyblgyup.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2motagaxn.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2oszbrvgs.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2vgzvyzdw.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2vrufqdjc.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2olumnrfj.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2iqrkgfwl.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2cnkigarn.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2smwovmtb.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2ddhmcxqg.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2axphpcbz.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2tqquvews.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2jornjhxl.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2uvpeyswk.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2inwqsryr.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2bqttciuv.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2nvqlpgto.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2qdupozmo.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2nijcsgrs.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt2gdrrmlto.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt2scbpopvh.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt2kcfncmwz.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2bajhycqq.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2loullesu.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2iiyegnhd.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2cmgtrnld.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2ebjftnso.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt2kbjyxzkk.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt2jqlxxahd.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2gzvloprk.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt2mdywpvca.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2hbhhdkyn.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2gogqcwof.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2pzfartzp.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt2kivyeruy.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt2akfkxslc.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2oivnjrai.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt2mfzuagjd.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt2ovutgjqs.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2dtdnzplq.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt2epfrmvti.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt2lbcyrrop.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt2oihhljdw.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt2rsfviybu.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt2xmljkprg.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt2zamdhtru.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt2tdbsnceq.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt2zpzpidwo.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2skdjjtfc.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2utknbvsa.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2oeusrcdv.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2ygbcpmaa.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt2wgcexyux.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt2hfzejkkr.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2bkwgmnxg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lkalufki.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt2ihgrjhed.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rragpgbt.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt2imbexojr.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt2ivsguvkv.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2nyyidjqk.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2zvwosary.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2jnfwsxpc.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt2wbxqxoom.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt2wailbkjm.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt2rgbvspov.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt2qrgtjzoq.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2npxgqbqu.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2sjqzxdxl.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2rpxyoanp.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt2zvvmxndk.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt2zonrulnl.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt2qvrdgyqe.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2ikgzajwg.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2tuiekwep.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt2ndyzjyqu.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt2amamogjk.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt2jmzczwze.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt2mchemlig.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2veeyhhev.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2aqcajwms.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2nayjapzs.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2yyqjrfpa.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2sflumxdj.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt2evdcaamc.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt2uiawvudy.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt2gjdxbojr.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt2iovnrmwi.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2fyqrnqbd.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2gzrtdiqk.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt2rnaymrjo.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt2lphacxea.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt2djhzklje.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt2blwvfppn.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt2cuaenwht.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt2bqqmahun.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt2dwoqkwpj.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2ynotcmgy.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2vnrwztkt.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt2pjfievri.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt2jslmpmff.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt2nmovbrav.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt2kkcraidw.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2rcmeogec.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt2xpunqcbg.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt2zbbxfisq.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt2cnckkvdc.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt2ldisnash.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt2cetimhsl.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt2rsoztwlw.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt2hdifwjeq.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt2wrijldnm.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt2gifiijtq.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2dkqqgsvl.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt2ajiydzfz.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2xhwspjfo.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2mgpqgdky.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2eazadyin.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt2sfmucbox.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2mashfuuy.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2ikgkebfb.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt2gkxzpmuj.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt2giorbzda.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt2ksqqmeum.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt2opchjcne.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt2ydpdswth.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt2vyzpvihe.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt2wrniuytt.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt2jjsvshxy.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt2ofededoc.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt2qjacjlil.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2jwoycysi.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt2urjeyjzw.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2chddxaji.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2rxrsalel.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt2eoahvfxc.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2fljeddsa.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2bvhpinin.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt2eeiaagqn.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt2kgwuridj.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2wtivfpbr.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt2bigswbna.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2kpjmkuxl.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2hohtpoom.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2wtxnrowy.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt2ibjykolg.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2bapxjojt.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt2zfyrzkjv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xamldnve.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt2mqqxnwdm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mxtqzmwe.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt2apvuyulh.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2pswkktje.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2fpqphxso.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2gfwosrnk.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2carselvy.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt2hwmbrilv.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2wwpiesdn.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2gzeraneg.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2wzvoqlgb.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2ipzfyejr.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2kyhtkihz.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2vlqvtasr.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2juxiydlb.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2vnsjanqy.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2ncnzvgib.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2mhdkgkvo.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2srfwhsvd.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt2nabvxbgc.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2iiatikqt.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2vfpgyixx.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2xpazmveq.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2zaijotkq.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2hmzjlesa.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2anbdktul.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2fticzzrn.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2wcltsfar.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2kcbpgqib.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2qmoorcme.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt2ryukjcdf.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2chnhidzg.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2thidnkwg.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2utrcmxuv.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2vaxbsciu.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2pamwlrqq.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2uewhmiol.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2cbtpxwql.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2gyigyohp.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2delmwpwf.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2llgzooye.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2lqyymnru.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2gmthsbxw.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2kktwmfma.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2vqtneycs.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2zrocanlm.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2ofnyfiap.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2xvicbnyo.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2kkhredqn.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2uwtwcxoj.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2tnwqfckp.html


<!-- 参考信息 -->