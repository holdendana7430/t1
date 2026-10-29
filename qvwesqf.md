代发 wailian999

TS:   throw new Error("错误信息");
来源：http://www.blog.zdbjq.cn/Article/details/gysaebhxg.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.m.share.fehbvm.com/Article/details/gnpbjkjrh.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.share.hesvh.cn/Article/details/ghacqtlzh.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.fehbvm.com/Article/details/gwxvrjjwq.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://m.share.fehbvm.com/Article/details/geytmshvp.sHtML

[H04] 自定义异常类型
来源：http://3g.zdbjq.cn/Article/details/gelzspsez.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.fehbvm.com/Article/details/gtltbhsey.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.fehbvm.com/Article/details/gwgtmuqnj.sHtML

JS:   class MyError extends Error {}
来源：http://www.m.share.fehbvm.com/Article/details/gykfszyua.sHtML

TS:   class MyError extends Error {}
来源：http://baike.fehbvm.com/Article/details/gqqarilbz.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.m.share.fehbvm.com/Article/details/gqlosgpmy.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mobile.zdbjq.cn/Article/details/gbjdjxsjj.sHtML

Ruby: class MyError < StandardError; end
来源：http://read.share.zdbjq.cn/Article/details/guwdngkos.sHtML

C#:   class MyException : Exception {}
来源：http://read.share.hesvh.cn/Article/details/goiiqsctw.sHtML

[H05] 捕获特定类型
来源：http://www.blog.zdbjq.cn/Article/details/gsldkmcuj.sHtML

Py:   except ValueError as e:
来源：http://blog.fehbvm.com/Article/details/gsyztmrzf.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://baike.zdbjq.cn/Article/details/gkzjtlnzi.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://3g.zdbjq.cn/Article/details/gpnfegzur.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://blog.hesvh.cn/Article/details/gssbyvghf.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://mobile.fehbvm.com/Article/details/gvlapowdy.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wap.zdbjq.cn/Article/details/gwsgkqvwc.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.m.share.fehbvm.com/Article/details/gzfjthdsu.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.m.share.hesvh.cn/Article/details/gtwahesme.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.blog.zdbjq.cn/Article/details/gmxjbcmrr.sHtML

Py:   value = d.get("k") or default
来源：http://3g.zdbjq.cn/Article/details/gktlwmxwp.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://mobile.zdbjq.cn/Article/details/gjzttqcfn.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.fehbvm.com/Article/details/gjusagfng.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.share.zdbjq.cn/Article/details/gjhshxeqp.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wap.hesvh.cn/Article/details/gyejrnmdp.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.m.share.hesvh.cn/Article/details/gzeabypla.sHtML

Ruby: d&.dig(:a, :b)
来源：http://read.share.hesvh.cn/Article/details/gcglhmvcx.sHtML

C#:   obj?.A?.B ?? default
来源：http://baike.zdbjq.cn/Article/details/gconunzdm.sHtML

[H07] 断言
来源：http://www.blog.zdbjq.cn/Article/details/gtworvglo.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.m.share.hesvh.cn/Article/details/gzkxqbktd.sHtML

PHP:  assert($x > 0);
来源：http://m.share.hesvh.cn/Article/details/gcqzvvlxz.sHtML

JS:   console.assert(x > 0);
来源：http://mobile.fehbvm.com/Article/details/ghozfwrug.sHtML

TS:   console.assert(x > 0);
来源：http://blog.hesvh.cn/Article/details/gctpiyxee.sHtML

Java: assert x > 0 : "必须为正";
来源：http://blog.zdbjq.cn/Article/details/gfgcneapt.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://m.share.fehbvm.com/Article/details/gamcimoju.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://wap.zdbjq.cn/Article/details/gmsnlqntm.sHtML

C#:   Debug.Assert(x > 0);
来源：http://3g.zdbjq.cn/Article/details/grdahfgno.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.share.fehbvm.com/Article/details/gthfncxag.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://3g.zdbjq.cn/Article/details/gkxdtyqlg.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://blog.zdbjq.cn/Article/details/gjvqbrjmh.sHtML

JS:   e.message;  e.stack
来源：http://www.blog.fehbvm.com/Article/details/gmyrgkdad.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://blog.zdbjq.cn/Article/details/gajsvjjtp.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://3g.fehbvm.com/Article/details/gjrbvoeru.sHtML

Go:   err.Error()
来源：http://m.share.fehbvm.com/Article/details/gceztfzai.sHtML

Ruby: e.message;  e.backtrace
来源：http://baike.hesvh.cn/Article/details/ghuybwpus.sHtML

C#:   e.Message;  e.StackTrace
来源：http://wap.fehbvm.com/Article/details/gqcopdjzn.sHtML

[H09] 带错误码的异常
来源：http://www.blog.hesvh.cn/Article/details/gfyqhpfmg.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wap.zdbjq.cn/Article/details/gigqbomdt.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.m.share.hesvh.cn/Article/details/gcusnzwvl.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://read.share.fehbvm.com/Article/details/geeeuhqpy.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://read.share.zdbjq.cn/Article/details/gdexjhaci.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://blog.zdbjq.cn/Article/details/golplnemu.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wap.fehbvm.com/Article/details/gbhmowzwb.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://mobile.hesvh.cn/Article/details/gstjiweqj.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.share.zdbjq.cn/Article/details/guioiczvr.sHtML

[H10] 资源自动释放
来源：http://blog.fehbvm.com/Article/details/gsseargmz.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://blog.hesvh.cn/Article/details/guxnesxij.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://3g.zdbjq.cn/Article/details/gdymwcpjd.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.zdbjq.cn/Article/details/gfrkjkkcj.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.hesvh.cn/Article/details/gyfelghhl.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://blog.hesvh.cn/Article/details/gesckfkqe.sHtML

Go:   defer f.Close()
来源：http://mobile.zdbjq.cn/Article/details/gvwjxjmfc.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://3g.hesvh.cn/Article/details/gqzibjpdg.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gspeyukky.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gmcccntfz.sHtML

I. 正则表达式
来源：http://m.share.fehbvm.com/Article/details/ganlotych.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gnizyyeoc.sHtML

[I01] 判断是否匹配
来源：http://m.share.zdbjq.cn/Article/details/gcgsgelyd.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://read.share.fehbvm.com/Article/details/gkafzrguo.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://baike.zdbjq.cn/Article/details/gizuipkuf.sHtML

JS:   /\d+/.test(s)
来源：http://wap.zdbjq.cn/Article/details/gvkfmujun.sHtML

TS:   /\d+/.test(s)
来源：http://www.share.fehbvm.com/Article/details/guhwcsazi.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://baike.fehbvm.com/Article/details/gpnaypawk.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gqimxrsco.sHtML

Ruby: s.match?(/\d+/)
来源：http://m.share.zdbjq.cn/Article/details/gnkoqckjn.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://baike.fehbvm.com/Article/details/glodxqxev.sHtML

[I02] 提取所有匹配
来源：http://www.m.share.hesvh.cn/Article/details/gltmbkbpb.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.blog.zdbjq.cn/Article/details/gejqxktjz.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://read.share.fehbvm.com/Article/details/gmajqfzej.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://read.share.hesvh.cn/Article/details/ggpuhedjr.sHtML

TS:   s.match(/\d+/g)
来源：http://www.blog.hesvh.cn/Article/details/gyfofooio.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://blog.zdbjq.cn/Article/details/gcrcivysz.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mobile.fehbvm.com/Article/details/gafuxvywl.sHtML

Ruby: s.scan(/\d+/)
来源：http://m.share.hesvh.cn/Article/details/gobdtjsok.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://m.share.hesvh.cn/Article/details/gapclmkrm.sHtML

[I03] 提取捕获分组
来源：http://wap.zdbjq.cn/Article/details/golpduryo.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mobile.fehbvm.com/Article/details/gbdjmxrid.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.blog.fehbvm.com/Article/details/goddfykaq.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.blog.hesvh.cn/Article/details/gocjsshwj.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://baike.hesvh.cn/Article/details/gfluvmrak.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.blog.fehbvm.com/Article/details/gxdhhrrfd.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://m.share.fehbvm.com/Article/details/ggsnucbil.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://read.share.hesvh.cn/Article/details/gcxvidgbq.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.m.share.fehbvm.com/Article/details/gttytbqwi.sHtML

[I04] 正则替换
来源：http://blog.fehbvm.com/Article/details/geeubvfig.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.m.share.fehbvm.com/Article/details/gyhbrozpi.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://baike.zdbjq.cn/Article/details/ggmbsludf.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.share.zdbjq.cn/Article/details/gxyfumptx.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://wap.hesvh.cn/Article/details/gedizlflo.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://m.share.fehbvm.com/Article/details/ghmmygckk.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://m.share.zdbjq.cn/Article/details/gyncwrivp.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://3g.hesvh.cn/Article/details/glbjkdwcz.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://wap.zdbjq.cn/Article/details/gihdjyywj.sHtML

[I05] 按正则拆分
来源：http://www.blog.hesvh.cn/Article/details/gxjrrhuvd.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://3g.fehbvm.com/Article/details/gtpvfulcd.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://m.share.fehbvm.com/Article/details/guxirhnup.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://blog.zdbjq.cn/Article/details/gjqmhskwh.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://wap.hesvh.cn/Article/details/gvaaogzge.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.share.zdbjq.cn/Article/details/glndgwvle.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.m.share.fehbvm.com/Article/details/grnnsspcr.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://3g.zdbjq.cn/Article/details/gczrcwxom.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://blog.fehbvm.com/Article/details/gicdwzrhg.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://baike.zdbjq.cn/Article/details/gjdflldtc.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://read.share.fehbvm.com/Article/details/gcnptzdup.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://baike.fehbvm.com/Article/details/giecvqvnx.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.fehbvm.com/Article/details/gmdwngwfb.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.hesvh.cn/Article/details/gagjdxpkt.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.share.hesvh.cn/Article/details/gnthhiupu.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.share.zdbjq.cn/Article/details/gjsslyyqp.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://blog.zdbjq.cn/Article/details/glqjyatss.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mobile.hesvh.cn/Article/details/gyolmfqrb.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.share.hesvh.cn/Article/details/gkephexde.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mobile.fehbvm.com/Article/details/gmciyuzfi.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://m.share.hesvh.cn/Article/details/gitsizxyp.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://blog.zdbjq.cn/Article/details/gjorrvpzi.sHtML

TS:   /error/gim
来源：http://m.share.hesvh.cn/Article/details/gomwujtwm.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.blog.hesvh.cn/Article/details/gsjxfogns.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://3g.zdbjq.cn/Article/details/gzoeiomwi.sHtML

Ruby: s.scan(/error/i)
来源：http://www.share.zdbjq.cn/Article/details/gheiqktkj.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.share.fehbvm.com/Article/details/grwlnwmhz.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://wap.zdbjq.cn/Article/details/gmqicfobl.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://blog.zdbjq.cn/Article/details/gorvzvjjc.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://m.share.zdbjq.cn/Article/details/gjoqlderw.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.fehbvm.com/Article/details/glffjaqla.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.hesvh.cn/Article/details/gsblvaqoh.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://3g.fehbvm.com/Article/details/gxbthlfmi.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://m.share.fehbvm.com/Article/details/ggvnwzbnr.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.share.hesvh.cn/Article/details/gxpzyrmlv.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://baike.zdbjq.cn/Article/details/ghcsmskrc.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gxbdwrqjd.sHtML

J. 日期与时间
来源：http://baike.hesvh.cn/Article/details/gmqxfgzkx.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gatsqsabn.sHtML

[J01] 获取当前时间
来源：http://www.m.share.fehbvm.com/Article/details/gcazoupeh.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.m.share.hesvh.cn/Article/details/gwwihbjvc.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://wap.zdbjq.cn/Article/details/gtxbkcnhn.sHtML

JS:   new Date();  Date.now()
来源：http://www.share.hesvh.cn/Article/details/gyvjyozvi.sHtML

TS:   new Date();  Date.now()
来源：http://www.blog.fehbvm.com/Article/details/gurwshwjd.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.share.zdbjq.cn/Article/details/gvbtsxmmr.sHtML

Go:   time.Now()
来源：http://mobile.hesvh.cn/Article/details/gtprgkzlc.sHtML

Ruby: Time.now
来源：http://www.share.zdbjq.cn/Article/details/gunnvmhkk.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://3g.fehbvm.com/Article/details/gyxttidqy.sHtML

[J02] 格式化输出
来源：http://blog.fehbvm.com/Article/details/gwayqythz.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.zdbjq.cn/Article/details/gjwugnhuh.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://3g.hesvh.cn/Article/details/gvummxmec.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.share.fehbvm.com/Article/details/gpqjusvfr.sHtML

TS:   d.toISOString()
来源：http://www.m.share.fehbvm.com/Article/details/gpcogbave.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://m.share.hesvh.cn/Article/details/guczqchgj.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.m.share.hesvh.cn/Article/details/gyhmfrlbm.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.fehbvm.com/Article/details/gibecztsj.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://3g.hesvh.cn/Article/details/gdatqgyvk.sHtML

[J03] 字符串解析为日期
来源：http://mobile.hesvh.cn/Article/details/gtrsvywzu.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://baike.hesvh.cn/Article/details/gktgibbwm.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://baike.hesvh.cn/Article/details/goquemoxs.sHtML

JS:   new Date("2024-01-02")
来源：http://blog.fehbvm.com/Article/details/gkppcjqhi.sHtML

TS:   new Date("2024-01-02")
来源：http://baike.fehbvm.com/Article/details/gfpiuofsf.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://baike.fehbvm.com/Article/details/gumjvfvul.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://read.share.hesvh.cn/Article/details/gnjckpybk.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.m.share.zdbjq.cn/Article/details/gqkmiwvok.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://baike.zdbjq.cn/Article/details/glycbawhu.sHtML

[J04] 时间戳与日期互转
来源：http://www.m.share.zdbjq.cn/Article/details/gxjzzghmo.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.share.zdbjq.cn/Article/details/gqzjvybwg.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://read.share.hesvh.cn/Article/details/givgqoyni.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.share.zdbjq.cn/Article/details/gcsyzqldr.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://3g.hesvh.cn/Article/details/gjaquxori.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://read.share.hesvh.cn/Article/details/gszfbnqiy.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://blog.zdbjq.cn/Article/details/ghznzjuwd.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://3g.hesvh.cn/Article/details/gipftzmml.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://read.share.fehbvm.com/Article/details/gbfaesbsa.sHtML

[J05] 时间加减（加 7 天）
来源：http://mobile.zdbjq.cn/Article/details/gntbowdvm.sHtML

Py:   now + timedelta(days=7)
来源：http://3g.hesvh.cn/Article/details/gorqrjsdw.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://read.share.hesvh.cn/Article/details/gavkzrgeh.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.fehbvm.com/Article/details/gzciwmapq.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.fehbvm.com/Article/details/glxybpvzk.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://baike.hesvh.cn/Article/details/gzodgugui.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://3g.zdbjq.cn/Article/details/gbixmxtvo.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.blog.zdbjq.cn/Article/details/gryaiviqu.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://baike.zdbjq.cn/Article/details/gagzkdhkx.sHtML

[J06] 计算两时间之差
来源：http://www.m.share.fehbvm.com/Article/details/gfbgqidda.sHtML

Py:   (end - start).total_seconds()
来源：http://3g.zdbjq.cn/Article/details/gmmwrteac.sHtML

PHP:  $end->diff($start)->days;
来源：http://read.share.zdbjq.cn/Article/details/gseyxfsdj.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://3g.fehbvm.com/Article/details/gduatjbkq.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://3g.zdbjq.cn/Article/details/grecnbjaz.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.share.hesvh.cn/Article/details/glhveraex.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.blog.fehbvm.com/Article/details/grplpntzj.sHtML

Ruby: end - start                 # 返回秒数
来源：http://baike.hesvh.cn/Article/details/gpumqyssb.sHtML

C#:   (end - start).TotalSeconds
来源：http://mobile.zdbjq.cn/Article/details/gyutfsasl.sHtML

[J07] 比较两个日期
来源：http://mobile.zdbjq.cn/Article/details/ggdcmibze.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://m.share.zdbjq.cn/Article/details/gzbqaacpd.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.share.zdbjq.cn/Article/details/gipwyogxd.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://wap.hesvh.cn/Article/details/gxnswbgvu.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.share.fehbvm.com/Article/details/gmmimpiht.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://m.share.zdbjq.cn/Article/details/gaxdhiucg.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://blog.fehbvm.com/Article/details/gxlsberql.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://blog.zdbjq.cn/Article/details/gszjuebop.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://mobile.zdbjq.cn/Article/details/gqzwwmwci.sHtML

[J08] 提取年月日与星期
来源：http://3g.fehbvm.com/Article/details/glajuymwh.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wap.hesvh.cn/Article/details/gegtuakkx.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://baike.hesvh.cn/Article/details/gucznallx.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.m.share.zdbjq.cn/Article/details/gjkkwxewi.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://read.share.fehbvm.com/Article/details/gcigaxnqk.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wap.hesvh.cn/Article/details/gdtgtmblt.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://baike.zdbjq.cn/Article/details/gbujtnfjc.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mobile.zdbjq.cn/Article/details/giiqiciyz.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.m.share.hesvh.cn/Article/details/gqyssgbil.sHtML

[J09] 时区处理
来源：http://m.share.fehbvm.com/Article/details/gvozebkrm.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://read.share.fehbvm.com/Article/details/gofqgiqfp.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://baike.hesvh.cn/Article/details/gbmzywcht.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.fehbvm.com/Article/details/ghuirjcpz.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.zdbjq.cn/Article/details/ghmkdoxil.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mobile.hesvh.cn/Article/details/gkquzmrng.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://baike.zdbjq.cn/Article/details/gmbdyflpy.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.m.share.hesvh.cn/Article/details/gsmeywxaw.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.m.share.zdbjq.cn/Article/details/grcrswktf.sHtML

[J10] 取今天 / 本月第一天
来源：http://3g.hesvh.cn/Article/details/guvxtjfpm.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://baike.zdbjq.cn/Article/details/gpztwwgxc.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.m.share.zdbjq.cn/Article/details/gkesrgpiu.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://blog.hesvh.cn/Article/details/gqmhmcire.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gbdyxhtmo.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://read.share.hesvh.cn/Article/details/gfuiwvuzh.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mobile.hesvh.cn/Article/details/gxlakvget.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://blog.hesvh.cn/Article/details/gwjyajdaz.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.blog.fehbvm.com/Article/details/gvmyhhnhd.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gavfockdd.sHtML

K. JSON 与序列化
来源：http://m.share.hesvh.cn/Article/details/gcmeutxxs.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gbhelrumx.sHtML

[K01] 对象转 JSON 字符串
来源：http://mobile.zdbjq.cn/Article/details/gzctcrwjh.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://blog.hesvh.cn/Article/details/gwkncddqo.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://m.share.hesvh.cn/Article/details/gqbapmuoj.sHtML

JS:   JSON.stringify(obj)
来源：http://3g.fehbvm.com/Article/details/gzdldrnxz.sHtML

TS:   JSON.stringify(obj)
来源：http://baike.hesvh.cn/Article/details/gptculinx.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.blog.zdbjq.cn/Article/details/glsqcbgqb.sHtML

Go:   json.Marshal(obj)
来源：http://www.blog.zdbjq.cn/Article/details/glnlsfqsl.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://m.share.zdbjq.cn/Article/details/gsgrzevhx.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.share.zdbjq.cn/Article/details/grnrmexjj.sHtML

[K02] JSON 字符串转对象
来源：http://www.m.share.fehbvm.com/Article/details/gtdthgqcn.sHtML

Py:   json.loads(s)
来源：http://www.blog.hesvh.cn/Article/details/gpzemveaq.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mobile.fehbvm.com/Article/details/grryvwnxe.sHtML

JS:   JSON.parse(s)
来源：http://baike.hesvh.cn/Article/details/gvsqhyioc.sHtML

TS:   JSON.parse(s)
来源：http://baike.hesvh.cn/Article/details/gvejkbohh.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://3g.fehbvm.com/Article/details/gjtnymfrk.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://3g.fehbvm.com/Article/details/ghjxbefvn.sHtML

Ruby: JSON.parse(s)
来源：http://baike.zdbjq.cn/Article/details/ghahskfgv.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://m.share.zdbjq.cn/Article/details/gnppovisa.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://wap.hesvh.cn/Article/details/gforvezzc.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://baike.hesvh.cn/Article/details/gtwdudrbe.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.share.hesvh.cn/Article/details/gfifdfuxj.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://mobile.fehbvm.com/Article/details/gdweqmyxb.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://3g.zdbjq.cn/Article/details/gomxkaasq.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mobile.fehbvm.com/Article/details/gqtnamrqd.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://blog.hesvh.cn/Article/details/gsnnpwxxk.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://blog.fehbvm.com/Article/details/gdgwqrayj.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://baike.hesvh.cn/Article/details/giwfixzpn.sHtML

[K04] 读取 JSON 文件
来源：http://www.m.share.fehbvm.com/Article/details/gasbzksbl.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://baike.fehbvm.com/Article/details/gbwswmkci.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://3g.hesvh.cn/Article/details/gmvyrdfti.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.hesvh.cn/Article/details/geccjlhjf.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.fehbvm.com/Article/details/gekpvagyh.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wap.hesvh.cn/Article/details/geicixxbt.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mobile.hesvh.cn/Article/details/gxalccxvi.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://blog.zdbjq.cn/Article/details/gbhrhumta.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wap.hesvh.cn/Article/details/geodmrgng.sHtML

[K05] 深拷贝对象
来源：http://3g.fehbvm.com/Article/details/gwuhprvxf.sHtML

Py:   copy.deepcopy(obj)
来源：http://wap.hesvh.cn/Article/details/gmoxjgkxp.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.share.fehbvm.com/Article/details/giquhrjzf.sHtML

JS:   structuredClone(obj)
来源：http://baike.fehbvm.com/Article/details/goqnwwhxm.sHtML

TS:   structuredClone(obj)
来源：http://3g.fehbvm.com/Article/details/gnmmdkzre.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.m.share.zdbjq.cn/Article/details/gxcqahcwf.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.m.share.fehbvm.com/Article/details/gujllxwkj.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://blog.zdbjq.cn/Article/details/gzkgfxkof.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.blog.hesvh.cn/Article/details/gxfguqqon.sHtML

[K06] 解析 URL 查询串
来源：http://baike.fehbvm.com/Article/details/gmjihxlqq.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://3g.hesvh.cn/Article/details/ghboifxds.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wap.fehbvm.com/Article/details/gxotwctje.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.zdbjq.cn/Article/details/gimyvucez.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.fehbvm.com/Article/details/grqsjzolb.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://m.share.fehbvm.com/Article/details/gqtxqrisr.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://blog.zdbjq.cn/Article/details/ggfweiump.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.m.share.hesvh.cn/Article/details/gxazotfad.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.share.zdbjq.cn/Article/details/grkrxduio.sHtML

[K07] 进制转换
来源：http://mobile.fehbvm.com/Article/details/grisotjfa.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://blog.fehbvm.com/Article/details/gqcbqdocy.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://baike.zdbjq.cn/Article/details/gjhcxaght.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.blog.fehbvm.com/Article/details/gkmcztxbv.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.blog.hesvh.cn/Article/details/gjplkwzje.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://m.share.fehbvm.com/Article/details/gtkizsfjz.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mobile.zdbjq.cn/Article/details/gdatxklgo.sHtML


<!-- 参考信息 -->