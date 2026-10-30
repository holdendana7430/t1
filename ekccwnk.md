代发 wailian999

PHP:  get_object_vars($obj);
来源：http://read.share.fanxiaobao.xyz/Article/details/gaocufotx.sHtML

JS:   Object.entries(obj)
来源：http://baike.fanxiaobao.xyz/Article/details/ghnlqftea.sHtML

TS:   Object.entries(obj)
来源：http://m.share.fanxiaobao.xyz/Article/details/gijthkmca.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.fanxiaobao.xyz/Article/details/grtqebqpr.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.fanxiaobao.xyz/Article/details/gmlnscyra.sHtML

Ruby: obj.instance_variables
来源：http://blog.fanxiaobao.xyz/Article/details/gopharhqy.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.fanxiaobao.xyz/Article/details/gtgqsapdz.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gdhaxmvgj.sHtML

H. 异常与错误处理
来源：http://baike.fanxiaobao.xyz/Article/details/gnbxolkmi.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/glgroijbx.sHtML

[H01] try / catch 基础
来源：http://m.share.fanxiaobao.xyz/Article/details/gpbgkfxjo.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.fanxiaobao.xyz/Article/details/guvodnudu.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mobile.fanxiaobao.xyz/Article/details/glyhqmjdy.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gduvtvyqm.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://3g.fanxiaobao.xyz/Article/details/gdkhmxkme.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gzhixetcc.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mobile.fanxiaobao.xyz/Article/details/gsezdjdyk.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsarvzvkf.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.fanxiaobao.xyz/Article/details/goaszfksv.sHtML

[H02] finally / ensure 收尾
来源：http://3g.fanxiaobao.xyz/Article/details/gjmqkylmv.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://baike.fanxiaobao.xyz/Article/details/gwxibrwus.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gkubqxhjm.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggqilrkeq.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gsftljpot.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.fanxiaobao.xyz/Article/details/gmylkefye.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.blog.fanxiaobao.xyz/Article/details/gowkypkml.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.share.fanxiaobao.xyz/Article/details/gwfliulcr.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gtvxvtyqj.sHtML

[H03] 主动抛出异常
来源：http://blog.fanxiaobao.xyz/Article/details/glwdjlzzs.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.share.fanxiaobao.xyz/Article/details/gnaddmxil.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.fanxiaobao.xyz/Article/details/gilmsrbyx.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.fanxiaobao.xyz/Article/details/gpyxmofyb.sHtML

TS:   throw new Error("错误信息");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gclgrbmhy.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://read.share.fanxiaobao.xyz/Article/details/gfbdgyqiq.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://read.share.fanxiaobao.xyz/Article/details/glduhlwql.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://blog.fanxiaobao.xyz/Article/details/gacgsytyq.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gflmcgsch.sHtML

[H04] 自定义异常类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggjofdeqw.sHtML

Py:   class MyError(Exception): pass
来源：http://3g.fanxiaobao.xyz/Article/details/gcwpjwsyn.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqlxtopes.sHtML

JS:   class MyError extends Error {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gufpiropq.sHtML

TS:   class MyError extends Error {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gdctvqogl.sHtML

Java: class MyException extends RuntimeException {}
来源：http://wap.fanxiaobao.xyz/Article/details/gxcocuwai.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxbqxokbm.sHtML

Ruby: class MyError < StandardError; end
来源：http://m.share.fanxiaobao.xyz/Article/details/gxuzvuuex.sHtML

C#:   class MyException : Exception {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gfziexbsc.sHtML

[H05] 捕获特定类型
来源：http://www.share.fanxiaobao.xyz/Article/details/gdlbexpec.sHtML

Py:   except ValueError as e:
来源：http://baike.fanxiaobao.xyz/Article/details/gkiqpxqam.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://m.share.fanxiaobao.xyz/Article/details/gudofzaap.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://3g.fanxiaobao.xyz/Article/details/gupfnehcf.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://wap.fanxiaobao.xyz/Article/details/guoeitilg.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/glahfkrzd.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.share.fanxiaobao.xyz/Article/details/gckmnlamv.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.fanxiaobao.xyz/Article/details/gugzrzxqi.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wap.fanxiaobao.xyz/Article/details/gghcuceze.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcwebagmw.sHtML

Py:   value = d.get("k") or default
来源：http://3g.fanxiaobao.xyz/Article/details/gefacrghs.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://blog.fanxiaobao.xyz/Article/details/goqpxnpgr.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbcncjtna.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://read.share.fanxiaobao.xyz/Article/details/ggkpzajtd.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghlhreizp.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://read.share.fanxiaobao.xyz/Article/details/gjpiseedp.sHtML

Ruby: d&.dig(:a, :b)
来源：http://read.share.fanxiaobao.xyz/Article/details/gozrvppoz.sHtML

C#:   obj?.A?.B ?? default
来源：http://mobile.fanxiaobao.xyz/Article/details/gytlvhjop.sHtML

[H07] 断言
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gixakcdlq.sHtML

Py:   assert x > 0, "必须为正"
来源：http://blog.fanxiaobao.xyz/Article/details/gplvdhlcw.sHtML

PHP:  assert($x > 0);
来源：http://blog.fanxiaobao.xyz/Article/details/ghfcdvspc.sHtML

JS:   console.assert(x > 0);
来源：http://3g.fanxiaobao.xyz/Article/details/godtbpvdq.sHtML

TS:   console.assert(x > 0);
来源：http://read.share.fanxiaobao.xyz/Article/details/gtlytxeqv.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyfmuoqlp.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://3g.fanxiaobao.xyz/Article/details/gizjvjoxg.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://baike.fanxiaobao.xyz/Article/details/gngopwtqv.sHtML

C#:   Debug.Assert(x > 0);
来源：http://mobile.fanxiaobao.xyz/Article/details/gtmfnekua.sHtML

[H08] 获取错误信息与堆栈
来源：http://blog.fanxiaobao.xyz/Article/details/gtlrylclk.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://baike.fanxiaobao.xyz/Article/details/gokbkhsnf.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://baike.fanxiaobao.xyz/Article/details/gltyxnruv.sHtML

JS:   e.message;  e.stack
来源：http://mobile.fanxiaobao.xyz/Article/details/gelkbmika.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.share.fanxiaobao.xyz/Article/details/gugagzooz.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guplxrwcy.sHtML

Go:   err.Error()
来源：http://3g.fanxiaobao.xyz/Article/details/ggostmgey.sHtML

Ruby: e.message;  e.backtrace
来源：http://3g.fanxiaobao.xyz/Article/details/gkndgdgdr.sHtML

C#:   e.Message;  e.StackTrace
来源：http://blog.fanxiaobao.xyz/Article/details/guzhsvtiy.sHtML

[H09] 带错误码的异常
来源：http://3g.fanxiaobao.xyz/Article/details/giozussng.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://m.share.fanxiaobao.xyz/Article/details/gcvjjptcs.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://mobile.fanxiaobao.xyz/Article/details/gkdlcomdj.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://blog.fanxiaobao.xyz/Article/details/ginvtdzah.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://m.share.fanxiaobao.xyz/Article/details/gneiighua.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpbejnbov.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://3g.fanxiaobao.xyz/Article/details/gxudqoqos.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://blog.fanxiaobao.xyz/Article/details/gcmrcwkil.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://3g.fanxiaobao.xyz/Article/details/gqgvnjlci.sHtML

[H10] 资源自动释放
来源：http://blog.fanxiaobao.xyz/Article/details/gmmcgvelu.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzovhvopw.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.share.fanxiaobao.xyz/Article/details/gtkymlngs.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.fanxiaobao.xyz/Article/details/gyntmxjum.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.fanxiaobao.xyz/Article/details/guwxyxriy.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://blog.fanxiaobao.xyz/Article/details/ghzhvepyh.sHtML

Go:   defer f.Close()
来源：http://baike.fanxiaobao.xyz/Article/details/gpuxhtdud.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://baike.fanxiaobao.xyz/Article/details/ggrwapydu.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://m.share.fanxiaobao.xyz/Article/details/gquxazhlz.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gubaayasy.sHtML

I. 正则表达式
来源：http://m.share.fanxiaobao.xyz/Article/details/gvdllkewi.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/giioyvwvt.sHtML

[I01] 判断是否匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpnkhsvhh.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gbiwtgdvi.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://3g.fanxiaobao.xyz/Article/details/gicqgjjoj.sHtML

JS:   /\d+/.test(s)
来源：http://3g.fanxiaobao.xyz/Article/details/ggyonbtgi.sHtML

TS:   /\d+/.test(s)
来源：http://baike.fanxiaobao.xyz/Article/details/gnuxkflit.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://read.share.fanxiaobao.xyz/Article/details/gwfylospm.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gpcskisud.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geikebhmh.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://blog.fanxiaobao.xyz/Article/details/gppbazxsw.sHtML

[I02] 提取所有匹配
来源：http://3g.fanxiaobao.xyz/Article/details/ggnrojjju.sHtML

Py:   re.findall(r"\d+", s)
来源：http://read.share.fanxiaobao.xyz/Article/details/guonmjnjp.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mobile.fanxiaobao.xyz/Article/details/gpdlaugkk.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://m.share.fanxiaobao.xyz/Article/details/gugkqpwxj.sHtML

TS:   s.match(/\d+/g)
来源：http://read.share.fanxiaobao.xyz/Article/details/garyrkoxs.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggjfhftkw.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gwiitrttb.sHtML

Ruby: s.scan(/\d+/)
来源：http://3g.fanxiaobao.xyz/Article/details/gudinkxjt.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.share.fanxiaobao.xyz/Article/details/gctedobgs.sHtML

[I03] 提取捕获分组
来源：http://wap.fanxiaobao.xyz/Article/details/gfjuadpkt.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://read.share.fanxiaobao.xyz/Article/details/ghefizmae.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.blog.fanxiaobao.xyz/Article/details/grppslbcf.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://3g.fanxiaobao.xyz/Article/details/gpyrqsbox.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://blog.fanxiaobao.xyz/Article/details/gwbcaqobq.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://3g.fanxiaobao.xyz/Article/details/gkhejglfq.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wap.fanxiaobao.xyz/Article/details/gifmkxcvx.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.blog.fanxiaobao.xyz/Article/details/geaeqiaeq.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://3g.fanxiaobao.xyz/Article/details/ghntestiv.sHtML

[I04] 正则替换
来源：http://blog.fanxiaobao.xyz/Article/details/gfziaqswk.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdshgcomv.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://read.share.fanxiaobao.xyz/Article/details/gdsxbyzsk.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://wap.fanxiaobao.xyz/Article/details/gqcrfxyak.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://blog.fanxiaobao.xyz/Article/details/ggrwlgyub.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxxbxgfay.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyohvdynt.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://baike.fanxiaobao.xyz/Article/details/gxojgqafv.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://blog.fanxiaobao.xyz/Article/details/ghejfjtoy.sHtML

[I05] 按正则拆分
来源：http://www.blog.fanxiaobao.xyz/Article/details/godxtzlkn.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqdmkdwxs.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://m.share.fanxiaobao.xyz/Article/details/gkacqqgya.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://baike.fanxiaobao.xyz/Article/details/gawxaeuya.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.share.fanxiaobao.xyz/Article/details/gwhzpobyx.sHtML

Java: s.split("\\s*,\\s*")
来源：http://read.share.fanxiaobao.xyz/Article/details/gombwsvsr.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wap.fanxiaobao.xyz/Article/details/gnbpcgrks.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://wap.fanxiaobao.xyz/Article/details/gdefiwgrv.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://baike.fanxiaobao.xyz/Article/details/grlumjaoo.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtfwojbzy.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wap.fanxiaobao.xyz/Article/details/gqzmnwpns.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://m.share.fanxiaobao.xyz/Article/details/gssteawqf.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.fanxiaobao.xyz/Article/details/gmzakggdl.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.fanxiaobao.xyz/Article/details/gdabfimdz.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wap.fanxiaobao.xyz/Article/details/gckwhwllw.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://baike.fanxiaobao.xyz/Article/details/gxcbvtlif.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.share.fanxiaobao.xyz/Article/details/gggsqpxsq.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://baike.fanxiaobao.xyz/Article/details/gzzagenvk.sHtML

[I07] 忽略大小写与多行模式
来源：http://wap.fanxiaobao.xyz/Article/details/gyyedrdqn.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://baike.fanxiaobao.xyz/Article/details/gwlzwpboo.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdiqhbrly.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gchcdkgvy.sHtML

TS:   /error/gim
来源：http://3g.fanxiaobao.xyz/Article/details/gvwhomviu.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://read.share.fanxiaobao.xyz/Article/details/galwmqvoy.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://baike.fanxiaobao.xyz/Article/details/gutqvvmdw.sHtML

Ruby: s.scan(/error/i)
来源：http://m.share.fanxiaobao.xyz/Article/details/gkjmhybeu.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goulsksud.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://baike.fanxiaobao.xyz/Article/details/gsipzmpqw.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjagnlccr.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://read.share.fanxiaobao.xyz/Article/details/gsmpfptci.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.fanxiaobao.xyz/Article/details/ghfzkznod.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.fanxiaobao.xyz/Article/details/gqqdygdkp.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://mobile.fanxiaobao.xyz/Article/details/ggtnbfuvv.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://mobile.fanxiaobao.xyz/Article/details/gbpkpkbac.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.share.fanxiaobao.xyz/Article/details/gcvrsqqfk.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.share.fanxiaobao.xyz/Article/details/gkurgrkxi.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/girolakcq.sHtML

J. 日期与时间
来源：http://wap.fanxiaobao.xyz/Article/details/gbhxjnnzc.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gegtcrrog.sHtML

[J01] 获取当前时间
来源：http://blog.fanxiaobao.xyz/Article/details/giylfvufw.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://m.share.fanxiaobao.xyz/Article/details/ghmdfkzdp.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://3g.fanxiaobao.xyz/Article/details/gmvjkmirk.sHtML

JS:   new Date();  Date.now()
来源：http://baike.fanxiaobao.xyz/Article/details/gnbllgfgm.sHtML

TS:   new Date();  Date.now()
来源：http://wap.fanxiaobao.xyz/Article/details/gxvfrfmbo.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://baike.fanxiaobao.xyz/Article/details/goltdfdeu.sHtML

Go:   time.Now()
来源：http://blog.fanxiaobao.xyz/Article/details/gidpfubvp.sHtML

Ruby: Time.now
来源：http://m.share.fanxiaobao.xyz/Article/details/gbtkzjszc.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://baike.fanxiaobao.xyz/Article/details/glpxhuptz.sHtML

[J02] 格式化输出
来源：http://baike.fanxiaobao.xyz/Article/details/gcpmmbjrx.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.fanxiaobao.xyz/Article/details/gvxrttzot.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wap.fanxiaobao.xyz/Article/details/gjxtqhkvd.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://blog.fanxiaobao.xyz/Article/details/gkiepueqw.sHtML

TS:   d.toISOString()
来源：http://blog.fanxiaobao.xyz/Article/details/gxxfbjumu.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.share.fanxiaobao.xyz/Article/details/gxqmofeuc.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.share.fanxiaobao.xyz/Article/details/ghqdsoshq.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.fanxiaobao.xyz/Article/details/gricabeal.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggijaxicx.sHtML

[J03] 字符串解析为日期
来源：http://www.blog.fanxiaobao.xyz/Article/details/gttobuove.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://mobile.fanxiaobao.xyz/Article/details/gcrwcqaok.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcklxqxcx.sHtML

JS:   new Date("2024-01-02")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcnfetpuc.sHtML

TS:   new Date("2024-01-02")
来源：http://mobile.fanxiaobao.xyz/Article/details/gvxewfzwv.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://wap.fanxiaobao.xyz/Article/details/gqzoafptp.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.share.fanxiaobao.xyz/Article/details/gmjabqpwx.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://mobile.fanxiaobao.xyz/Article/details/gisdftuag.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://m.share.fanxiaobao.xyz/Article/details/gbqebhqyb.sHtML

[J04] 时间戳与日期互转
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfcjrboze.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://baike.fanxiaobao.xyz/Article/details/gsptjzcno.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://blog.fanxiaobao.xyz/Article/details/gvalhrekl.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://wap.fanxiaobao.xyz/Article/details/gjlsxjyhf.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.share.fanxiaobao.xyz/Article/details/gttmvwhov.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://mobile.fanxiaobao.xyz/Article/details/gbydxiwgs.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wap.fanxiaobao.xyz/Article/details/grehnvdwl.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://baike.fanxiaobao.xyz/Article/details/gbwhczhme.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdzgidiza.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.share.fanxiaobao.xyz/Article/details/gjaduaftl.sHtML

Py:   now + timedelta(days=7)
来源：http://m.share.fanxiaobao.xyz/Article/details/gyjsjdkax.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://m.share.fanxiaobao.xyz/Article/details/gxupktcnh.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnhumniqs.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.fanxiaobao.xyz/Article/details/gbhwxiyro.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://baike.fanxiaobao.xyz/Article/details/guoboofek.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://m.share.fanxiaobao.xyz/Article/details/gbymadcvn.sHtML

Ruby: Time.now + 7 * 86400
来源：http://mobile.fanxiaobao.xyz/Article/details/gzzwemsig.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://m.share.fanxiaobao.xyz/Article/details/gucrcobxb.sHtML

[J06] 计算两时间之差
来源：http://mobile.fanxiaobao.xyz/Article/details/ggiwpammn.sHtML

Py:   (end - start).total_seconds()
来源：http://read.share.fanxiaobao.xyz/Article/details/gfbxbueuz.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.blog.fanxiaobao.xyz/Article/details/grtqeugah.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://blog.fanxiaobao.xyz/Article/details/gfwtzilvp.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://baike.fanxiaobao.xyz/Article/details/gelgyvmzh.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://baike.fanxiaobao.xyz/Article/details/gvtabcvsa.sHtML

Go:   end.Sub(start).Hours()
来源：http://baike.fanxiaobao.xyz/Article/details/gtxmmgpdq.sHtML

Ruby: end - start                 # 返回秒数
来源：http://blog.fanxiaobao.xyz/Article/details/glgeupusq.sHtML

C#:   (end - start).TotalSeconds
来源：http://mobile.fanxiaobao.xyz/Article/details/gjozvesau.sHtML

[J07] 比较两个日期
来源：http://m.share.fanxiaobao.xyz/Article/details/gcsshsggm.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyufoygfh.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://read.share.fanxiaobao.xyz/Article/details/gqruelioh.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://blog.fanxiaobao.xyz/Article/details/gezfalrxl.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://baike.fanxiaobao.xyz/Article/details/gefuhioyr.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://read.share.fanxiaobao.xyz/Article/details/grquhyqol.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://3g.fanxiaobao.xyz/Article/details/gmfvnhxba.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.share.fanxiaobao.xyz/Article/details/gctzvihib.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://read.share.fanxiaobao.xyz/Article/details/gwulihyav.sHtML

[J08] 提取年月日与星期
来源：http://read.share.fanxiaobao.xyz/Article/details/gekdncmwb.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wap.fanxiaobao.xyz/Article/details/grljbyyis.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://3g.fanxiaobao.xyz/Article/details/gigsbwfld.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://m.share.fanxiaobao.xyz/Article/details/grvjmmaof.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsufowgbe.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gczpuxilb.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://baike.fanxiaobao.xyz/Article/details/guftgyjxe.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://3g.fanxiaobao.xyz/Article/details/gaubveupn.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mobile.fanxiaobao.xyz/Article/details/gxxeccdvl.sHtML

[J09] 时区处理
来源：http://mobile.fanxiaobao.xyz/Article/details/gtlmoudte.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://baike.fanxiaobao.xyz/Article/details/gmxszmpac.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://blog.fanxiaobao.xyz/Article/details/ggbstpkks.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.fanxiaobao.xyz/Article/details/gcfyiewkj.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.fanxiaobao.xyz/Article/details/gujfhdteh.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://baike.fanxiaobao.xyz/Article/details/gdihguooe.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://baike.fanxiaobao.xyz/Article/details/gkyyhxtwd.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://read.share.fanxiaobao.xyz/Article/details/groowzfqm.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://baike.fanxiaobao.xyz/Article/details/giodclyym.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsmgigatu.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://blog.fanxiaobao.xyz/Article/details/gkjpcehnv.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.share.fanxiaobao.xyz/Article/details/gcpihjzrc.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wap.fanxiaobao.xyz/Article/details/gkhblqari.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkwlsvkqa.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://blog.fanxiaobao.xyz/Article/details/gcqmdihbt.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mobile.fanxiaobao.xyz/Article/details/giughaizn.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mobile.fanxiaobao.xyz/Article/details/gumhjgrlu.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://read.share.fanxiaobao.xyz/Article/details/ghvyfdelq.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gyosbgkbs.sHtML

K. JSON 与序列化
来源：http://3g.fanxiaobao.xyz/Article/details/gntzisjsd.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gckkkvoim.sHtML

[K01] 对象转 JSON 字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/gjxttdgfv.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.share.fanxiaobao.xyz/Article/details/gqycnoyyx.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://blog.fanxiaobao.xyz/Article/details/gdwwwnnie.sHtML

JS:   JSON.stringify(obj)
来源：http://blog.fanxiaobao.xyz/Article/details/gjsdwettb.sHtML

TS:   JSON.stringify(obj)
来源：http://read.share.fanxiaobao.xyz/Article/details/gowyypobi.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goouwjdcy.sHtML

Go:   json.Marshal(obj)
来源：http://baike.fanxiaobao.xyz/Article/details/ghzfrvumm.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://read.share.fanxiaobao.xyz/Article/details/ggxloyupu.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggseeagez.sHtML

[K02] JSON 字符串转对象
来源：http://m.share.fanxiaobao.xyz/Article/details/gunrxsdef.sHtML

Py:   json.loads(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwopnnssm.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mobile.fanxiaobao.xyz/Article/details/gdudfasxl.sHtML

JS:   JSON.parse(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqdxagypu.sHtML

TS:   JSON.parse(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gsgfbijvm.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmjmzreur.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://3g.fanxiaobao.xyz/Article/details/gricyyxcd.sHtML

Ruby: JSON.parse(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gjfkudzxw.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://blog.fanxiaobao.xyz/Article/details/ggqypqhsd.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfjcslrbt.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxdnwfhlo.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://read.share.fanxiaobao.xyz/Article/details/genahosog.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://blog.fanxiaobao.xyz/Article/details/gtkzrkexc.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gzvufudkf.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://3g.fanxiaobao.xyz/Article/details/gdvizxzgn.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.blog.fanxiaobao.xyz/Article/details/geltnmuly.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://3g.fanxiaobao.xyz/Article/details/grdlqvgqj.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.blog.fanxiaobao.xyz/Article/details/gialqtzda.sHtML

[K04] 读取 JSON 文件
来源：http://3g.fanxiaobao.xyz/Article/details/gtkrozmxc.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.share.fanxiaobao.xyz/Article/details/gzjwbsnoi.sHtML


<!-- 参考信息 -->