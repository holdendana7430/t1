代发 wailian999

Py:   try: f()⏎finally: cleanup()
来源：http://3g.zdbjq.cn/Article/details/grlsqklnv.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://3g.hesvh.cn/Article/details/gaikjrkfg.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://3g.fehbvm.com/Article/details/glizgesvg.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.zdbjq.cn/Article/details/gviizpjqu.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.m.share.hesvh.cn/Article/details/gqrekmvmj.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.blog.fehbvm.com/Article/details/gltxqejpv.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.hesvh.cn/Article/details/gvdcuegbv.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.share.fehbvm.com/Article/details/gjazajtpd.sHtML

[H03] 主动抛出异常
来源：http://wap.zdbjq.cn/Article/details/gnyohmagv.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.zdbjq.cn/Article/details/gcsatfpve.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://baike.hesvh.cn/Article/details/glmklqhok.sHtML

JS:   throw new Error("错误信息");
来源：http://www.share.hesvh.cn/Article/details/gtxchathb.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.fehbvm.com/Article/details/gejdubbaf.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.fehbvm.com/Article/details/gysugswwi.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wap.hesvh.cn/Article/details/gioujzgdo.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://m.share.hesvh.cn/Article/details/goaydjlgs.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://wap.hesvh.cn/Article/details/gklilpcwi.sHtML

[H04] 自定义异常类型
来源：http://www.blog.zdbjq.cn/Article/details/glvsmupod.sHtML

Py:   class MyError(Exception): pass
来源：http://www.m.share.fehbvm.com/Article/details/gwkonidnv.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://blog.zdbjq.cn/Article/details/guzxjchkk.sHtML

JS:   class MyError extends Error {}
来源：http://www.share.hesvh.cn/Article/details/gfjkueobu.sHtML

TS:   class MyError extends Error {}
来源：http://mobile.hesvh.cn/Article/details/gdpabdibu.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.fehbvm.com/Article/details/gicfulhej.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.zdbjq.cn/Article/details/grjqecytb.sHtML

Ruby: class MyError < StandardError; end
来源：http://3g.hesvh.cn/Article/details/gvrolxsht.sHtML

C#:   class MyException : Exception {}
来源：http://3g.zdbjq.cn/Article/details/gwwsczzpb.sHtML

[H05] 捕获特定类型
来源：http://read.share.hesvh.cn/Article/details/ggnqrifcr.sHtML

Py:   except ValueError as e:
来源：http://www.share.zdbjq.cn/Article/details/gwwtnzdim.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://m.share.zdbjq.cn/Article/details/gclcjnqhz.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://baike.fehbvm.com/Article/details/gtijsdrfy.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.blog.hesvh.cn/Article/details/gfdxeanyv.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://baike.hesvh.cn/Article/details/goijlagun.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://3g.hesvh.cn/Article/details/gfccayrbv.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.blog.zdbjq.cn/Article/details/goibahajw.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://read.share.zdbjq.cn/Article/details/gsvledhvw.sHtML

[H06] 可选值 / 空值安全访问
来源：http://wap.zdbjq.cn/Article/details/gxlmgjbcq.sHtML

Py:   value = d.get("k") or default
来源：http://blog.zdbjq.cn/Article/details/gutbkfdkg.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.m.share.fehbvm.com/Article/details/ghkbwyirc.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://read.share.zdbjq.cn/Article/details/gsdbsempq.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://read.share.hesvh.cn/Article/details/gkdilbotf.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mobile.hesvh.cn/Article/details/gsxfennwb.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://blog.fehbvm.com/Article/details/gpebkeegu.sHtML

Ruby: d&.dig(:a, :b)
来源：http://baike.hesvh.cn/Article/details/gjlednxsk.sHtML

C#:   obj?.A?.B ?? default
来源：http://baike.fehbvm.com/Article/details/gwpqmjrgt.sHtML

[H07] 断言
来源：http://blog.hesvh.cn/Article/details/grsjlxvmp.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.share.zdbjq.cn/Article/details/gcsimuuts.sHtML

PHP:  assert($x > 0);
来源：http://wap.fehbvm.com/Article/details/galkephkv.sHtML

JS:   console.assert(x > 0);
来源：http://mobile.zdbjq.cn/Article/details/gtqvxioku.sHtML

TS:   console.assert(x > 0);
来源：http://read.share.fehbvm.com/Article/details/gpqrawach.sHtML

Java: assert x > 0 : "必须为正";
来源：http://m.share.fehbvm.com/Article/details/gfgpiewsn.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mobile.fehbvm.com/Article/details/gsxmqpksx.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.share.zdbjq.cn/Article/details/gpckknyoh.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.blog.hesvh.cn/Article/details/gnmrojguy.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.blog.zdbjq.cn/Article/details/glzkfjweu.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.share.hesvh.cn/Article/details/gvvguvfud.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://m.share.fehbvm.com/Article/details/gdktisjjl.sHtML

JS:   e.message;  e.stack
来源：http://wap.zdbjq.cn/Article/details/gaquuspcz.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://blog.hesvh.cn/Article/details/gjrfutzpj.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://mobile.hesvh.cn/Article/details/gzxrikpjx.sHtML

Go:   err.Error()
来源：http://3g.zdbjq.cn/Article/details/gkwmnfebu.sHtML

Ruby: e.message;  e.backtrace
来源：http://wap.zdbjq.cn/Article/details/gjhdsiifz.sHtML

C#:   e.Message;  e.StackTrace
来源：http://wap.hesvh.cn/Article/details/glfanmgbf.sHtML

[H09] 带错误码的异常
来源：http://read.share.zdbjq.cn/Article/details/glyurizfd.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mobile.hesvh.cn/Article/details/gifdjhblj.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://blog.hesvh.cn/Article/details/gmjcynjsm.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.share.fehbvm.com/Article/details/gsdptzshm.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mobile.zdbjq.cn/Article/details/gxmexxawe.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mobile.fehbvm.com/Article/details/gifvzranc.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.m.share.fehbvm.com/Article/details/grjtdrgos.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.m.share.zdbjq.cn/Article/details/gwcybejjn.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://3g.hesvh.cn/Article/details/gkkiyaytf.sHtML

[H10] 资源自动释放
来源：http://www.share.fehbvm.com/Article/details/gygbyyexv.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.blog.fehbvm.com/Article/details/gtenndmro.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wap.fehbvm.com/Article/details/gctzjvdcw.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.zdbjq.cn/Article/details/gqjfftiij.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.zdbjq.cn/Article/details/gyityospq.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mobile.fehbvm.com/Article/details/gkowkpwhv.sHtML

Go:   defer f.Close()
来源：http://www.m.share.fehbvm.com/Article/details/gamphqrtn.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.m.share.hesvh.cn/Article/details/gpyglghrf.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gvsiwmcbn.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gfkwepnzq.sHtML

I. 正则表达式
来源：http://read.share.fehbvm.com/Article/details/gnastvqob.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gfhwcxjlz.sHtML

[I01] 判断是否匹配
来源：http://mobile.zdbjq.cn/Article/details/glsoaigst.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://3g.zdbjq.cn/Article/details/gyctluuis.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://3g.fehbvm.com/Article/details/gvkbaenry.sHtML

JS:   /\d+/.test(s)
来源：http://www.blog.hesvh.cn/Article/details/gecqrggsa.sHtML

TS:   /\d+/.test(s)
来源：http://m.share.fehbvm.com/Article/details/grdkgytvj.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wap.hesvh.cn/Article/details/gdqilgvkz.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://m.share.fehbvm.com/Article/details/gfmfhoqzg.sHtML

Ruby: s.match?(/\d+/)
来源：http://read.share.zdbjq.cn/Article/details/gemkeylxm.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.blog.hesvh.cn/Article/details/gzhbbfxjk.sHtML

[I02] 提取所有匹配
来源：http://baike.zdbjq.cn/Article/details/gvlcsflqh.sHtML

Py:   re.findall(r"\d+", s)
来源：http://baike.hesvh.cn/Article/details/gerkyeqot.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://baike.fehbvm.com/Article/details/gniwmblnc.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://blog.hesvh.cn/Article/details/gnzmwryro.sHtML

TS:   s.match(/\d+/g)
来源：http://3g.hesvh.cn/Article/details/gusvylrsd.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://m.share.hesvh.cn/Article/details/gsjkokldd.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://read.share.hesvh.cn/Article/details/gqcjxspib.sHtML

Ruby: s.scan(/\d+/)
来源：http://read.share.hesvh.cn/Article/details/gxcdvwlba.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://read.share.hesvh.cn/Article/details/gtconesvs.sHtML

[I03] 提取捕获分组
来源：http://3g.zdbjq.cn/Article/details/gxsibpfwq.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://baike.zdbjq.cn/Article/details/gpmonogyi.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mobile.fehbvm.com/Article/details/gfnbneexk.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.blog.hesvh.cn/Article/details/gqcfjokan.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wap.hesvh.cn/Article/details/gavmoqsaa.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.m.share.zdbjq.cn/Article/details/gsyolbvly.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.m.share.zdbjq.cn/Article/details/gzxddpsly.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://blog.hesvh.cn/Article/details/gpkcquqbx.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.share.fehbvm.com/Article/details/guhyekoaw.sHtML

[I04] 正则替换
来源：http://mobile.zdbjq.cn/Article/details/gexfnmkgk.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://m.share.fehbvm.com/Article/details/gczgipkcw.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://3g.hesvh.cn/Article/details/gtinyfqzc.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://mobile.zdbjq.cn/Article/details/gsknfplki.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://wap.fehbvm.com/Article/details/gtmikqtet.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.m.share.zdbjq.cn/Article/details/guiizjudg.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.share.fehbvm.com/Article/details/gmbyderac.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://read.share.fehbvm.com/Article/details/gcvzmvwpl.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://3g.fehbvm.com/Article/details/gcgcstuya.sHtML

[I05] 按正则拆分
来源：http://wap.zdbjq.cn/Article/details/gthqpbdjb.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://mobile.hesvh.cn/Article/details/glpyfaxze.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://blog.fehbvm.com/Article/details/gzasjzglp.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://mobile.fehbvm.com/Article/details/gspdvyvga.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://wap.fehbvm.com/Article/details/ghyivpbbg.sHtML

Java: s.split("\\s*,\\s*")
来源：http://blog.zdbjq.cn/Article/details/gzrdpqzqi.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.blog.hesvh.cn/Article/details/gzznlakhc.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://baike.fehbvm.com/Article/details/ghdegvlkg.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://m.share.fehbvm.com/Article/details/ghbyqmmvv.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.m.share.fehbvm.com/Article/details/gqzzhwxec.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://mobile.hesvh.cn/Article/details/gyilfamfp.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://read.share.zdbjq.cn/Article/details/givfyoubt.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.fehbvm.com/Article/details/golyhsqpm.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.fehbvm.com/Article/details/geafysjxz.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://read.share.hesvh.cn/Article/details/grcdahvwc.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wap.hesvh.cn/Article/details/gjdnnifti.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://3g.fehbvm.com/Article/details/gulvprlxa.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.share.zdbjq.cn/Article/details/ghssnxoea.sHtML

[I07] 忽略大小写与多行模式
来源：http://mobile.hesvh.cn/Article/details/govobqmah.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://m.share.hesvh.cn/Article/details/gqqvgkbyr.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://3g.hesvh.cn/Article/details/gqqifywvq.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://m.share.zdbjq.cn/Article/details/gjuazkhma.sHtML

TS:   /error/gim
来源：http://www.blog.fehbvm.com/Article/details/geixucwaa.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://read.share.hesvh.cn/Article/details/grszoxjei.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.share.zdbjq.cn/Article/details/gpbojmfyt.sHtML

Ruby: s.scan(/error/i)
来源：http://www.m.share.fehbvm.com/Article/details/gvrniwzfh.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://m.share.zdbjq.cn/Article/details/gvvitrfyo.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.m.share.zdbjq.cn/Article/details/grustvgkn.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://blog.zdbjq.cn/Article/details/gmxhvyjnt.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mobile.fehbvm.com/Article/details/gdyweccol.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.fehbvm.com/Article/details/ggxvzzhlx.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.fehbvm.com/Article/details/gpqflzkeu.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://baike.fehbvm.com/Article/details/ghsbkwntn.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://mobile.hesvh.cn/Article/details/gckypebac.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wap.hesvh.cn/Article/details/gutycsgct.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.m.share.hesvh.cn/Article/details/gwxrvvymx.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/ggmnkmnmf.sHtML

J. 日期与时间
来源：http://blog.zdbjq.cn/Article/details/goxazykev.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gqiwikmgz.sHtML

[J01] 获取当前时间
来源：http://blog.fehbvm.com/Article/details/gcncepogf.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://wap.hesvh.cn/Article/details/gxacpneas.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://read.share.zdbjq.cn/Article/details/gqdofxddi.sHtML

JS:   new Date();  Date.now()
来源：http://3g.fehbvm.com/Article/details/gbbvtiqhk.sHtML

TS:   new Date();  Date.now()
来源：http://www.share.hesvh.cn/Article/details/ghuudumee.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.share.fehbvm.com/Article/details/gdoozqous.sHtML

Go:   time.Now()
来源：http://www.share.fehbvm.com/Article/details/gascrplvc.sHtML

Ruby: Time.now
来源：http://mobile.fehbvm.com/Article/details/gzfusngau.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.m.share.hesvh.cn/Article/details/gftnirpcg.sHtML

[J02] 格式化输出
来源：http://www.blog.zdbjq.cn/Article/details/gtpdeutdi.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.zdbjq.cn/Article/details/ghayarocg.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mobile.zdbjq.cn/Article/details/gqmcjuref.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://blog.hesvh.cn/Article/details/guhvceere.sHtML

TS:   d.toISOString()
来源：http://www.blog.fehbvm.com/Article/details/gvxtgrwgm.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.m.share.fehbvm.com/Article/details/ggugjzzqa.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://blog.zdbjq.cn/Article/details/gtrpjubvk.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.zdbjq.cn/Article/details/gmakzmyej.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://read.share.fehbvm.com/Article/details/gpyygoqtp.sHtML

[J03] 字符串解析为日期
来源：http://3g.fehbvm.com/Article/details/gssyggtck.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://3g.zdbjq.cn/Article/details/gdctzwsfn.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://read.share.hesvh.cn/Article/details/gdrgnqzmf.sHtML

JS:   new Date("2024-01-02")
来源：http://read.share.zdbjq.cn/Article/details/grjzsdcqb.sHtML

TS:   new Date("2024-01-02")
来源：http://www.blog.zdbjq.cn/Article/details/gjiiaxmaj.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://3g.zdbjq.cn/Article/details/gqsiywkzy.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.m.share.hesvh.cn/Article/details/gdxwgnxpt.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://3g.zdbjq.cn/Article/details/gbnsyhrkw.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://baike.fehbvm.com/Article/details/gosniyigv.sHtML

[J04] 时间戳与日期互转
来源：http://blog.zdbjq.cn/Article/details/gegstrkyl.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://m.share.fehbvm.com/Article/details/guirohtoj.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://mobile.fehbvm.com/Article/details/gzowzwxzn.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://wap.fehbvm.com/Article/details/gnprqsgbh.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://read.share.hesvh.cn/Article/details/gsclwivbq.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://blog.hesvh.cn/Article/details/glkzwczve.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://read.share.hesvh.cn/Article/details/gzoohtpui.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://3g.zdbjq.cn/Article/details/gjhwqaigv.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://blog.fehbvm.com/Article/details/ggnmzvydq.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.m.share.zdbjq.cn/Article/details/gzlziqxwx.sHtML

Py:   now + timedelta(days=7)
来源：http://3g.fehbvm.com/Article/details/geijaazxb.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://baike.hesvh.cn/Article/details/goldvmref.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.fehbvm.com/Article/details/glarpwvuw.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.fehbvm.com/Article/details/gbhgnvftw.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://mobile.hesvh.cn/Article/details/ghjuoyjri.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://wap.zdbjq.cn/Article/details/gjddfndvk.sHtML

Ruby: Time.now + 7 * 86400
来源：http://3g.fehbvm.com/Article/details/ghugboznw.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.blog.fehbvm.com/Article/details/gjkblylfo.sHtML

[J06] 计算两时间之差
来源：http://wap.hesvh.cn/Article/details/gmlozlchy.sHtML

Py:   (end - start).total_seconds()
来源：http://read.share.zdbjq.cn/Article/details/gpflfvzzb.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.share.zdbjq.cn/Article/details/giverrpwn.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.share.fehbvm.com/Article/details/gzoqmjrke.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://3g.hesvh.cn/Article/details/grwsohuni.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://blog.fehbvm.com/Article/details/gphelfpzt.sHtML

Go:   end.Sub(start).Hours()
来源：http://mobile.hesvh.cn/Article/details/gxhbwqryd.sHtML

Ruby: end - start                 # 返回秒数
来源：http://mobile.hesvh.cn/Article/details/gbjnuwkwo.sHtML

C#:   (end - start).TotalSeconds
来源：http://baike.fehbvm.com/Article/details/ggzvlecnd.sHtML

[J07] 比较两个日期
来源：http://m.share.hesvh.cn/Article/details/glfriqxjz.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://mobile.zdbjq.cn/Article/details/gasoerjmg.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://blog.fehbvm.com/Article/details/gwfbrouiu.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://blog.zdbjq.cn/Article/details/glzcgwzdm.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://m.share.zdbjq.cn/Article/details/gpnbrgolc.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://read.share.hesvh.cn/Article/details/gfzczhxtk.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://mobile.hesvh.cn/Article/details/geglcahjk.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://wap.zdbjq.cn/Article/details/gshzsuxwg.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://m.share.zdbjq.cn/Article/details/gmcnwbzco.sHtML

[J08] 提取年月日与星期
来源：http://www.share.fehbvm.com/Article/details/gwaphwxfv.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://baike.hesvh.cn/Article/details/gntmuljuq.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mobile.fehbvm.com/Article/details/gcqrhucjn.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.share.fehbvm.com/Article/details/guvdnzcst.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://wap.hesvh.cn/Article/details/gadremjhy.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.blog.hesvh.cn/Article/details/gsqrhgkkl.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://baike.hesvh.cn/Article/details/gkwjvvnmx.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.m.share.hesvh.cn/Article/details/gyrhqdvwv.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://3g.fehbvm.com/Article/details/gprfdpppr.sHtML

[J09] 时区处理
来源：http://baike.fehbvm.com/Article/details/gghnakwku.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://read.share.zdbjq.cn/Article/details/gnapawaqr.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://3g.hesvh.cn/Article/details/gunvlvlgr.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.hesvh.cn/Article/details/grbagdfpk.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.zdbjq.cn/Article/details/ggnhwxwhq.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mobile.fehbvm.com/Article/details/gspwqjsen.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://3g.zdbjq.cn/Article/details/gpsxmqnho.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.blog.hesvh.cn/Article/details/gfksrkkdi.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://read.share.fehbvm.com/Article/details/gqqtfkblu.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.m.share.hesvh.cn/Article/details/ggpxcuaom.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://read.share.fehbvm.com/Article/details/ghkobsivv.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mobile.hesvh.cn/Article/details/ghvcatdeb.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://blog.hesvh.cn/Article/details/gsvswyyqj.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://blog.fehbvm.com/Article/details/gzhbtwvnd.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.share.hesvh.cn/Article/details/gxaepvhoz.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://m.share.fehbvm.com/Article/details/gmaidnuic.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://m.share.zdbjq.cn/Article/details/gugakgipj.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://3g.zdbjq.cn/Article/details/gbvrpfuty.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/glnjdcewo.sHtML

K. JSON 与序列化
来源：http://read.share.hesvh.cn/Article/details/gfhtpcnoc.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gwmdvyvmm.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.share.zdbjq.cn/Article/details/gszcmkmzv.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.m.share.zdbjq.cn/Article/details/gloadfqyd.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mobile.fehbvm.com/Article/details/gmptjbbcs.sHtML

JS:   JSON.stringify(obj)
来源：http://read.share.zdbjq.cn/Article/details/gisxodbgq.sHtML

TS:   JSON.stringify(obj)
来源：http://www.share.hesvh.cn/Article/details/gsjusikzm.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.blog.hesvh.cn/Article/details/gbgpqevtt.sHtML

Go:   json.Marshal(obj)
来源：http://www.blog.hesvh.cn/Article/details/gwujgazzf.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://m.share.fehbvm.com/Article/details/gdzeokanf.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://m.share.hesvh.cn/Article/details/gjmzsvbix.sHtML

[K02] JSON 字符串转对象
来源：http://blog.hesvh.cn/Article/details/grpcxsozm.sHtML

Py:   json.loads(s)
来源：http://3g.hesvh.cn/Article/details/galbcjpst.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://read.share.fehbvm.com/Article/details/gbhankwwg.sHtML

JS:   JSON.parse(s)
来源：http://3g.fehbvm.com/Article/details/ghuylqrjw.sHtML

TS:   JSON.parse(s)
来源：http://m.share.hesvh.cn/Article/details/gvvvfwsxx.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://read.share.hesvh.cn/Article/details/grkukhfhr.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://blog.fehbvm.com/Article/details/gyoggtfuy.sHtML

Ruby: JSON.parse(s)
来源：http://mobile.hesvh.cn/Article/details/gkaponhhg.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.share.zdbjq.cn/Article/details/gzhvquxpv.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.m.share.zdbjq.cn/Article/details/gdbugietr.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://blog.fehbvm.com/Article/details/guwypcivz.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.zdbjq.cn/Article/details/gflrvuypo.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.share.hesvh.cn/Article/details/gbhogwtpw.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.share.fehbvm.com/Article/details/gvzqavrvy.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://m.share.hesvh.cn/Article/details/gerxukorr.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.blog.hesvh.cn/Article/details/grgpdwcqs.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://m.share.fehbvm.com/Article/details/gkuadglcs.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://blog.hesvh.cn/Article/details/gdsafmxwf.sHtML

[K04] 读取 JSON 文件
来源：http://www.share.fehbvm.com/Article/details/gjblvsyfm.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.blog.fehbvm.com/Article/details/ghyxahoid.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.blog.hesvh.cn/Article/details/gjlbefpyp.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.zdbjq.cn/Article/details/gssdegvqe.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.hesvh.cn/Article/details/gyjsumojh.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://3g.fehbvm.com/Article/details/gsvfczznd.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://blog.zdbjq.cn/Article/details/gobkvddnt.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://m.share.zdbjq.cn/Article/details/gkxongbnc.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.m.share.hesvh.cn/Article/details/gkyyhuvte.sHtML

[K05] 深拷贝对象
来源：http://www.m.share.fehbvm.com/Article/details/gvzasoczz.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.share.zdbjq.cn/Article/details/gzhoosjro.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.share.fehbvm.com/Article/details/gfgvtjmkf.sHtML

JS:   structuredClone(obj)
来源：http://wap.hesvh.cn/Article/details/gcyhbqyye.sHtML

TS:   structuredClone(obj)
来源：http://baike.hesvh.cn/Article/details/gxbtvxudo.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.share.zdbjq.cn/Article/details/gmuwylfmo.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.m.share.hesvh.cn/Article/details/gnhsugotk.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.share.zdbjq.cn/Article/details/gobyawfmw.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://blog.zdbjq.cn/Article/details/glumlxule.sHtML

[K06] 解析 URL 查询串
来源：http://3g.fehbvm.com/Article/details/gltxrqagy.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://m.share.hesvh.cn/Article/details/gupyorseh.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://m.share.hesvh.cn/Article/details/gbqlpveqc.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.fehbvm.com/Article/details/ggkhzmvop.sHtML


<!-- 参考信息 -->