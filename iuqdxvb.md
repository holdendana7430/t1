代发 wailian999

[H03] 主动抛出异常
来源：http://www.m.share.fehbvm.com/Article/details/gnbjpwwzr.sHtML

Py:   raise ValueError("错误信息")
来源：http://baike.zdbjq.cn/Article/details/gbatpqsbo.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mobile.hesvh.cn/Article/details/gtkuczuzu.sHtML

JS:   throw new Error("错误信息");
来源：http://www.share.zdbjq.cn/Article/details/gghygtnhu.sHtML

TS:   throw new Error("错误信息");
来源：http://wap.zdbjq.cn/Article/details/gdukmasyf.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.hesvh.cn/Article/details/gxrtmshfv.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wap.zdbjq.cn/Article/details/gsnvfxkrm.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://m.share.zdbjq.cn/Article/details/gmfficmoo.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.blog.fehbvm.com/Article/details/ghvsuiokc.sHtML

[H04] 自定义异常类型
来源：http://www.blog.zdbjq.cn/Article/details/gerdfflmm.sHtML

Py:   class MyError(Exception): pass
来源：http://baike.hesvh.cn/Article/details/gmpltrgnp.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.m.share.zdbjq.cn/Article/details/gmpjdmhvg.sHtML

JS:   class MyError extends Error {}
来源：http://m.share.hesvh.cn/Article/details/goiwfsklx.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.fehbvm.com/Article/details/gumcuhczx.sHtML

Java: class MyException extends RuntimeException {}
来源：http://wap.hesvh.cn/Article/details/gsijqudry.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.zdbjq.cn/Article/details/gxhklqzgi.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.share.hesvh.cn/Article/details/gsuxvtucb.sHtML

C#:   class MyException : Exception {}
来源：http://www.share.zdbjq.cn/Article/details/gnawjueno.sHtML

[H05] 捕获特定类型
来源：http://www.blog.zdbjq.cn/Article/details/gtkozohrj.sHtML

Py:   except ValueError as e:
来源：http://read.share.fehbvm.com/Article/details/gpfadmtpd.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://read.share.hesvh.cn/Article/details/ggagguzzs.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://wap.zdbjq.cn/Article/details/gyjzrzzei.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://blog.fehbvm.com/Article/details/ggqfyuhen.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://wap.hesvh.cn/Article/details/gzsttgmet.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.m.share.hesvh.cn/Article/details/gyjnlhqht.sHtML

Ruby: rescue ArgumentError => e
来源：http://blog.fehbvm.com/Article/details/gybqhpavw.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.blog.fehbvm.com/Article/details/gwcfmxjxa.sHtML

[H06] 可选值 / 空值安全访问
来源：http://blog.hesvh.cn/Article/details/gsnzrjvgq.sHtML

Py:   value = d.get("k") or default
来源：http://baike.fehbvm.com/Article/details/ghyegsfzi.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://3g.hesvh.cn/Article/details/gjnmpynef.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.share.zdbjq.cn/Article/details/gakuwjeec.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://3g.hesvh.cn/Article/details/ggpnukyli.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.share.zdbjq.cn/Article/details/gyssqnohw.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://baike.zdbjq.cn/Article/details/geafbsmlw.sHtML

Ruby: d&.dig(:a, :b)
来源：http://wap.fehbvm.com/Article/details/gjpigeobk.sHtML

C#:   obj?.A?.B ?? default
来源：http://3g.hesvh.cn/Article/details/gjedzwely.sHtML

[H07] 断言
来源：http://blog.fehbvm.com/Article/details/gygnciouz.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.share.hesvh.cn/Article/details/ggebbpeqp.sHtML

PHP:  assert($x > 0);
来源：http://read.share.hesvh.cn/Article/details/gtyxgzhje.sHtML

JS:   console.assert(x > 0);
来源：http://wap.hesvh.cn/Article/details/gqzoiaafc.sHtML

TS:   console.assert(x > 0);
来源：http://wap.zdbjq.cn/Article/details/gpzbqnlbf.sHtML

Java: assert x > 0 : "必须为正";
来源：http://wap.zdbjq.cn/Article/details/gbelwdczd.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://read.share.hesvh.cn/Article/details/gauqfqrgc.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://m.share.fehbvm.com/Article/details/gfakqlvml.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.blog.zdbjq.cn/Article/details/geykaizzn.sHtML

[H08] 获取错误信息与堆栈
来源：http://read.share.hesvh.cn/Article/details/gszjcjpfz.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://blog.hesvh.cn/Article/details/ggodnqkda.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mobile.hesvh.cn/Article/details/gazcpxomz.sHtML

JS:   e.message;  e.stack
来源：http://read.share.fehbvm.com/Article/details/gjpomhkwr.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://mobile.zdbjq.cn/Article/details/gfjijptjh.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://3g.zdbjq.cn/Article/details/gwxktcrzw.sHtML

Go:   err.Error()
来源：http://baike.fehbvm.com/Article/details/gbvbxglmu.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.blog.hesvh.cn/Article/details/gmvfuxssl.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.share.hesvh.cn/Article/details/gcwxhzygb.sHtML

[H09] 带错误码的异常
来源：http://read.share.zdbjq.cn/Article/details/gjnbwmzcu.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.m.share.fehbvm.com/Article/details/gwkqeyxla.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.blog.hesvh.cn/Article/details/gnkpvgwnj.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://baike.fehbvm.com/Article/details/gyeytyiac.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://read.share.fehbvm.com/Article/details/ghckxsimw.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://read.share.zdbjq.cn/Article/details/gxixjybjl.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wap.zdbjq.cn/Article/details/grcaxnzbk.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://wap.hesvh.cn/Article/details/gdprkthcd.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://read.share.hesvh.cn/Article/details/gmmemkpbb.sHtML

[H10] 资源自动释放
来源：http://www.share.hesvh.cn/Article/details/gvnufbrvh.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://m.share.hesvh.cn/Article/details/gmdwzblkw.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.m.share.hesvh.cn/Article/details/gdsxggaen.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.fehbvm.com/Article/details/gebzedqrb.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.zdbjq.cn/Article/details/gpsrfysab.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mobile.fehbvm.com/Article/details/gxhxlxpwc.sHtML

Go:   defer f.Close()
来源：http://www.m.share.fehbvm.com/Article/details/gdjaxsmjr.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.blog.fehbvm.com/Article/details/geptvbxrg.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://3g.fehbvm.com/Article/details/gjwljfaus.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gsxlpkdab.sHtML

I. 正则表达式
来源：http://m.share.hesvh.cn/Article/details/gvxdabdrh.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gozeifqsj.sHtML

[I01] 判断是否匹配
来源：http://wap.fehbvm.com/Article/details/gezmcbqac.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wap.hesvh.cn/Article/details/gkltbvsuo.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://m.share.zdbjq.cn/Article/details/glxbcmeah.sHtML

JS:   /\d+/.test(s)
来源：http://www.share.zdbjq.cn/Article/details/gitmxxouj.sHtML

TS:   /\d+/.test(s)
来源：http://wap.hesvh.cn/Article/details/gzujjjjgn.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.share.hesvh.cn/Article/details/gyjjtzihs.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wap.hesvh.cn/Article/details/gkdfiitbl.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.m.share.hesvh.cn/Article/details/gxfcpbwjq.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wap.fehbvm.com/Article/details/gffwaivku.sHtML

[I02] 提取所有匹配
来源：http://read.share.zdbjq.cn/Article/details/gdcnzjrbk.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.blog.fehbvm.com/Article/details/gzbhiodyy.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.share.hesvh.cn/Article/details/grxdzlbzg.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wap.hesvh.cn/Article/details/gvhqugjgs.sHtML

TS:   s.match(/\d+/g)
来源：http://m.share.hesvh.cn/Article/details/gellnvkts.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.blog.fehbvm.com/Article/details/gmfkefwpe.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://blog.zdbjq.cn/Article/details/gtqfgovkf.sHtML

Ruby: s.scan(/\d+/)
来源：http://baike.hesvh.cn/Article/details/gwlvlcrax.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://read.share.hesvh.cn/Article/details/gnwqpujgx.sHtML

[I03] 提取捕获分组
来源：http://wap.fehbvm.com/Article/details/gadyhvlcq.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.share.hesvh.cn/Article/details/gpvlyawbg.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://blog.zdbjq.cn/Article/details/gcuuefhwx.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mobile.zdbjq.cn/Article/details/gettvdqsj.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://m.share.hesvh.cn/Article/details/gblubybar.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.blog.zdbjq.cn/Article/details/gmgziolor.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://m.share.fehbvm.com/Article/details/gxwlocgxn.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://baike.fehbvm.com/Article/details/gsguiwqhf.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://mobile.hesvh.cn/Article/details/gkqsdxhqp.sHtML

[I04] 正则替换
来源：http://3g.fehbvm.com/Article/details/gyqctmkmd.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://3g.zdbjq.cn/Article/details/gadummyau.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://3g.fehbvm.com/Article/details/gbtpcszlz.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://blog.hesvh.cn/Article/details/gnlcmdtkx.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://read.share.fehbvm.com/Article/details/gxipgehah.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://mobile.zdbjq.cn/Article/details/ghdapzflw.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.share.hesvh.cn/Article/details/ggadbabrz.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.blog.fehbvm.com/Article/details/gkdfrlzvn.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mobile.fehbvm.com/Article/details/gbbzehnjv.sHtML

[I05] 按正则拆分
来源：http://www.blog.zdbjq.cn/Article/details/gkjztpwtn.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://m.share.fehbvm.com/Article/details/gamvbhshw.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://blog.zdbjq.cn/Article/details/gdqubbmae.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.m.share.hesvh.cn/Article/details/grldqjsvi.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://read.share.zdbjq.cn/Article/details/gxciaokjg.sHtML

Java: s.split("\\s*,\\s*")
来源：http://baike.fehbvm.com/Article/details/gimdjfzxw.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.m.share.hesvh.cn/Article/details/gjmoxmwtq.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.m.share.fehbvm.com/Article/details/gamdhsfop.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.m.share.fehbvm.com/Article/details/ghaahdikz.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://m.share.zdbjq.cn/Article/details/gwerzifwx.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://3g.zdbjq.cn/Article/details/glexzazqw.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://mobile.hesvh.cn/Article/details/gsnjkkdbf.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.fehbvm.com/Article/details/gzmhynmah.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.fehbvm.com/Article/details/gmkvkwptc.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.m.share.fehbvm.com/Article/details/gueeryamk.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.m.share.hesvh.cn/Article/details/gacpurqde.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://baike.hesvh.cn/Article/details/gojppctjy.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://3g.hesvh.cn/Article/details/ghrlxgles.sHtML

[I07] 忽略大小写与多行模式
来源：http://baike.fehbvm.com/Article/details/gxzrwhacz.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.m.share.hesvh.cn/Article/details/ggcsgtsot.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://3g.zdbjq.cn/Article/details/gztvmqxkx.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.blog.hesvh.cn/Article/details/gjbsmzsby.sHtML

TS:   /error/gim
来源：http://www.share.fehbvm.com/Article/details/gbbhjlicc.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.m.share.zdbjq.cn/Article/details/gfmcueefz.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.blog.fehbvm.com/Article/details/gdhxyqber.sHtML

Ruby: s.scan(/error/i)
来源：http://wap.fehbvm.com/Article/details/ggnfoevzu.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://wap.fehbvm.com/Article/details/gjqbsyfrw.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://mobile.hesvh.cn/Article/details/ggbnxopev.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://blog.zdbjq.cn/Article/details/grfdrszgx.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://baike.fehbvm.com/Article/details/gveylapmy.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.hesvh.cn/Article/details/gkgsykcsm.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.fehbvm.com/Article/details/gktgejhrf.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://mobile.zdbjq.cn/Article/details/ggfmpzkhx.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://baike.hesvh.cn/Article/details/glpwejixd.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://read.share.fehbvm.com/Article/details/gctwspiad.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.share.zdbjq.cn/Article/details/gvnsajfth.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gzmpphjpi.sHtML

J. 日期与时间
来源：http://blog.zdbjq.cn/Article/details/gmfqfnzfs.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gxpqpgsjc.sHtML

[J01] 获取当前时间
来源：http://mobile.fehbvm.com/Article/details/geybmhkix.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://3g.hesvh.cn/Article/details/glrtnapdm.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://read.share.zdbjq.cn/Article/details/gqqufhrom.sHtML

JS:   new Date();  Date.now()
来源：http://blog.zdbjq.cn/Article/details/gxilnyzce.sHtML

TS:   new Date();  Date.now()
来源：http://mobile.zdbjq.cn/Article/details/gooznjoye.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.blog.fehbvm.com/Article/details/gavzmzore.sHtML

Go:   time.Now()
来源：http://www.m.share.zdbjq.cn/Article/details/gymhceejy.sHtML

Ruby: Time.now
来源：http://www.blog.fehbvm.com/Article/details/gxumehoto.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://m.share.hesvh.cn/Article/details/gginomqoi.sHtML

[J02] 格式化输出
来源：http://read.share.zdbjq.cn/Article/details/gznnggeqd.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.hesvh.cn/Article/details/gfqfrgixl.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mobile.hesvh.cn/Article/details/gvpefcggg.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.m.share.hesvh.cn/Article/details/gfrflhoyv.sHtML

TS:   d.toISOString()
来源：http://3g.zdbjq.cn/Article/details/guvfpcsdz.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://baike.fehbvm.com/Article/details/gstxtcrxe.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://m.share.fehbvm.com/Article/details/gdekogint.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.zdbjq.cn/Article/details/ggbvijyfj.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.m.share.hesvh.cn/Article/details/gxlidowkr.sHtML

[J03] 字符串解析为日期
来源：http://www.share.fehbvm.com/Article/details/gsbqojpen.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://baike.hesvh.cn/Article/details/gqkqdaxpx.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wap.hesvh.cn/Article/details/ggtzbmebs.sHtML

JS:   new Date("2024-01-02")
来源：http://www.blog.zdbjq.cn/Article/details/gcyayocmx.sHtML

TS:   new Date("2024-01-02")
来源：http://wap.fehbvm.com/Article/details/gnhzyrmtj.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.blog.fehbvm.com/Article/details/geyvasdng.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://baike.zdbjq.cn/Article/details/gqsnyczam.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://m.share.zdbjq.cn/Article/details/gcnrzbqhb.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.m.share.hesvh.cn/Article/details/gqnmmqghz.sHtML

[J04] 时间戳与日期互转
来源：http://www.share.zdbjq.cn/Article/details/gurrbxive.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.blog.fehbvm.com/Article/details/gxtrepevh.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://mobile.fehbvm.com/Article/details/ggzlbgicj.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mobile.zdbjq.cn/Article/details/gfdiebihd.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://blog.hesvh.cn/Article/details/gygfwxrkq.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://mobile.hesvh.cn/Article/details/gzbbaqudx.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://mobile.hesvh.cn/Article/details/gyrcpboax.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wap.hesvh.cn/Article/details/grjfdyuoa.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://baike.fehbvm.com/Article/details/gekakutai.sHtML

[J05] 时间加减（加 7 天）
来源：http://blog.hesvh.cn/Article/details/gpqctxknw.sHtML

Py:   now + timedelta(days=7)
来源：http://baike.hesvh.cn/Article/details/gralvpanz.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://mobile.hesvh.cn/Article/details/gbeusiegy.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.zdbjq.cn/Article/details/gwdniodfo.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.fehbvm.com/Article/details/ghpvpdier.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://read.share.hesvh.cn/Article/details/gssuunisl.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://3g.zdbjq.cn/Article/details/gzxrltgzk.sHtML

Ruby: Time.now + 7 * 86400
来源：http://wap.zdbjq.cn/Article/details/gamooopst.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://3g.hesvh.cn/Article/details/gvqinovhr.sHtML

[J06] 计算两时间之差
来源：http://www.blog.hesvh.cn/Article/details/gfielmlnk.sHtML

Py:   (end - start).total_seconds()
来源：http://www.m.share.hesvh.cn/Article/details/ghduqsoca.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.blog.hesvh.cn/Article/details/gazbwqcul.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.blog.zdbjq.cn/Article/details/gambrykaj.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wap.hesvh.cn/Article/details/ggfiwopzi.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.blog.hesvh.cn/Article/details/gzocykmhv.sHtML

Go:   end.Sub(start).Hours()
来源：http://baike.hesvh.cn/Article/details/gcocpdekh.sHtML

Ruby: end - start                 # 返回秒数
来源：http://mobile.hesvh.cn/Article/details/goruxathd.sHtML

C#:   (end - start).TotalSeconds
来源：http://3g.fehbvm.com/Article/details/ghsfpfsen.sHtML

[J07] 比较两个日期
来源：http://read.share.fehbvm.com/Article/details/gzuuhjqoj.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://3g.hesvh.cn/Article/details/glqdqvwok.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.share.hesvh.cn/Article/details/gzatmjpjn.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://blog.fehbvm.com/Article/details/gkwohdacu.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://blog.fehbvm.com/Article/details/gdxxnoddj.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://baike.hesvh.cn/Article/details/gwdgheoou.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://mobile.fehbvm.com/Article/details/gicewtgdz.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://baike.hesvh.cn/Article/details/gasgidgjz.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://baike.fehbvm.com/Article/details/gcjzflwnm.sHtML

[J08] 提取年月日与星期
来源：http://baike.zdbjq.cn/Article/details/gbfvymtkl.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mobile.hesvh.cn/Article/details/gidgjmbhr.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wap.hesvh.cn/Article/details/gukzrhdje.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.share.fehbvm.com/Article/details/gcwgtnqpp.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://wap.hesvh.cn/Article/details/ggdbyxbbs.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.blog.zdbjq.cn/Article/details/gmihwjyhm.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://m.share.zdbjq.cn/Article/details/gmukcklpi.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wap.hesvh.cn/Article/details/grrwpsigv.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.share.hesvh.cn/Article/details/gjgvsxfyd.sHtML

[J09] 时区处理
来源：http://baike.fehbvm.com/Article/details/gcsajghtv.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.share.hesvh.cn/Article/details/gwhdpdisu.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wap.zdbjq.cn/Article/details/gtobmvrht.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.zdbjq.cn/Article/details/gdhzlefvy.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.zdbjq.cn/Article/details/gomvgbtgg.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mobile.fehbvm.com/Article/details/gebnkjduk.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.share.zdbjq.cn/Article/details/gbrbsyhcp.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.share.zdbjq.cn/Article/details/gwnogvtyy.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://blog.hesvh.cn/Article/details/gkcbitubr.sHtML

[J10] 取今天 / 本月第一天
来源：http://read.share.hesvh.cn/Article/details/gtswmbbrk.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://mobile.zdbjq.cn/Article/details/gaodapyjh.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wap.hesvh.cn/Article/details/galzuyxau.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://3g.zdbjq.cn/Article/details/gzybaqoqf.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wap.hesvh.cn/Article/details/gypwgrjvx.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://blog.zdbjq.cn/Article/details/gndawbkbf.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://read.share.zdbjq.cn/Article/details/ghdzdurtd.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://blog.zdbjq.cn/Article/details/gdoqoahuw.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://read.share.hesvh.cn/Article/details/gzwfghaxj.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gddkiocme.sHtML

K. JSON 与序列化
来源：http://www.blog.fehbvm.com/Article/details/germjkvkx.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/geodftjrb.sHtML

[K01] 对象转 JSON 字符串
来源：http://baike.fehbvm.com/Article/details/gdoynhsov.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://baike.hesvh.cn/Article/details/gwrmjhkmz.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://blog.hesvh.cn/Article/details/gvtdhnrbb.sHtML

JS:   JSON.stringify(obj)
来源：http://baike.hesvh.cn/Article/details/gkmesckxv.sHtML

TS:   JSON.stringify(obj)
来源：http://www.share.hesvh.cn/Article/details/ghoaeufcg.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.blog.hesvh.cn/Article/details/gyhyvvjsn.sHtML

Go:   json.Marshal(obj)
来源：http://read.share.zdbjq.cn/Article/details/gardlvxmc.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.m.share.zdbjq.cn/Article/details/gzqmvsqxb.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://blog.hesvh.cn/Article/details/gdpglhdqg.sHtML

[K02] JSON 字符串转对象
来源：http://mobile.fehbvm.com/Article/details/gxeudilvm.sHtML

Py:   json.loads(s)
来源：http://read.share.zdbjq.cn/Article/details/gxxlycpss.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.blog.fehbvm.com/Article/details/gmbmpqlsq.sHtML

JS:   JSON.parse(s)
来源：http://blog.hesvh.cn/Article/details/gcnfehtyh.sHtML

TS:   JSON.parse(s)
来源：http://m.share.zdbjq.cn/Article/details/gxnsbbfrk.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://blog.zdbjq.cn/Article/details/gcyzjtqjm.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://read.share.fehbvm.com/Article/details/goricjmit.sHtML

Ruby: JSON.parse(s)
来源：http://baike.zdbjq.cn/Article/details/gqfkajqrn.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.m.share.hesvh.cn/Article/details/gbidetsax.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.m.share.hesvh.cn/Article/details/gdqgowahq.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.blog.zdbjq.cn/Article/details/gwjmewtvx.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.hesvh.cn/Article/details/gpqjmwjvm.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.hesvh.cn/Article/details/gergquygf.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://3g.fehbvm.com/Article/details/gecvqqxxp.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://blog.fehbvm.com/Article/details/gepzwnids.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.blog.hesvh.cn/Article/details/gmpruhtbf.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.m.share.fehbvm.com/Article/details/ggrwelyrz.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wap.fehbvm.com/Article/details/gpoarmdzd.sHtML

[K04] 读取 JSON 文件
来源：http://3g.hesvh.cn/Article/details/gtxkwblox.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.blog.zdbjq.cn/Article/details/gkyuibujd.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.share.zdbjq.cn/Article/details/glcqztflv.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.zdbjq.cn/Article/details/ghziccbdq.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.hesvh.cn/Article/details/guukvmmzr.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://baike.hesvh.cn/Article/details/gtbnrdxmx.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://baike.zdbjq.cn/Article/details/gkcndlcix.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://wap.hesvh.cn/Article/details/gitmoatfc.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.share.hesvh.cn/Article/details/glfahliyd.sHtML

[K05] 深拷贝对象
来源：http://www.m.share.fehbvm.com/Article/details/gsokdlpcg.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.blog.fehbvm.com/Article/details/gydtokajn.sHtML

PHP:  unserialize(serialize($obj));
来源：http://mobile.fehbvm.com/Article/details/gbknwyupv.sHtML

JS:   structuredClone(obj)
来源：http://www.share.zdbjq.cn/Article/details/giivdchhx.sHtML

TS:   structuredClone(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gncychivx.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://3g.zdbjq.cn/Article/details/gzjrlqvdh.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://baike.zdbjq.cn/Article/details/gkifaybmy.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://m.share.fehbvm.com/Article/details/gfkaazimo.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://wap.fehbvm.com/Article/details/gbqjjjtcj.sHtML

[K06] 解析 URL 查询串
来源：http://3g.zdbjq.cn/Article/details/gydkivmld.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mobile.fehbvm.com/Article/details/gaqqqwuey.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://read.share.hesvh.cn/Article/details/gplwkobon.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.zdbjq.cn/Article/details/gebtcijwm.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.fehbvm.com/Article/details/guicjwlik.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mobile.zdbjq.cn/Article/details/glfaopguh.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://mobile.fehbvm.com/Article/details/ggbdpzyca.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://baike.fehbvm.com/Article/details/ggvdupvwv.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wap.hesvh.cn/Article/details/ggyylevsg.sHtML

[K07] 进制转换
来源：http://read.share.zdbjq.cn/Article/details/gjfalppvz.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.blog.fehbvm.com/Article/details/gllrdlnpz.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mobile.fehbvm.com/Article/details/gebbffyjy.sHtML


<!-- 参考信息 -->