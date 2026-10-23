代发 wailian999

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3chiimxkf.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3tzjmocqr.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3fhxjtnud.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3vlhqcttb.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3jizuhzfd.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3sfgnxvck.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3tsjoimhc.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3bwkwwiow.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3eoopbixs.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3qaixcqhj.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3kqpgxlzn.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3efqeptzs.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3gicehyfo.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3dizhxlah.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3lcxlzeol.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3wazerfzk.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3nqsuqpis.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3gxjgcqps.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3sszugqhc.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3eluxmrvc.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3jmrftjje.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xhaxsenv.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dtvotnpc.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gpsozhvm.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3jhvuwjjs.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3zmgnkqoc.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mkfohlnd.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3nrrgwmma.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3ulabejuv.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3vaowyycl.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3aqcrkdvo.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3dxlrmkdg.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3kidpfsvp.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3grfchdet.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3mhrmgcvz.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3uovyxquq.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3uzvvgniu.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3zxkyapjz.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3qzwqfjmc.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3edoovqqw.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3sviaegin.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3rndvdith.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3wlnwstqt.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3xmjuecul.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3oiwaxjoi.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3dhwtcvhz.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3cvevecgk.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3ehjtkrgc.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3zvgxmube.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3iqrweclm.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3bguextsh.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3yqqywyyo.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3sfqnwwmc.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3zephgaim.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3fcajbhyr.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3htiwhmse.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3bqehbpob.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3akcichlg.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3nlyleazl.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3fvznktxe.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3ajafswpv.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3domqtqbe.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3cmbmtlur.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3uyejesbe.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3xunsokoh.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3lzkileem.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3tbunucwa.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3xrnvrfqf.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3bnmlfvcf.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3nylglxit.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3gfgmxjuv.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3tlrhaihm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hddalllj.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3egyjoipq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lbkplqij.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3lkumryef.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3aahfztum.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ifbagzpe.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3ogcewlvk.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3yfvjrbml.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3xjoquweg.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3hugbzklg.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3idggdatv.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3cdkhcoxk.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3bimrprej.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3xknwvums.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3iptgdhcp.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt3wviawpmm.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt3dxqxnxxb.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3yfhqwuaj.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3wbphxrzi.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3hfrzkrhb.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3eyjnqnuj.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3drfvueog.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3vgvyzcev.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3yxwiogti.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3cksyxaoc.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt3lxehddpf.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3gpzjbzmh.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt3yuehyydh.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt3iswowmrf.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt3fczccfxq.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt3iupdptwk.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3xwkfrlbs.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3cwjluklu.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3jkdaodir.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3yocdzhdm.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3tzxsbffw.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3pjgbrkcr.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3xbevalhh.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3agbqcehs.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt3fzidwjgm.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt3ejlwwpzq.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3xfdavqpf.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3gyigwdft.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3yoxwdpkq.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt3viytezhp.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3uzyjzexc.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3oddxgzof.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3jtmfccen.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt3fxsaivdz.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3lxwmxrcr.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt3ibcpwrni.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3iczrmcjr.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3tfhyizms.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3glmrixvz.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt3gpltvpkp.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt3dqypehfi.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3afcvirpd.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt3upswxuvt.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt3oudnisms.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3uzvujqdw.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt3qpagwjub.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt3wqctvnfl.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt3zmnxqejw.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt3hzfrijjt.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt3lthmgdvn.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt3euwagstq.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt3iuiatjwh.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt3nnnzbhbq.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3inwxfezh.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3jjnbxkyo.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3wkpentpo.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3etmjnvcm.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt3bmvtiwji.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt3xjmffuyw.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3kufdhnsg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zajfxzfd.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt3gnnfvdyp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jvqmbufn.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt3qdydmwpb.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt3nhbscbkc.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3wpcankxm.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3etzsbiig.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3jlfykzps.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt3croipnwk.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt3hbytprlk.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt3yzemlmie.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt3ahhlzbqp.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3upzphohf.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3mbmknucj.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3qttgwkda.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt3lwjddxwq.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt3ytxwzvlp.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt3erehkgyv.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt3nsxyjumk.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3smrevyac.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt3qgkiolpj.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt3ibglchrf.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt3jdrqbgas.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt3irrwtqwk.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3aykyhffo.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3fmcanvjp.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3hqjnhlvc.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3mcuuruon.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3cvakethd.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt3rdrmguop.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt3rlsjjmsp.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt3xpnnpoku.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt3ecisczqa.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3ygicabrs.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt3tmfthfmd.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3veoyqsif.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3snnlwljf.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3xwpbetks.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt3pznjwrdl.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt3crulpncg.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt3rwepdeiv.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt3szqzupon.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3hapvixgm.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3lupftmin.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3ktadbvsk.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt3zykpgcnx.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt3mldzhdsf.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt3mvhzxmdy.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt3sfafxhyy.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt3fzfffyam.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt3cqnclcax.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt3qfkhhrme.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt3kjwquvun.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt3jwozyeix.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt3dlfgpvtp.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt3djcdcsnj.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt3ocatdbva.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt3lvnofkhi.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3egbvgvhj.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt3agdweefh.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3zykkzyef.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3iagtuszq.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3jkvtigmn.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt3nsneufql.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3whvpnlgb.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3ujscvkws.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt3fkpgwsnh.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt3sigabiek.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt3atkygjck.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt3nvaqwwik.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt3kwhbhwja.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt3bekfwsdt.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt3mfncbtoh.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt3yvylvhba.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt3izjydjly.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt3ppcxfghl.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt3fjoqnwox.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt3zvojimtt.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3ksfxpwbi.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3xjxoduye.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt3dokdwhgl.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt3lpwwcunh.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt3esufuvjs.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt3yzzfjlhx.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt3dnhdkgvi.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt3klvauyxl.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt3bfpiewny.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt3oaukmjqc.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt3phrsuexf.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt3mxeoyrhj.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt3cbabggyf.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt3sjzuoxjq.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3mgpvwzei.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vtsplpkq.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt3vhhtetme.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nqybopjf.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt3lczydpob.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3xshbteyf.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3ycvlkety.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3isctvued.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3mwdtukvi.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt3burqgwdp.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3wxnibqjn.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt3ifnoceka.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3rbmmyhst.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3ueovqsyv.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3jkgyaxng.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3qhldyroc.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3ujudwsex.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3ioyvqjtr.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3ncfrfzbe.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3izogrjxp.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3wwmwnjfn.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3tsepjjlz.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3qbgzfyvh.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3alviqikt.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3nadirpnx.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3qarkzxnh.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3kxdhdekk.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3hspvslpi.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3xyezwjwr.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3egdnuzfi.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3dtvrmdav.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3qksbaywr.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3tgigjqdk.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3ylymsedh.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3qlcpxuuk.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3wekcuemn.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3zkxqewcl.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3fptjsuos.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3lkhqvsng.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3sjniecqj.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3ettdywio.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3gcbvrjlx.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3owvyrrjf.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3exwltrnp.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3xuptqtrn.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3hgveoyrv.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3gynjytvb.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3mjdnmnxp.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3pjermxum.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3dlsonqaz.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3gigbfoot.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3zfpmjpau.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3rbowhtvg.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3keqtlbdy.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3lklwrqdj.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3axjciszv.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3kjivszqk.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3ejzdtyhk.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3wnsxjccw.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3uefolirb.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3nwhultin.html


<!-- 参考信息 -->