代发 wailian999

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://blog.hesvh.cn/Article/details/gewbnelkt.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.share.fehbvm.com/Article/details/gdoqwaent.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.m.share.fehbvm.com/Article/details/gsilvrrsf.sHtML

[H02] finally / ensure 收尾
来源：http://www.m.share.fehbvm.com/Article/details/gryjjfpkq.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.hesvh.cn/Article/details/gylmhnzbf.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.share.fehbvm.com/Article/details/gheqvjysb.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gmjaibsqo.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.fehbvm.com/Article/details/gnyalxcdv.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/gdsbdbyik.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://m.share.zdbjq.cn/Article/details/gwykhoutm.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.share.zdbjq.cn/Article/details/gyjrnkoua.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://3g.hesvh.cn/Article/details/gkztmgpep.sHtML

[H03] 主动抛出异常
来源：http://www.blog.hesvh.cn/Article/details/gcqbwrvom.sHtML

Py:   raise ValueError("错误信息")
来源：http://read.share.hesvh.cn/Article/details/ggdocccrk.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://baike.zdbjq.cn/Article/details/gvqpgnvav.sHtML

JS:   throw new Error("错误信息");
来源：http://www.m.share.zdbjq.cn/Article/details/gchvckiig.sHtML

TS:   throw new Error("错误信息");
来源：http://read.share.fehbvm.com/Article/details/gnrgexuqy.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.m.share.fehbvm.com/Article/details/gkfshyiht.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.m.share.fehbvm.com/Article/details/gomcrhphd.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://baike.zdbjq.cn/Article/details/gluziajfb.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://mobile.hesvh.cn/Article/details/gglrybwff.sHtML

[H04] 自定义异常类型
来源：http://mobile.zdbjq.cn/Article/details/gfkmwpodp.sHtML

Py:   class MyError(Exception): pass
来源：http://wap.hesvh.cn/Article/details/gzgajungp.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://mobile.zdbjq.cn/Article/details/gzpnmjzfb.sHtML

JS:   class MyError extends Error {}
来源：http://www.share.hesvh.cn/Article/details/gcrmgrwjm.sHtML

TS:   class MyError extends Error {}
来源：http://www.share.zdbjq.cn/Article/details/gjttdtmyh.sHtML

Java: class MyException extends RuntimeException {}
来源：http://m.share.fehbvm.com/Article/details/gacbjyndy.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.m.share.hesvh.cn/Article/details/gtvqxnvyg.sHtML

Ruby: class MyError < StandardError; end
来源：http://3g.fehbvm.com/Article/details/gsjkhzwwl.sHtML

C#:   class MyException : Exception {}
来源：http://www.m.share.zdbjq.cn/Article/details/gkqxtvgzm.sHtML

[H05] 捕获特定类型
来源：http://baike.fehbvm.com/Article/details/ggnmsnqjx.sHtML

Py:   except ValueError as e:
来源：http://mobile.hesvh.cn/Article/details/gcyaurkbv.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.blog.zdbjq.cn/Article/details/gpnqphygm.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://baike.fehbvm.com/Article/details/geleudctx.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.blog.hesvh.cn/Article/details/ggcwipcyl.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gmexxsstc.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.blog.zdbjq.cn/Article/details/gqqxsipke.sHtML

Ruby: rescue ArgumentError => e
来源：http://blog.hesvh.cn/Article/details/gkbdrshta.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://blog.fehbvm.com/Article/details/gwbukzrgf.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.zdbjq.cn/Article/details/gqrjkeekg.sHtML

Py:   value = d.get("k") or default
来源：http://www.m.share.zdbjq.cn/Article/details/gcukyqluv.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.zdbjq.cn/Article/details/gfljivujh.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://baike.zdbjq.cn/Article/details/gzvyvaiql.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://m.share.zdbjq.cn/Article/details/gnjdsbptp.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://baike.zdbjq.cn/Article/details/gvqvczuzg.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://read.share.hesvh.cn/Article/details/gmxsaupdl.sHtML

Ruby: d&.dig(:a, :b)
来源：http://mobile.zdbjq.cn/Article/details/gqowzkuzh.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.share.hesvh.cn/Article/details/glqjuyzcs.sHtML

[H07] 断言
来源：http://blog.fehbvm.com/Article/details/gqutrpqto.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.blog.zdbjq.cn/Article/details/gwlshcukg.sHtML

PHP:  assert($x > 0);
来源：http://3g.zdbjq.cn/Article/details/gzpvymzwc.sHtML

JS:   console.assert(x > 0);
来源：http://3g.zdbjq.cn/Article/details/gzeugfvuz.sHtML

TS:   console.assert(x > 0);
来源：http://3g.fehbvm.com/Article/details/gpvxmmkqw.sHtML

Java: assert x > 0 : "必须为正";
来源：http://3g.fehbvm.com/Article/details/gijrgjsml.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://blog.hesvh.cn/Article/details/gtxkcaxfu.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.m.share.zdbjq.cn/Article/details/gtowwmtjt.sHtML

C#:   Debug.Assert(x > 0);
来源：http://3g.hesvh.cn/Article/details/ggvrfxxad.sHtML

[H08] 获取错误信息与堆栈
来源：http://mobile.fehbvm.com/Article/details/glqlvovnp.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.m.share.hesvh.cn/Article/details/gxzpstbsf.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.blog.fehbvm.com/Article/details/gilerjtat.sHtML

JS:   e.message;  e.stack
来源：http://www.blog.fehbvm.com/Article/details/ggqkjhtfn.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.share.zdbjq.cn/Article/details/gvvgbysmg.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://wap.fehbvm.com/Article/details/gdoyqopnj.sHtML

Go:   err.Error()
来源：http://www.m.share.fehbvm.com/Article/details/gtmovmsch.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.share.hesvh.cn/Article/details/geibkrdgn.sHtML

C#:   e.Message;  e.StackTrace
来源：http://mobile.hesvh.cn/Article/details/gnqrhuiqn.sHtML

[H09] 带错误码的异常
来源：http://wap.hesvh.cn/Article/details/gsmbxqmth.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://blog.zdbjq.cn/Article/details/gfvdtmcyr.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://blog.fehbvm.com/Article/details/gpmwxsrbn.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://3g.zdbjq.cn/Article/details/gbgjygdnl.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.share.zdbjq.cn/Article/details/gikrgvonj.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://baike.fehbvm.com/Article/details/gyorhqnvm.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wap.fehbvm.com/Article/details/grbzactav.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.share.fehbvm.com/Article/details/ggsrhgfmn.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://mobile.hesvh.cn/Article/details/gthexwpby.sHtML

[H10] 资源自动释放
来源：http://blog.zdbjq.cn/Article/details/gsudbmsdl.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://wap.zdbjq.cn/Article/details/gthoayvct.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.m.share.hesvh.cn/Article/details/ggryppiqg.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.zdbjq.cn/Article/details/gawpywxva.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.fehbvm.com/Article/details/gqupfrlbv.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.share.zdbjq.cn/Article/details/gtsepeytm.sHtML

Go:   defer f.Close()
来源：http://mobile.fehbvm.com/Article/details/gcwocinxw.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://baike.zdbjq.cn/Article/details/gebsrmtlb.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gyskasdct.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gzmejandk.sHtML

I. 正则表达式
来源：http://www.blog.zdbjq.cn/Article/details/gbdebeupg.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gskoquvfl.sHtML

[I01] 判断是否匹配
来源：http://wap.fehbvm.com/Article/details/gblmlxari.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://blog.hesvh.cn/Article/details/gytqkblom.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://wap.zdbjq.cn/Article/details/gedqdzjsb.sHtML

JS:   /\d+/.test(s)
来源：http://www.share.hesvh.cn/Article/details/gcwwkepzf.sHtML

TS:   /\d+/.test(s)
来源：http://mobile.zdbjq.cn/Article/details/gugnefdol.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.share.fehbvm.com/Article/details/gzslnipiy.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.share.fehbvm.com/Article/details/gaurwbqbf.sHtML

Ruby: s.match?(/\d+/)
来源：http://m.share.zdbjq.cn/Article/details/gsgeurszb.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://baike.fehbvm.com/Article/details/gxvbtofqh.sHtML

[I02] 提取所有匹配
来源：http://read.share.zdbjq.cn/Article/details/ggsgxkaeq.sHtML

Py:   re.findall(r"\d+", s)
来源：http://blog.fehbvm.com/Article/details/ggousyvva.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.share.fehbvm.com/Article/details/gpbmsjjiy.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.blog.fehbvm.com/Article/details/gzmkyabpn.sHtML

TS:   s.match(/\d+/g)
来源：http://wap.hesvh.cn/Article/details/glirfupoh.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://m.share.hesvh.cn/Article/details/gqetzfljz.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.blog.hesvh.cn/Article/details/godfbgdfo.sHtML

Ruby: s.scan(/\d+/)
来源：http://baike.hesvh.cn/Article/details/gbgefjfjx.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://blog.fehbvm.com/Article/details/gdjdrovwf.sHtML

[I03] 提取捕获分组
来源：http://3g.zdbjq.cn/Article/details/gbfxeoxgi.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gzsvlrerd.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.share.hesvh.cn/Article/details/gfhshssqz.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wap.fehbvm.com/Article/details/gsqhzjsxx.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mobile.fehbvm.com/Article/details/gzisazrqt.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.m.share.zdbjq.cn/Article/details/gukrfgrbz.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.share.zdbjq.cn/Article/details/gmfadkigr.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.share.fehbvm.com/Article/details/gbcshfwab.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://read.share.fehbvm.com/Article/details/geipgkiso.sHtML

[I04] 正则替换
来源：http://www.blog.fehbvm.com/Article/details/ghloefquw.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.blog.zdbjq.cn/Article/details/gnxjfxaip.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wap.zdbjq.cn/Article/details/gunybypvw.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://baike.zdbjq.cn/Article/details/gtfhrnpbt.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://3g.zdbjq.cn/Article/details/gvnfhqode.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.blog.hesvh.cn/Article/details/grpntkuyd.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://wap.fehbvm.com/Article/details/gtpbxinlz.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://mobile.zdbjq.cn/Article/details/gnclyypwh.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://3g.hesvh.cn/Article/details/ganrrkkjn.sHtML

[I05] 按正则拆分
来源：http://mobile.hesvh.cn/Article/details/gujjoqujk.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://3g.fehbvm.com/Article/details/gacalocvz.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.blog.hesvh.cn/Article/details/gdgfnsjck.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://wap.zdbjq.cn/Article/details/gsgxnlnib.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.m.share.zdbjq.cn/Article/details/gxohmfges.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.m.share.fehbvm.com/Article/details/ghixxlozr.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.share.zdbjq.cn/Article/details/gktqqimqj.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.blog.fehbvm.com/Article/details/ggzaihivw.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.m.share.zdbjq.cn/Article/details/gvamsnxzx.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wap.hesvh.cn/Article/details/gzqjyaiag.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://m.share.zdbjq.cn/Article/details/giywbaxme.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.share.fehbvm.com/Article/details/gqzmvxceb.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.zdbjq.cn/Article/details/gbaswfqku.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.zdbjq.cn/Article/details/grzqwgfkr.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://blog.fehbvm.com/Article/details/glaqtnpqt.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://read.share.zdbjq.cn/Article/details/gwwxoixnf.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://read.share.fehbvm.com/Article/details/giwkngfbi.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.share.fehbvm.com/Article/details/gqtapqayr.sHtML

[I07] 忽略大小写与多行模式
来源：http://blog.hesvh.cn/Article/details/glfzxjrdb.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://read.share.zdbjq.cn/Article/details/gbhbmnsej.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mobile.hesvh.cn/Article/details/gmthivxdn.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mobile.fehbvm.com/Article/details/gelcsectg.sHtML

TS:   /error/gim
来源：http://blog.fehbvm.com/Article/details/gddjwomip.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.blog.hesvh.cn/Article/details/gfpochvgx.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.blog.zdbjq.cn/Article/details/gmctrvnbc.sHtML

Ruby: s.scan(/error/i)
来源：http://m.share.fehbvm.com/Article/details/gqtjdnjay.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://wap.hesvh.cn/Article/details/govutpenr.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://m.share.fehbvm.com/Article/details/gavjczrwn.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://baike.hesvh.cn/Article/details/goqvhmkdd.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://baike.zdbjq.cn/Article/details/gzedkgjte.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.fehbvm.com/Article/details/ghqbdkqxh.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.zdbjq.cn/Article/details/ggllkuezy.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.m.share.hesvh.cn/Article/details/gnhluhsrz.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://baike.hesvh.cn/Article/details/gdpfkouyw.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://3g.hesvh.cn/Article/details/grfdpbtbj.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://read.share.hesvh.cn/Article/details/gdusqauzp.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/grvdsenet.sHtML

J. 日期与时间
来源：http://baike.zdbjq.cn/Article/details/grfosuqjn.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gskaesxjh.sHtML

[J01] 获取当前时间
来源：http://read.share.fehbvm.com/Article/details/gtufphjgm.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://3g.fehbvm.com/Article/details/gxzcbbkrk.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://blog.zdbjq.cn/Article/details/govonjbkr.sHtML

JS:   new Date();  Date.now()
来源：http://read.share.zdbjq.cn/Article/details/gfjpdhyjy.sHtML

TS:   new Date();  Date.now()
来源：http://www.m.share.fehbvm.com/Article/details/gjcwbrctp.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://read.share.zdbjq.cn/Article/details/gwrageinp.sHtML

Go:   time.Now()
来源：http://wap.fehbvm.com/Article/details/gioobbyvc.sHtML

Ruby: Time.now
来源：http://www.share.hesvh.cn/Article/details/gpcycbamq.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.blog.zdbjq.cn/Article/details/glsxvqalm.sHtML

[J02] 格式化输出
来源：http://blog.fehbvm.com/Article/details/gvlwkhiaa.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.fehbvm.com/Article/details/gfsdqtkvf.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wap.fehbvm.com/Article/details/gdraycxjr.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://blog.fehbvm.com/Article/details/gdoohmkpf.sHtML

TS:   d.toISOString()
来源：http://baike.zdbjq.cn/Article/details/gtijkuolf.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://m.share.fehbvm.com/Article/details/gxpqkkgkq.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.share.hesvh.cn/Article/details/ghhqhjpaj.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.fehbvm.com/Article/details/gjmvoqxdc.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://3g.zdbjq.cn/Article/details/gxpkjabzc.sHtML

[J03] 字符串解析为日期
来源：http://blog.fehbvm.com/Article/details/gpojejipr.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://m.share.zdbjq.cn/Article/details/gijtytlbc.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://3g.zdbjq.cn/Article/details/gempdxgim.sHtML

JS:   new Date("2024-01-02")
来源：http://www.m.share.hesvh.cn/Article/details/gitaighoo.sHtML

TS:   new Date("2024-01-02")
来源：http://read.share.zdbjq.cn/Article/details/grosaidge.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.share.hesvh.cn/Article/details/gnclgdhlm.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://m.share.zdbjq.cn/Article/details/gbossuhzx.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.m.share.zdbjq.cn/Article/details/ghbuapatl.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.m.share.fehbvm.com/Article/details/gplplhjto.sHtML

[J04] 时间戳与日期互转
来源：http://www.share.zdbjq.cn/Article/details/gxskppvhe.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://baike.fehbvm.com/Article/details/gookiitqj.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.m.share.hesvh.cn/Article/details/ghsazkxlh.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://wap.zdbjq.cn/Article/details/gneyifcsg.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.share.hesvh.cn/Article/details/gljtnxhll.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://read.share.fehbvm.com/Article/details/gvxqsxmyk.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.share.hesvh.cn/Article/details/gkmhzxato.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://read.share.hesvh.cn/Article/details/gxhykytqj.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://3g.hesvh.cn/Article/details/gxahovskn.sHtML

[J05] 时间加减（加 7 天）
来源：http://baike.hesvh.cn/Article/details/gkwhmhydl.sHtML

Py:   now + timedelta(days=7)
来源：http://3g.fehbvm.com/Article/details/gariozjzy.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://blog.zdbjq.cn/Article/details/gocaeorjh.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.fehbvm.com/Article/details/gxuuzucxs.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.zdbjq.cn/Article/details/gbngbjxqi.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://blog.zdbjq.cn/Article/details/glmuyxmgj.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://m.share.zdbjq.cn/Article/details/glzzaxiqm.sHtML

Ruby: Time.now + 7 * 86400
来源：http://baike.fehbvm.com/Article/details/gayebinlx.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.blog.zdbjq.cn/Article/details/gkobucuiq.sHtML

[J06] 计算两时间之差
来源：http://baike.fehbvm.com/Article/details/gyodxifes.sHtML

Py:   (end - start).total_seconds()
来源：http://m.share.hesvh.cn/Article/details/gpqhbgfmu.sHtML

PHP:  $end->diff($start)->days;
来源：http://m.share.fehbvm.com/Article/details/gyzswztmk.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://m.share.hesvh.cn/Article/details/grjbylpxc.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.share.fehbvm.com/Article/details/gvvlbgyvd.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://m.share.zdbjq.cn/Article/details/gzqcwqcwo.sHtML

Go:   end.Sub(start).Hours()
来源：http://wap.fehbvm.com/Article/details/gjmyhqogb.sHtML

Ruby: end - start                 # 返回秒数
来源：http://m.share.fehbvm.com/Article/details/gybqfnbno.sHtML

C#:   (end - start).TotalSeconds
来源：http://3g.zdbjq.cn/Article/details/gfjhqptyu.sHtML

[J07] 比较两个日期
来源：http://www.share.zdbjq.cn/Article/details/gzyqxrvku.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://mobile.fehbvm.com/Article/details/gmvaeciln.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://baike.hesvh.cn/Article/details/gxqsczakw.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://baike.fehbvm.com/Article/details/gwghtskjl.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.hesvh.cn/Article/details/gkjohkgqu.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://m.share.fehbvm.com/Article/details/ghpsjqdtv.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://mobile.zdbjq.cn/Article/details/gpjtnfcwh.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://wap.hesvh.cn/Article/details/girdncjbx.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://mobile.fehbvm.com/Article/details/gtoqaqlgm.sHtML

[J08] 提取年月日与星期
来源：http://www.share.hesvh.cn/Article/details/geppygseg.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.m.share.fehbvm.com/Article/details/gjjxzjftr.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://m.share.fehbvm.com/Article/details/glpjkzefa.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wap.zdbjq.cn/Article/details/gaqykxuez.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.m.share.zdbjq.cn/Article/details/gygycgiyk.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://read.share.fehbvm.com/Article/details/gfaqogkwx.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wap.fehbvm.com/Article/details/gnbsnxfho.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://read.share.zdbjq.cn/Article/details/guafhttet.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mobile.hesvh.cn/Article/details/gklzyecfs.sHtML

[J09] 时区处理
来源：http://www.share.fehbvm.com/Article/details/ghgweirys.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.m.share.zdbjq.cn/Article/details/gakwrwqtl.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://blog.hesvh.cn/Article/details/gkdwukfre.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.hesvh.cn/Article/details/glqhyevdp.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.zdbjq.cn/Article/details/gjhefbmbh.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.m.share.zdbjq.cn/Article/details/gtrxitoee.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.m.share.fehbvm.com/Article/details/gphmmjhwj.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.share.fehbvm.com/Article/details/gacjrocxi.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.m.share.hesvh.cn/Article/details/gzlphwgru.sHtML

[J10] 取今天 / 本月第一天
来源：http://baike.fehbvm.com/Article/details/gwsnszqgj.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://baike.fehbvm.com/Article/details/gcivnpgax.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://3g.fehbvm.com/Article/details/gzzsmsowd.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://baike.zdbjq.cn/Article/details/gkpoiettj.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.blog.hesvh.cn/Article/details/gwobihbmv.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://read.share.hesvh.cn/Article/details/gdqhoywbq.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://blog.hesvh.cn/Article/details/gezefdqfu.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.share.zdbjq.cn/Article/details/gnghlgyya.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mobile.fehbvm.com/Article/details/gofaxqpts.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gelyyywnh.sHtML

K. JSON 与序列化
来源：http://mobile.fehbvm.com/Article/details/gbkvxazqm.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gyxbdiowj.sHtML

[K01] 对象转 JSON 字符串
来源：http://read.share.fehbvm.com/Article/details/gqyqypxhu.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mobile.fehbvm.com/Article/details/ggkanbilh.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://blog.fehbvm.com/Article/details/gyfdinjzd.sHtML

JS:   JSON.stringify(obj)
来源：http://wap.hesvh.cn/Article/details/gqydywtug.sHtML

TS:   JSON.stringify(obj)
来源：http://mobile.fehbvm.com/Article/details/gmeizhfda.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mobile.zdbjq.cn/Article/details/gstvgojlo.sHtML

Go:   json.Marshal(obj)
来源：http://www.share.fehbvm.com/Article/details/gdjkohaxh.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.blog.zdbjq.cn/Article/details/gwsrpyqfe.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.blog.hesvh.cn/Article/details/gxwagdzem.sHtML

[K02] JSON 字符串转对象
来源：http://read.share.zdbjq.cn/Article/details/gxqbpqnmo.sHtML

Py:   json.loads(s)
来源：http://wap.fehbvm.com/Article/details/gerhjmzls.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.blog.hesvh.cn/Article/details/gqxhyumak.sHtML

JS:   JSON.parse(s)
来源：http://blog.fehbvm.com/Article/details/gzzkgemfo.sHtML

TS:   JSON.parse(s)
来源：http://3g.hesvh.cn/Article/details/gvgosmtrl.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.blog.zdbjq.cn/Article/details/gnqokzbwb.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://mobile.hesvh.cn/Article/details/gzgwkjtvf.sHtML

Ruby: JSON.parse(s)
来源：http://m.share.fehbvm.com/Article/details/gqfhqlwyj.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mobile.fehbvm.com/Article/details/gzopqtpsx.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://3g.fehbvm.com/Article/details/gqamjzvdx.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mobile.zdbjq.cn/Article/details/ghauzfbyq.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mobile.fehbvm.com/Article/details/gfokgxjum.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://baike.hesvh.cn/Article/details/gngmbjqie.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://blog.fehbvm.com/Article/details/giyhcfuee.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.share.fehbvm.com/Article/details/ghrumpesv.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.blog.hesvh.cn/Article/details/gogaqklfz.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://baike.hesvh.cn/Article/details/ghfccyzhs.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.blog.hesvh.cn/Article/details/gpefgadoj.sHtML

[K04] 读取 JSON 文件
来源：http://blog.hesvh.cn/Article/details/gcqdyjcbn.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.m.share.hesvh.cn/Article/details/gelwjszto.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.share.hesvh.cn/Article/details/gmfobudxu.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.zdbjq.cn/Article/details/gjxzehhhw.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.fehbvm.com/Article/details/gzsxkqvnv.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.blog.hesvh.cn/Article/details/gbtufgefw.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://3g.zdbjq.cn/Article/details/gfllgxoxg.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://read.share.fehbvm.com/Article/details/guhvezkxo.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://read.share.hesvh.cn/Article/details/gkpnuyaxd.sHtML

[K05] 深拷贝对象
来源：http://mobile.hesvh.cn/Article/details/gfpxfnqcm.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gmukjqveb.sHtML

PHP:  unserialize(serialize($obj));
来源：http://wap.hesvh.cn/Article/details/ghabbbrue.sHtML

JS:   structuredClone(obj)
来源：http://blog.hesvh.cn/Article/details/gacjyoirh.sHtML

TS:   structuredClone(obj)
来源：http://baike.hesvh.cn/Article/details/gqcmewgge.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://baike.hesvh.cn/Article/details/gflvkdrgc.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://m.share.hesvh.cn/Article/details/gjdtcoydo.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wap.zdbjq.cn/Article/details/gbkfmvgyu.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://read.share.fehbvm.com/Article/details/gfdodadjh.sHtML


<!-- 参考信息 -->