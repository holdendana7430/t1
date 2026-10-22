代发 wailian999

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2jthmwngk.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2zdqbreya.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2bmuaevai.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2dtujbuft.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2ztmyywpg.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2fqhmyvka.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2bsmulwmz.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2teygkgri.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2opqbcnsy.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2udkakuxs.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2jzfqbvxy.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2nogrhznn.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2cbbfqvko.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2lfgokqzu.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2fxxxdwme.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2pmfmqica.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2upsofnbc.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2ronliduq.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2vwcsnkwf.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2mwtkqjps.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2pqbmrdoi.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2gulrmyqo.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2bcxnckuk.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2nikmnwfj.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2ctadgvqb.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vvflintc.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2kipmeyci.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zhvqjpag.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2uhrssvyr.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2essvkgpg.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pddzghff.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2cjigckxs.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2skxqcstr.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2vxxgcfta.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2kabwwrmq.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2aoaagsyl.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2hrnzmjcy.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2nmllnbvn.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2kknoumrf.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2fmoqktze.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2gbzhqnmj.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2zeqswmbp.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2tjnqmgil.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2stwphsqs.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2vnqkjnqr.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2fjahrtyi.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2hqnzooao.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2fkffmosy.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2bbiogyys.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2vqmdqlko.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2liekbgbl.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2omyfeqjv.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2khsuqbtp.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2dndgxlvm.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2ehscmkfe.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2vrcclnnz.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2eyadzxqo.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2msvjbrwj.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2wmsuvuis.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2mlvqocxf.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2ldmsacol.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2rmxvxhzr.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2yxqqbxfm.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2tadzzlpx.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2tdmtwkjh.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2njvixhzs.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2mccwvwra.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2yjbwhjbq.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2dfhmmcrc.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2xwdzcdzz.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2cxknbmuy.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2wcdkbbes.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2vvparolc.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2crkkizpx.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2rnjvzcst.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2fpthboyj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2olfnaawi.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2kfkcluct.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kblbttld.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2cnkakrih.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2mtowsjke.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2sedkejtf.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2tuqhleuq.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tctxgqhc.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2xiudhdai.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tpcgtfmf.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2docjzhrx.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2syahpdje.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2dwhpzmpa.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2emxkyqpz.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2rtnvsmya.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2cjxxqqju.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2oarvtpjs.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2ojixxyoh.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2pbxlkbmw.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2ralqvdbu.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2lbysmcvn.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2feqhvfdt.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2aqzusgfw.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2heomgkla.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2hknhysgf.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2aygxckya.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2rmgpziuo.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2yhcqohop.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2jzedyfyc.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2xdnwebrn.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2jffymboo.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2chpuykcm.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2vugvgfpu.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2uncwnnaw.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2xtrnngvy.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2czadbhnq.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2pytpjzgk.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2dbpydmlj.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2clizqeaq.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt2idlrqptn.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt2ghluggjr.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt2bohpjrjc.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2uqosuvpa.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2xsoorbnq.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2pvdqtmli.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2zynkukfv.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2ctafjqmy.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt2frkelorr.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt2vhrnuhqt.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2cqdbyhwv.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt2jsaaesgw.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2inlsbvrp.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2loaokeql.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2jokzjnrj.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt2hefueswb.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt2fwuvgtia.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2szecnunz.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt2kheteejm.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt2dutldeuw.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2kwikagwm.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt2ubwpkcku.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt2kjnvqfef.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt2iilameio.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt2mnlnikyg.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt2mwxiatho.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt2ucmilakf.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt2tyzobfpk.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt2dslqykbv.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2dsrvcmgs.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2nilhnavn.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2otrcahoy.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2prhzfrza.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt2lnfwvapd.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt2ubcyudyu.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2qwowcksv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cbzgjefy.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt2kaksvodp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tcdjtfjx.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2ndxlefns.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt2mnsludrm.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2arsaomwk.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2oszdmfli.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2lqwujkbc.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt2uwhbuxqb.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt2jvhwwfkb.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt2gooesqll.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt2okubgwus.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt2zfllabek.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2fqzzdegj.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2smxporvu.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt2xmquhmef.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt2jvrdysql.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt2zcoessrd.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2ajupkukc.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2qgtxnevf.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt2jxvavqeq.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt2jqjoygvk.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt2ypgkdpxq.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt2aelnyrru.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2zkfucjzu.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2fxhstgqz.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2cvocbfai.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2mpuneyhe.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2xojjrlai.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt2bzrhimfd.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt2ykusypow.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2nvrzchpv.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt2hqraajnl.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt2xhnfpuze.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt2taoqokaf.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2nwtpbeor.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt2ypwpmpho.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2obyyiuxu.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2bemmuivz.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt2sccwwizj.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt2ofwiaiye.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt2vzbykhrt.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2mskrkvod.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2sqmrycdw.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt2gbocajaz.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt2zyuiqgvd.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt2uzjzrzqu.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt2eomwstes.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2jhsvpjjz.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt2xzbwthek.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt2ecwaoxuc.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt2rsbrlcye.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt2mkzdzlfc.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt2cgimtgrq.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt2fxhlmyao.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2njpilwmp.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt2gfrurxqv.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt2zinyopde.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2cfigdita.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt2trrdxmnr.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2hubqxxnx.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2vucbiymr.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2lcnczwqz.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt2fgiusmyd.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2frddqjdp.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2zybcwsir.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt2oqpfnyij.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt2qwubjbhq.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt2pvmvpihu.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt2hrujaydd.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt2vhuohxse.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt2cwypwroj.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt2glxfimuf.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt2tctqhjta.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt2rtkpjwvc.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt2zoumltlm.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt2hgohvxzc.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt2drelxnyg.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2dxxkevqv.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2gqdhedrm.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2jozjluth.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2yulryavt.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt2pljpjoeb.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt2wasomckd.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt2eyeopkuu.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2vatroufm.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt2czhsqegi.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2bvydbwqs.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt2glznbpnx.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt2hdtahumi.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt2jqfiojhd.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt2wrhtaeow.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt2shbkkfrc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ncjyjjhe.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt2pqvoymsd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2awcuslpt.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt2vcapkaul.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2jyyxveok.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2unikxsfs.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2mbkbcxpx.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2nffbmopp.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2xldbftnb.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2glzqaoza.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2iylwcfpn.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2dqmotlbj.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt2iorrfhfd.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dxnanjae.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2excrnqbb.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2vvyrtjxw.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2svzkbyln.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2ibtydvnm.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2ppjxoudc.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xvuwauan.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2wqmkdqwi.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2unfbhztx.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2cmirdejw.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2amtjlvmc.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2bpajshxk.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2zqkitsau.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2eluidxyi.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2vnrpwlno.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2sijjrxmr.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2hpcgpuqp.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2ubvrbxmd.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2gdswsnxl.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2bhrethpm.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2thhjpmrn.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2thdqgpyt.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2ypdkqbrg.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2qyrypcfq.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2akyqyqgn.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2eheqfjmm.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2wcvqtghy.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2smbecsgf.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2jgjeszoe.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2ztrlfdsy.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2qdbyccvf.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2ioxdfzap.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2ckmalnrf.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2hiwmwskz.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2ehhzukqo.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2cxjyqjsb.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2divuqefx.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2pmcundjx.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2jgcjgxkt.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2djhqlnpb.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2gqmsdgzq.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2ziqizaqk.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2rvzxutiu.html


<!-- 参考信息 -->