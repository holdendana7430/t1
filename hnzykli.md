代发 wailian999

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.fehbvm.com/Article/details/gjreceyoq.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.zdbjq.cn/Article/details/gcfriiwjf.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.fehbvm.com/Article/details/guqjtuuxu.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.fehbvm.com/Article/details/gpuiorfvx.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.fehbvm.com/Article/details/gnpmbyqcf.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.share.zdbjq.cn/Article/details/gnonivqcd.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.fehbvm.com/Article/details/gdxrspuyr.sHtML

[H02] finally / ensure 收尾
来源：http://blog.hesvh.cn/Article/details/gcdebiyjy.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://mobile.hesvh.cn/Article/details/giuuegkgs.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/ggqvlbsow.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/gmewyyyuv.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.hesvh.cn/Article/details/gjojgzcrx.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.fehbvm.com/Article/details/gfxyskuaq.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.zdbjq.cn/Article/details/gyofnxdnj.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.share.fehbvm.com/Article/details/ggirkfapt.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://3g.hesvh.cn/Article/details/grmufjxuv.sHtML

[H03] 主动抛出异常
来源：http://m.share.hesvh.cn/Article/details/gwknkoajb.sHtML

Py:   raise ValueError("错误信息")
来源：http://baike.fehbvm.com/Article/details/gncbeordm.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.blog.fehbvm.com/Article/details/gqbkdnqfs.sHtML

JS:   throw new Error("错误信息");
来源：http://www.blog.fehbvm.com/Article/details/gtaleawxz.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.hesvh.cn/Article/details/guffucgyg.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/gmiyuxncg.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wap.fehbvm.com/Article/details/gtavjyxrq.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://m.share.fehbvm.com/Article/details/gmlsqbhbl.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.share.hesvh.cn/Article/details/gnksyicsw.sHtML

[H04] 自定义异常类型
来源：http://www.blog.zdbjq.cn/Article/details/gfpxmnovr.sHtML

Py:   class MyError(Exception): pass
来源：http://www.blog.hesvh.cn/Article/details/ghtbykieo.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.share.fehbvm.com/Article/details/gfxdpiaqe.sHtML

JS:   class MyError extends Error {}
来源：http://m.share.fehbvm.com/Article/details/glebnxaxg.sHtML

TS:   class MyError extends Error {}
来源：http://www.blog.hesvh.cn/Article/details/grmezvsvb.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.blog.fehbvm.com/Article/details/grbmezouh.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://baike.hesvh.cn/Article/details/gcaytxxfe.sHtML

Ruby: class MyError < StandardError; end
来源：http://blog.hesvh.cn/Article/details/gekbrfvge.sHtML

C#:   class MyException : Exception {}
来源：http://www.share.hesvh.cn/Article/details/gxiwgijyj.sHtML

[H05] 捕获特定类型
来源：http://3g.hesvh.cn/Article/details/gnsymyfcu.sHtML

Py:   except ValueError as e:
来源：http://www.share.hesvh.cn/Article/details/gmtddzgii.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.share.hesvh.cn/Article/details/giqpjfppq.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://wap.zdbjq.cn/Article/details/gmgrwujhf.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://blog.zdbjq.cn/Article/details/gkpzjvbie.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://blog.fehbvm.com/Article/details/gpnmpugej.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mobile.zdbjq.cn/Article/details/glhbewbag.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.m.share.hesvh.cn/Article/details/gfcltpjti.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mobile.zdbjq.cn/Article/details/gdwpfvvjo.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.share.fehbvm.com/Article/details/gbwhcswyx.sHtML

Py:   value = d.get("k") or default
来源：http://blog.zdbjq.cn/Article/details/gorvtnliv.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://baike.fehbvm.com/Article/details/gmnnqhhcn.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.blog.zdbjq.cn/Article/details/gjckjhjou.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://mobile.zdbjq.cn/Article/details/gquqefzhf.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.m.share.zdbjq.cn/Article/details/gisvlqaol.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://blog.fehbvm.com/Article/details/ghbejafmm.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.m.share.zdbjq.cn/Article/details/gtawpkijf.sHtML

C#:   obj?.A?.B ?? default
来源：http://wap.fehbvm.com/Article/details/gbxzhtekh.sHtML

[H07] 断言
来源：http://read.share.zdbjq.cn/Article/details/giaqreyyd.sHtML

Py:   assert x > 0, "必须为正"
来源：http://read.share.hesvh.cn/Article/details/gfnfkniav.sHtML

PHP:  assert($x > 0);
来源：http://m.share.hesvh.cn/Article/details/ghqasitkr.sHtML

JS:   console.assert(x > 0);
来源：http://www.m.share.fehbvm.com/Article/details/gvumxsjan.sHtML

TS:   console.assert(x > 0);
来源：http://wap.hesvh.cn/Article/details/gvqdvckbv.sHtML

Java: assert x > 0 : "必须为正";
来源：http://3g.hesvh.cn/Article/details/gtmjuachp.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://m.share.fehbvm.com/Article/details/gdnvjesdc.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://baike.fehbvm.com/Article/details/gbrrdvjsm.sHtML

C#:   Debug.Assert(x > 0);
来源：http://baike.hesvh.cn/Article/details/gkasorwei.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.blog.hesvh.cn/Article/details/gfygoiboj.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://m.share.zdbjq.cn/Article/details/gregnwyud.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://read.share.zdbjq.cn/Article/details/giqthprbj.sHtML

JS:   e.message;  e.stack
来源：http://www.blog.zdbjq.cn/Article/details/gjjbnxetq.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.share.zdbjq.cn/Article/details/gbkzxvvsq.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.blog.fehbvm.com/Article/details/glxuvvhal.sHtML

Go:   err.Error()
来源：http://3g.zdbjq.cn/Article/details/gavdqydys.sHtML

Ruby: e.message;  e.backtrace
来源：http://m.share.zdbjq.cn/Article/details/ggooymazp.sHtML

C#:   e.Message;  e.StackTrace
来源：http://mobile.hesvh.cn/Article/details/glcqbfqur.sHtML

[H09] 带错误码的异常
来源：http://www.blog.fehbvm.com/Article/details/gmrkqqtqj.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://3g.zdbjq.cn/Article/details/gbyulhbxn.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://wap.zdbjq.cn/Article/details/gkxzrzvya.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.m.share.hesvh.cn/Article/details/gxpnlhang.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wap.hesvh.cn/Article/details/ghnwnjekn.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.share.hesvh.cn/Article/details/glcovxbtq.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.share.zdbjq.cn/Article/details/gehjteihb.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.m.share.zdbjq.cn/Article/details/gitlpwzar.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.m.share.fehbvm.com/Article/details/gndnlvgdd.sHtML

[H10] 资源自动释放
来源：http://www.share.fehbvm.com/Article/details/gsknmegso.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://3g.hesvh.cn/Article/details/gqhzrqrrn.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://m.share.hesvh.cn/Article/details/ghxuwhsvh.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.fehbvm.com/Article/details/gklmqgzxv.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.zdbjq.cn/Article/details/gvwwjchce.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://m.share.zdbjq.cn/Article/details/geidfybuq.sHtML

Go:   defer f.Close()
来源：http://mobile.zdbjq.cn/Article/details/gcevfiavp.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mobile.fehbvm.com/Article/details/gsvgplznk.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gdvsceupd.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/grvzzcymo.sHtML

I. 正则表达式
来源：http://blog.hesvh.cn/Article/details/gnyfhfasn.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/ghsowvikm.sHtML

[I01] 判断是否匹配
来源：http://3g.hesvh.cn/Article/details/gtfizkhbf.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.m.share.zdbjq.cn/Article/details/gwgelasbz.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://3g.zdbjq.cn/Article/details/gaanlrqbz.sHtML

JS:   /\d+/.test(s)
来源：http://www.share.zdbjq.cn/Article/details/gikhnkacr.sHtML

TS:   /\d+/.test(s)
来源：http://3g.hesvh.cn/Article/details/gmehxycvh.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wap.fehbvm.com/Article/details/gszsixgqs.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://m.share.zdbjq.cn/Article/details/glnudonlh.sHtML

Ruby: s.match?(/\d+/)
来源：http://baike.fehbvm.com/Article/details/gkdzntoet.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.share.fehbvm.com/Article/details/gtrqvflds.sHtML

[I02] 提取所有匹配
来源：http://www.share.zdbjq.cn/Article/details/gnrucalrm.sHtML

Py:   re.findall(r"\d+", s)
来源：http://m.share.hesvh.cn/Article/details/gcgeklica.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://blog.hesvh.cn/Article/details/gbwgppplw.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://3g.zdbjq.cn/Article/details/gbmtglzsl.sHtML

TS:   s.match(/\d+/g)
来源：http://baike.zdbjq.cn/Article/details/gkgyyotjx.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://3g.fehbvm.com/Article/details/gwzpirxqj.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.m.share.fehbvm.com/Article/details/gahcuavzq.sHtML

Ruby: s.scan(/\d+/)
来源：http://3g.zdbjq.cn/Article/details/gdqowmnww.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://baike.hesvh.cn/Article/details/gehcfarqh.sHtML

[I03] 提取捕获分组
来源：http://blog.hesvh.cn/Article/details/gatomnlip.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mobile.zdbjq.cn/Article/details/giznpchib.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.share.fehbvm.com/Article/details/gntgnzaol.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://blog.fehbvm.com/Article/details/gokfamvow.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://read.share.hesvh.cn/Article/details/gcglzgwkf.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://baike.zdbjq.cn/Article/details/gfeusvihh.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wap.hesvh.cn/Article/details/gquafmuwe.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://m.share.fehbvm.com/Article/details/grresqsgh.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://mobile.zdbjq.cn/Article/details/gjqkwwqez.sHtML

[I04] 正则替换
来源：http://blog.zdbjq.cn/Article/details/gsttbndwv.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://mobile.fehbvm.com/Article/details/gchusubsc.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://m.share.zdbjq.cn/Article/details/gijjngscy.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://mobile.fehbvm.com/Article/details/gpnglmexp.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://blog.zdbjq.cn/Article/details/gpexnvbng.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://read.share.hesvh.cn/Article/details/goiimimxx.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://read.share.zdbjq.cn/Article/details/gzujbxnsx.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://wap.fehbvm.com/Article/details/gdnmrmnxm.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://m.share.zdbjq.cn/Article/details/gvidorcgp.sHtML

[I05] 按正则拆分
来源：http://www.m.share.hesvh.cn/Article/details/gqwmqdkca.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.share.hesvh.cn/Article/details/gonlosiyt.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.share.zdbjq.cn/Article/details/gkauwycsq.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://read.share.zdbjq.cn/Article/details/gprscywzw.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.m.share.hesvh.cn/Article/details/gboccdowx.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.blog.fehbvm.com/Article/details/gsnfyinap.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://mobile.hesvh.cn/Article/details/gbjogjnkp.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://blog.hesvh.cn/Article/details/gfrwcamaa.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wap.zdbjq.cn/Article/details/groglhhlp.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.blog.zdbjq.cn/Article/details/garcalyvd.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.blog.hesvh.cn/Article/details/gkydqggxh.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.m.share.hesvh.cn/Article/details/gvbgieoyh.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.fehbvm.com/Article/details/gxdtpfbsk.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.zdbjq.cn/Article/details/gphoxmetw.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://blog.fehbvm.com/Article/details/gjwkcvwvz.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://3g.fehbvm.com/Article/details/gvsmykimx.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wap.hesvh.cn/Article/details/giqcipute.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://baike.zdbjq.cn/Article/details/gadaxsqed.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.share.fehbvm.com/Article/details/gkseocune.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://read.share.zdbjq.cn/Article/details/gvfwtioxu.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mobile.hesvh.cn/Article/details/gzkwsfvaj.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mobile.hesvh.cn/Article/details/gwojxljbf.sHtML

TS:   /error/gim
来源：http://read.share.hesvh.cn/Article/details/gnestgaxz.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://read.share.zdbjq.cn/Article/details/glkgkixks.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wap.fehbvm.com/Article/details/gsurofiae.sHtML

Ruby: s.scan(/error/i)
来源：http://www.m.share.zdbjq.cn/Article/details/gtcmowvzz.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://read.share.fehbvm.com/Article/details/gujxkefqj.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://blog.fehbvm.com/Article/details/gnihbkkzh.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://baike.zdbjq.cn/Article/details/gpnsgcurq.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.blog.zdbjq.cn/Article/details/gvbzhpleu.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.hesvh.cn/Article/details/gqpggxmda.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.zdbjq.cn/Article/details/grvsntlbp.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://m.share.zdbjq.cn/Article/details/gbxggvgaw.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://read.share.fehbvm.com/Article/details/ghamwtywp.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://baike.zdbjq.cn/Article/details/gbosqauqp.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://blog.hesvh.cn/Article/details/gwkvjrksi.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gyzypzpof.sHtML

J. 日期与时间
来源：http://blog.zdbjq.cn/Article/details/getnvojbs.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/glbclwyfe.sHtML

[J01] 获取当前时间
来源：http://www.blog.hesvh.cn/Article/details/gvofendgg.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://3g.hesvh.cn/Article/details/gzbdfynbd.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mobile.hesvh.cn/Article/details/gjnxxowdg.sHtML

JS:   new Date();  Date.now()
来源：http://3g.hesvh.cn/Article/details/gzbkbzxpn.sHtML

TS:   new Date();  Date.now()
来源：http://3g.fehbvm.com/Article/details/gnrllmdlp.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://m.share.hesvh.cn/Article/details/gdlqpcznw.sHtML

Go:   time.Now()
来源：http://wap.zdbjq.cn/Article/details/gzbjudoze.sHtML

Ruby: Time.now
来源：http://wap.zdbjq.cn/Article/details/gpzreopgb.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://read.share.zdbjq.cn/Article/details/gibojmhru.sHtML

[J02] 格式化输出
来源：http://www.share.hesvh.cn/Article/details/gavayyuwz.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.hesvh.cn/Article/details/gnjjcpytr.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.blog.zdbjq.cn/Article/details/gmlireezh.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://baike.fehbvm.com/Article/details/gsdxopjvj.sHtML

TS:   d.toISOString()
来源：http://www.m.share.fehbvm.com/Article/details/geepcllup.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://blog.hesvh.cn/Article/details/gfgicxmxj.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://3g.fehbvm.com/Article/details/gcwdlujwo.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.zdbjq.cn/Article/details/gvgduzupj.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.m.share.fehbvm.com/Article/details/gxvwamrkc.sHtML

[J03] 字符串解析为日期
来源：http://www.share.hesvh.cn/Article/details/glarbrgmy.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://mobile.fehbvm.com/Article/details/gpnlehahl.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://read.share.zdbjq.cn/Article/details/gjbfasbhc.sHtML

JS:   new Date("2024-01-02")
来源：http://read.share.zdbjq.cn/Article/details/gtqvpvwxm.sHtML

TS:   new Date("2024-01-02")
来源：http://www.blog.zdbjq.cn/Article/details/gbxknqtpj.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://mobile.fehbvm.com/Article/details/gbyqsibwa.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wap.zdbjq.cn/Article/details/gnpfrgzru.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://blog.zdbjq.cn/Article/details/gclrktxch.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.blog.fehbvm.com/Article/details/gapjamhwe.sHtML

[J04] 时间戳与日期互转
来源：http://www.blog.zdbjq.cn/Article/details/gnxmqakaz.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://blog.fehbvm.com/Article/details/gbrsauxrw.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.blog.zdbjq.cn/Article/details/gzjautxjs.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.m.share.zdbjq.cn/Article/details/gftunyvdl.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://read.share.zdbjq.cn/Article/details/gvnphavqy.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.m.share.fehbvm.com/Article/details/grajgzcnv.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.share.hesvh.cn/Article/details/gvmyslneh.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://m.share.fehbvm.com/Article/details/gbnrzjigv.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://blog.fehbvm.com/Article/details/gilftmloc.sHtML

[J05] 时间加减（加 7 天）
来源：http://read.share.hesvh.cn/Article/details/gifxuvonl.sHtML

Py:   now + timedelta(days=7)
来源：http://www.share.zdbjq.cn/Article/details/grjofvmlw.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.blog.hesvh.cn/Article/details/gsrxpxuce.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.fehbvm.com/Article/details/gvnjhydpb.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.hesvh.cn/Article/details/gjrznqune.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://wap.fehbvm.com/Article/details/gprrjzmms.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mobile.zdbjq.cn/Article/details/gukozcemb.sHtML

Ruby: Time.now + 7 * 86400
来源：http://read.share.fehbvm.com/Article/details/glisvhqpr.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://baike.hesvh.cn/Article/details/gdtuqrrnu.sHtML

[J06] 计算两时间之差
来源：http://wap.zdbjq.cn/Article/details/gebztxupa.sHtML

Py:   (end - start).total_seconds()
来源：http://baike.hesvh.cn/Article/details/gjtdifhxi.sHtML

PHP:  $end->diff($start)->days;
来源：http://mobile.zdbjq.cn/Article/details/gyphgsyzq.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.share.zdbjq.cn/Article/details/gubfjippm.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mobile.zdbjq.cn/Article/details/gbeuunwqr.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.m.share.fehbvm.com/Article/details/gkmqoyhkw.sHtML

Go:   end.Sub(start).Hours()
来源：http://baike.zdbjq.cn/Article/details/gvqlglgaa.sHtML

Ruby: end - start                 # 返回秒数
来源：http://blog.zdbjq.cn/Article/details/gdypllnev.sHtML

C#:   (end - start).TotalSeconds
来源：http://wap.zdbjq.cn/Article/details/gfasihkri.sHtML

[J07] 比较两个日期
来源：http://www.share.zdbjq.cn/Article/details/gnjuokxyv.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://read.share.zdbjq.cn/Article/details/gznedunrz.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://mobile.fehbvm.com/Article/details/gqolmmpno.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://baike.fehbvm.com/Article/details/gdymtigkw.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.fehbvm.com/Article/details/gfepvgltm.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://m.share.zdbjq.cn/Article/details/ghkfyxrfc.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://baike.fehbvm.com/Article/details/grmflktaf.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://blog.fehbvm.com/Article/details/ghxuvndep.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.blog.zdbjq.cn/Article/details/gstxyfolr.sHtML

[J08] 提取年月日与星期
来源：http://read.share.hesvh.cn/Article/details/gbgdaqdxj.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.blog.zdbjq.cn/Article/details/ghvrbmkkk.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://read.share.hesvh.cn/Article/details/gelnrqpzh.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.share.hesvh.cn/Article/details/gzqcahbhk.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.share.hesvh.cn/Article/details/gojbkhkjq.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://3g.hesvh.cn/Article/details/gyitejpzh.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://m.share.zdbjq.cn/Article/details/gqfqflppb.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.share.hesvh.cn/Article/details/gbcgfjpff.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.blog.hesvh.cn/Article/details/glyrlijru.sHtML

[J09] 时区处理
来源：http://www.share.fehbvm.com/Article/details/glwiaowbf.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.share.hesvh.cn/Article/details/gyjxqmqil.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wap.zdbjq.cn/Article/details/gkxvxsaka.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.fehbvm.com/Article/details/gjsdmdfqa.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.fehbvm.com/Article/details/gkmgqcnqm.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://m.share.zdbjq.cn/Article/details/goyzwscbl.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mobile.zdbjq.cn/Article/details/gkavzocho.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.share.fehbvm.com/Article/details/gplahgngm.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://m.share.fehbvm.com/Article/details/ggczqumvu.sHtML

[J10] 取今天 / 本月第一天
来源：http://wap.hesvh.cn/Article/details/gyqvnskjt.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.blog.zdbjq.cn/Article/details/gmsrgsjva.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wap.zdbjq.cn/Article/details/gpponrjlu.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gpjipvznd.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gxybnrkco.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.share.zdbjq.cn/Article/details/gbcxznmik.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://3g.fehbvm.com/Article/details/gjfsogppf.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mobile.hesvh.cn/Article/details/gfcsecqqv.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.m.share.fehbvm.com/Article/details/gxxcyzbfy.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gghxlmafy.sHtML

K. JSON 与序列化
来源：http://m.share.fehbvm.com/Article/details/godprmxwh.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/genaguzwe.sHtML

[K01] 对象转 JSON 字符串
来源：http://wap.zdbjq.cn/Article/details/gsegbijbi.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://m.share.zdbjq.cn/Article/details/gbbbjwlwy.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://blog.hesvh.cn/Article/details/gqzznisge.sHtML

JS:   JSON.stringify(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gbjpuifjk.sHtML

TS:   JSON.stringify(obj)
来源：http://www.blog.hesvh.cn/Article/details/gbcbrdvkw.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://baike.zdbjq.cn/Article/details/gtgsbzgcy.sHtML

Go:   json.Marshal(obj)
来源：http://m.share.hesvh.cn/Article/details/gscgnqzza.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://blog.zdbjq.cn/Article/details/gayrsskbb.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gckyjbjsr.sHtML

[K02] JSON 字符串转对象
来源：http://blog.hesvh.cn/Article/details/gywazhita.sHtML

Py:   json.loads(s)
来源：http://wap.hesvh.cn/Article/details/gswzgjhdv.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mobile.zdbjq.cn/Article/details/gnultbmuw.sHtML

JS:   JSON.parse(s)
来源：http://blog.zdbjq.cn/Article/details/gjzomdgcu.sHtML

TS:   JSON.parse(s)
来源：http://www.blog.zdbjq.cn/Article/details/govyaxpvr.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.share.zdbjq.cn/Article/details/grvxpgzgx.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://wap.hesvh.cn/Article/details/gjbxeltgj.sHtML

Ruby: JSON.parse(s)
来源：http://m.share.zdbjq.cn/Article/details/grdeyklri.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://3g.fehbvm.com/Article/details/gjhcsjpux.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.m.share.fehbvm.com/Article/details/gyledlsoj.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://m.share.hesvh.cn/Article/details/gmaussbis.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://3g.hesvh.cn/Article/details/gbqspephh.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.share.hesvh.cn/Article/details/gexfffkws.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.share.zdbjq.cn/Article/details/guktfrggb.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://read.share.hesvh.cn/Article/details/gqytzbyag.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.blog.hesvh.cn/Article/details/gheklprip.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://blog.fehbvm.com/Article/details/gwvahkida.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://3g.zdbjq.cn/Article/details/gwlsccouo.sHtML

[K04] 读取 JSON 文件
来源：http://wap.fehbvm.com/Article/details/gyhbsqdhk.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.blog.hesvh.cn/Article/details/gcqiqpusw.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://m.share.zdbjq.cn/Article/details/guareajbi.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.zdbjq.cn/Article/details/glyaqbwby.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.fehbvm.com/Article/details/gryqlhxov.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.m.share.hesvh.cn/Article/details/gboitjciq.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.m.share.fehbvm.com/Article/details/gttchohnv.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://wap.hesvh.cn/Article/details/gbdjofjvh.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://blog.fehbvm.com/Article/details/gqijogvqi.sHtML

[K05] 深拷贝对象
来源：http://www.m.share.zdbjq.cn/Article/details/gwrisxrgz.sHtML

Py:   copy.deepcopy(obj)
来源：http://wap.fehbvm.com/Article/details/gyvzclokp.sHtML

PHP:  unserialize(serialize($obj));
来源：http://mobile.hesvh.cn/Article/details/gxrqvflkz.sHtML

JS:   structuredClone(obj)
来源：http://m.share.fehbvm.com/Article/details/gajxljssk.sHtML

TS:   structuredClone(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gqteefdvv.sHtML


<!-- 参考信息 -->