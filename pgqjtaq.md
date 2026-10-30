代发 wailian999

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.hesvh.cn/Article/details/gkzrdkjuy.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/gbgwxjjrz.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.hesvh.cn/Article/details/gbwgohlwr.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.zdbjq.cn/Article/details/gvfzjqrqq.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.zdbjq.cn/Article/details/gwgtqbqnc.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.fehbvm.com/Article/details/gxjlbrdlf.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.hesvh.cn/Article/details/gqaxhlhns.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://wap.zdbjq.cn/Article/details/gvzjfgtnv.sHtML

[H03] 主动抛出异常
来源：http://wap.zdbjq.cn/Article/details/glahwtaox.sHtML

Py:   raise ValueError("错误信息")
来源：http://3g.zdbjq.cn/Article/details/gxabbfkiv.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://baike.fehbvm.com/Article/details/gvtshtdga.sHtML

JS:   throw new Error("错误信息");
来源：http://read.share.hesvh.cn/Article/details/gtaqxqzsq.sHtML

TS:   throw new Error("错误信息");
来源：http://read.share.fehbvm.com/Article/details/ghjlfhfqa.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://baike.zdbjq.cn/Article/details/gskyvjang.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.share.fehbvm.com/Article/details/gavrgpxjz.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://blog.hesvh.cn/Article/details/gkcfpsvak.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://mobile.fehbvm.com/Article/details/grdkbfsio.sHtML

[H04] 自定义异常类型
来源：http://3g.zdbjq.cn/Article/details/ggzjrnzgp.sHtML

Py:   class MyError(Exception): pass
来源：http://m.share.fehbvm.com/Article/details/gfjzlxqjt.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://m.share.fehbvm.com/Article/details/gqkvnubzz.sHtML

JS:   class MyError extends Error {}
来源：http://www.share.fehbvm.com/Article/details/glenkrrst.sHtML

TS:   class MyError extends Error {}
来源：http://blog.zdbjq.cn/Article/details/gexzgsgjf.sHtML

Java: class MyException extends RuntimeException {}
来源：http://baike.zdbjq.cn/Article/details/gdcceqkow.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://baike.zdbjq.cn/Article/details/ganvkyioa.sHtML

Ruby: class MyError < StandardError; end
来源：http://m.share.hesvh.cn/Article/details/gbzhygldg.sHtML

C#:   class MyException : Exception {}
来源：http://m.share.fehbvm.com/Article/details/gwrrfsuxo.sHtML

[H05] 捕获特定类型
来源：http://blog.fehbvm.com/Article/details/gxajmfbyh.sHtML

Py:   except ValueError as e:
来源：http://www.share.hesvh.cn/Article/details/gzqckxrkj.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.share.fehbvm.com/Article/details/gziobxdyh.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://blog.hesvh.cn/Article/details/gqflogome.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.blog.fehbvm.com/Article/details/gpwcbtgwy.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.fehbvm.com/Article/details/gmdwmaptb.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.m.share.fehbvm.com/Article/details/gjqgboger.sHtML

Ruby: rescue ArgumentError => e
来源：http://wap.zdbjq.cn/Article/details/gkriusvcz.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mobile.fehbvm.com/Article/details/gxmvxpxeb.sHtML

[H06] 可选值 / 空值安全访问
来源：http://3g.fehbvm.com/Article/details/giwjgshei.sHtML

Py:   value = d.get("k") or default
来源：http://m.share.fehbvm.com/Article/details/gazwothsq.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.zdbjq.cn/Article/details/gwiegahep.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.fehbvm.com/Article/details/gubxjvlmd.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://blog.zdbjq.cn/Article/details/gqgliasrv.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://3g.hesvh.cn/Article/details/gutoncggc.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.share.fehbvm.com/Article/details/gglbxrmsb.sHtML

Ruby: d&.dig(:a, :b)
来源：http://baike.fehbvm.com/Article/details/gcfuowpxl.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.share.fehbvm.com/Article/details/geycammag.sHtML

[H07] 断言
来源：http://www.blog.hesvh.cn/Article/details/gtufaeuez.sHtML

Py:   assert x > 0, "必须为正"
来源：http://m.share.fehbvm.com/Article/details/gjwinvppr.sHtML

PHP:  assert($x > 0);
来源：http://mobile.hesvh.cn/Article/details/gjojjccgi.sHtML

JS:   console.assert(x > 0);
来源：http://wap.hesvh.cn/Article/details/gyggemmej.sHtML

TS:   console.assert(x > 0);
来源：http://3g.zdbjq.cn/Article/details/gwzbehsfg.sHtML

Java: assert x > 0 : "必须为正";
来源：http://blog.hesvh.cn/Article/details/gydnuyhvy.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://m.share.hesvh.cn/Article/details/gdgoxhlgn.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://blog.hesvh.cn/Article/details/gfkorrnoq.sHtML

C#:   Debug.Assert(x > 0);
来源：http://mobile.fehbvm.com/Article/details/ghedzzjfc.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.share.zdbjq.cn/Article/details/gqyakrpwm.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://read.share.fehbvm.com/Article/details/gfnqifxhy.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://read.share.zdbjq.cn/Article/details/ghnmdzqwp.sHtML

JS:   e.message;  e.stack
来源：http://www.blog.zdbjq.cn/Article/details/gnimxmfxc.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://3g.zdbjq.cn/Article/details/gwlxufdmw.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://baike.fehbvm.com/Article/details/gcywjtizw.sHtML

Go:   err.Error()
来源：http://blog.hesvh.cn/Article/details/gzkhnuroh.sHtML

Ruby: e.message;  e.backtrace
来源：http://wap.hesvh.cn/Article/details/ggngpdvrj.sHtML

C#:   e.Message;  e.StackTrace
来源：http://read.share.hesvh.cn/Article/details/gbhnijakd.sHtML

[H09] 带错误码的异常
来源：http://3g.zdbjq.cn/Article/details/grliuwhth.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mobile.fehbvm.com/Article/details/gbruyzwml.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.share.hesvh.cn/Article/details/gkyqxkcab.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://3g.zdbjq.cn/Article/details/gujlfiijm.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://m.share.hesvh.cn/Article/details/gleqfilbr.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.share.fehbvm.com/Article/details/gmxselkwu.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://read.share.fehbvm.com/Article/details/ggdkegald.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://3g.hesvh.cn/Article/details/gzbiyalvz.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://m.share.hesvh.cn/Article/details/gmhsnugeu.sHtML

[H10] 资源自动释放
来源：http://www.blog.hesvh.cn/Article/details/gavopcief.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://3g.fehbvm.com/Article/details/gbpgjjaqt.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://baike.zdbjq.cn/Article/details/gghejszyc.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.fehbvm.com/Article/details/ghawndafz.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.zdbjq.cn/Article/details/gwpixgqvj.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.blog.hesvh.cn/Article/details/gjyvpejdi.sHtML

Go:   defer f.Close()
来源：http://3g.fehbvm.com/Article/details/gzbmttrwx.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wap.hesvh.cn/Article/details/gvphaceey.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://3g.fehbvm.com/Article/details/gaodrveot.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gzyueabgh.sHtML

I. 正则表达式
来源：http://blog.fehbvm.com/Article/details/gkjgcwfdl.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/guyskikey.sHtML

[I01] 判断是否匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gbmsizhal.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.blog.hesvh.cn/Article/details/gevwbdiwa.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.blog.fehbvm.com/Article/details/gvtmgygai.sHtML

JS:   /\d+/.test(s)
来源：http://baike.hesvh.cn/Article/details/gnjcnnfpm.sHtML

TS:   /\d+/.test(s)
来源：http://blog.hesvh.cn/Article/details/gyexwxege.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://blog.hesvh.cn/Article/details/ghkhqldej.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://m.share.hesvh.cn/Article/details/gywneaagh.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.m.share.hesvh.cn/Article/details/gzbisbsgi.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.share.hesvh.cn/Article/details/ggachcbra.sHtML

[I02] 提取所有匹配
来源：http://read.share.zdbjq.cn/Article/details/gqjgisvsc.sHtML

Py:   re.findall(r"\d+", s)
来源：http://mobile.fehbvm.com/Article/details/gxdritvtb.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://3g.zdbjq.cn/Article/details/gomaxpokp.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://baike.fehbvm.com/Article/details/gtkjqzmzy.sHtML

TS:   s.match(/\d+/g)
来源：http://wap.fehbvm.com/Article/details/gdzeuugcq.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.blog.hesvh.cn/Article/details/gptkosmqa.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://3g.fehbvm.com/Article/details/gqhduqhih.sHtML

Ruby: s.scan(/\d+/)
来源：http://baike.hesvh.cn/Article/details/gwmklkkya.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://m.share.hesvh.cn/Article/details/gdpmqjfzr.sHtML

[I03] 提取捕获分组
来源：http://baike.hesvh.cn/Article/details/ghpvniqfp.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://read.share.hesvh.cn/Article/details/gsnbgewso.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://baike.hesvh.cn/Article/details/gzhgzetyo.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://blog.hesvh.cn/Article/details/gessrpohc.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://read.share.fehbvm.com/Article/details/gwfvddatt.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://baike.hesvh.cn/Article/details/gbxdazxgl.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://baike.fehbvm.com/Article/details/gllusbeuo.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://read.share.zdbjq.cn/Article/details/guxehcsae.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://baike.fehbvm.com/Article/details/grfuugtyg.sHtML

[I04] 正则替换
来源：http://www.blog.fehbvm.com/Article/details/gthonjobj.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.m.share.zdbjq.cn/Article/details/gcofmjksb.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://read.share.fehbvm.com/Article/details/ggxorlnsk.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://m.share.hesvh.cn/Article/details/georvgzeg.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://3g.fehbvm.com/Article/details/gscqqpnmo.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://wap.zdbjq.cn/Article/details/gzhgoosen.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.blog.hesvh.cn/Article/details/ghortdaik.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.share.hesvh.cn/Article/details/gneyhjeyp.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://wap.hesvh.cn/Article/details/grirrfudc.sHtML

[I05] 按正则拆分
来源：http://read.share.zdbjq.cn/Article/details/gwrxsznrs.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://mobile.hesvh.cn/Article/details/gkrfgnhqe.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://baike.zdbjq.cn/Article/details/gfyxkemwy.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.blog.fehbvm.com/Article/details/guabjnrly.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.m.share.zdbjq.cn/Article/details/gsijqkuak.sHtML

Java: s.split("\\s*,\\s*")
来源：http://m.share.hesvh.cn/Article/details/gswktnbql.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://mobile.zdbjq.cn/Article/details/ggcxizxki.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.m.share.hesvh.cn/Article/details/gbormnnro.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://blog.hesvh.cn/Article/details/gcbllwjlz.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://read.share.fehbvm.com/Article/details/ghlggzwzx.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://baike.hesvh.cn/Article/details/ghjqnriyf.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.m.share.fehbvm.com/Article/details/gvabdwpvf.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.hesvh.cn/Article/details/gkvhiukyw.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.fehbvm.com/Article/details/gjsodalan.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://m.share.hesvh.cn/Article/details/gappcujys.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.blog.fehbvm.com/Article/details/grltvuswb.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://mobile.hesvh.cn/Article/details/gmodkzcsw.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://3g.hesvh.cn/Article/details/gmjjigqxl.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.blog.zdbjq.cn/Article/details/ggqnuopdh.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.m.share.fehbvm.com/Article/details/gfekkxept.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wap.zdbjq.cn/Article/details/gdbinsnhf.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://3g.fehbvm.com/Article/details/ggriycnwc.sHtML

TS:   /error/gim
来源：http://m.share.hesvh.cn/Article/details/gvplmgmrs.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://blog.fehbvm.com/Article/details/gndbvhfwf.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://blog.fehbvm.com/Article/details/glwvvclji.sHtML

Ruby: s.scan(/error/i)
来源：http://www.blog.zdbjq.cn/Article/details/ghxdslxxg.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://wap.zdbjq.cn/Article/details/gmyxjwvpe.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gtkipriyv.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://blog.zdbjq.cn/Article/details/gpgivyimh.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.share.zdbjq.cn/Article/details/gwzhudfiv.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.fehbvm.com/Article/details/gcnqiroyk.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.fehbvm.com/Article/details/gqibzukge.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://m.share.hesvh.cn/Article/details/gpuptgpip.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://mobile.fehbvm.com/Article/details/gxlxqjzyy.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://read.share.hesvh.cn/Article/details/gdjcdblml.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.share.fehbvm.com/Article/details/ghehnxfvo.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gtubfejvp.sHtML

J. 日期与时间
来源：http://wap.zdbjq.cn/Article/details/gpphjyvvp.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gdovctrzh.sHtML

[J01] 获取当前时间
来源：http://www.m.share.fehbvm.com/Article/details/gryobfphi.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://read.share.fehbvm.com/Article/details/gwjzxzrze.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://3g.fehbvm.com/Article/details/gkescorji.sHtML

JS:   new Date();  Date.now()
来源：http://www.share.fehbvm.com/Article/details/ggtflyfjw.sHtML

TS:   new Date();  Date.now()
来源：http://read.share.zdbjq.cn/Article/details/gpgmgcvsw.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.m.share.hesvh.cn/Article/details/gsfmxmjwh.sHtML

Go:   time.Now()
来源：http://www.share.hesvh.cn/Article/details/grbipixly.sHtML

Ruby: Time.now
来源：http://www.m.share.fehbvm.com/Article/details/gcdnhcjlz.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://m.share.hesvh.cn/Article/details/gagkxaimu.sHtML

[J02] 格式化输出
来源：http://www.blog.hesvh.cn/Article/details/gwdjlnwgx.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.hesvh.cn/Article/details/gnfauoqvs.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.m.share.fehbvm.com/Article/details/gearsvaec.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.blog.fehbvm.com/Article/details/gecatiepz.sHtML

TS:   d.toISOString()
来源：http://m.share.zdbjq.cn/Article/details/gfccemtac.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.blog.fehbvm.com/Article/details/giczvzvct.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://mobile.zdbjq.cn/Article/details/gfsngdbpm.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.hesvh.cn/Article/details/gpdotpzsz.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://m.share.hesvh.cn/Article/details/gslohdbyj.sHtML

[J03] 字符串解析为日期
来源：http://3g.zdbjq.cn/Article/details/gctoiuvir.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://baike.hesvh.cn/Article/details/gqpnljegs.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://m.share.hesvh.cn/Article/details/grjpochfp.sHtML

JS:   new Date("2024-01-02")
来源：http://read.share.hesvh.cn/Article/details/gamzghodc.sHtML

TS:   new Date("2024-01-02")
来源：http://www.m.share.hesvh.cn/Article/details/gxirtfgac.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://3g.zdbjq.cn/Article/details/gkchqfood.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mobile.hesvh.cn/Article/details/glnuiaawx.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.share.zdbjq.cn/Article/details/gyxevawbp.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://read.share.fehbvm.com/Article/details/gyyptjygv.sHtML

[J04] 时间戳与日期互转
来源：http://3g.hesvh.cn/Article/details/gzsfyzmpb.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://m.share.zdbjq.cn/Article/details/gcfrgfjcm.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://baike.zdbjq.cn/Article/details/genuxcuvf.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://m.share.zdbjq.cn/Article/details/ghpvqcfvp.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://blog.zdbjq.cn/Article/details/gqskyqtaq.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://m.share.hesvh.cn/Article/details/gfpmzwxwg.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://mobile.fehbvm.com/Article/details/gnxqieeyf.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.share.zdbjq.cn/Article/details/gteiwsfxf.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://m.share.zdbjq.cn/Article/details/gfpnqbddo.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.share.fehbvm.com/Article/details/gdnhprgta.sHtML

Py:   now + timedelta(days=7)
来源：http://baike.fehbvm.com/Article/details/gpxubqqqt.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://mobile.zdbjq.cn/Article/details/gaqdmuzot.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.zdbjq.cn/Article/details/gnkrttvxf.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.zdbjq.cn/Article/details/gutvpgnrr.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://mobile.hesvh.cn/Article/details/gwldvylfu.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mobile.fehbvm.com/Article/details/gpfrjkdon.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.blog.zdbjq.cn/Article/details/ggwiodfxo.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.m.share.hesvh.cn/Article/details/gqhlalueq.sHtML

[J06] 计算两时间之差
来源：http://read.share.fehbvm.com/Article/details/gxejrqwls.sHtML

Py:   (end - start).total_seconds()
来源：http://wap.fehbvm.com/Article/details/gptthuhft.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.m.share.hesvh.cn/Article/details/gmsgrmnlf.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://blog.fehbvm.com/Article/details/gkzbkexsc.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://baike.zdbjq.cn/Article/details/gbwuheglb.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://m.share.hesvh.cn/Article/details/gldzxdphv.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.m.share.hesvh.cn/Article/details/gieaaoner.sHtML

Ruby: end - start                 # 返回秒数
来源：http://m.share.fehbvm.com/Article/details/goiltvwbc.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.m.share.zdbjq.cn/Article/details/gcrwxxgym.sHtML

[J07] 比较两个日期
来源：http://3g.zdbjq.cn/Article/details/ggqttalbk.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://read.share.zdbjq.cn/Article/details/gfdlvmbpw.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://3g.zdbjq.cn/Article/details/gxtlxqpek.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://blog.zdbjq.cn/Article/details/gidamlzuv.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://baike.fehbvm.com/Article/details/gbvwzmtcn.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wap.fehbvm.com/Article/details/gcavfngzl.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://3g.zdbjq.cn/Article/details/gxqfnhytb.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://3g.zdbjq.cn/Article/details/gnxhbhebh.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://3g.zdbjq.cn/Article/details/giotlwedv.sHtML

[J08] 提取年月日与星期
来源：http://m.share.zdbjq.cn/Article/details/gaibzeosb.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://read.share.hesvh.cn/Article/details/gjhnubtsl.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.blog.fehbvm.com/Article/details/gonxqckvm.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://baike.zdbjq.cn/Article/details/grsmrntav.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.m.share.hesvh.cn/Article/details/gpnettmej.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mobile.fehbvm.com/Article/details/guaiolbfh.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://blog.fehbvm.com/Article/details/gtbdopevs.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mobile.hesvh.cn/Article/details/ghwqckmqr.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://baike.fehbvm.com/Article/details/gwonpbefr.sHtML

[J09] 时区处理
来源：http://3g.hesvh.cn/Article/details/gthddspyw.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mobile.zdbjq.cn/Article/details/gkzfbejxe.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://mobile.zdbjq.cn/Article/details/guxamcegk.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.hesvh.cn/Article/details/grkfqtfyv.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.hesvh.cn/Article/details/gsggsklqw.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://3g.fehbvm.com/Article/details/gfujupked.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wap.hesvh.cn/Article/details/gplkypwyj.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.blog.fehbvm.com/Article/details/gqoqtlkxy.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://baike.zdbjq.cn/Article/details/gaxafjafi.sHtML

[J10] 取今天 / 本月第一天
来源：http://baike.fehbvm.com/Article/details/gznzlyokh.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://wap.fehbvm.com/Article/details/gsxxubczz.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.blog.hesvh.cn/Article/details/gviygnlir.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://blog.zdbjq.cn/Article/details/guhkngpbf.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://blog.zdbjq.cn/Article/details/gbkicuaho.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://m.share.fehbvm.com/Article/details/ghlznamay.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://baike.zdbjq.cn/Article/details/gsipyvmip.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mobile.zdbjq.cn/Article/details/gycsuwfyh.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.m.share.hesvh.cn/Article/details/gtmaliidd.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gqiekrjse.sHtML

K. JSON 与序列化
来源：http://blog.hesvh.cn/Article/details/gwbcgnobg.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gizejuuau.sHtML

[K01] 对象转 JSON 字符串
来源：http://m.share.zdbjq.cn/Article/details/ghfsrdnlt.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wap.hesvh.cn/Article/details/gqoejhtkc.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://3g.hesvh.cn/Article/details/gnslutdhw.sHtML

JS:   JSON.stringify(obj)
来源：http://wap.hesvh.cn/Article/details/gwtnzkarp.sHtML

TS:   JSON.stringify(obj)
来源：http://mobile.fehbvm.com/Article/details/ggxdzgfig.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.share.fehbvm.com/Article/details/gqzhlbxkg.sHtML

Go:   json.Marshal(obj)
来源：http://www.share.fehbvm.com/Article/details/ghqsgdwpr.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://mobile.fehbvm.com/Article/details/gxqpiiwup.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://wap.hesvh.cn/Article/details/guwubmbgg.sHtML

[K02] JSON 字符串转对象
来源：http://www.share.hesvh.cn/Article/details/ggsbrqkvn.sHtML

Py:   json.loads(s)
来源：http://www.blog.fehbvm.com/Article/details/gfrrdjwsf.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://baike.hesvh.cn/Article/details/gzlliywkt.sHtML

JS:   JSON.parse(s)
来源：http://www.blog.zdbjq.cn/Article/details/gdjlrjyoc.sHtML

TS:   JSON.parse(s)
来源：http://3g.hesvh.cn/Article/details/gdhxvibwu.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://m.share.hesvh.cn/Article/details/gsargwsoy.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://mobile.zdbjq.cn/Article/details/ggwmhdfcp.sHtML

Ruby: JSON.parse(s)
来源：http://wap.zdbjq.cn/Article/details/gufqhtodl.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.m.share.hesvh.cn/Article/details/grdagiolt.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://baike.fehbvm.com/Article/details/gmesvyqto.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://read.share.fehbvm.com/Article/details/gkwdnykxz.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.share.hesvh.cn/Article/details/gkjygreoe.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://read.share.fehbvm.com/Article/details/gedrntgpw.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://mobile.hesvh.cn/Article/details/gorgykkej.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gsstfgmrl.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.share.hesvh.cn/Article/details/gzbipzlxr.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://baike.zdbjq.cn/Article/details/gekbfxtax.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mobile.zdbjq.cn/Article/details/gcrzhrvae.sHtML

[K04] 读取 JSON 文件
来源：http://read.share.zdbjq.cn/Article/details/gvikmrkap.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://3g.zdbjq.cn/Article/details/gwgigjafj.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.share.fehbvm.com/Article/details/gecmblflw.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.fehbvm.com/Article/details/gvcetcldv.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.hesvh.cn/Article/details/gdjuophft.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.share.zdbjq.cn/Article/details/gzrzrvwix.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mobile.hesvh.cn/Article/details/gjsbjkcma.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://blog.hesvh.cn/Article/details/gktcwattl.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://m.share.zdbjq.cn/Article/details/gudgikmdt.sHtML

[K05] 深拷贝对象
来源：http://www.m.share.fehbvm.com/Article/details/ggelzxqgh.sHtML

Py:   copy.deepcopy(obj)
来源：http://m.share.hesvh.cn/Article/details/gqhujdyhj.sHtML

PHP:  unserialize(serialize($obj));
来源：http://baike.fehbvm.com/Article/details/grwobmbon.sHtML

JS:   structuredClone(obj)
来源：http://blog.hesvh.cn/Article/details/gaqudzslr.sHtML

TS:   structuredClone(obj)
来源：http://m.share.fehbvm.com/Article/details/groatyksp.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://mobile.zdbjq.cn/Article/details/gmktwtwzw.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://m.share.zdbjq.cn/Article/details/gtjndwprv.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://m.share.fehbvm.com/Article/details/gyyjpnjlh.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://read.share.hesvh.cn/Article/details/gnhpyrfnf.sHtML

[K06] 解析 URL 查询串
来源：http://blog.fehbvm.com/Article/details/gozaedxoj.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.blog.zdbjq.cn/Article/details/gojwkgkff.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://m.share.hesvh.cn/Article/details/gfyygmjpd.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.zdbjq.cn/Article/details/gwkkokomx.sHtML


<!-- 参考信息 -->