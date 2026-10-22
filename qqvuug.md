代发 wailian999

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2eyyizhia.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2zygpyijb.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2fjyrpxsv.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2hxtwvbkr.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2cdfzdcab.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2vratidjg.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2pktctcgy.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2tsuatszk.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2stujoitn.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2pldmjfws.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2ayfemihu.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2jddaqbbn.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2zhibtxaz.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2qbjfeckp.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2lthdsktu.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2xyierwjm.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2boucjkne.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2gwykthks.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2vqsrxqey.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2khzrvkxv.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2koemjpst.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2wttfseoq.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2qhdvfvjl.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2kfrylmnu.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2ozdmnyrs.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2gllfsqcp.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2hvqvujha.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2iepfcwyt.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2msbjkbyo.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2xtjjhjdh.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2akrldbjn.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2edavplgm.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2cuxcvemz.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2hzdenofh.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2qgraufrm.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2vshfdeyv.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2gzlsutug.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2jumgdcqy.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2uxjiaarz.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2zyvjiklo.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2hsoeyrzj.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2buqkbgom.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2palyxgzw.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2wvwutsev.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2nszkxoys.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2kolmjluf.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2dyafbqrj.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2xdfmpltz.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2cdkmjyvs.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2doujohub.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2auxmpnnz.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2vukmernq.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2brwxdigv.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2tsreyepo.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2xcyvtxql.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2mytzykzu.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2tmwxtzss.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2nkwcdnyd.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2lpplvcnd.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2uqupnhwi.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2xbbtzwsy.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2ojvxmqcz.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2rrkohfpa.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2tzdoudmu.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2ygrkoojj.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2xvrnkchp.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2mefejigp.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2lejmyjak.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2rrjyumzi.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2hhxmodpd.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2kxdjgway.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2ucpkdkld.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2itqhzycf.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2dizfaohs.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2wfijvqoc.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2yddwnktp.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2arpuxwdn.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2ihenyeju.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2ttyeiwwn.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2kzylclko.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2rppacjkq.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2ydyxaogs.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2oenarupr.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ofujgpmh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jfeexiyg.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2ktzcvlbh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xzqfkwbo.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2wwnnxzer.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2bpzwfjry.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2bfmogbtx.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2cwtvhxhm.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2lmchtyjt.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2uornlkqk.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2cjlgezvt.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2gegxucti.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2wpgxjkim.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2zpieybqa.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2qityjzdr.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2wfrskiio.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2trumwbdu.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2dvreozlt.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2yeaxpscf.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2ykzzdojr.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2thhwciqz.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2nhvxiiwd.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2zhfwatsj.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2yvcwrxbj.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2rsdlefyt.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2mnsigrfg.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2sqyruueu.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2empsswwk.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2pulmlzwf.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2bodzgphc.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2wzqrrdek.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2kxdckkji.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2wreiqskg.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2zsxhyhhn.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2xvigfcqq.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2giacljpn.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2xnfwbosr.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2vrrlbrtt.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2txlslbgs.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2cuizwufs.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt2idryoxts.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt2bohdatql.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2pracuoem.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2meggzabp.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2bemhadkz.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2ujzsfbfp.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2addishgb.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2pecnuyvs.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2qneukitm.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt2fyapdlhg.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2vaiypocn.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt2iwywlgnu.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2hilmzchc.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2opykjvvd.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2ckddsumn.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt2fmtqdtom.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt2keoylljj.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2bouvzese.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt2dcgptnrd.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt2sgeuxwah.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2eequgpxw.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt2ewuyvwgv.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt2hrlzesgy.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt2zvreguwg.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt2lgecqtfo.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt2gtdoncyi.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt2zotkjzqs.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt2lrprbblc.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt2mdloklpy.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2vkgmilrz.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2dcsghjhk.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2apfxmvdh.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2haoutprj.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt2skwdzmok.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt2myzagxll.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2sidxrotr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2isjzcstb.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt2clqfeaeg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lgpbjphs.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2gosqnqoc.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt2rjqvlwng.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2hegbeknz.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2uvcwnxyt.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2rlhfamth.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt2xdftlssh.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt2oblekptd.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt2wcknsqvz.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt2qcvytnhx.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt2uopkqslh.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2jwgbopeq.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2lnuptgom.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt2wwfnktta.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt2pparvtap.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt2tbgkkxfr.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2yeefpdhi.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2lbjdtvch.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt2kresdpvy.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt2rszghpqk.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt2bcxxskyl.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt2tbmvqjnw.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2icuqxsqd.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2gcgqmnox.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2gdsggduv.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2hvneffxl.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2sxxobqwa.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt2aunfeubz.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt2ovsffpkg.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt2xdweniml.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt2lihfjvow.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt2hjrwqvmt.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt2xnxleyji.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt2zjplexxu.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt2qecggkuy.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt2hsfuaxqv.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2vibxznfz.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt2xfzcvjlu.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt2kqdlfygb.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt2zttrlyyb.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2tgtnlkch.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2qeuyypat.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt2nyqloucu.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt2iwswrdfy.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt2wpqgmuos.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2obtilndq.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt2ankftjdc.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt2yirwltii.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt2tmjkgsey.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt2ovzlvpgy.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt2gaudwxyx.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt2ulsbqnhp.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt2mqpwijam.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2nczhfdcg.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt2eszamcar.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt2acionwzw.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2xihptzyl.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt2otpqqfxt.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2hoyaxtxa.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2liiawzcd.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2rhvughfp.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt2jfhwwchs.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2vqqthagg.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2clzbqgly.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt2zziqgqvj.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt2tmzugunj.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt2pvdhpvao.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt2xiamgzas.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt2nqieimrl.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt2ynitchmh.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt2opcnipke.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt2okvsiaip.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt2gxyyotzg.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt2jthrjpri.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt2gtmplpis.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt2cdtwkqzv.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2vrpysrrt.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2cihbxzry.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt2voxszifw.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2xhsnftdt.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2mvdkgrma.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt2xtmkkjhg.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt2iwedzirm.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2fpxdewif.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt2mxeddcwo.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt2gqhpypez.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt2mfkonmig.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2glrpnrgv.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt2lutntshe.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2hxwkgmvn.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt2dcmrahxp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sqlsegnh.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2qgwpsjmd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pcdacjuf.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt2nmfxxhqs.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2jtgkgceo.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2xgdpvurj.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2ootagaal.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2sgrwxdxo.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt2mhsdpgxy.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ubuusnyo.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2gmgyhcqa.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ogszzorg.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt2yotigpxn.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ngvvpxjk.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2lsdhpbgv.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wdrrjnec.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2xtkzrrum.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2vlbfixmv.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2mhzsmbud.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2klljiaju.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hmvwwxnx.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2klcwjdza.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2aqfajwty.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2liorqcqx.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qougdsgb.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2heakibis.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2oqodnljq.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2fdvcxlbb.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2fxenrsyu.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2npccfwfv.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2feennlye.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2tmdxeyno.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2qperkstf.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2xhzgeoxt.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2khsqpvta.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2mzbvfqye.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2ezliquid.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2egviguqv.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2ntnopsoi.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2mgdzybpf.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2mhdwcjjt.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2nvgavbrw.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2btfkymjs.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2nytuacdl.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2auivddqv.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2qpnuvfvk.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2glyhspwd.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2dzlyczxs.html


<!-- 参考信息 -->