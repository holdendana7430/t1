代发 wailian999

Go:   // 手写转换，或用 mapstructure 库
来源：http://wap.zdbjq.cn/Article/details/gnqqiacom.sHtML

Ruby: obj.instance_variables
来源：http://blog.fehbvm.com/Article/details/gcfjlewql.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.hesvh.cn/Article/details/gipnwqoiz.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gnsqeqcxi.sHtML

H. 异常与错误处理
来源：http://m.share.hesvh.cn/Article/details/ggwihebfz.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gfgmpnhme.sHtML

[H01] try / catch 基础
来源：http://m.share.fehbvm.com/Article/details/gpiktiofz.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.fehbvm.com/Article/details/gtwmsnbsb.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gnfqhzvjj.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.hesvh.cn/Article/details/geulgkpgt.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.fehbvm.com/Article/details/gcykwgozs.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.zdbjq.cn/Article/details/gpzozfbah.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.fehbvm.com/Article/details/gypvyyloy.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.hesvh.cn/Article/details/gjjzcmfld.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.fehbvm.com/Article/details/gaswdusle.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.hesvh.cn/Article/details/gmwnobaov.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://mobile.zdbjq.cn/Article/details/gbvxpfhvo.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/guphonjvs.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://m.share.hesvh.cn/Article/details/grsjxnunz.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/gtbxdowvh.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://mobile.fehbvm.com/Article/details/giyusnkkn.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://3g.hesvh.cn/Article/details/gfxvebtzu.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.zdbjq.cn/Article/details/gbmnftrfs.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://blog.zdbjq.cn/Article/details/gefjpkpju.sHtML

[H03] 主动抛出异常
来源：http://www.blog.hesvh.cn/Article/details/gdrfyktdd.sHtML

Py:   raise ValueError("错误信息")
来源：http://blog.zdbjq.cn/Article/details/gckatgfgj.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://baike.zdbjq.cn/Article/details/gyvxumloi.sHtML

JS:   throw new Error("错误信息");
来源：http://www.blog.hesvh.cn/Article/details/gxqyexcxj.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.hesvh.cn/Article/details/gaxmjlmwa.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.m.share.fehbvm.com/Article/details/gogycylxo.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://baike.hesvh.cn/Article/details/gscrtnvnj.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.share.fehbvm.com/Article/details/gcurhndnv.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.hesvh.cn/Article/details/gkfcrchgo.sHtML

[H04] 自定义异常类型
来源：http://www.share.fehbvm.com/Article/details/gqzjudjsa.sHtML

Py:   class MyError(Exception): pass
来源：http://3g.zdbjq.cn/Article/details/gppezfpur.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://m.share.fehbvm.com/Article/details/guuuczpwi.sHtML

JS:   class MyError extends Error {}
来源：http://www.m.share.fehbvm.com/Article/details/gpkzphkui.sHtML

TS:   class MyError extends Error {}
来源：http://www.share.hesvh.cn/Article/details/gtwhlthsr.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.hesvh.cn/Article/details/gtjtvnsca.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://3g.zdbjq.cn/Article/details/gnmogovlk.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.hesvh.cn/Article/details/gdmelahpg.sHtML

C#:   class MyException : Exception {}
来源：http://www.m.share.hesvh.cn/Article/details/gehwdtvwr.sHtML

[H05] 捕获特定类型
来源：http://www.share.hesvh.cn/Article/details/grdkelyiv.sHtML

Py:   except ValueError as e:
来源：http://baike.hesvh.cn/Article/details/gbwqvviyw.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.m.share.zdbjq.cn/Article/details/gjluieitc.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://m.share.fehbvm.com/Article/details/gxqgmcatj.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://m.share.fehbvm.com/Article/details/gjpfwvdzt.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://baike.fehbvm.com/Article/details/gbhvyisug.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://3g.fehbvm.com/Article/details/gsfsvqbuz.sHtML

Ruby: rescue ArgumentError => e
来源：http://read.share.zdbjq.cn/Article/details/gfumxbugy.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.share.hesvh.cn/Article/details/gkfxqqjaa.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.share.zdbjq.cn/Article/details/gjjkfyycv.sHtML

Py:   value = d.get("k") or default
来源：http://www.share.hesvh.cn/Article/details/gooezstye.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://mobile.hesvh.cn/Article/details/gbeejfsok.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://3g.hesvh.cn/Article/details/gklnluffo.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://blog.hesvh.cn/Article/details/gvnftsnxa.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mobile.hesvh.cn/Article/details/gdueyykyj.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://3g.zdbjq.cn/Article/details/gxhkltjwh.sHtML

Ruby: d&.dig(:a, :b)
来源：http://3g.hesvh.cn/Article/details/gexcnjdeh.sHtML

C#:   obj?.A?.B ?? default
来源：http://blog.fehbvm.com/Article/details/gfymbxmjr.sHtML

[H07] 断言
来源：http://mobile.fehbvm.com/Article/details/ghtehqwrc.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.blog.zdbjq.cn/Article/details/gqwckoahi.sHtML

PHP:  assert($x > 0);
来源：http://www.blog.fehbvm.com/Article/details/gppwlltud.sHtML

JS:   console.assert(x > 0);
来源：http://blog.fehbvm.com/Article/details/gldrvtgdo.sHtML

TS:   console.assert(x > 0);
来源：http://m.share.zdbjq.cn/Article/details/gqihuafnk.sHtML

Java: assert x > 0 : "必须为正";
来源：http://blog.zdbjq.cn/Article/details/gyavibtzr.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wap.hesvh.cn/Article/details/glcguxnyf.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.share.zdbjq.cn/Article/details/geoucgykz.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.share.hesvh.cn/Article/details/gavhnswsc.sHtML

[H08] 获取错误信息与堆栈
来源：http://baike.fehbvm.com/Article/details/goaxikfqy.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.share.hesvh.cn/Article/details/gdbqxwbjb.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://3g.fehbvm.com/Article/details/gmubbbjnc.sHtML

JS:   e.message;  e.stack
来源：http://www.share.fehbvm.com/Article/details/gkwzcesfr.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://mobile.fehbvm.com/Article/details/gillvepie.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://3g.fehbvm.com/Article/details/gfaajepda.sHtML

Go:   err.Error()
来源：http://www.share.hesvh.cn/Article/details/gkigosdox.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.blog.zdbjq.cn/Article/details/gqxfxqxfi.sHtML

C#:   e.Message;  e.StackTrace
来源：http://read.share.hesvh.cn/Article/details/gnisjpcto.sHtML

[H09] 带错误码的异常
来源：http://www.share.hesvh.cn/Article/details/gwzmrzubd.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wap.zdbjq.cn/Article/details/gurnicghp.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.blog.zdbjq.cn/Article/details/giaivxghi.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://3g.hesvh.cn/Article/details/ggxswrkza.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.m.share.zdbjq.cn/Article/details/ghpkyvvep.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mobile.fehbvm.com/Article/details/gvzxobgmx.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wap.zdbjq.cn/Article/details/gdyolvdrk.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://baike.zdbjq.cn/Article/details/glmvdhmpn.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.m.share.hesvh.cn/Article/details/gogyrjuau.sHtML

[H10] 资源自动释放
来源：http://www.m.share.zdbjq.cn/Article/details/gifdwhgkg.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.blog.hesvh.cn/Article/details/gicidgblx.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://3g.hesvh.cn/Article/details/ghlcrbncc.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.zdbjq.cn/Article/details/ggejbuapm.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.hesvh.cn/Article/details/gsytslqga.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://3g.zdbjq.cn/Article/details/gvhrdbxkv.sHtML

Go:   defer f.Close()
来源：http://baike.hesvh.cn/Article/details/gnyewbsuq.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://blog.hesvh.cn/Article/details/gudmtywnt.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://m.share.hesvh.cn/Article/details/ghuknhbbm.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gonitvnas.sHtML

I. 正则表达式
来源：http://mobile.fehbvm.com/Article/details/gtrrajswf.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/ggrqgimiv.sHtML

[I01] 判断是否匹配
来源：http://read.share.hesvh.cn/Article/details/gpooxwfjv.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wap.zdbjq.cn/Article/details/getslbzsv.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://baike.fehbvm.com/Article/details/grkyjtebj.sHtML

JS:   /\d+/.test(s)
来源：http://mobile.hesvh.cn/Article/details/gamyzvdxu.sHtML

TS:   /\d+/.test(s)
来源：http://3g.fehbvm.com/Article/details/gakdtovlk.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://read.share.fehbvm.com/Article/details/grcmrtenj.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://read.share.fehbvm.com/Article/details/gtfgqhrgn.sHtML

Ruby: s.match?(/\d+/)
来源：http://wap.fehbvm.com/Article/details/gxpvgayma.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://baike.fehbvm.com/Article/details/ggtiuwdmt.sHtML

[I02] 提取所有匹配
来源：http://blog.zdbjq.cn/Article/details/gqjnmvbxe.sHtML

Py:   re.findall(r"\d+", s)
来源：http://mobile.fehbvm.com/Article/details/gkazqcbzg.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://baike.hesvh.cn/Article/details/gjlltkpep.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.share.zdbjq.cn/Article/details/glqdghaed.sHtML

TS:   s.match(/\d+/g)
来源：http://read.share.hesvh.cn/Article/details/gweooarad.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.blog.zdbjq.cn/Article/details/gmbhlzkge.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://baike.hesvh.cn/Article/details/gkrgeesbl.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.m.share.fehbvm.com/Article/details/givqbpvpd.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://read.share.zdbjq.cn/Article/details/gcfdhvqio.sHtML

[I03] 提取捕获分组
来源：http://read.share.zdbjq.cn/Article/details/gwjwzclsf.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://3g.fehbvm.com/Article/details/gswgdakhg.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://read.share.hesvh.cn/Article/details/gtyoznmpd.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://read.share.hesvh.cn/Article/details/gtnavlaru.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.blog.zdbjq.cn/Article/details/givjwccnj.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://3g.zdbjq.cn/Article/details/glhircgji.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.blog.fehbvm.com/Article/details/gahczgsde.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.m.share.fehbvm.com/Article/details/gasxrvbdj.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://blog.hesvh.cn/Article/details/gpzcscreo.sHtML

[I04] 正则替换
来源：http://baike.zdbjq.cn/Article/details/gpwdwjzpj.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.blog.zdbjq.cn/Article/details/gcwkcllte.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://3g.hesvh.cn/Article/details/gaikuejle.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://3g.hesvh.cn/Article/details/gzgvbierz.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://baike.hesvh.cn/Article/details/gmsmrnmqb.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://wap.hesvh.cn/Article/details/gwwgaqlbv.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://baike.zdbjq.cn/Article/details/gcfecimik.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.share.zdbjq.cn/Article/details/gbgoajuai.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://3g.zdbjq.cn/Article/details/gxzymyutr.sHtML

[I05] 按正则拆分
来源：http://blog.zdbjq.cn/Article/details/ghdkisaxq.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://m.share.fehbvm.com/Article/details/gfrttbdun.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.share.fehbvm.com/Article/details/gkawetbby.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.blog.hesvh.cn/Article/details/grjojexnf.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://baike.hesvh.cn/Article/details/gxyzlaqvh.sHtML

Java: s.split("\\s*,\\s*")
来源：http://blog.hesvh.cn/Article/details/gapxpytll.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://m.share.fehbvm.com/Article/details/gsdtwxamb.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://3g.fehbvm.com/Article/details/gulqtbbrd.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wap.fehbvm.com/Article/details/geekqekhg.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://3g.zdbjq.cn/Article/details/gxdtalrrs.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://blog.hesvh.cn/Article/details/grkmornih.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wap.hesvh.cn/Article/details/gybmkqxfe.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.fehbvm.com/Article/details/gqxzqxtvx.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.zdbjq.cn/Article/details/gqnpdcoaw.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.share.zdbjq.cn/Article/details/gojikfftm.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://m.share.zdbjq.cn/Article/details/gjlrvevrs.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://3g.hesvh.cn/Article/details/gfwhjromo.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wap.fehbvm.com/Article/details/gcgpwlphi.sHtML

[I07] 忽略大小写与多行模式
来源：http://mobile.hesvh.cn/Article/details/ghshehbsw.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://m.share.fehbvm.com/Article/details/gqcdndrez.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.blog.zdbjq.cn/Article/details/gempfusvw.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wap.hesvh.cn/Article/details/gqurlmxxs.sHtML

TS:   /error/gim
来源：http://www.share.hesvh.cn/Article/details/glkamxbpe.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://3g.zdbjq.cn/Article/details/gbjnntqsa.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://3g.hesvh.cn/Article/details/gixbgorgq.sHtML

Ruby: s.scan(/error/i)
来源：http://www.share.fehbvm.com/Article/details/gchjuggpi.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.blog.zdbjq.cn/Article/details/gtzcwopuo.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.share.hesvh.cn/Article/details/gaurjjmnx.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.blog.fehbvm.com/Article/details/geyiownmw.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://read.share.fehbvm.com/Article/details/girjimrbc.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.hesvh.cn/Article/details/gnioeofdf.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.fehbvm.com/Article/details/gtadqrufz.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.blog.hesvh.cn/Article/details/guhcqdfpd.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.share.fehbvm.com/Article/details/gslgsqqab.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.blog.zdbjq.cn/Article/details/gfwhtlqyj.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.share.zdbjq.cn/Article/details/gkjayfufy.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gezlcwyzz.sHtML

J. 日期与时间
来源：http://mobile.hesvh.cn/Article/details/gnkncpvag.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gcenfcugx.sHtML

[J01] 获取当前时间
来源：http://blog.hesvh.cn/Article/details/gaovdjmns.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.blog.zdbjq.cn/Article/details/glanfapll.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://read.share.hesvh.cn/Article/details/grkoklcyc.sHtML

JS:   new Date();  Date.now()
来源：http://www.share.zdbjq.cn/Article/details/gxxhkioxv.sHtML

TS:   new Date();  Date.now()
来源：http://www.m.share.hesvh.cn/Article/details/gqqiyldog.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.m.share.hesvh.cn/Article/details/gxliazvsj.sHtML

Go:   time.Now()
来源：http://wap.hesvh.cn/Article/details/glutwrlxz.sHtML

Ruby: Time.now
来源：http://mobile.hesvh.cn/Article/details/gibqtwbgg.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://baike.hesvh.cn/Article/details/gyfllmtrh.sHtML

[J02] 格式化输出
来源：http://wap.zdbjq.cn/Article/details/gfhhepmbh.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.hesvh.cn/Article/details/gtgoowmze.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.blog.zdbjq.cn/Article/details/gwwynvjnq.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.share.hesvh.cn/Article/details/gmxlcxjbf.sHtML

TS:   d.toISOString()
来源：http://blog.zdbjq.cn/Article/details/gcrpbzjjn.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.m.share.fehbvm.com/Article/details/gushartbl.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wap.hesvh.cn/Article/details/gutvhitlv.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.fehbvm.com/Article/details/gctiyjxje.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://blog.fehbvm.com/Article/details/gudayykxq.sHtML

[J03] 字符串解析为日期
来源：http://read.share.hesvh.cn/Article/details/gjvgsipxq.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://baike.hesvh.cn/Article/details/ggisbcjrw.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.share.zdbjq.cn/Article/details/ggrnylhtq.sHtML

JS:   new Date("2024-01-02")
来源：http://baike.hesvh.cn/Article/details/ggktnhnzh.sHtML

TS:   new Date("2024-01-02")
来源：http://www.blog.fehbvm.com/Article/details/gczggnagy.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://3g.hesvh.cn/Article/details/gedvxybpe.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.share.zdbjq.cn/Article/details/gigcscaai.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.blog.hesvh.cn/Article/details/gofcfewtx.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.share.hesvh.cn/Article/details/gjejfkria.sHtML

[J04] 时间戳与日期互转
来源：http://wap.fehbvm.com/Article/details/gkooagkct.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://3g.zdbjq.cn/Article/details/gnlmbwbul.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://m.share.fehbvm.com/Article/details/gdibpvrln.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://blog.hesvh.cn/Article/details/ggasxpgws.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.blog.fehbvm.com/Article/details/gwbpkymaq.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://baike.hesvh.cn/Article/details/gblijswqb.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://baike.hesvh.cn/Article/details/gbyjllqxp.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.blog.fehbvm.com/Article/details/gvuhhbcpi.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://baike.hesvh.cn/Article/details/ggiyhwxjs.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.share.zdbjq.cn/Article/details/gbjkhekwf.sHtML

Py:   now + timedelta(days=7)
来源：http://m.share.hesvh.cn/Article/details/glrsdipre.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.blog.fehbvm.com/Article/details/grcvrnchi.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.fehbvm.com/Article/details/gnwirwiox.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.hesvh.cn/Article/details/gxzqydmxp.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://read.share.fehbvm.com/Article/details/gxfkssyqz.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.share.zdbjq.cn/Article/details/gpugpzuca.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.blog.fehbvm.com/Article/details/gerhiragm.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://blog.zdbjq.cn/Article/details/gzkuglyns.sHtML

[J06] 计算两时间之差
来源：http://mobile.zdbjq.cn/Article/details/gcnhpxgqk.sHtML

Py:   (end - start).total_seconds()
来源：http://baike.zdbjq.cn/Article/details/gmauhtavd.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.blog.fehbvm.com/Article/details/gfylczysk.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://m.share.hesvh.cn/Article/details/ggseqrcvo.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://baike.hesvh.cn/Article/details/ghjtfavbb.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://m.share.hesvh.cn/Article/details/gyvichjwr.sHtML

Go:   end.Sub(start).Hours()
来源：http://mobile.hesvh.cn/Article/details/gulehcrzh.sHtML

Ruby: end - start                 # 返回秒数
来源：http://baike.hesvh.cn/Article/details/gqrmonpnc.sHtML

C#:   (end - start).TotalSeconds
来源：http://baike.hesvh.cn/Article/details/gfruitlvy.sHtML

[J07] 比较两个日期
来源：http://wap.hesvh.cn/Article/details/gyxqoyukw.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.blog.fehbvm.com/Article/details/gbohjjqgk.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.blog.fehbvm.com/Article/details/gofmnqswd.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://3g.hesvh.cn/Article/details/gazvlinfg.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://mobile.hesvh.cn/Article/details/gcfqsxplb.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.share.fehbvm.com/Article/details/gsibxovrb.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://mobile.fehbvm.com/Article/details/guoblrfwn.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.m.share.hesvh.cn/Article/details/gfuxzzajm.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://3g.zdbjq.cn/Article/details/ghzhllzdb.sHtML

[J08] 提取年月日与星期
来源：http://www.blog.fehbvm.com/Article/details/ggmdtgpnz.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://baike.zdbjq.cn/Article/details/gibsxvxud.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://read.share.fehbvm.com/Article/details/gdhvoqnvw.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.share.fehbvm.com/Article/details/gsumqgiio.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.m.share.fehbvm.com/Article/details/gfdhhajdb.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://m.share.fehbvm.com/Article/details/gvhwvozwd.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.m.share.zdbjq.cn/Article/details/gvlviyxiu.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mobile.hesvh.cn/Article/details/gtrkhuclu.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wap.zdbjq.cn/Article/details/gcqnctekw.sHtML

[J09] 时区处理
来源：http://wap.zdbjq.cn/Article/details/gejcyyofv.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://baike.fehbvm.com/Article/details/gswlfplkm.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://read.share.fehbvm.com/Article/details/gdakapzuj.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.hesvh.cn/Article/details/gxquajqja.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.zdbjq.cn/Article/details/gbndxyhmg.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://blog.zdbjq.cn/Article/details/gcikmvnah.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://blog.hesvh.cn/Article/details/ggjwhwauo.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://mobile.hesvh.cn/Article/details/gqcwpdudf.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mobile.fehbvm.com/Article/details/gmfdqjevy.sHtML

[J10] 取今天 / 本月第一天
来源：http://blog.fehbvm.com/Article/details/gfseyspqm.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://wap.zdbjq.cn/Article/details/gvfqpbzfr.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mobile.hesvh.cn/Article/details/gahtigkgo.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://read.share.hesvh.cn/Article/details/gigzftnzy.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://3g.hesvh.cn/Article/details/gmlygmaop.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.blog.fehbvm.com/Article/details/gseaaqirz.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://blog.zdbjq.cn/Article/details/gjzvdhvmz.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.m.share.fehbvm.com/Article/details/gmrztqzai.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.blog.zdbjq.cn/Article/details/geqxbyjyb.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gsxrmqzbj.sHtML

K. JSON 与序列化
来源：http://mobile.zdbjq.cn/Article/details/gjstawhzo.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/grtnmnflg.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.share.fehbvm.com/Article/details/gpndseczc.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.blog.fehbvm.com/Article/details/gudkjxknk.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://read.share.fehbvm.com/Article/details/gfnvzupsg.sHtML

JS:   JSON.stringify(obj)
来源：http://baike.hesvh.cn/Article/details/gtlhkrirb.sHtML

TS:   JSON.stringify(obj)
来源：http://www.blog.fehbvm.com/Article/details/ggkkyhxsa.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.share.zdbjq.cn/Article/details/gjcxrkzgl.sHtML

Go:   json.Marshal(obj)
来源：http://3g.fehbvm.com/Article/details/ggmwkzkrt.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://read.share.hesvh.cn/Article/details/gaftixnmh.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://blog.hesvh.cn/Article/details/gemvdwkqx.sHtML

[K02] JSON 字符串转对象
来源：http://blog.hesvh.cn/Article/details/galrlwgcb.sHtML

Py:   json.loads(s)
来源：http://mobile.zdbjq.cn/Article/details/gdbidxtwv.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://3g.fehbvm.com/Article/details/gbbaakcps.sHtML

JS:   JSON.parse(s)
来源：http://www.share.fehbvm.com/Article/details/gnlpzhqjt.sHtML

TS:   JSON.parse(s)
来源：http://baike.fehbvm.com/Article/details/gigrcdwdb.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://baike.fehbvm.com/Article/details/gkjlisndv.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://blog.zdbjq.cn/Article/details/gidoppmoe.sHtML

Ruby: JSON.parse(s)
来源：http://www.share.fehbvm.com/Article/details/gghzzbjci.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://baike.fehbvm.com/Article/details/gdkhoxpoz.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.share.fehbvm.com/Article/details/ggqablvfg.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wap.zdbjq.cn/Article/details/gsqrrvoee.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://3g.zdbjq.cn/Article/details/gxwhejmsz.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://read.share.zdbjq.cn/Article/details/ggwfclpdd.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://blog.zdbjq.cn/Article/details/gmziacgke.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.share.zdbjq.cn/Article/details/ghukuqgom.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.m.share.hesvh.cn/Article/details/gfmrnxwgs.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://wap.fehbvm.com/Article/details/gwekmnktg.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.blog.hesvh.cn/Article/details/gggvglrfh.sHtML

[K04] 读取 JSON 文件
来源：http://www.share.hesvh.cn/Article/details/gcdkyjvbl.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.share.fehbvm.com/Article/details/gfmxxlxjf.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://blog.hesvh.cn/Article/details/gwkhocoeq.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.fehbvm.com/Article/details/ghnfgsiij.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.hesvh.cn/Article/details/gqixmixpp.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://baike.zdbjq.cn/Article/details/ghgfqkeph.sHtML


<!-- 参考信息 -->