代发 wailian999

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://3g.fehbvm.com/Article/details/gqihivchv.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.share.zdbjq.cn/Article/details/gmzfkshxm.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://3g.hesvh.cn/Article/details/ggirexmop.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.zdbjq.cn/Article/details/gvbwxjzej.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://read.share.hesvh.cn/Article/details/gecowhnbj.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.hesvh.cn/Article/details/grxufsxym.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.zdbjq.cn/Article/details/gcyhenocn.sHtML

[H02] finally / ensure 收尾
来源：http://www.m.share.zdbjq.cn/Article/details/greyprezc.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.zdbjq.cn/Article/details/gvlkmdqhj.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://3g.fehbvm.com/Article/details/gsrmgtwro.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://blog.fehbvm.com/Article/details/gzvbjdhey.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.fehbvm.com/Article/details/gxqzwcaxk.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.share.zdbjq.cn/Article/details/gduxlaqfl.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.blog.zdbjq.cn/Article/details/gfolazxvr.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.m.share.hesvh.cn/Article/details/gkrvitimx.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.share.hesvh.cn/Article/details/gsojgrsyl.sHtML

[H03] 主动抛出异常
来源：http://m.share.zdbjq.cn/Article/details/gituhemxl.sHtML

Py:   raise ValueError("错误信息")
来源：http://read.share.fehbvm.com/Article/details/gzvekrwde.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.hesvh.cn/Article/details/gsshxdlqh.sHtML

JS:   throw new Error("错误信息");
来源：http://www.m.share.hesvh.cn/Article/details/gqdobtkmo.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.zdbjq.cn/Article/details/gbbdzxfpx.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://m.share.fehbvm.com/Article/details/ghdozrmvm.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://m.share.zdbjq.cn/Article/details/gpwcvcqmv.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://wap.fehbvm.com/Article/details/gsfzctzqm.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.hesvh.cn/Article/details/glpylwtzs.sHtML

[H04] 自定义异常类型
来源：http://m.share.fehbvm.com/Article/details/gqxsviqdg.sHtML

Py:   class MyError(Exception): pass
来源：http://wap.zdbjq.cn/Article/details/gefqobwxe.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.m.share.hesvh.cn/Article/details/gushujnty.sHtML

JS:   class MyError extends Error {}
来源：http://wap.zdbjq.cn/Article/details/goloodvtu.sHtML

TS:   class MyError extends Error {}
来源：http://blog.hesvh.cn/Article/details/gproiinlk.sHtML

Java: class MyException extends RuntimeException {}
来源：http://3g.fehbvm.com/Article/details/gshriwntp.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wap.hesvh.cn/Article/details/gzvmjyctx.sHtML

Ruby: class MyError < StandardError; end
来源：http://blog.hesvh.cn/Article/details/gxwzliinq.sHtML

C#:   class MyException : Exception {}
来源：http://3g.fehbvm.com/Article/details/gjjhwitos.sHtML

[H05] 捕获特定类型
来源：http://3g.fehbvm.com/Article/details/gobzyqxhg.sHtML

Py:   except ValueError as e:
来源：http://m.share.fehbvm.com/Article/details/gdaadmjno.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.m.share.fehbvm.com/Article/details/gezrrgibf.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://read.share.fehbvm.com/Article/details/gezegljwu.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.share.hesvh.cn/Article/details/gphxvvnmr.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.m.share.zdbjq.cn/Article/details/ghrgqegel.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://baike.fehbvm.com/Article/details/gzvxmgtvj.sHtML

Ruby: rescue ArgumentError => e
来源：http://read.share.hesvh.cn/Article/details/ggquzkovp.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://read.share.zdbjq.cn/Article/details/ghpzjtodb.sHtML

[H06] 可选值 / 空值安全访问
来源：http://wap.hesvh.cn/Article/details/gkmsgxqqn.sHtML

Py:   value = d.get("k") or default
来源：http://www.share.hesvh.cn/Article/details/gjfclpzpr.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.m.share.zdbjq.cn/Article/details/gvdkjilnm.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://mobile.fehbvm.com/Article/details/gzfocxtnw.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://m.share.zdbjq.cn/Article/details/ggabwfgnc.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://m.share.zdbjq.cn/Article/details/gncqjsyfa.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.share.zdbjq.cn/Article/details/gefputjqf.sHtML

Ruby: d&.dig(:a, :b)
来源：http://wap.hesvh.cn/Article/details/gphmusuce.sHtML

C#:   obj?.A?.B ?? default
来源：http://m.share.zdbjq.cn/Article/details/gzroooxpz.sHtML

[H07] 断言
来源：http://www.blog.zdbjq.cn/Article/details/gwnldvcdl.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.m.share.fehbvm.com/Article/details/ghgkccvpy.sHtML

PHP:  assert($x > 0);
来源：http://www.blog.zdbjq.cn/Article/details/gshungmwg.sHtML

JS:   console.assert(x > 0);
来源：http://wap.hesvh.cn/Article/details/gonnnncwa.sHtML

TS:   console.assert(x > 0);
来源：http://mobile.zdbjq.cn/Article/details/ghobwntup.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.zdbjq.cn/Article/details/gtipoqigh.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.share.fehbvm.com/Article/details/gzznytelg.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://3g.zdbjq.cn/Article/details/gxelrypyo.sHtML

C#:   Debug.Assert(x > 0);
来源：http://read.share.hesvh.cn/Article/details/gurmrbabu.sHtML

[H08] 获取错误信息与堆栈
来源：http://wap.hesvh.cn/Article/details/gyvcoqdgw.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://read.share.zdbjq.cn/Article/details/gpirfdrum.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.share.zdbjq.cn/Article/details/gpvpzbogt.sHtML

JS:   e.message;  e.stack
来源：http://baike.hesvh.cn/Article/details/gbvwfeknr.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.m.share.hesvh.cn/Article/details/gqcmcixkd.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.m.share.zdbjq.cn/Article/details/gzigzizvr.sHtML

Go:   err.Error()
来源：http://read.share.zdbjq.cn/Article/details/glzjqvfau.sHtML

Ruby: e.message;  e.backtrace
来源：http://baike.fehbvm.com/Article/details/ghthwvfiq.sHtML

C#:   e.Message;  e.StackTrace
来源：http://blog.fehbvm.com/Article/details/gnazknoir.sHtML

[H09] 带错误码的异常
来源：http://m.share.fehbvm.com/Article/details/gzdfodnyd.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mobile.zdbjq.cn/Article/details/grmluhmin.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://baike.hesvh.cn/Article/details/gfazhlqoz.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://baike.hesvh.cn/Article/details/gmmwklesw.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wap.zdbjq.cn/Article/details/gktkihgnf.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.blog.zdbjq.cn/Article/details/glxqrxagp.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://baike.zdbjq.cn/Article/details/gvfwttxqc.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://blog.fehbvm.com/Article/details/grstudxiu.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.m.share.hesvh.cn/Article/details/gejegkoqs.sHtML

[H10] 资源自动释放
来源：http://mobile.zdbjq.cn/Article/details/gdnhzyirq.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.blog.zdbjq.cn/Article/details/gtcdjszva.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://m.share.hesvh.cn/Article/details/gxypkkbar.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.hesvh.cn/Article/details/gdhkpnlxw.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.fehbvm.com/Article/details/gsdhgltpc.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.blog.zdbjq.cn/Article/details/gknrjixey.sHtML

Go:   defer f.Close()
来源：http://baike.zdbjq.cn/Article/details/gcdevqsmw.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://3g.hesvh.cn/Article/details/gblaeekxe.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://baike.zdbjq.cn/Article/details/ghdrteeal.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/glkiwqwes.sHtML

I. 正则表达式
来源：http://blog.hesvh.cn/Article/details/gpsafdgtj.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gqbbxildp.sHtML

[I01] 判断是否匹配
来源：http://m.share.zdbjq.cn/Article/details/gtjyggebg.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.share.hesvh.cn/Article/details/gpqunhbiu.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://read.share.fehbvm.com/Article/details/gdwecpwyp.sHtML

JS:   /\d+/.test(s)
来源：http://blog.zdbjq.cn/Article/details/gabsmsfph.sHtML

TS:   /\d+/.test(s)
来源：http://blog.zdbjq.cn/Article/details/gsipznyor.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.m.share.zdbjq.cn/Article/details/gcccefjjs.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://3g.hesvh.cn/Article/details/gxwvghpdw.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.blog.zdbjq.cn/Article/details/giytsejlb.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://3g.hesvh.cn/Article/details/gjrkibwhk.sHtML

[I02] 提取所有匹配
来源：http://blog.hesvh.cn/Article/details/guyibfrle.sHtML

Py:   re.findall(r"\d+", s)
来源：http://baike.fehbvm.com/Article/details/gmrzsnlwi.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.share.hesvh.cn/Article/details/gqyekmzhm.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wap.hesvh.cn/Article/details/gnssbsqzf.sHtML

TS:   s.match(/\d+/g)
来源：http://wap.zdbjq.cn/Article/details/gdaawosip.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://3g.zdbjq.cn/Article/details/goifvusaf.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.m.share.fehbvm.com/Article/details/goknbgcmt.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.share.fehbvm.com/Article/details/gutoxrzyb.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://m.share.hesvh.cn/Article/details/gmxfxhezo.sHtML

[I03] 提取捕获分组
来源：http://mobile.hesvh.cn/Article/details/gfloteriw.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://m.share.hesvh.cn/Article/details/gyskhbnkc.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.blog.zdbjq.cn/Article/details/gpljlwxxc.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://3g.zdbjq.cn/Article/details/gfakqwxho.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://3g.zdbjq.cn/Article/details/gnyedhdge.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://mobile.zdbjq.cn/Article/details/gsqkxrvxu.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.blog.zdbjq.cn/Article/details/gqyibplur.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://read.share.zdbjq.cn/Article/details/gnuvlwybz.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.share.fehbvm.com/Article/details/gdelnhesp.sHtML

[I04] 正则替换
来源：http://www.share.hesvh.cn/Article/details/gystqzegl.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.blog.fehbvm.com/Article/details/gyydrjxgp.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.fehbvm.com/Article/details/gheglzoyn.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.share.zdbjq.cn/Article/details/gakqxwvzv.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.zdbjq.cn/Article/details/gphaxkqkf.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.m.share.fehbvm.com/Article/details/gtjbnzpds.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://mobile.hesvh.cn/Article/details/gusjzalay.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://blog.hesvh.cn/Article/details/gpyhgniae.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://baike.zdbjq.cn/Article/details/glmuizpab.sHtML

[I05] 按正则拆分
来源：http://www.m.share.zdbjq.cn/Article/details/gvfqjxwam.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://3g.zdbjq.cn/Article/details/guswsrqfx.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://3g.fehbvm.com/Article/details/ggppjzmmm.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://baike.hesvh.cn/Article/details/gfryjqpwj.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://mobile.fehbvm.com/Article/details/gpkzxzlzp.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.m.share.fehbvm.com/Article/details/gaegxpdsk.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://blog.hesvh.cn/Article/details/gleaffctm.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://baike.zdbjq.cn/Article/details/gqcqrskdb.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://baike.fehbvm.com/Article/details/gggneurot.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://blog.zdbjq.cn/Article/details/gemlhyhpo.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.m.share.hesvh.cn/Article/details/gwfzkvgrq.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.share.fehbvm.com/Article/details/gnrdiffcw.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.fehbvm.com/Article/details/ghsyeynkm.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.fehbvm.com/Article/details/gsfltqwio.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://3g.fehbvm.com/Article/details/gadiyhekt.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wap.zdbjq.cn/Article/details/ggglnsxoi.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://blog.hesvh.cn/Article/details/gnjvlybaz.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mobile.fehbvm.com/Article/details/gafdydwid.sHtML

[I07] 忽略大小写与多行模式
来源：http://wap.zdbjq.cn/Article/details/gfwscuoqn.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.m.share.zdbjq.cn/Article/details/gtuvaueya.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://m.share.zdbjq.cn/Article/details/ggehotmdm.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://3g.zdbjq.cn/Article/details/gpvmibien.sHtML

TS:   /error/gim
来源：http://3g.zdbjq.cn/Article/details/gbqqjvafs.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mobile.zdbjq.cn/Article/details/gqcteyqhv.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mobile.fehbvm.com/Article/details/gaiecihig.sHtML

Ruby: s.scan(/error/i)
来源：http://m.share.fehbvm.com/Article/details/glodolnal.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.share.fehbvm.com/Article/details/gnhtcbxro.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://3g.fehbvm.com/Article/details/gukwnqghd.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://3g.hesvh.cn/Article/details/gfztnhkmx.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://3g.zdbjq.cn/Article/details/gbgipggzh.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.fehbvm.com/Article/details/gmvxfheki.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.zdbjq.cn/Article/details/gpxxwjnui.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.blog.zdbjq.cn/Article/details/gfvolvlan.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://read.share.fehbvm.com/Article/details/gojftdqrq.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mobile.fehbvm.com/Article/details/gnjcayrff.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wap.hesvh.cn/Article/details/gfwpiyfay.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gigclojes.sHtML

J. 日期与时间
来源：http://www.m.share.fehbvm.com/Article/details/grlhxxqlj.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gkjyjdfir.sHtML

[J01] 获取当前时间
来源：http://www.m.share.fehbvm.com/Article/details/gjeoanepp.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://mobile.fehbvm.com/Article/details/gywsqvaen.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.share.hesvh.cn/Article/details/gdfsxcjfo.sHtML

JS:   new Date();  Date.now()
来源：http://www.share.zdbjq.cn/Article/details/gjjeoimeg.sHtML

TS:   new Date();  Date.now()
来源：http://blog.zdbjq.cn/Article/details/gmurpwzyh.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://baike.hesvh.cn/Article/details/gmecccfwd.sHtML

Go:   time.Now()
来源：http://www.share.fehbvm.com/Article/details/glodagoie.sHtML

Ruby: Time.now
来源：http://m.share.hesvh.cn/Article/details/glbpsojtq.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://m.share.fehbvm.com/Article/details/gkcomwsse.sHtML

[J02] 格式化输出
来源：http://blog.hesvh.cn/Article/details/gqyialbau.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.hesvh.cn/Article/details/gcdxdcmvj.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://3g.hesvh.cn/Article/details/gludhblym.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wap.fehbvm.com/Article/details/ggeigvcsx.sHtML

TS:   d.toISOString()
来源：http://www.share.hesvh.cn/Article/details/glewtgmvr.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://read.share.hesvh.cn/Article/details/gdrdsdkxo.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://read.share.hesvh.cn/Article/details/gmwymmisg.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.fehbvm.com/Article/details/gsqyiynvm.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://3g.fehbvm.com/Article/details/ghahayyyr.sHtML

[J03] 字符串解析为日期
来源：http://m.share.fehbvm.com/Article/details/gwcsqilaq.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://baike.fehbvm.com/Article/details/gyjlfjhyr.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.m.share.fehbvm.com/Article/details/groaerrvf.sHtML

JS:   new Date("2024-01-02")
来源：http://baike.hesvh.cn/Article/details/glphljkzl.sHtML

TS:   new Date("2024-01-02")
来源：http://read.share.hesvh.cn/Article/details/grkejiypd.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.share.zdbjq.cn/Article/details/goygviebf.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://read.share.zdbjq.cn/Article/details/gjabnzyvv.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://wap.zdbjq.cn/Article/details/ggzxdjftb.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mobile.fehbvm.com/Article/details/gvsotydwk.sHtML

[J04] 时间戳与日期互转
来源：http://mobile.fehbvm.com/Article/details/gxohaisgh.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://blog.zdbjq.cn/Article/details/gvdzjwyrs.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://baike.hesvh.cn/Article/details/gkzkkmxeu.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.blog.hesvh.cn/Article/details/gbdywskik.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://read.share.hesvh.cn/Article/details/gcdxqmojh.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://blog.zdbjq.cn/Article/details/gtojvyupe.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://m.share.zdbjq.cn/Article/details/gpwuphduf.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://blog.hesvh.cn/Article/details/guacdenpi.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.m.share.hesvh.cn/Article/details/gyovbqlak.sHtML

[J05] 时间加减（加 7 天）
来源：http://wap.fehbvm.com/Article/details/gxweazecs.sHtML

Py:   now + timedelta(days=7)
来源：http://www.share.hesvh.cn/Article/details/gnvlpnqbw.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://m.share.hesvh.cn/Article/details/goieadade.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.hesvh.cn/Article/details/gxvnitipi.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.hesvh.cn/Article/details/gdnnrgdph.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.share.zdbjq.cn/Article/details/gfpmkduwm.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://read.share.zdbjq.cn/Article/details/gizkustsd.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.share.fehbvm.com/Article/details/glxwygnbp.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://read.share.zdbjq.cn/Article/details/gcjclziio.sHtML

[J06] 计算两时间之差
来源：http://read.share.hesvh.cn/Article/details/gbzlzebzd.sHtML

Py:   (end - start).total_seconds()
来源：http://www.share.fehbvm.com/Article/details/gaukgqgpr.sHtML

PHP:  $end->diff($start)->days;
来源：http://m.share.fehbvm.com/Article/details/gimwsrare.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://read.share.hesvh.cn/Article/details/giallensp.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://read.share.hesvh.cn/Article/details/gvbyixmbt.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://blog.fehbvm.com/Article/details/guvdzfzsc.sHtML

Go:   end.Sub(start).Hours()
来源：http://mobile.hesvh.cn/Article/details/giscemhjf.sHtML

Ruby: end - start                 # 返回秒数
来源：http://m.share.hesvh.cn/Article/details/geltloeci.sHtML

C#:   (end - start).TotalSeconds
来源：http://read.share.zdbjq.cn/Article/details/gpvjnyuds.sHtML

[J07] 比较两个日期
来源：http://3g.fehbvm.com/Article/details/gfhwqypvw.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.share.hesvh.cn/Article/details/gtndchtrp.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://m.share.zdbjq.cn/Article/details/gbfulclsm.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://3g.hesvh.cn/Article/details/gxtzwxgsr.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://baike.hesvh.cn/Article/details/gcueulvph.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://3g.fehbvm.com/Article/details/gddjdwzoc.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://read.share.fehbvm.com/Article/details/gxnjbtptv.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://mobile.zdbjq.cn/Article/details/gxijwdztc.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.share.zdbjq.cn/Article/details/guxpzqswg.sHtML

[J08] 提取年月日与星期
来源：http://www.m.share.fehbvm.com/Article/details/gehjdyktx.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://blog.hesvh.cn/Article/details/gxhkfilmd.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://m.share.hesvh.cn/Article/details/gkfelgkzu.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://baike.zdbjq.cn/Article/details/gdblaedjz.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://read.share.hesvh.cn/Article/details/gvizclgeo.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.blog.zdbjq.cn/Article/details/gdkmjwave.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://m.share.hesvh.cn/Article/details/gnpapjwtc.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://3g.zdbjq.cn/Article/details/gsqjbikqj.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://m.share.hesvh.cn/Article/details/gpnouterh.sHtML

[J09] 时区处理
来源：http://www.blog.zdbjq.cn/Article/details/gkxqoxuvv.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://read.share.zdbjq.cn/Article/details/gdyayqzor.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.m.share.fehbvm.com/Article/details/gcfeyrodn.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.zdbjq.cn/Article/details/grawybrww.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.hesvh.cn/Article/details/grpnnhtpb.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wap.hesvh.cn/Article/details/gsogoebfu.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.m.share.fehbvm.com/Article/details/glsxkeeyp.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://wap.hesvh.cn/Article/details/gozsmvveh.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.share.zdbjq.cn/Article/details/gpuxcxxcv.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.blog.fehbvm.com/Article/details/gxdumzbhx.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://3g.zdbjq.cn/Article/details/gzamucbqb.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://read.share.hesvh.cn/Article/details/ghqrklglr.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://m.share.hesvh.cn/Article/details/gsenoaaxf.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://m.share.hesvh.cn/Article/details/gofthjskg.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.blog.zdbjq.cn/Article/details/geaxuvpxk.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://blog.zdbjq.cn/Article/details/gcbyqhtpp.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mobile.hesvh.cn/Article/details/ggxxmsppm.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.blog.zdbjq.cn/Article/details/ggphsorza.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gdfmhcqka.sHtML

K. JSON 与序列化
来源：http://blog.fehbvm.com/Article/details/glddzalap.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gojbzzrdu.sHtML

[K01] 对象转 JSON 字符串
来源：http://baike.hesvh.cn/Article/details/gwnjxwrkg.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://read.share.fehbvm.com/Article/details/gnusmrxiq.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mobile.hesvh.cn/Article/details/ggjrpiyrg.sHtML

JS:   JSON.stringify(obj)
来源：http://www.share.hesvh.cn/Article/details/gvwpolddl.sHtML

TS:   JSON.stringify(obj)
来源：http://www.blog.fehbvm.com/Article/details/gbgouitan.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://baike.zdbjq.cn/Article/details/gaplxrcsz.sHtML

Go:   json.Marshal(obj)
来源：http://mobile.zdbjq.cn/Article/details/gxeqkkrrd.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://baike.fehbvm.com/Article/details/gmcebmkap.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://read.share.fehbvm.com/Article/details/gvfelexrw.sHtML

[K02] JSON 字符串转对象
来源：http://mobile.fehbvm.com/Article/details/goxmzdedl.sHtML

Py:   json.loads(s)
来源：http://read.share.hesvh.cn/Article/details/gczqsnyjh.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wap.zdbjq.cn/Article/details/gvvvtaldn.sHtML

JS:   JSON.parse(s)
来源：http://www.blog.zdbjq.cn/Article/details/giorezkaf.sHtML

TS:   JSON.parse(s)
来源：http://wap.hesvh.cn/Article/details/gvhxhaida.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://3g.fehbvm.com/Article/details/ginjzyxlm.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://m.share.fehbvm.com/Article/details/gjkiorxue.sHtML

Ruby: JSON.parse(s)
来源：http://wap.fehbvm.com/Article/details/grxabsbum.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://3g.fehbvm.com/Article/details/ggyyibyah.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.blog.hesvh.cn/Article/details/gewczfcim.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://read.share.fehbvm.com/Article/details/gmliaynyf.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://m.share.hesvh.cn/Article/details/gdtphtfei.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.hesvh.cn/Article/details/gmkouoftg.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://3g.fehbvm.com/Article/details/ggokgmywp.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://blog.hesvh.cn/Article/details/gdghavclo.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.share.hesvh.cn/Article/details/geagegdwu.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.share.fehbvm.com/Article/details/gyskkiqba.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mobile.fehbvm.com/Article/details/gzkaxiowc.sHtML

[K04] 读取 JSON 文件
来源：http://read.share.zdbjq.cn/Article/details/gjagcvyna.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wap.hesvh.cn/Article/details/gxdjqvuko.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wap.fehbvm.com/Article/details/ggfqlpdff.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.hesvh.cn/Article/details/gheulvxek.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.fehbvm.com/Article/details/gkywxcwrq.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.share.hesvh.cn/Article/details/gznxupnol.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.blog.fehbvm.com/Article/details/gburfrlso.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://wap.hesvh.cn/Article/details/gqhijqxvu.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://blog.zdbjq.cn/Article/details/girnpggnd.sHtML

[K05] 深拷贝对象
来源：http://m.share.zdbjq.cn/Article/details/gpwabqmvy.sHtML

Py:   copy.deepcopy(obj)
来源：http://3g.fehbvm.com/Article/details/gmckovvgz.sHtML

PHP:  unserialize(serialize($obj));
来源：http://baike.zdbjq.cn/Article/details/gaylschmm.sHtML

JS:   structuredClone(obj)
来源：http://baike.fehbvm.com/Article/details/gatfkgzyq.sHtML

TS:   structuredClone(obj)
来源：http://mobile.hesvh.cn/Article/details/gcozigjdh.sHtML


<!-- 参考信息 -->