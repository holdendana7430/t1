代发 wailian999

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.fanxiaobao.xyz/Article/details/gvgyqgdcf.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.fanxiaobao.xyz/Article/details/gqtwrmxcx.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.fanxiaobao.xyz/Article/details/giiasthcg.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mobile.fanxiaobao.xyz/Article/details/garuujrqb.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mobile.fanxiaobao.xyz/Article/details/gootxatci.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://3g.fanxiaobao.xyz/Article/details/gfngwtdpd.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwuaupqar.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.fanxiaobao.xyz/Article/details/gulhwlkpj.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.fanxiaobao.xyz/Article/details/grpymbfrs.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://blog.fanxiaobao.xyz/Article/details/gvwsqwmcj.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gawyuavwe.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqeimtedo.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.fanxiaobao.xyz/Article/details/ggkdrpjds.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.share.fanxiaobao.xyz/Article/details/ghjzxricv.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.share.fanxiaobao.xyz/Article/details/gkgvhyjnl.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gpajeglpb.sHtML

[H03] 主动抛出异常
来源：http://read.share.fanxiaobao.xyz/Article/details/gytovddta.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.fanxiaobao.xyz/Article/details/gjpydurml.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.fanxiaobao.xyz/Article/details/gzfvdxiyo.sHtML

JS:   throw new Error("错误信息");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdiafifxv.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.fanxiaobao.xyz/Article/details/gfdthstwu.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.fanxiaobao.xyz/Article/details/gpphtbgic.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.share.fanxiaobao.xyz/Article/details/gzxglhdxf.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://3g.fanxiaobao.xyz/Article/details/gzpwdvenw.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://wap.fanxiaobao.xyz/Article/details/gmwbxdafr.sHtML

[H04] 自定义异常类型
来源：http://m.share.fanxiaobao.xyz/Article/details/gdupeqxgd.sHtML

Py:   class MyError(Exception): pass
来源：http://3g.fanxiaobao.xyz/Article/details/geagfvmlf.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gtfcyfcev.sHtML

JS:   class MyError extends Error {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnbtzlmzg.sHtML

TS:   class MyError extends Error {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gipszkfna.sHtML

Java: class MyException extends RuntimeException {}
来源：http://mobile.fanxiaobao.xyz/Article/details/ggfpatayo.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.share.fanxiaobao.xyz/Article/details/gjptnlrru.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggopyxxog.sHtML

C#:   class MyException : Exception {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqwacjpul.sHtML

[H05] 捕获特定类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdmmvfnya.sHtML

Py:   except ValueError as e:
来源：http://baike.fanxiaobao.xyz/Article/details/gvigfefjq.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.fanxiaobao.xyz/Article/details/gqjfqwvgg.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://baike.fanxiaobao.xyz/Article/details/gvdkfeesj.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://3g.fanxiaobao.xyz/Article/details/gcrixwphj.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/ghhbuyvfl.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqiaplefu.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gygbkjvjc.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnztnxbub.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsipjqmfv.sHtML

Py:   value = d.get("k") or default
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gssrtpapp.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://m.share.fanxiaobao.xyz/Article/details/gzqwnbqmv.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://wap.fanxiaobao.xyz/Article/details/gdhqeurzt.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://m.share.fanxiaobao.xyz/Article/details/gakxujpuj.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvpfvgekb.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfvqpoeqc.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxzjhrxgy.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmhuypwwd.sHtML

[H07] 断言
来源：http://blog.fanxiaobao.xyz/Article/details/gwevknngf.sHtML

Py:   assert x > 0, "必须为正"
来源：http://wap.fanxiaobao.xyz/Article/details/giywchzar.sHtML

PHP:  assert($x > 0);
来源：http://mobile.fanxiaobao.xyz/Article/details/gkcgoxkip.sHtML

JS:   console.assert(x > 0);
来源：http://www.share.fanxiaobao.xyz/Article/details/gwbhoiqjz.sHtML

TS:   console.assert(x > 0);
来源：http://wap.fanxiaobao.xyz/Article/details/glbpebtlh.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghxntzcxs.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://read.share.fanxiaobao.xyz/Article/details/gegqurajs.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvkgaskwl.sHtML

C#:   Debug.Assert(x > 0);
来源：http://baike.fanxiaobao.xyz/Article/details/gdyuppggf.sHtML

[H08] 获取错误信息与堆栈
来源：http://read.share.fanxiaobao.xyz/Article/details/gqqzrmlvk.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://read.share.fanxiaobao.xyz/Article/details/gehwsveur.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.blog.fanxiaobao.xyz/Article/details/goaepfzcc.sHtML

JS:   e.message;  e.stack
来源：http://blog.fanxiaobao.xyz/Article/details/gitkkitng.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://m.share.fanxiaobao.xyz/Article/details/graoikrcd.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gviobijmr.sHtML

Go:   err.Error()
来源：http://wap.fanxiaobao.xyz/Article/details/gboovwifx.sHtML

Ruby: e.message;  e.backtrace
来源：http://baike.fanxiaobao.xyz/Article/details/gaxompfka.sHtML

C#:   e.Message;  e.StackTrace
来源：http://baike.fanxiaobao.xyz/Article/details/gvymeehyo.sHtML

[H09] 带错误码的异常
来源：http://baike.fanxiaobao.xyz/Article/details/glyikijar.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://3g.fanxiaobao.xyz/Article/details/guftbmwiy.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://read.share.fanxiaobao.xyz/Article/details/gpktjxmzo.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://baike.fanxiaobao.xyz/Article/details/gyodcvbmr.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.share.fanxiaobao.xyz/Article/details/gbptycwqc.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gzvylojgw.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://read.share.fanxiaobao.xyz/Article/details/gxtnrwawb.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzfyiaxgk.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqrzkwkmz.sHtML

[H10] 资源自动释放
来源：http://read.share.fanxiaobao.xyz/Article/details/goxbdskvc.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://3g.fanxiaobao.xyz/Article/details/gasajcntd.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gufxcmpkm.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.fanxiaobao.xyz/Article/details/gwibuunky.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.fanxiaobao.xyz/Article/details/gvtaeaqnx.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://blog.fanxiaobao.xyz/Article/details/gwdmqcdew.sHtML

Go:   defer f.Close()
来源：http://wap.fanxiaobao.xyz/Article/details/gmzibaxug.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://3g.fanxiaobao.xyz/Article/details/gfdrbfejq.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://blog.fanxiaobao.xyz/Article/details/gbikxgxuj.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwfbngpsr.sHtML

I. 正则表达式
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnoptvsqj.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gfjxhijrj.sHtML

[I01] 判断是否匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqkruhgfd.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gycwaqinc.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.share.fanxiaobao.xyz/Article/details/gkbetanrz.sHtML

JS:   /\d+/.test(s)
来源：http://3g.fanxiaobao.xyz/Article/details/gdxoqgtaf.sHtML

TS:   /\d+/.test(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/ghdscxadl.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://blog.fanxiaobao.xyz/Article/details/goruolibd.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://3g.fanxiaobao.xyz/Article/details/gcudyljnf.sHtML

Ruby: s.match?(/\d+/)
来源：http://m.share.fanxiaobao.xyz/Article/details/gnwesrxuu.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://read.share.fanxiaobao.xyz/Article/details/geswwhfsj.sHtML

[I02] 提取所有匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghjqzlqng.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gbofulqou.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://read.share.fanxiaobao.xyz/Article/details/ggusbzxkw.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://m.share.fanxiaobao.xyz/Article/details/gilhzkrtz.sHtML

TS:   s.match(/\d+/g)
来源：http://3g.fanxiaobao.xyz/Article/details/grfwubtfm.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://3g.fanxiaobao.xyz/Article/details/gioewfhgd.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gskebpbti.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.share.fanxiaobao.xyz/Article/details/gjxlasmog.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://baike.fanxiaobao.xyz/Article/details/gejooyiqw.sHtML

[I03] 提取捕获分组
来源：http://baike.fanxiaobao.xyz/Article/details/gyuqjxath.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gkeqdnftm.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjfjcwikz.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://baike.fanxiaobao.xyz/Article/details/gkftumyoa.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gebpfmuee.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.share.fanxiaobao.xyz/Article/details/gmccyhmkx.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://3g.fanxiaobao.xyz/Article/details/gxyorlnox.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://3g.fanxiaobao.xyz/Article/details/gibapefor.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://read.share.fanxiaobao.xyz/Article/details/ggyxmyijd.sHtML

[I04] 正则替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gsprppjeu.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://wap.fanxiaobao.xyz/Article/details/gjfzqhphj.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzsqwgnxm.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://baike.fanxiaobao.xyz/Article/details/gdqzrbwcg.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://blog.fanxiaobao.xyz/Article/details/gtwjjahgr.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://m.share.fanxiaobao.xyz/Article/details/giwiulpqq.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://mobile.fanxiaobao.xyz/Article/details/gchosthgl.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpnobgcqx.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.share.fanxiaobao.xyz/Article/details/gxwmkxheq.sHtML

[I05] 按正则拆分
来源：http://www.share.fanxiaobao.xyz/Article/details/gnamtwwjv.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gtgukamvd.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://blog.fanxiaobao.xyz/Article/details/gttrqkftk.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://3g.fanxiaobao.xyz/Article/details/gzqalznxw.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://baike.fanxiaobao.xyz/Article/details/gumovahzu.sHtML

Java: s.split("\\s*,\\s*")
来源：http://read.share.fanxiaobao.xyz/Article/details/grqkptzav.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbxjvuqvm.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://blog.fanxiaobao.xyz/Article/details/gncxuhhhf.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtapzllmy.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpdscxucu.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://baike.fanxiaobao.xyz/Article/details/gqmidmgsv.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.share.fanxiaobao.xyz/Article/details/gegnvocni.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.fanxiaobao.xyz/Article/details/gdlxcykmk.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxbmvaxue.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://m.share.fanxiaobao.xyz/Article/details/gcjponzle.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.share.fanxiaobao.xyz/Article/details/goobcemhz.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://mobile.fanxiaobao.xyz/Article/details/gwgosxhih.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mobile.fanxiaobao.xyz/Article/details/gqdlnfjil.sHtML

[I07] 忽略大小写与多行模式
来源：http://mobile.fanxiaobao.xyz/Article/details/gydjvjlkd.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvcashiis.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://3g.fanxiaobao.xyz/Article/details/gjuirenuv.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mobile.fanxiaobao.xyz/Article/details/gwucjngdr.sHtML

TS:   /error/gim
来源：http://read.share.fanxiaobao.xyz/Article/details/gmodfuyze.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mobile.fanxiaobao.xyz/Article/details/gyhyyqluc.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.share.fanxiaobao.xyz/Article/details/gqodkmubd.sHtML

Ruby: s.scan(/error/i)
来源：http://mobile.fanxiaobao.xyz/Article/details/gajaerwjp.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://baike.fanxiaobao.xyz/Article/details/gdolnyhaq.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://baike.fanxiaobao.xyz/Article/details/ghkzyemth.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goiulrpen.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://3g.fanxiaobao.xyz/Article/details/gwouazurh.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvecqaxwc.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvdkqizqr.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaqrpueig.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.share.fanxiaobao.xyz/Article/details/gagqcvdwk.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://baike.fanxiaobao.xyz/Article/details/gbaucpljy.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://m.share.fanxiaobao.xyz/Article/details/gkpchcugh.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/ggijthzuf.sHtML

J. 日期与时间
来源：http://3g.fanxiaobao.xyz/Article/details/gdyrkohvs.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gjmmsttgf.sHtML

[J01] 获取当前时间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtyizrppk.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://3g.fanxiaobao.xyz/Article/details/gdfkbfksq.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://read.share.fanxiaobao.xyz/Article/details/gjrzxetzf.sHtML

JS:   new Date();  Date.now()
来源：http://mobile.fanxiaobao.xyz/Article/details/gwlyisgdc.sHtML

TS:   new Date();  Date.now()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxjitggaf.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.share.fanxiaobao.xyz/Article/details/gkjbfuiyp.sHtML

Go:   time.Now()
来源：http://wap.fanxiaobao.xyz/Article/details/gyxrsgmlr.sHtML

Ruby: Time.now
来源：http://baike.fanxiaobao.xyz/Article/details/gztqsfpgu.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://mobile.fanxiaobao.xyz/Article/details/gwdpcncnp.sHtML

[J02] 格式化输出
来源：http://read.share.fanxiaobao.xyz/Article/details/gfzhkfjdi.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.fanxiaobao.xyz/Article/details/gkqjylwrf.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdqbbncfn.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://read.share.fanxiaobao.xyz/Article/details/glqntojcj.sHtML

TS:   d.toISOString()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gumwbaewr.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mobile.fanxiaobao.xyz/Article/details/ghibfveys.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.share.fanxiaobao.xyz/Article/details/ghbtdfcad.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.fanxiaobao.xyz/Article/details/gbfwafeny.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmxukayyf.sHtML

[J03] 字符串解析为日期
来源：http://baike.fanxiaobao.xyz/Article/details/gzxxazqve.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://m.share.fanxiaobao.xyz/Article/details/gzjpkxrix.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://blog.fanxiaobao.xyz/Article/details/gwdplflpy.sHtML

JS:   new Date("2024-01-02")
来源：http://read.share.fanxiaobao.xyz/Article/details/gfsqsxeex.sHtML

TS:   new Date("2024-01-02")
来源：http://m.share.fanxiaobao.xyz/Article/details/gqhgfxnlh.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://baike.fanxiaobao.xyz/Article/details/gmdqlruag.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyilzmehb.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://baike.fanxiaobao.xyz/Article/details/grfcootaz.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://baike.fanxiaobao.xyz/Article/details/glecqayhr.sHtML

[J04] 时间戳与日期互转
来源：http://www.blog.fanxiaobao.xyz/Article/details/glgazuuit.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wap.fanxiaobao.xyz/Article/details/gtslrwdbh.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wap.fanxiaobao.xyz/Article/details/gqdvscxtc.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://wap.fanxiaobao.xyz/Article/details/ggnbosfxr.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnmeugtpl.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnvbhvpvu.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://3g.fanxiaobao.xyz/Article/details/gydcnfpfo.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://baike.fanxiaobao.xyz/Article/details/gcfspxraj.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqkoguzik.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gznodrniv.sHtML

Py:   now + timedelta(days=7)
来源：http://mobile.fanxiaobao.xyz/Article/details/gasxnpuya.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://m.share.fanxiaobao.xyz/Article/details/gbzmclrzg.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.fanxiaobao.xyz/Article/details/grevtdxeo.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggqborqtj.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbvohgmts.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://read.share.fanxiaobao.xyz/Article/details/gldocllgz.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkcmxyokn.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://read.share.fanxiaobao.xyz/Article/details/grdvxwqin.sHtML

[J06] 计算两时间之差
来源：http://blog.fanxiaobao.xyz/Article/details/gnffvqrct.sHtML

Py:   (end - start).total_seconds()
来源：http://www.share.fanxiaobao.xyz/Article/details/gsgrdfspd.sHtML

PHP:  $end->diff($start)->days;
来源：http://m.share.fanxiaobao.xyz/Article/details/guvvxndus.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.share.fanxiaobao.xyz/Article/details/gipisrogc.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://read.share.fanxiaobao.xyz/Article/details/gimkqufsp.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.share.fanxiaobao.xyz/Article/details/gzaaxlhrz.sHtML

Go:   end.Sub(start).Hours()
来源：http://3g.fanxiaobao.xyz/Article/details/gvgdyxodr.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcglcdjsf.sHtML

C#:   (end - start).TotalSeconds
来源：http://m.share.fanxiaobao.xyz/Article/details/gazxkbdlc.sHtML

[J07] 比较两个日期
来源：http://mobile.fanxiaobao.xyz/Article/details/gzjtllter.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://m.share.fanxiaobao.xyz/Article/details/gctjxpdtl.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://baike.fanxiaobao.xyz/Article/details/gcmewulcy.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.share.fanxiaobao.xyz/Article/details/gdenayddq.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://baike.fanxiaobao.xyz/Article/details/ghuftrnvh.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gjtpqaorx.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://3g.fanxiaobao.xyz/Article/details/gkinahpex.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://blog.fanxiaobao.xyz/Article/details/gcijtiuuk.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://mobile.fanxiaobao.xyz/Article/details/guejsajua.sHtML

[J08] 提取年月日与星期
来源：http://3g.fanxiaobao.xyz/Article/details/ghaguoknb.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://read.share.fanxiaobao.xyz/Article/details/guxtpkjtc.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gohmgdgfr.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcvufzvij.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://blog.fanxiaobao.xyz/Article/details/gepruqvbt.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://baike.fanxiaobao.xyz/Article/details/gkhmgsvsk.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://3g.fanxiaobao.xyz/Article/details/ghyusbliw.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://3g.fanxiaobao.xyz/Article/details/gfhtlvphk.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://3g.fanxiaobao.xyz/Article/details/gvxtwzjfp.sHtML

[J09] 时区处理
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqvowfaqo.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mobile.fanxiaobao.xyz/Article/details/ggalmfipv.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://read.share.fanxiaobao.xyz/Article/details/gjxblcgiq.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.fanxiaobao.xyz/Article/details/gcadpszvd.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.fanxiaobao.xyz/Article/details/geudhqhcy.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.share.fanxiaobao.xyz/Article/details/gkzryblvf.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtdntttug.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://wap.fanxiaobao.xyz/Article/details/gpcyfrafy.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mobile.fanxiaobao.xyz/Article/details/gjiaxqbbj.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.share.fanxiaobao.xyz/Article/details/gzuerzmwp.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gebgaxgkr.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.share.fanxiaobao.xyz/Article/details/gdnampdab.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://blog.fanxiaobao.xyz/Article/details/gzwrwbqjf.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wap.fanxiaobao.xyz/Article/details/gpwuakcfp.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gshhdnkdm.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwbzfjhki.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://read.share.fanxiaobao.xyz/Article/details/gmxooeoba.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geywqufez.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gvykvtnih.sHtML

K. JSON 与序列化
来源：http://3g.fanxiaobao.xyz/Article/details/gnmmixjtw.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gngdqfaeg.sHtML

[K01] 对象转 JSON 字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gkgchxojx.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wap.fanxiaobao.xyz/Article/details/gvuiqqrer.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.blog.fanxiaobao.xyz/Article/details/glamaqhqc.sHtML

JS:   JSON.stringify(obj)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbzeqgwfy.sHtML

TS:   JSON.stringify(obj)
来源：http://wap.fanxiaobao.xyz/Article/details/gtseobwqe.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://baike.fanxiaobao.xyz/Article/details/gfbyfdtjp.sHtML

Go:   json.Marshal(obj)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geuscpugm.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://read.share.fanxiaobao.xyz/Article/details/gbdeyxgxx.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://read.share.fanxiaobao.xyz/Article/details/ghxydakwb.sHtML

[K02] JSON 字符串转对象
来源：http://mobile.fanxiaobao.xyz/Article/details/gbpsaeezs.sHtML

Py:   json.loads(s)
来源：http://3g.fanxiaobao.xyz/Article/details/gfpccqphb.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpmszitei.sHtML

JS:   JSON.parse(s)
来源：http://blog.fanxiaobao.xyz/Article/details/gktlkugii.sHtML

TS:   JSON.parse(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gfvhzabhx.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mobile.fanxiaobao.xyz/Article/details/gdzlloeer.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://wap.fanxiaobao.xyz/Article/details/gslnulsfi.sHtML

Ruby: JSON.parse(s)
来源：http://wap.fanxiaobao.xyz/Article/details/gpryghemx.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grdsjnolt.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsparxxrj.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mobile.fanxiaobao.xyz/Article/details/gamirgbqg.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbhoaagcx.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gktrsvxmd.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gjlayqugo.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://baike.fanxiaobao.xyz/Article/details/gcswqshyb.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wap.fanxiaobao.xyz/Article/details/gobxqpudt.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.share.fanxiaobao.xyz/Article/details/gmewcmqzp.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjiswgpkk.sHtML

[K04] 读取 JSON 文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxnibbcwp.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://m.share.fanxiaobao.xyz/Article/details/gqfgduphv.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://3g.fanxiaobao.xyz/Article/details/gbcubrhzt.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.fanxiaobao.xyz/Article/details/gevvjhepa.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gutkyjzeh.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmxdghkuh.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gndstffao.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://m.share.fanxiaobao.xyz/Article/details/gdxwfnhsl.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://blog.fanxiaobao.xyz/Article/details/ggzdzillx.sHtML

[K05] 深拷贝对象
来源：http://baike.fanxiaobao.xyz/Article/details/gxdcdtutc.sHtML

Py:   copy.deepcopy(obj)
来源：http://blog.fanxiaobao.xyz/Article/details/gmjjbhpmm.sHtML

PHP:  unserialize(serialize($obj));
来源：http://blog.fanxiaobao.xyz/Article/details/glwpiryfo.sHtML

JS:   structuredClone(obj)
来源：http://3g.fanxiaobao.xyz/Article/details/grkofbfws.sHtML

TS:   structuredClone(obj)
来源：http://baike.fanxiaobao.xyz/Article/details/gdqwghrwh.sHtML


<!-- 参考信息 -->