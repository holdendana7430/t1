代发 wailian999

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.fehbvm.com/Article/details/gbvvpwprd.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.zdbjq.cn/Article/details/gbkqbbmra.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mobile.zdbjq.cn/Article/details/gncvoqlsx.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://baike.zdbjq.cn/Article/details/gygcuxllj.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://m.share.hesvh.cn/Article/details/gjelrxaes.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.zdbjq.cn/Article/details/gzjmtdgcj.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.fehbvm.com/Article/details/gdgmtuski.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.fehbvm.com/Article/details/gfzqlqrbg.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.hesvh.cn/Article/details/gdpfykqgw.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://3g.hesvh.cn/Article/details/gufczhrya.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.fehbvm.com/Article/details/gicjmraqu.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.hesvh.cn/Article/details/glfyixzzb.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.hesvh.cn/Article/details/geztonzww.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://read.share.hesvh.cn/Article/details/gvgyvhddd.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.hesvh.cn/Article/details/gjpepouao.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/gnapazrif.sHtML

[H03] 主动抛出异常
来源：http://wap.zdbjq.cn/Article/details/gobrojbom.sHtML

Py:   raise ValueError("错误信息")
来源：http://wap.hesvh.cn/Article/details/gvltlsaln.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://3g.zdbjq.cn/Article/details/gdxtufrjw.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.fehbvm.com/Article/details/gicmcgnga.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.fehbvm.com/Article/details/gmrjmixpk.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://m.share.fehbvm.com/Article/details/gpvjngiri.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.share.hesvh.cn/Article/details/gcaifzzrw.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.m.share.fehbvm.com/Article/details/guaxxuyga.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://blog.fehbvm.com/Article/details/gqhoyyssp.sHtML

[H04] 自定义异常类型
来源：http://wap.zdbjq.cn/Article/details/glfkkxmsp.sHtML

Py:   class MyError(Exception): pass
来源：http://read.share.zdbjq.cn/Article/details/gkfmlyluk.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://baike.fehbvm.com/Article/details/gyxultbxe.sHtML

JS:   class MyError extends Error {}
来源：http://read.share.hesvh.cn/Article/details/gdcndkcbu.sHtML

TS:   class MyError extends Error {}
来源：http://baike.fehbvm.com/Article/details/ggmfzvjzt.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.share.fehbvm.com/Article/details/grvfkszou.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.share.zdbjq.cn/Article/details/govgokjcj.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.m.share.zdbjq.cn/Article/details/gmfhpiqyi.sHtML

C#:   class MyException : Exception {}
来源：http://3g.hesvh.cn/Article/details/gyixpehvv.sHtML

[H05] 捕获特定类型
来源：http://www.m.share.zdbjq.cn/Article/details/gssjxvnoh.sHtML

Py:   except ValueError as e:
来源：http://read.share.fehbvm.com/Article/details/gwnutfsom.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.blog.zdbjq.cn/Article/details/gwytjvykf.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://m.share.hesvh.cn/Article/details/gupukbyho.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.m.share.fehbvm.com/Article/details/gfozmiiyq.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.hesvh.cn/Article/details/grgrwvjmc.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mobile.zdbjq.cn/Article/details/gkipcecjd.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.m.share.zdbjq.cn/Article/details/gdpgwsrsa.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.m.share.hesvh.cn/Article/details/gsmsoayzz.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.m.share.zdbjq.cn/Article/details/ggwtxpifx.sHtML

Py:   value = d.get("k") or default
来源：http://read.share.zdbjq.cn/Article/details/gpiobsbtm.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://baike.hesvh.cn/Article/details/gnymrufmo.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.hesvh.cn/Article/details/ghkmigjau.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://blog.zdbjq.cn/Article/details/gxtxjfaig.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://read.share.zdbjq.cn/Article/details/gvyaaovxh.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.share.zdbjq.cn/Article/details/gyvoksjse.sHtML

Ruby: d&.dig(:a, :b)
来源：http://blog.zdbjq.cn/Article/details/gaewusqkq.sHtML

C#:   obj?.A?.B ?? default
来源：http://mobile.fehbvm.com/Article/details/gwcxwjtsa.sHtML

[H07] 断言
来源：http://m.share.hesvh.cn/Article/details/gvcmojknf.sHtML

Py:   assert x > 0, "必须为正"
来源：http://wap.fehbvm.com/Article/details/ghkrbnfpf.sHtML

PHP:  assert($x > 0);
来源：http://www.share.fehbvm.com/Article/details/gyuuevady.sHtML

JS:   console.assert(x > 0);
来源：http://www.blog.hesvh.cn/Article/details/gnhuhvdtf.sHtML

TS:   console.assert(x > 0);
来源：http://mobile.fehbvm.com/Article/details/gclvrxflz.sHtML

Java: assert x > 0 : "必须为正";
来源：http://read.share.fehbvm.com/Article/details/grmrukhfj.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wap.hesvh.cn/Article/details/gblqpbozb.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://baike.fehbvm.com/Article/details/gvpmtwwsf.sHtML

C#:   Debug.Assert(x > 0);
来源：http://blog.zdbjq.cn/Article/details/guxxqoabf.sHtML

[H08] 获取错误信息与堆栈
来源：http://mobile.fehbvm.com/Article/details/gffbenlxb.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://baike.hesvh.cn/Article/details/gbzhxpynv.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://baike.fehbvm.com/Article/details/gcsbovfoy.sHtML

JS:   e.message;  e.stack
来源：http://blog.hesvh.cn/Article/details/ghizmjoor.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.blog.zdbjq.cn/Article/details/ghahxvdsi.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://m.share.fehbvm.com/Article/details/grdlkjbyh.sHtML

Go:   err.Error()
来源：http://3g.zdbjq.cn/Article/details/gnvynqplk.sHtML

Ruby: e.message;  e.backtrace
来源：http://3g.hesvh.cn/Article/details/gmyfrtnwi.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.blog.hesvh.cn/Article/details/gkynzkhrl.sHtML

[H09] 带错误码的异常
来源：http://baike.zdbjq.cn/Article/details/gletetalz.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wap.hesvh.cn/Article/details/gdzrkqqfs.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.m.share.hesvh.cn/Article/details/gecwyoaxy.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://baike.hesvh.cn/Article/details/gwikgxsyp.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wap.hesvh.cn/Article/details/gephqlasq.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.share.zdbjq.cn/Article/details/gxlvdqxhf.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://read.share.hesvh.cn/Article/details/gzybfwadk.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://blog.zdbjq.cn/Article/details/gzqkivuso.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.m.share.zdbjq.cn/Article/details/gymstblqg.sHtML

[H10] 资源自动释放
来源：http://wap.fehbvm.com/Article/details/gijiyrcgf.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://3g.zdbjq.cn/Article/details/gpqnrpuky.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://m.share.zdbjq.cn/Article/details/gngwerxpz.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.zdbjq.cn/Article/details/gmtclfjps.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.hesvh.cn/Article/details/gloganpgp.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://blog.fehbvm.com/Article/details/gmgltlnrv.sHtML

Go:   defer f.Close()
来源：http://www.blog.fehbvm.com/Article/details/gdcyysyyo.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wap.fehbvm.com/Article/details/gyswlwpnu.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gaicimxys.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gljgdenjv.sHtML

I. 正则表达式
来源：http://mobile.hesvh.cn/Article/details/grggkstis.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gxbdfuqam.sHtML

[I01] 判断是否匹配
来源：http://www.blog.hesvh.cn/Article/details/gvqtowhhs.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://blog.hesvh.cn/Article/details/guqwypxrx.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://3g.hesvh.cn/Article/details/gusaxvdtq.sHtML

JS:   /\d+/.test(s)
来源：http://read.share.hesvh.cn/Article/details/gisanqssr.sHtML

TS:   /\d+/.test(s)
来源：http://mobile.fehbvm.com/Article/details/gujevkdtt.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://read.share.fehbvm.com/Article/details/gauispsax.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://blog.fehbvm.com/Article/details/gyxoyggos.sHtML

Ruby: s.match?(/\d+/)
来源：http://wap.zdbjq.cn/Article/details/gosjpknbm.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.m.share.hesvh.cn/Article/details/gltksjewv.sHtML

[I02] 提取所有匹配
来源：http://baike.zdbjq.cn/Article/details/gmffeqvrx.sHtML

Py:   re.findall(r"\d+", s)
来源：http://mobile.hesvh.cn/Article/details/gtfhwoqpu.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://baike.zdbjq.cn/Article/details/glybrhosa.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wap.zdbjq.cn/Article/details/gfsvlhays.sHtML

TS:   s.match(/\d+/g)
来源：http://wap.hesvh.cn/Article/details/gnkscoofg.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://read.share.fehbvm.com/Article/details/gxobxvvzh.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://m.share.zdbjq.cn/Article/details/gyueaahdx.sHtML

Ruby: s.scan(/\d+/)
来源：http://read.share.hesvh.cn/Article/details/guxmaajof.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://m.share.fehbvm.com/Article/details/gaifwqbbb.sHtML

[I03] 提取捕获分组
来源：http://www.share.fehbvm.com/Article/details/gzkthopfy.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://m.share.hesvh.cn/Article/details/gwaihwskj.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://blog.zdbjq.cn/Article/details/gecdahmlm.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://read.share.zdbjq.cn/Article/details/guzdvoyad.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.share.hesvh.cn/Article/details/gfukptqbu.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://read.share.hesvh.cn/Article/details/gswzgdcpe.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://blog.zdbjq.cn/Article/details/garjcyinj.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.blog.zdbjq.cn/Article/details/gbkrzgtvp.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://m.share.zdbjq.cn/Article/details/gbmfvssqf.sHtML

[I04] 正则替换
来源：http://www.share.hesvh.cn/Article/details/gowfixgoe.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://blog.fehbvm.com/Article/details/gnzecdguj.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://3g.zdbjq.cn/Article/details/gdgdhdyor.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://read.share.fehbvm.com/Article/details/gqbwwiiuy.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://wap.fehbvm.com/Article/details/gdyfqdrit.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://mobile.hesvh.cn/Article/details/gtamlpswq.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://mobile.zdbjq.cn/Article/details/gwayfozis.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://mobile.fehbvm.com/Article/details/gpwtzxlgd.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.m.share.zdbjq.cn/Article/details/glffomoug.sHtML

[I05] 按正则拆分
来源：http://wap.zdbjq.cn/Article/details/ghthkqxvo.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.m.share.hesvh.cn/Article/details/gotomgewx.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mobile.zdbjq.cn/Article/details/gtlvakgmn.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://baike.fehbvm.com/Article/details/ghbnxziey.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://blog.hesvh.cn/Article/details/gtrutmeex.sHtML

Java: s.split("\\s*,\\s*")
来源：http://3g.fehbvm.com/Article/details/gztyepbkg.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://read.share.fehbvm.com/Article/details/gnkthtgws.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://mobile.fehbvm.com/Article/details/ghmpfltfd.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.blog.fehbvm.com/Article/details/gabbnubab.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://read.share.fehbvm.com/Article/details/gyelryiow.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://3g.hesvh.cn/Article/details/gpirntalz.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://m.share.fehbvm.com/Article/details/griwcnvcg.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.fehbvm.com/Article/details/gwomjpnae.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.fehbvm.com/Article/details/glfamhsyh.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://3g.fehbvm.com/Article/details/gcrchsqgj.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://read.share.fehbvm.com/Article/details/ghdamjksc.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.m.share.fehbvm.com/Article/details/gxhhthjnc.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wap.hesvh.cn/Article/details/gwwdfcngx.sHtML

[I07] 忽略大小写与多行模式
来源：http://m.share.fehbvm.com/Article/details/ghpezatbz.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.m.share.zdbjq.cn/Article/details/gkztndkfj.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://3g.fehbvm.com/Article/details/gfsgxjkxb.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://blog.fehbvm.com/Article/details/gpjurammw.sHtML

TS:   /error/gim
来源：http://read.share.zdbjq.cn/Article/details/gzyqjjriu.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.share.zdbjq.cn/Article/details/gwjshbxmi.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.blog.hesvh.cn/Article/details/guffjvdoc.sHtML

Ruby: s.scan(/error/i)
来源：http://m.share.zdbjq.cn/Article/details/gjhpvkgml.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.blog.zdbjq.cn/Article/details/grnvkdhmq.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://wap.fehbvm.com/Article/details/gajtvauqt.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.share.hesvh.cn/Article/details/gfflrofhh.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wap.zdbjq.cn/Article/details/gpswxyxeb.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.hesvh.cn/Article/details/gcrsomkrc.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.fehbvm.com/Article/details/gsircbcnn.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.m.share.fehbvm.com/Article/details/gyrdcizod.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://read.share.hesvh.cn/Article/details/gwwmmbohk.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://m.share.fehbvm.com/Article/details/gsguvxgpc.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://baike.fehbvm.com/Article/details/gojosbfju.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gpxzyopyh.sHtML

J. 日期与时间
来源：http://read.share.hesvh.cn/Article/details/gewcjvkgn.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gfzmvsklm.sHtML

[J01] 获取当前时间
来源：http://3g.fehbvm.com/Article/details/gcphwddff.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://read.share.zdbjq.cn/Article/details/gbybxofhg.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://3g.zdbjq.cn/Article/details/gmpuatodp.sHtML

JS:   new Date();  Date.now()
来源：http://www.m.share.zdbjq.cn/Article/details/gvtcqzdaz.sHtML

TS:   new Date();  Date.now()
来源：http://m.share.hesvh.cn/Article/details/gotbebwfe.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.share.fehbvm.com/Article/details/gewdrqrbw.sHtML

Go:   time.Now()
来源：http://blog.zdbjq.cn/Article/details/gomaopqgx.sHtML

Ruby: Time.now
来源：http://m.share.zdbjq.cn/Article/details/guvbzmzuh.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.m.share.hesvh.cn/Article/details/gkfdhnepe.sHtML

[J02] 格式化输出
来源：http://read.share.fehbvm.com/Article/details/ghwhiojif.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.hesvh.cn/Article/details/gjpximnck.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://baike.hesvh.cn/Article/details/gkgvomfmj.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.m.share.zdbjq.cn/Article/details/glljtmtyj.sHtML

TS:   d.toISOString()
来源：http://www.share.zdbjq.cn/Article/details/gukrsjhiu.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mobile.zdbjq.cn/Article/details/gdyslozbv.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.m.share.fehbvm.com/Article/details/gdbqwklsp.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.hesvh.cn/Article/details/gyqhdnjpt.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://mobile.fehbvm.com/Article/details/gjzbwpmpb.sHtML

[J03] 字符串解析为日期
来源：http://3g.zdbjq.cn/Article/details/gdbeloqfg.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wap.fehbvm.com/Article/details/gvdsfjsgp.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.blog.fehbvm.com/Article/details/gluiqfybm.sHtML

JS:   new Date("2024-01-02")
来源：http://blog.fehbvm.com/Article/details/guowtcnmq.sHtML

TS:   new Date("2024-01-02")
来源：http://www.m.share.fehbvm.com/Article/details/gwsuvtelj.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://m.share.fehbvm.com/Article/details/gdwataaok.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wap.fehbvm.com/Article/details/guknzbjqv.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://3g.zdbjq.cn/Article/details/gtwnluvju.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://m.share.zdbjq.cn/Article/details/gfqcztigp.sHtML

[J04] 时间戳与日期互转
来源：http://baike.fehbvm.com/Article/details/gcewmejxb.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://blog.hesvh.cn/Article/details/gzfzyifzq.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://mobile.hesvh.cn/Article/details/gljnevdmz.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://wap.zdbjq.cn/Article/details/gmbausfia.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://wap.zdbjq.cn/Article/details/gktuzepmc.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://m.share.hesvh.cn/Article/details/gdaecudcd.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://read.share.hesvh.cn/Article/details/gjiaaysht.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.share.hesvh.cn/Article/details/geuwbfejo.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://blog.hesvh.cn/Article/details/gfblfdygv.sHtML

[J05] 时间加减（加 7 天）
来源：http://baike.fehbvm.com/Article/details/gpjdqtglx.sHtML

Py:   now + timedelta(days=7)
来源：http://www.share.hesvh.cn/Article/details/gjlgdkcok.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://mobile.hesvh.cn/Article/details/gevynuqcx.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.fehbvm.com/Article/details/gwdrihwrp.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.hesvh.cn/Article/details/geexltuqx.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://blog.fehbvm.com/Article/details/gxlujtakk.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://3g.hesvh.cn/Article/details/gzighxqmt.sHtML

Ruby: Time.now + 7 * 86400
来源：http://read.share.fehbvm.com/Article/details/gtevgnnqe.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.blog.fehbvm.com/Article/details/gjwnjtcpc.sHtML

[J06] 计算两时间之差
来源：http://3g.zdbjq.cn/Article/details/gyoyqbyko.sHtML

Py:   (end - start).total_seconds()
来源：http://read.share.hesvh.cn/Article/details/gnfvzzgha.sHtML

PHP:  $end->diff($start)->days;
来源：http://m.share.zdbjq.cn/Article/details/grhwzjjsz.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.blog.hesvh.cn/Article/details/gculrcpez.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://read.share.zdbjq.cn/Article/details/gzxjktdxg.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.m.share.zdbjq.cn/Article/details/guholidvr.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.share.hesvh.cn/Article/details/gietefgsn.sHtML

Ruby: end - start                 # 返回秒数
来源：http://blog.zdbjq.cn/Article/details/gayxbtxdy.sHtML

C#:   (end - start).TotalSeconds
来源：http://baike.zdbjq.cn/Article/details/gmxbdnnth.sHtML

[J07] 比较两个日期
来源：http://www.share.hesvh.cn/Article/details/glliqqrvf.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://baike.hesvh.cn/Article/details/gvurittpq.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.blog.zdbjq.cn/Article/details/gjzgczagu.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://wap.hesvh.cn/Article/details/gmynutyoi.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://mobile.zdbjq.cn/Article/details/gimpoqzke.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://read.share.zdbjq.cn/Article/details/gokkekhoe.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://m.share.fehbvm.com/Article/details/gqupwvfni.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://m.share.fehbvm.com/Article/details/gsbmrkoii.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://blog.fehbvm.com/Article/details/gezulrjht.sHtML

[J08] 提取年月日与星期
来源：http://www.m.share.hesvh.cn/Article/details/gzgutoxbw.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.blog.hesvh.cn/Article/details/gvaeobvqa.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.m.share.fehbvm.com/Article/details/gxghmgeoy.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://baike.fehbvm.com/Article/details/gcjsrbmna.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.blog.fehbvm.com/Article/details/gkhrvbqam.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wap.zdbjq.cn/Article/details/gvezhxjae.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.share.fehbvm.com/Article/details/gnwutwein.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://m.share.fehbvm.com/Article/details/ghbcxrjxu.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://blog.zdbjq.cn/Article/details/gvvqktexm.sHtML

[J09] 时区处理
来源：http://www.share.zdbjq.cn/Article/details/gfjcdbpko.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.m.share.zdbjq.cn/Article/details/gncrphzxb.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://3g.fehbvm.com/Article/details/gtpwusqzd.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.zdbjq.cn/Article/details/gikztenwb.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.zdbjq.cn/Article/details/ghbyuyctx.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.blog.fehbvm.com/Article/details/gppnssdyj.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.share.zdbjq.cn/Article/details/gfzlqpcqm.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.share.fehbvm.com/Article/details/gmppsnhrp.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.blog.fehbvm.com/Article/details/gssadaxrk.sHtML

[J10] 取今天 / 本月第一天
来源：http://wap.zdbjq.cn/Article/details/gmztqvkhn.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://3g.fehbvm.com/Article/details/gslmbmyba.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://m.share.fehbvm.com/Article/details/gdewvxooo.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.share.hesvh.cn/Article/details/guanljcle.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://blog.fehbvm.com/Article/details/gkapljjwj.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://3g.fehbvm.com/Article/details/glelvomut.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://blog.fehbvm.com/Article/details/getncytxc.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://3g.fehbvm.com/Article/details/gknhvcyyd.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wap.hesvh.cn/Article/details/gewmxhrmn.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gybbxibkh.sHtML

K. JSON 与序列化
来源：http://read.share.zdbjq.cn/Article/details/gtaxtfdvy.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/ghieznrky.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.share.zdbjq.cn/Article/details/gjwtrzjtu.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://m.share.hesvh.cn/Article/details/gdsqtrfkw.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mobile.hesvh.cn/Article/details/gciixyaby.sHtML

JS:   JSON.stringify(obj)
来源：http://www.share.fehbvm.com/Article/details/gbkmvafrs.sHtML

TS:   JSON.stringify(obj)
来源：http://3g.hesvh.cn/Article/details/ghhdkisys.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://3g.zdbjq.cn/Article/details/gzcsirnvw.sHtML

Go:   json.Marshal(obj)
来源：http://wap.zdbjq.cn/Article/details/gteadlndn.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://baike.zdbjq.cn/Article/details/gpwsauzhs.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.blog.hesvh.cn/Article/details/gulzsgydo.sHtML

[K02] JSON 字符串转对象
来源：http://www.m.share.zdbjq.cn/Article/details/gkbxbxbwm.sHtML

Py:   json.loads(s)
来源：http://m.share.fehbvm.com/Article/details/gzrpzeomq.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://read.share.zdbjq.cn/Article/details/gmimkrxxm.sHtML

JS:   JSON.parse(s)
来源：http://read.share.fehbvm.com/Article/details/gxyjqtjsn.sHtML

TS:   JSON.parse(s)
来源：http://baike.zdbjq.cn/Article/details/galcmavyv.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://3g.zdbjq.cn/Article/details/geckfrgol.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://wap.fehbvm.com/Article/details/gulglujyb.sHtML

Ruby: JSON.parse(s)
来源：http://www.m.share.hesvh.cn/Article/details/gqqemmgph.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.blog.zdbjq.cn/Article/details/gimcymmhz.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://mobile.zdbjq.cn/Article/details/gvewgwcks.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://m.share.zdbjq.cn/Article/details/gutysqgde.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://m.share.fehbvm.com/Article/details/gwrlmpxbe.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.share.hesvh.cn/Article/details/glktsvbli.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://read.share.zdbjq.cn/Article/details/gkiuamcmj.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://m.share.fehbvm.com/Article/details/gccpaynhi.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://3g.zdbjq.cn/Article/details/ggmdyruud.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://wap.hesvh.cn/Article/details/gxzitlmjj.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.blog.zdbjq.cn/Article/details/gtatymnvq.sHtML

[K04] 读取 JSON 文件
来源：http://read.share.hesvh.cn/Article/details/gwvctwcde.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://blog.hesvh.cn/Article/details/goifsfpuz.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://blog.zdbjq.cn/Article/details/gbhiqlykx.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.fehbvm.com/Article/details/gbsncynup.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.zdbjq.cn/Article/details/ghnmxgvpk.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.blog.hesvh.cn/Article/details/gaqvfnnba.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://read.share.fehbvm.com/Article/details/ghktedaxs.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.m.share.zdbjq.cn/Article/details/gzgjiwuhi.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.blog.hesvh.cn/Article/details/gwbmlhpfe.sHtML

[K05] 深拷贝对象
来源：http://www.m.share.hesvh.cn/Article/details/gadtwiyed.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gbpipayef.sHtML

PHP:  unserialize(serialize($obj));
来源：http://blog.zdbjq.cn/Article/details/gjnyrbsxc.sHtML

JS:   structuredClone(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/ghnvetzqt.sHtML

TS:   structuredClone(obj)
来源：http://www.share.fehbvm.com/Article/details/grlqesfng.sHtML


<!-- 参考信息 -->