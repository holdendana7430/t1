代发 wailian999

C#:   throw new ArgumentException("错误信息");
来源：http://blog.zdbjq.cn/Article/details/gnabfxkso.sHtML

[H04] 自定义异常类型
来源：http://baike.hesvh.cn/Article/details/glgkzdwbj.sHtML

Py:   class MyError(Exception): pass
来源：http://blog.hesvh.cn/Article/details/ghavsqjrq.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.zdbjq.cn/Article/details/gyjtaesta.sHtML

JS:   class MyError extends Error {}
来源：http://blog.hesvh.cn/Article/details/glldnplfl.sHtML

TS:   class MyError extends Error {}
来源：http://mobile.fehbvm.com/Article/details/gfldycqxz.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.blog.hesvh.cn/Article/details/gthtenfxr.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mobile.hesvh.cn/Article/details/glzlnbcqz.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.share.hesvh.cn/Article/details/gdcedazxt.sHtML

C#:   class MyException : Exception {}
来源：http://www.blog.fehbvm.com/Article/details/gshuaevsd.sHtML

[H05] 捕获特定类型
来源：http://3g.hesvh.cn/Article/details/grqkltejd.sHtML

Py:   except ValueError as e:
来源：http://blog.hesvh.cn/Article/details/gbmwcntih.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.m.share.hesvh.cn/Article/details/gbrafdpoq.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://read.share.hesvh.cn/Article/details/gpokeilgj.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.m.share.fehbvm.com/Article/details/gwchpvatp.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://m.share.hesvh.cn/Article/details/grzglxdbc.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://read.share.hesvh.cn/Article/details/gmwhqsfid.sHtML

Ruby: rescue ArgumentError => e
来源：http://mobile.zdbjq.cn/Article/details/ghqdgrmls.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://blog.hesvh.cn/Article/details/gmqypleom.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.m.share.fehbvm.com/Article/details/gibhzqnsz.sHtML

Py:   value = d.get("k") or default
来源：http://blog.zdbjq.cn/Article/details/gmewqobqc.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://3g.zdbjq.cn/Article/details/gtliotdsp.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.share.fehbvm.com/Article/details/gbnbjjtna.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.hesvh.cn/Article/details/gcdsxbvhv.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.blog.fehbvm.com/Article/details/gnwyuekig.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://m.share.fehbvm.com/Article/details/gjwuvohxz.sHtML

Ruby: d&.dig(:a, :b)
来源：http://3g.hesvh.cn/Article/details/gdckprjvm.sHtML

C#:   obj?.A?.B ?? default
来源：http://blog.fehbvm.com/Article/details/gaywmqays.sHtML

[H07] 断言
来源：http://baike.fehbvm.com/Article/details/gdjexsntn.sHtML

Py:   assert x > 0, "必须为正"
来源：http://baike.zdbjq.cn/Article/details/gbbludolb.sHtML

PHP:  assert($x > 0);
来源：http://m.share.fehbvm.com/Article/details/gfyhihmeh.sHtML

JS:   console.assert(x > 0);
来源：http://www.m.share.fehbvm.com/Article/details/gbfdqvlru.sHtML

TS:   console.assert(x > 0);
来源：http://m.share.zdbjq.cn/Article/details/gsxgaewfg.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.zdbjq.cn/Article/details/gxufyskvd.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.blog.fehbvm.com/Article/details/gqwvididu.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://blog.hesvh.cn/Article/details/gbyzpwudl.sHtML

C#:   Debug.Assert(x > 0);
来源：http://read.share.zdbjq.cn/Article/details/gcjduccmi.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.blog.hesvh.cn/Article/details/gggyzwyxs.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://3g.hesvh.cn/Article/details/gcnvueqiz.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.m.share.hesvh.cn/Article/details/gezxlurpx.sHtML

JS:   e.message;  e.stack
来源：http://mobile.hesvh.cn/Article/details/glmtjansq.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://3g.hesvh.cn/Article/details/getwmmghx.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://baike.fehbvm.com/Article/details/gsjlbzhte.sHtML

Go:   err.Error()
来源：http://baike.hesvh.cn/Article/details/gpitbiutv.sHtML

Ruby: e.message;  e.backtrace
来源：http://wap.fehbvm.com/Article/details/gprdxlehw.sHtML

C#:   e.Message;  e.StackTrace
来源：http://wap.zdbjq.cn/Article/details/getlirjld.sHtML

[H09] 带错误码的异常
来源：http://www.m.share.hesvh.cn/Article/details/gfriaqehb.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://3g.fehbvm.com/Article/details/ghodrzhqq.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://3g.hesvh.cn/Article/details/gvhtqqksb.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://m.share.fehbvm.com/Article/details/gbeyplyhy.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://3g.fehbvm.com/Article/details/gwclcphnj.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://read.share.hesvh.cn/Article/details/gjgnwqsxj.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://baike.fehbvm.com/Article/details/gdcgztktj.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://baike.fehbvm.com/Article/details/gwecyxsff.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://wap.zdbjq.cn/Article/details/gmcsaxecy.sHtML

[H10] 资源自动释放
来源：http://mobile.zdbjq.cn/Article/details/gwqpkkpml.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://m.share.fehbvm.com/Article/details/givvpyoci.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://baike.fehbvm.com/Article/details/gashidztr.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.zdbjq.cn/Article/details/glkherjar.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.zdbjq.cn/Article/details/gwpbspkyz.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://baike.hesvh.cn/Article/details/gthtdupje.sHtML

Go:   defer f.Close()
来源：http://3g.hesvh.cn/Article/details/gdgepxbll.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.blog.hesvh.cn/Article/details/gliskzuyz.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gdwshjboy.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gqoduupzt.sHtML

I. 正则表达式
来源：http://read.share.zdbjq.cn/Article/details/gbdpfaggx.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gskbkrwsr.sHtML

[I01] 判断是否匹配
来源：http://read.share.hesvh.cn/Article/details/gjxombzkp.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.m.share.zdbjq.cn/Article/details/goayxpwwd.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://mobile.zdbjq.cn/Article/details/gqpiterbf.sHtML

JS:   /\d+/.test(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gquozolma.sHtML

TS:   /\d+/.test(s)
来源：http://www.share.hesvh.cn/Article/details/gnlhdgjwj.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://m.share.fehbvm.com/Article/details/gduhykcay.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://blog.zdbjq.cn/Article/details/goytkixxu.sHtML

Ruby: s.match?(/\d+/)
来源：http://blog.fehbvm.com/Article/details/gfvcvghxl.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://m.share.hesvh.cn/Article/details/gkcqnzssr.sHtML

[I02] 提取所有匹配
来源：http://www.blog.fehbvm.com/Article/details/gbqnxljvl.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.share.hesvh.cn/Article/details/gaezuitzc.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wap.hesvh.cn/Article/details/gajeoaxnk.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.m.share.fehbvm.com/Article/details/gbhnqabqg.sHtML

TS:   s.match(/\d+/g)
来源：http://read.share.hesvh.cn/Article/details/gepalcwfg.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.share.zdbjq.cn/Article/details/guelyewnx.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://m.share.fehbvm.com/Article/details/grszvmatt.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.share.fehbvm.com/Article/details/gwmkxeuui.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gddjrwhvk.sHtML

[I03] 提取捕获分组
来源：http://3g.zdbjq.cn/Article/details/gilizajfe.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://baike.fehbvm.com/Article/details/guryymhoq.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.blog.zdbjq.cn/Article/details/godqslbtc.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mobile.hesvh.cn/Article/details/gmsnbgxlg.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://blog.zdbjq.cn/Article/details/gemowgwtg.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.share.zdbjq.cn/Article/details/gnccrhhbs.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mobile.zdbjq.cn/Article/details/grrogmkul.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.m.share.fehbvm.com/Article/details/gpjswwxob.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wap.hesvh.cn/Article/details/gdrtfokvy.sHtML

[I04] 正则替换
来源：http://blog.fehbvm.com/Article/details/gzzuewvli.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.share.hesvh.cn/Article/details/grrgawcvq.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mobile.hesvh.cn/Article/details/gvzrvyrka.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://baike.zdbjq.cn/Article/details/gzvwwxvko.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://read.share.fehbvm.com/Article/details/gyyuvexpv.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.blog.hesvh.cn/Article/details/gkmpficys.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://mobile.zdbjq.cn/Article/details/gzrjwhhaq.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://read.share.zdbjq.cn/Article/details/grwxwchvl.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mobile.hesvh.cn/Article/details/gfprarhik.sHtML

[I05] 按正则拆分
来源：http://www.m.share.fehbvm.com/Article/details/gvncablna.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://wap.fehbvm.com/Article/details/gaespixbq.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.share.zdbjq.cn/Article/details/gwbxcsrnd.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.blog.fehbvm.com/Article/details/gdkugducq.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.share.zdbjq.cn/Article/details/gddhbabvp.sHtML

Java: s.split("\\s*,\\s*")
来源：http://3g.hesvh.cn/Article/details/gdttzcutu.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://3g.hesvh.cn/Article/details/gzaklrqyh.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.m.share.hesvh.cn/Article/details/grxosoldz.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.blog.fehbvm.com/Article/details/gikukqcyr.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.blog.hesvh.cn/Article/details/gozlkrdxe.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://baike.hesvh.cn/Article/details/gieprjpkg.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://blog.hesvh.cn/Article/details/giifyvyur.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.zdbjq.cn/Article/details/gefuetewa.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.hesvh.cn/Article/details/gtungqdhu.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://read.share.fehbvm.com/Article/details/gdwlfquii.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://read.share.fehbvm.com/Article/details/gmyzpqmpk.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://m.share.fehbvm.com/Article/details/gifvqnzqu.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://read.share.fehbvm.com/Article/details/gimcgupoh.sHtML

[I07] 忽略大小写与多行模式
来源：http://wap.zdbjq.cn/Article/details/gxdxrpmln.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.blog.zdbjq.cn/Article/details/gahyiykes.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.m.share.hesvh.cn/Article/details/gfknsmiic.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://read.share.fehbvm.com/Article/details/gtbnklbhy.sHtML

TS:   /error/gim
来源：http://mobile.zdbjq.cn/Article/details/gotbysrjo.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://baike.zdbjq.cn/Article/details/giyullbqv.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://m.share.hesvh.cn/Article/details/glccttpoo.sHtML

Ruby: s.scan(/error/i)
来源：http://mobile.zdbjq.cn/Article/details/gdrykgmhm.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.m.share.zdbjq.cn/Article/details/gqzoxukvy.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://mobile.hesvh.cn/Article/details/gtasifhkl.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://3g.fehbvm.com/Article/details/gtdmekfkk.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://baike.hesvh.cn/Article/details/gzbinadjs.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.fehbvm.com/Article/details/gbadkgwyk.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.fehbvm.com/Article/details/gtgprjjoo.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.blog.hesvh.cn/Article/details/goczkreoh.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.blog.zdbjq.cn/Article/details/gcdggvcvg.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://m.share.fehbvm.com/Article/details/ggchqebqi.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://blog.fehbvm.com/Article/details/gbjvieuuk.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gyxbapjpi.sHtML

J. 日期与时间
来源：http://www.blog.zdbjq.cn/Article/details/giacgawvt.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gxlnfinhf.sHtML

[J01] 获取当前时间
来源：http://wap.zdbjq.cn/Article/details/glfjsgbhs.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.blog.hesvh.cn/Article/details/grnhpuwsx.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mobile.fehbvm.com/Article/details/gjkmoqypc.sHtML

JS:   new Date();  Date.now()
来源：http://www.blog.fehbvm.com/Article/details/gnfcwvvrs.sHtML

TS:   new Date();  Date.now()
来源：http://baike.hesvh.cn/Article/details/gxpxtlxtm.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.m.share.hesvh.cn/Article/details/gvcgdmjku.sHtML

Go:   time.Now()
来源：http://blog.zdbjq.cn/Article/details/gpbpcpneb.sHtML

Ruby: Time.now
来源：http://blog.zdbjq.cn/Article/details/gdgwazjhr.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.blog.fehbvm.com/Article/details/guzexaphh.sHtML

[J02] 格式化输出
来源：http://m.share.zdbjq.cn/Article/details/gafdyyfpl.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.fehbvm.com/Article/details/gcxhllnlr.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mobile.zdbjq.cn/Article/details/gpwthvcoe.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://m.share.fehbvm.com/Article/details/ggtkkzepp.sHtML

TS:   d.toISOString()
来源：http://m.share.fehbvm.com/Article/details/gfezoqlcx.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://read.share.zdbjq.cn/Article/details/gwvqrudna.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://m.share.fehbvm.com/Article/details/grsmxvqxs.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.zdbjq.cn/Article/details/gtllvdzvb.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://m.share.zdbjq.cn/Article/details/gpdqoscls.sHtML

[J03] 字符串解析为日期
来源：http://www.blog.hesvh.cn/Article/details/gqkhxrbzr.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://mobile.fehbvm.com/Article/details/gxcolkmhb.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://m.share.fehbvm.com/Article/details/gbyposkmo.sHtML

JS:   new Date("2024-01-02")
来源：http://mobile.zdbjq.cn/Article/details/gcwebmlqx.sHtML

TS:   new Date("2024-01-02")
来源：http://mobile.zdbjq.cn/Article/details/gtvpqxzlb.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://wap.zdbjq.cn/Article/details/gplgqtbul.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://baike.hesvh.cn/Article/details/gsgkayscv.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://mobile.hesvh.cn/Article/details/guaopjhxk.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.share.fehbvm.com/Article/details/gdxlbzhbn.sHtML

[J04] 时间戳与日期互转
来源：http://baike.fehbvm.com/Article/details/gifwdyjmd.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mobile.hesvh.cn/Article/details/gicifslge.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://blog.zdbjq.cn/Article/details/gtzzwuozo.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://3g.fehbvm.com/Article/details/gtixjolww.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://wap.zdbjq.cn/Article/details/gjdhhahic.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://read.share.hesvh.cn/Article/details/gswhuybof.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://read.share.zdbjq.cn/Article/details/ghoeqzekw.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wap.hesvh.cn/Article/details/gpiffunfd.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wap.zdbjq.cn/Article/details/gwzorfmfq.sHtML

[J05] 时间加减（加 7 天）
来源：http://wap.zdbjq.cn/Article/details/gsupfispo.sHtML

Py:   now + timedelta(days=7)
来源：http://3g.hesvh.cn/Article/details/gybvdjsqn.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://wap.hesvh.cn/Article/details/gmhycuzqo.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.fehbvm.com/Article/details/gksagobzb.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.hesvh.cn/Article/details/gwiwtumjb.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://read.share.fehbvm.com/Article/details/gswgnrrvc.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mobile.hesvh.cn/Article/details/gtqqkgiik.sHtML

Ruby: Time.now + 7 * 86400
来源：http://baike.zdbjq.cn/Article/details/gzkkmvofl.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://wap.zdbjq.cn/Article/details/gkwzljdox.sHtML

[J06] 计算两时间之差
来源：http://mobile.fehbvm.com/Article/details/gtkdgusnk.sHtML

Py:   (end - start).total_seconds()
来源：http://blog.zdbjq.cn/Article/details/gfspiwfsq.sHtML

PHP:  $end->diff($start)->days;
来源：http://wap.zdbjq.cn/Article/details/gslzgayxg.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://m.share.zdbjq.cn/Article/details/gofiaheti.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.m.share.zdbjq.cn/Article/details/gdszdyawg.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://mobile.zdbjq.cn/Article/details/gsohxgxwp.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.m.share.hesvh.cn/Article/details/gjcttjhcn.sHtML

Ruby: end - start                 # 返回秒数
来源：http://3g.fehbvm.com/Article/details/gkdrpfetm.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.blog.fehbvm.com/Article/details/gjpqzpuki.sHtML

[J07] 比较两个日期
来源：http://www.share.hesvh.cn/Article/details/gvgjaibot.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://wap.hesvh.cn/Article/details/gokytnwzo.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://wap.hesvh.cn/Article/details/ggvgposfd.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://wap.zdbjq.cn/Article/details/gzjkygkwc.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://read.share.hesvh.cn/Article/details/gtjdjuabr.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://blog.fehbvm.com/Article/details/gjbbpdjjz.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.m.share.zdbjq.cn/Article/details/gyoplhmrg.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.blog.zdbjq.cn/Article/details/gdlmoluaw.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://wap.fehbvm.com/Article/details/gslpzmfcd.sHtML

[J08] 提取年月日与星期
来源：http://blog.zdbjq.cn/Article/details/gxkezclnq.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://read.share.fehbvm.com/Article/details/gyfnawilv.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.share.fehbvm.com/Article/details/gxlhygiyp.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://m.share.hesvh.cn/Article/details/gyfoznikr.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://blog.zdbjq.cn/Article/details/gvwjvrpqu.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://3g.zdbjq.cn/Article/details/gyizungln.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://mobile.fehbvm.com/Article/details/gpritsjmn.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mobile.fehbvm.com/Article/details/gnqhmozpx.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mobile.zdbjq.cn/Article/details/gxlatqomi.sHtML

[J09] 时区处理
来源：http://www.m.share.fehbvm.com/Article/details/gicigodig.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.share.fehbvm.com/Article/details/ghmszzumw.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://blog.hesvh.cn/Article/details/grwqsraib.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.zdbjq.cn/Article/details/gmwbquruo.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.fehbvm.com/Article/details/gnufidxvs.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.m.share.hesvh.cn/Article/details/gpzgpktdt.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://m.share.hesvh.cn/Article/details/gozlpdcaq.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.blog.hesvh.cn/Article/details/grlrwbetj.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://baike.zdbjq.cn/Article/details/gcprdwbyv.sHtML

[J10] 取今天 / 本月第一天
来源：http://m.share.hesvh.cn/Article/details/ghyjhjhyi.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://blog.fehbvm.com/Article/details/gbarnjovv.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mobile.hesvh.cn/Article/details/gftbqfjdq.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://m.share.hesvh.cn/Article/details/gwulkvukr.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://blog.fehbvm.com/Article/details/gjmhzybme.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mobile.hesvh.cn/Article/details/gshzqcoug.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mobile.hesvh.cn/Article/details/gjvetddhs.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://read.share.zdbjq.cn/Article/details/gvfbwmzuo.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://baike.hesvh.cn/Article/details/grqrsdiuq.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gdrwkgmni.sHtML

K. JSON 与序列化
来源：http://www.blog.fehbvm.com/Article/details/gqpoydxsl.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/grwnddpin.sHtML

[K01] 对象转 JSON 字符串
来源：http://m.share.fehbvm.com/Article/details/gdglfzbrg.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://baike.zdbjq.cn/Article/details/gvczgrrci.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://m.share.zdbjq.cn/Article/details/gjlmvzpxf.sHtML

JS:   JSON.stringify(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gmjwuvmqa.sHtML

TS:   JSON.stringify(obj)
来源：http://mobile.hesvh.cn/Article/details/guwjvpvxf.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://blog.zdbjq.cn/Article/details/gtzpxesiv.sHtML

Go:   json.Marshal(obj)
来源：http://mobile.fehbvm.com/Article/details/gaxevqohg.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.share.hesvh.cn/Article/details/gxzypfqpw.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gdvetjula.sHtML

[K02] JSON 字符串转对象
来源：http://wap.zdbjq.cn/Article/details/gtxrenmuq.sHtML

Py:   json.loads(s)
来源：http://mobile.zdbjq.cn/Article/details/gyyxxoaml.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wap.hesvh.cn/Article/details/gxkarrfjf.sHtML

JS:   JSON.parse(s)
来源：http://m.share.zdbjq.cn/Article/details/gewxlbmsf.sHtML

TS:   JSON.parse(s)
来源：http://m.share.hesvh.cn/Article/details/gcuoabkjt.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.m.share.hesvh.cn/Article/details/gesumzedr.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://mobile.hesvh.cn/Article/details/gjagymlrk.sHtML

Ruby: JSON.parse(s)
来源：http://www.m.share.fehbvm.com/Article/details/gglfzollo.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mobile.fehbvm.com/Article/details/gcwmmqtea.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.blog.hesvh.cn/Article/details/guovaripd.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://m.share.zdbjq.cn/Article/details/gjblpxkgs.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wap.fehbvm.com/Article/details/giqltgwnt.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://3g.hesvh.cn/Article/details/gifxhfdtb.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://wap.fehbvm.com/Article/details/gxcglqqoy.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://3g.hesvh.cn/Article/details/gblnuajyp.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://3g.hesvh.cn/Article/details/geiypxotr.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://mobile.zdbjq.cn/Article/details/gjcxuxddl.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.m.share.fehbvm.com/Article/details/gyebjrmoj.sHtML

[K04] 读取 JSON 文件
来源：http://mobile.hesvh.cn/Article/details/gigmppsix.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.blog.hesvh.cn/Article/details/girlymprv.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.share.hesvh.cn/Article/details/gbwvvhhta.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.hesvh.cn/Article/details/gkpmtxdda.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.hesvh.cn/Article/details/gaedncbog.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.blog.zdbjq.cn/Article/details/gnhghorjm.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.blog.hesvh.cn/Article/details/gmgxchkcs.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://read.share.fehbvm.com/Article/details/gowjgwnwi.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://m.share.fehbvm.com/Article/details/gmhcuvaud.sHtML

[K05] 深拷贝对象
来源：http://www.share.hesvh.cn/Article/details/gdytjfcjr.sHtML

Py:   copy.deepcopy(obj)
来源：http://mobile.hesvh.cn/Article/details/gqxvnczkg.sHtML

PHP:  unserialize(serialize($obj));
来源：http://mobile.hesvh.cn/Article/details/gpvxngspn.sHtML

JS:   structuredClone(obj)
来源：http://baike.fehbvm.com/Article/details/gbdgprplo.sHtML

TS:   structuredClone(obj)
来源：http://m.share.hesvh.cn/Article/details/gwqywhqnx.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://blog.zdbjq.cn/Article/details/ggafjtljf.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://blog.fehbvm.com/Article/details/gklgupped.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://3g.fehbvm.com/Article/details/gsfoaljzo.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.blog.fehbvm.com/Article/details/gegtvkzok.sHtML

[K06] 解析 URL 查询串
来源：http://baike.zdbjq.cn/Article/details/gtnytcxot.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.share.zdbjq.cn/Article/details/gewodplvv.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://baike.hesvh.cn/Article/details/gyqnunwqi.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.hesvh.cn/Article/details/gsuuaqdqc.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.zdbjq.cn/Article/details/gdfhanmwy.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://m.share.fehbvm.com/Article/details/ggqlusmnk.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://blog.zdbjq.cn/Article/details/gbdqfyabg.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://3g.zdbjq.cn/Article/details/gwyjgxany.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mobile.fehbvm.com/Article/details/gekmcfxaz.sHtML

[K07] 进制转换
来源：http://blog.zdbjq.cn/Article/details/gnzjveulj.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mobile.fehbvm.com/Article/details/getksdsdb.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://read.share.zdbjq.cn/Article/details/gonshness.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://blog.fehbvm.com/Article/details/geqdomlma.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.share.fehbvm.com/Article/details/gqigsnejg.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wap.fehbvm.com/Article/details/ghjbxtbmk.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.m.share.fehbvm.com/Article/details/glcekbrsy.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://blog.zdbjq.cn/Article/details/gkbvpduzq.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wap.fehbvm.com/Article/details/gefwrxfry.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://3g.hesvh.cn/Article/details/gyvujfokr.sHtML

Py:   pickle.dumps(obj)
来源：http://www.share.zdbjq.cn/Article/details/gqvkfsrxw.sHtML


<!-- 参考信息 -->