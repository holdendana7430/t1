代发 wailian999

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.blog.fanxiaobao.xyz/Article/details/gixkrfitr.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxprrrlkl.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvurgveik.sHtML

[H02] finally / ensure 收尾
来源：http://wap.fanxiaobao.xyz/Article/details/gjsnktawb.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghsdzjvnm.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.fanxiaobao.xyz/Article/details/gwkahabuf.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gqvjqhkkg.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaupisces.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.fanxiaobao.xyz/Article/details/gtrubuhfk.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.share.fanxiaobao.xyz/Article/details/gdxzbiyej.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://3g.fanxiaobao.xyz/Article/details/gttteytbc.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gyaylxcla.sHtML

[H03] 主动抛出异常
来源：http://wap.fanxiaobao.xyz/Article/details/gxdiwckgz.sHtML

Py:   raise ValueError("错误信息")
来源：http://blog.fanxiaobao.xyz/Article/details/gguuloeih.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghgzmmlpk.sHtML

JS:   throw new Error("错误信息");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbxdulhjg.sHtML

TS:   throw new Error("错误信息");
来源：http://www.share.fanxiaobao.xyz/Article/details/gotldetqw.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.fanxiaobao.xyz/Article/details/gsxhzkybt.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://m.share.fanxiaobao.xyz/Article/details/guxkhzjbo.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://wap.fanxiaobao.xyz/Article/details/gsujnarnf.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://baike.fanxiaobao.xyz/Article/details/gsrvhleat.sHtML

[H04] 自定义异常类型
来源：http://www.share.fanxiaobao.xyz/Article/details/gpoduppdi.sHtML

Py:   class MyError(Exception): pass
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvlsjtcce.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gkdgdgcjz.sHtML

JS:   class MyError extends Error {}
来源：http://baike.fanxiaobao.xyz/Article/details/gmeudaryo.sHtML

TS:   class MyError extends Error {}
来源：http://wap.fanxiaobao.xyz/Article/details/ggurnoydz.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gixeufnwl.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://3g.fanxiaobao.xyz/Article/details/gdcioludh.sHtML

Ruby: class MyError < StandardError; end
来源：http://mobile.fanxiaobao.xyz/Article/details/gvbfwlkae.sHtML

C#:   class MyException : Exception {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnolhuzdz.sHtML

[H05] 捕获特定类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/gersqrfav.sHtML

Py:   except ValueError as e:
来源：http://wap.fanxiaobao.xyz/Article/details/gmuwgixfq.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.share.fanxiaobao.xyz/Article/details/gxrbkvfic.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwmbzhwon.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://baike.fanxiaobao.xyz/Article/details/geohkzyur.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdrvcdjxh.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://m.share.fanxiaobao.xyz/Article/details/gwumuczxk.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxjsxxqfz.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gyusxpwri.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyfruyltx.sHtML

Py:   value = d.get("k") or default
来源：http://3g.fanxiaobao.xyz/Article/details/gogcawphj.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://mobile.fanxiaobao.xyz/Article/details/ghzosyuwl.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.fanxiaobao.xyz/Article/details/giwyobgff.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzzykffbq.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wap.fanxiaobao.xyz/Article/details/gaqmutyuv.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmtrunioc.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdbnweruw.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcbsepoxb.sHtML

[H07] 断言
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gltiedwes.sHtML

Py:   assert x > 0, "必须为正"
来源：http://read.share.fanxiaobao.xyz/Article/details/gqwfjxuov.sHtML

PHP:  assert($x > 0);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glhaneccp.sHtML

JS:   console.assert(x > 0);
来源：http://www.share.fanxiaobao.xyz/Article/details/gqzhtyefv.sHtML

TS:   console.assert(x > 0);
来源：http://blog.fanxiaobao.xyz/Article/details/gvyqnepou.sHtML

Java: assert x > 0 : "必须为正";
来源：http://3g.fanxiaobao.xyz/Article/details/guqjnxson.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://read.share.fanxiaobao.xyz/Article/details/gmiptpzdk.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://blog.fanxiaobao.xyz/Article/details/gyfotcxtp.sHtML

C#:   Debug.Assert(x > 0);
来源：http://wap.fanxiaobao.xyz/Article/details/glhsvqyve.sHtML

[H08] 获取错误信息与堆栈
来源：http://m.share.fanxiaobao.xyz/Article/details/gctwghapi.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://m.share.fanxiaobao.xyz/Article/details/glqjjyjab.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtnhvmahr.sHtML

JS:   e.message;  e.stack
来源：http://wap.fanxiaobao.xyz/Article/details/gqxhjrlah.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://m.share.fanxiaobao.xyz/Article/details/gvvhrzlcb.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://wap.fanxiaobao.xyz/Article/details/gkfafbxjp.sHtML

Go:   err.Error()
来源：http://m.share.fanxiaobao.xyz/Article/details/gvxkfoquc.sHtML

Ruby: e.message;  e.backtrace
来源：http://baike.fanxiaobao.xyz/Article/details/goktdulkx.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.blog.fanxiaobao.xyz/Article/details/gapkwmnyt.sHtML

[H09] 带错误码的异常
来源：http://read.share.fanxiaobao.xyz/Article/details/gdfijaimi.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://m.share.fanxiaobao.xyz/Article/details/gbhmwsbkm.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://wap.fanxiaobao.xyz/Article/details/gaqxwmveo.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://3g.fanxiaobao.xyz/Article/details/gejerlsgj.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.share.fanxiaobao.xyz/Article/details/glyaevbas.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://blog.fanxiaobao.xyz/Article/details/grtxjsjgr.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mobile.fanxiaobao.xyz/Article/details/gyroflspn.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://m.share.fanxiaobao.xyz/Article/details/gznfqnwlj.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://read.share.fanxiaobao.xyz/Article/details/gkaazvhtm.sHtML

[H10] 资源自动释放
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsucovmxt.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://mobile.fanxiaobao.xyz/Article/details/gzoprbigr.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://m.share.fanxiaobao.xyz/Article/details/gqzswsgyq.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.fanxiaobao.xyz/Article/details/gstvabsdp.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.fanxiaobao.xyz/Article/details/gosvyupgm.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://read.share.fanxiaobao.xyz/Article/details/gmebzffcm.sHtML

Go:   defer f.Close()
来源：http://www.share.fanxiaobao.xyz/Article/details/ggdutucqp.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://baike.fanxiaobao.xyz/Article/details/gfpfstosd.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghrhlrlzf.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwrjezubp.sHtML

I. 正则表达式
来源：http://read.share.fanxiaobao.xyz/Article/details/geevhuzkl.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gnosfebvq.sHtML

[I01] 判断是否匹配
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfdaozkib.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://3g.fanxiaobao.xyz/Article/details/gsllaejpu.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://read.share.fanxiaobao.xyz/Article/details/giiqpyqjr.sHtML

JS:   /\d+/.test(s)
来源：http://baike.fanxiaobao.xyz/Article/details/gotbircpy.sHtML

TS:   /\d+/.test(s)
来源：http://3g.fanxiaobao.xyz/Article/details/gjoclsxme.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://blog.fanxiaobao.xyz/Article/details/gtqfsivjr.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://blog.fanxiaobao.xyz/Article/details/gjzcbpfxo.sHtML

Ruby: s.match?(/\d+/)
来源：http://wap.fanxiaobao.xyz/Article/details/gyegvxaks.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gknwiyozt.sHtML

[I02] 提取所有匹配
来源：http://baike.fanxiaobao.xyz/Article/details/gjevznxmo.sHtML

Py:   re.findall(r"\d+", s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gyizpdapn.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://baike.fanxiaobao.xyz/Article/details/gjxznzdsb.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://blog.fanxiaobao.xyz/Article/details/gxzjuolqx.sHtML

TS:   s.match(/\d+/g)
来源：http://read.share.fanxiaobao.xyz/Article/details/gdfqbffyj.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.share.fanxiaobao.xyz/Article/details/gwsnhzlls.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://blog.fanxiaobao.xyz/Article/details/gllgcugdv.sHtML

Ruby: s.scan(/\d+/)
来源：http://blog.fanxiaobao.xyz/Article/details/gfuldzvbt.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmudrvjmf.sHtML

[I03] 提取捕获分组
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggwefuedx.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://blog.fanxiaobao.xyz/Article/details/ggaixueto.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://blog.fanxiaobao.xyz/Article/details/gwnwhjbbo.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.share.fanxiaobao.xyz/Article/details/giuosthub.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzniawovs.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.share.fanxiaobao.xyz/Article/details/gdqkrnzuc.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://3g.fanxiaobao.xyz/Article/details/glomjgwdx.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://baike.fanxiaobao.xyz/Article/details/gcnqvdlup.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://3g.fanxiaobao.xyz/Article/details/gbrnqddtf.sHtML

[I04] 正则替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtxyxzehu.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gwqoldikm.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://read.share.fanxiaobao.xyz/Article/details/gsusiqted.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://baike.fanxiaobao.xyz/Article/details/gdoogcfnu.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnzpqvkkm.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://mobile.fanxiaobao.xyz/Article/details/gyafefhtd.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnsdieheq.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghhjkxafv.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gutudwbmj.sHtML

[I05] 按正则拆分
来源：http://m.share.fanxiaobao.xyz/Article/details/gismovquv.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gmvckauzk.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://read.share.fanxiaobao.xyz/Article/details/gahpjoveu.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmuvupjrq.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.blog.fanxiaobao.xyz/Article/details/grapdqgqz.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnhncxikb.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://3g.fanxiaobao.xyz/Article/details/gimdkylsw.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://3g.fanxiaobao.xyz/Article/details/gnptmcwuo.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mobile.fanxiaobao.xyz/Article/details/gvxfslqfg.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.share.fanxiaobao.xyz/Article/details/gobqoexsm.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.share.fanxiaobao.xyz/Article/details/gzacdoyta.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://mobile.fanxiaobao.xyz/Article/details/gosdamhxf.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.fanxiaobao.xyz/Article/details/gsoprqneg.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.fanxiaobao.xyz/Article/details/gcwckohak.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://read.share.fanxiaobao.xyz/Article/details/ggryeeauu.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://blog.fanxiaobao.xyz/Article/details/gergxawuc.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://baike.fanxiaobao.xyz/Article/details/gtaxngrxx.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://blog.fanxiaobao.xyz/Article/details/guwomxcmd.sHtML

[I07] 忽略大小写与多行模式
来源：http://wap.fanxiaobao.xyz/Article/details/gbgeklbvy.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://blog.fanxiaobao.xyz/Article/details/ggqgtvijs.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wap.fanxiaobao.xyz/Article/details/gvkjwolan.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxsbomwep.sHtML

TS:   /error/gim
来源：http://blog.fanxiaobao.xyz/Article/details/gwzoeewmo.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://baike.fanxiaobao.xyz/Article/details/ggytrwqty.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.share.fanxiaobao.xyz/Article/details/gcxjoheol.sHtML

Ruby: s.scan(/error/i)
来源：http://blog.fanxiaobao.xyz/Article/details/gbeuyatsa.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://read.share.fanxiaobao.xyz/Article/details/guvisgwlt.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.share.fanxiaobao.xyz/Article/details/ggxjsqwfz.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.share.fanxiaobao.xyz/Article/details/gzhuttkce.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.share.fanxiaobao.xyz/Article/details/gkwtjmjle.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxziqyiij.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gixxfxffe.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://m.share.fanxiaobao.xyz/Article/details/gpnnvtvop.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.blog.fanxiaobao.xyz/Article/details/gldcbufob.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://baike.fanxiaobao.xyz/Article/details/gfgmvzgjx.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gluujqzjl.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gwfjveiqm.sHtML

J. 日期与时间
来源：http://m.share.fanxiaobao.xyz/Article/details/ghfvgueyn.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gdedpehvz.sHtML

[J01] 获取当前时间
来源：http://3g.fanxiaobao.xyz/Article/details/gaawwywkr.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://read.share.fanxiaobao.xyz/Article/details/gtirnbnga.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mobile.fanxiaobao.xyz/Article/details/gxzzkjypc.sHtML

JS:   new Date();  Date.now()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbvkasywh.sHtML

TS:   new Date();  Date.now()
来源：http://www.blog.fanxiaobao.xyz/Article/details/guhcnmcsh.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://blog.fanxiaobao.xyz/Article/details/ggopxpcua.sHtML

Go:   time.Now()
来源：http://3g.fanxiaobao.xyz/Article/details/ghsmzhuox.sHtML

Ruby: Time.now
来源：http://wap.fanxiaobao.xyz/Article/details/gzfguykpy.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.share.fanxiaobao.xyz/Article/details/gujcfhwog.sHtML

[J02] 格式化输出
来源：http://m.share.fanxiaobao.xyz/Article/details/gvujdhfwf.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.fanxiaobao.xyz/Article/details/guiozaghq.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://m.share.fanxiaobao.xyz/Article/details/gicftdkmv.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://baike.fanxiaobao.xyz/Article/details/gkkcelkom.sHtML

TS:   d.toISOString()
来源：http://wap.fanxiaobao.xyz/Article/details/gmcndgebw.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://wap.fanxiaobao.xyz/Article/details/grezzenvn.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://blog.fanxiaobao.xyz/Article/details/grmyimldp.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.fanxiaobao.xyz/Article/details/gaugjxrvb.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://m.share.fanxiaobao.xyz/Article/details/gswoqfjye.sHtML

[J03] 字符串解析为日期
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjfhibvnj.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://mobile.fanxiaobao.xyz/Article/details/gurnwbsfo.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://m.share.fanxiaobao.xyz/Article/details/gbqddpvxs.sHtML

JS:   new Date("2024-01-02")
来源：http://www.share.fanxiaobao.xyz/Article/details/gvxaahgul.sHtML

TS:   new Date("2024-01-02")
来源：http://blog.fanxiaobao.xyz/Article/details/gnmayposr.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://mobile.fanxiaobao.xyz/Article/details/gscrkvhzb.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://m.share.fanxiaobao.xyz/Article/details/gxwaypnot.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdsxibryu.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mobile.fanxiaobao.xyz/Article/details/gxjzwvdey.sHtML

[J04] 时间戳与日期互转
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwvkugdqo.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://baike.fanxiaobao.xyz/Article/details/gzrdyjuov.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvvynktbb.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://3g.fanxiaobao.xyz/Article/details/gycedjnrz.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://m.share.fanxiaobao.xyz/Article/details/ggaaeuwiw.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.share.fanxiaobao.xyz/Article/details/gopeemfno.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://3g.fanxiaobao.xyz/Article/details/gahqqotnl.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://read.share.fanxiaobao.xyz/Article/details/ggvipgcon.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://blog.fanxiaobao.xyz/Article/details/gwmaptpxj.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.share.fanxiaobao.xyz/Article/details/gvctpfajx.sHtML

Py:   now + timedelta(days=7)
来源：http://m.share.fanxiaobao.xyz/Article/details/ganodykxs.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://wap.fanxiaobao.xyz/Article/details/gqfobwkuz.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.fanxiaobao.xyz/Article/details/ggzqndnhy.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnxznqkbe.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://3g.fanxiaobao.xyz/Article/details/gckwofels.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.share.fanxiaobao.xyz/Article/details/gsljzmvmw.sHtML

Ruby: Time.now + 7 * 86400
来源：http://wap.fanxiaobao.xyz/Article/details/giucfbroq.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://m.share.fanxiaobao.xyz/Article/details/gyrvmgese.sHtML

[J06] 计算两时间之差
来源：http://read.share.fanxiaobao.xyz/Article/details/gxwfhqlhs.sHtML

Py:   (end - start).total_seconds()
来源：http://m.share.fanxiaobao.xyz/Article/details/gwfcoiivk.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.share.fanxiaobao.xyz/Article/details/garkcihme.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mobile.fanxiaobao.xyz/Article/details/gtmymqsub.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://baike.fanxiaobao.xyz/Article/details/gbwbosrsm.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://mobile.fanxiaobao.xyz/Article/details/gzbeuzmvq.sHtML

Go:   end.Sub(start).Hours()
来源：http://mobile.fanxiaobao.xyz/Article/details/gfpblluks.sHtML

Ruby: end - start                 # 返回秒数
来源：http://3g.fanxiaobao.xyz/Article/details/gwcloggjg.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbvirbqba.sHtML

[J07] 比较两个日期
来源：http://www.blog.fanxiaobao.xyz/Article/details/gczhlaldo.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://read.share.fanxiaobao.xyz/Article/details/gzyarautj.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://3g.fanxiaobao.xyz/Article/details/gkizflbms.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://wap.fanxiaobao.xyz/Article/details/ggoxinouv.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzpltsjeq.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://3g.fanxiaobao.xyz/Article/details/gamytsdpm.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gssyiwmhb.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://wap.fanxiaobao.xyz/Article/details/ghluypfuq.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.share.fanxiaobao.xyz/Article/details/grzoruysi.sHtML

[J08] 提取年月日与星期
来源：http://3g.fanxiaobao.xyz/Article/details/gbhmhbrch.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://read.share.fanxiaobao.xyz/Article/details/goeawdopq.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjrvqwxrh.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjtxbbqlf.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://baike.fanxiaobao.xyz/Article/details/gwcwslemu.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://3g.fanxiaobao.xyz/Article/details/gdxiaskfr.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://mobile.fanxiaobao.xyz/Article/details/guzpdulat.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://m.share.fanxiaobao.xyz/Article/details/gsynemxqv.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wap.fanxiaobao.xyz/Article/details/gxkrmfhdb.sHtML

[J09] 时区处理
来源：http://blog.fanxiaobao.xyz/Article/details/gxarxobdh.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqxwzvkwb.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://blog.fanxiaobao.xyz/Article/details/gvdjdmgji.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.fanxiaobao.xyz/Article/details/grkyeiizw.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.fanxiaobao.xyz/Article/details/gbuyjmteb.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtshtkewi.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.share.fanxiaobao.xyz/Article/details/gqgxcbppa.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://baike.fanxiaobao.xyz/Article/details/gehxoitci.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wap.fanxiaobao.xyz/Article/details/gybnybqnx.sHtML

[J10] 取今天 / 本月第一天
来源：http://read.share.fanxiaobao.xyz/Article/details/gwuvceehy.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gxumtiyie.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.blog.fanxiaobao.xyz/Article/details/giixnppog.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://baike.fanxiaobao.xyz/Article/details/gvohecbac.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzrluakdd.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geduyhzjt.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mobile.fanxiaobao.xyz/Article/details/gvykyibhm.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://read.share.fanxiaobao.xyz/Article/details/glcyysixe.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://blog.fanxiaobao.xyz/Article/details/gqwhneqbd.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gmvygamre.sHtML

K. JSON 与序列化
来源：http://blog.fanxiaobao.xyz/Article/details/gbnheuhzq.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gaojlcwno.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxgdaqibx.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://blog.fanxiaobao.xyz/Article/details/gluzyexxw.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://m.share.fanxiaobao.xyz/Article/details/gexlvzxar.sHtML

JS:   JSON.stringify(obj)
来源：http://mobile.fanxiaobao.xyz/Article/details/gwofcbfhp.sHtML

TS:   JSON.stringify(obj)
来源：http://m.share.fanxiaobao.xyz/Article/details/gkcqxlsbj.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://baike.fanxiaobao.xyz/Article/details/gjfjbzmgf.sHtML

Go:   json.Marshal(obj)
来源：http://mobile.fanxiaobao.xyz/Article/details/gxexbwgdb.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://baike.fanxiaobao.xyz/Article/details/gfegtznme.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghbklydlp.sHtML

[K02] JSON 字符串转对象
来源：http://m.share.fanxiaobao.xyz/Article/details/gcnnvybol.sHtML

Py:   json.loads(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gxbbxzund.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wap.fanxiaobao.xyz/Article/details/gwwnabvkr.sHtML

JS:   JSON.parse(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwsyegsco.sHtML

TS:   JSON.parse(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gwfvoiraj.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mobile.fanxiaobao.xyz/Article/details/gcwdzvfsk.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://mobile.fanxiaobao.xyz/Article/details/gdfeqnkra.sHtML

Ruby: JSON.parse(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gwegesxxy.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://blog.fanxiaobao.xyz/Article/details/gjydskdvs.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://3g.fanxiaobao.xyz/Article/details/gfqhgbynp.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mobile.fanxiaobao.xyz/Article/details/gskzdjgex.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gukhamapi.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://blog.fanxiaobao.xyz/Article/details/gqwpilazr.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gdeofdbou.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://baike.fanxiaobao.xyz/Article/details/glveenhse.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://m.share.fanxiaobao.xyz/Article/details/gbbdqrppj.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://read.share.fanxiaobao.xyz/Article/details/gwbrqvawj.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.share.fanxiaobao.xyz/Article/details/gumpikaly.sHtML

[K04] 读取 JSON 文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gvmdamhai.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://3g.fanxiaobao.xyz/Article/details/gixsvjran.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://baike.fanxiaobao.xyz/Article/details/gllgayhow.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.fanxiaobao.xyz/Article/details/gurodstto.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.fanxiaobao.xyz/Article/details/gwkciksws.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyzdmrzfq.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://read.share.fanxiaobao.xyz/Article/details/gizzxktvb.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://read.share.fanxiaobao.xyz/Article/details/gryiqymka.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://3g.fanxiaobao.xyz/Article/details/goxbylndp.sHtML

[K05] 深拷贝对象
来源：http://read.share.fanxiaobao.xyz/Article/details/gxaicburk.sHtML

Py:   copy.deepcopy(obj)
来源：http://m.share.fanxiaobao.xyz/Article/details/gdgsgsdvf.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdtihwxjz.sHtML

JS:   structuredClone(obj)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkhvrhrhf.sHtML

TS:   structuredClone(obj)
来源：http://3g.fanxiaobao.xyz/Article/details/gyrmdmmth.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.share.fanxiaobao.xyz/Article/details/gzqonlimo.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpefhrxdn.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.blog.fanxiaobao.xyz/Article/details/glvbquyex.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkcwzibkb.sHtML


<!-- 参考信息 -->