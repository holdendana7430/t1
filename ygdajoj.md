代发 wailian999

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.zdbjq.cn/Article/details/gfmmmcyfq.sHtML

Ruby: obj.instance_variables
来源：http://mobile.zdbjq.cn/Article/details/ggabermch.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.zdbjq.cn/Article/details/ghryronsv.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gslajijsv.sHtML

H. 异常与错误处理
来源：http://www.share.zdbjq.cn/Article/details/gzqynvbzj.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gwtgkldpq.sHtML

[H01] try / catch 基础
来源：http://www.blog.hesvh.cn/Article/details/gqcidnzlv.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.zdbjq.cn/Article/details/gmsivynjs.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.hesvh.cn/Article/details/gglhtlqhd.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.share.fehbvm.com/Article/details/gwfecwqax.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://m.share.hesvh.cn/Article/details/gswzemaus.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.blog.zdbjq.cn/Article/details/gppmwknvo.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.blog.fehbvm.com/Article/details/girjrmecg.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.zdbjq.cn/Article/details/gyfloyakk.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.hesvh.cn/Article/details/gnxlfylxo.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.zdbjq.cn/Article/details/gojoblfcl.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.fehbvm.com/Article/details/gizjzfvjm.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://3g.fehbvm.com/Article/details/gaixhntst.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/gfsrktdhh.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/gbngppyux.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://wap.fehbvm.com/Article/details/gadekxmnq.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.fehbvm.com/Article/details/gzsehejgx.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.share.hesvh.cn/Article/details/gdgfilacl.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://m.share.hesvh.cn/Article/details/gtewjegmg.sHtML

[H03] 主动抛出异常
来源：http://www.blog.fehbvm.com/Article/details/ggizxjbqz.sHtML

Py:   raise ValueError("错误信息")
来源：http://read.share.hesvh.cn/Article/details/gsywgrxkv.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blog.zdbjq.cn/Article/details/gnlxftvrs.sHtML

JS:   throw new Error("错误信息");
来源：http://blog.zdbjq.cn/Article/details/geysnmnjm.sHtML

TS:   throw new Error("错误信息");
来源：http://wap.zdbjq.cn/Article/details/griivbqiy.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.hesvh.cn/Article/details/gfngnqgoi.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://3g.hesvh.cn/Article/details/gocywqpui.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://blog.zdbjq.cn/Article/details/gskxnjrjs.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.blog.zdbjq.cn/Article/details/gbwurgrdd.sHtML

[H04] 自定义异常类型
来源：http://read.share.zdbjq.cn/Article/details/gtcqgwpfo.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.fehbvm.com/Article/details/gpxqtwedl.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.share.zdbjq.cn/Article/details/gbmyzpjem.sHtML

JS:   class MyError extends Error {}
来源：http://www.blog.fehbvm.com/Article/details/gxmntbmrg.sHtML

TS:   class MyError extends Error {}
来源：http://baike.hesvh.cn/Article/details/gmjitrhvg.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.fehbvm.com/Article/details/gpotbgemw.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.blog.fehbvm.com/Article/details/gmhlpcgcn.sHtML

Ruby: class MyError < StandardError; end
来源：http://m.share.zdbjq.cn/Article/details/gdkgxkbkb.sHtML

C#:   class MyException : Exception {}
来源：http://www.m.share.fehbvm.com/Article/details/gbkhryrcl.sHtML

[H05] 捕获特定类型
来源：http://blog.fehbvm.com/Article/details/gjnuuzlwk.sHtML

Py:   except ValueError as e:
来源：http://read.share.zdbjq.cn/Article/details/guqccmtqv.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.hesvh.cn/Article/details/gyanvlcwt.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://m.share.fehbvm.com/Article/details/gvdjiytie.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://mobile.zdbjq.cn/Article/details/gjpumqopi.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.m.share.fehbvm.com/Article/details/grkxnunrx.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wap.zdbjq.cn/Article/details/ggpptgees.sHtML

Ruby: rescue ArgumentError => e
来源：http://3g.fehbvm.com/Article/details/gjeismhhz.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wap.zdbjq.cn/Article/details/gqnpwvalj.sHtML

[H06] 可选值 / 空值安全访问
来源：http://mobile.fehbvm.com/Article/details/gjdxgkqxb.sHtML

Py:   value = d.get("k") or default
来源：http://m.share.fehbvm.com/Article/details/gaevprmxl.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://m.share.zdbjq.cn/Article/details/geaocwkxk.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.blog.hesvh.cn/Article/details/gbfqqycwd.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.blog.zdbjq.cn/Article/details/gqdtkhudy.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://blog.fehbvm.com/Article/details/gvsgkoewl.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://wap.zdbjq.cn/Article/details/giazdhgnw.sHtML

Ruby: d&.dig(:a, :b)
来源：http://wap.fehbvm.com/Article/details/ghpmefvzq.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.share.fehbvm.com/Article/details/gfcnqsoav.sHtML

[H07] 断言
来源：http://baike.hesvh.cn/Article/details/gdwotwajf.sHtML

Py:   assert x > 0, "必须为正"
来源：http://3g.zdbjq.cn/Article/details/gvnmfooah.sHtML

PHP:  assert($x > 0);
来源：http://www.share.hesvh.cn/Article/details/gaqiqwnlo.sHtML

JS:   console.assert(x > 0);
来源：http://www.blog.zdbjq.cn/Article/details/gzvtxkwej.sHtML

TS:   console.assert(x > 0);
来源：http://www.share.zdbjq.cn/Article/details/gmqgoipdh.sHtML

Java: assert x > 0 : "必须为正";
来源：http://baike.zdbjq.cn/Article/details/gwxjkrkjv.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.blog.fehbvm.com/Article/details/gyqxgbkss.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.share.zdbjq.cn/Article/details/gvbvszqix.sHtML

C#:   Debug.Assert(x > 0);
来源：http://3g.zdbjq.cn/Article/details/gljagurnu.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.blog.fehbvm.com/Article/details/glcjooerz.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://blog.zdbjq.cn/Article/details/gondnfleo.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://blog.hesvh.cn/Article/details/gwciqtojc.sHtML

JS:   e.message;  e.stack
来源：http://baike.zdbjq.cn/Article/details/gtvbrxoou.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://mobile.fehbvm.com/Article/details/gjhyuvclw.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://m.share.hesvh.cn/Article/details/gydiuxkte.sHtML

Go:   err.Error()
来源：http://baike.fehbvm.com/Article/details/gncuhszsw.sHtML

Ruby: e.message;  e.backtrace
来源：http://read.share.fehbvm.com/Article/details/gojomewag.sHtML

C#:   e.Message;  e.StackTrace
来源：http://3g.zdbjq.cn/Article/details/gazluimxc.sHtML

[H09] 带错误码的异常
来源：http://m.share.fehbvm.com/Article/details/gpuvlbons.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.share.hesvh.cn/Article/details/gukajueeo.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.share.fehbvm.com/Article/details/gbvlipvep.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.m.share.fehbvm.com/Article/details/gjmpspftv.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.share.zdbjq.cn/Article/details/gzwsenokm.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.blog.fehbvm.com/Article/details/gdishprei.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://read.share.hesvh.cn/Article/details/gmqghlvzw.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.m.share.fehbvm.com/Article/details/gehzyfqhf.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://m.share.hesvh.cn/Article/details/gxwiubnnr.sHtML

[H10] 资源自动释放
来源：http://www.blog.hesvh.cn/Article/details/geyvkeuhq.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.m.share.zdbjq.cn/Article/details/gbcdhaefb.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wap.hesvh.cn/Article/details/gfmofvogm.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.hesvh.cn/Article/details/gjdwckurb.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.fehbvm.com/Article/details/gegltwkpo.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.blog.hesvh.cn/Article/details/gdejgjcjb.sHtML

Go:   defer f.Close()
来源：http://www.m.share.hesvh.cn/Article/details/geldadmqv.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.m.share.fehbvm.com/Article/details/gjjooobgi.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://baike.hesvh.cn/Article/details/gzsgxcvvk.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/ggsujkfrr.sHtML

I. 正则表达式
来源：http://wap.hesvh.cn/Article/details/gxkdmvehv.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gtjfrdgmp.sHtML

[I01] 判断是否匹配
来源：http://read.share.fehbvm.com/Article/details/gvukwefte.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://read.share.fehbvm.com/Article/details/gmkhitlyh.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.m.share.hesvh.cn/Article/details/gmasgxlht.sHtML

JS:   /\d+/.test(s)
来源：http://m.share.hesvh.cn/Article/details/gvcwimrfh.sHtML

TS:   /\d+/.test(s)
来源：http://mobile.hesvh.cn/Article/details/ghcsngath.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.m.share.zdbjq.cn/Article/details/gsmowpvtx.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://read.share.hesvh.cn/Article/details/gvqvtlnef.sHtML

Ruby: s.match?(/\d+/)
来源：http://3g.zdbjq.cn/Article/details/gbjkodcrq.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mobile.zdbjq.cn/Article/details/giylruegb.sHtML

[I02] 提取所有匹配
来源：http://read.share.zdbjq.cn/Article/details/ghdtyqsdo.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.share.fehbvm.com/Article/details/gjufkmptc.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://m.share.hesvh.cn/Article/details/gvlbdzbte.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.m.share.zdbjq.cn/Article/details/gavxolqdq.sHtML

TS:   s.match(/\d+/g)
来源：http://www.share.fehbvm.com/Article/details/gwdjqvwuh.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://3g.zdbjq.cn/Article/details/gkrlrkhql.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://baike.fehbvm.com/Article/details/gvxqtazle.sHtML

Ruby: s.scan(/\d+/)
来源：http://3g.fehbvm.com/Article/details/gtnyqowoi.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wap.fehbvm.com/Article/details/gyctgqiij.sHtML

[I03] 提取捕获分组
来源：http://www.blog.zdbjq.cn/Article/details/grfcvolcr.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://m.share.zdbjq.cn/Article/details/grsoxpxxp.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.blog.fehbvm.com/Article/details/gcuhnezrm.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://baike.zdbjq.cn/Article/details/gxjrjfdna.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.share.zdbjq.cn/Article/details/gjrnxgawf.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wap.zdbjq.cn/Article/details/gqczukrxj.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wap.zdbjq.cn/Article/details/gjxasqvgr.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://read.share.hesvh.cn/Article/details/gzxhqkavk.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://3g.hesvh.cn/Article/details/gbjikogcp.sHtML

[I04] 正则替换
来源：http://3g.hesvh.cn/Article/details/gjammxzby.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://wap.zdbjq.cn/Article/details/gigoeioaa.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://read.share.hesvh.cn/Article/details/gdknphuqo.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://3g.hesvh.cn/Article/details/glxlhknab.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.hesvh.cn/Article/details/gnqpudodx.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.share.hesvh.cn/Article/details/gyjgzjixk.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.blog.hesvh.cn/Article/details/gduiljctv.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://baike.zdbjq.cn/Article/details/gipjasrxz.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.blog.zdbjq.cn/Article/details/gwppoigao.sHtML

[I05] 按正则拆分
来源：http://mobile.fehbvm.com/Article/details/gyfmbvszb.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.share.fehbvm.com/Article/details/gkfnlblxc.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mobile.fehbvm.com/Article/details/gqieujugj.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://read.share.fehbvm.com/Article/details/govdomarc.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.m.share.hesvh.cn/Article/details/gahljtgos.sHtML

Java: s.split("\\s*,\\s*")
来源：http://3g.hesvh.cn/Article/details/gnndduxug.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://m.share.zdbjq.cn/Article/details/gaxrkejsj.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://mobile.zdbjq.cn/Article/details/gtswtgmxl.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.share.hesvh.cn/Article/details/gtdjglfsg.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mobile.fehbvm.com/Article/details/gnjitaidp.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://blog.fehbvm.com/Article/details/gvqvnzmls.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://3g.zdbjq.cn/Article/details/gkuwqyqjk.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.hesvh.cn/Article/details/gwsvoizke.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.fehbvm.com/Article/details/gizsoedbp.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.share.zdbjq.cn/Article/details/gkwtdvjqc.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://mobile.zdbjq.cn/Article/details/gjbiobzqe.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://blog.zdbjq.cn/Article/details/ggyquwysl.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mobile.fehbvm.com/Article/details/gebntlzkz.sHtML

[I07] 忽略大小写与多行模式
来源：http://blog.zdbjq.cn/Article/details/gmhimqfss.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://m.share.hesvh.cn/Article/details/gjjubpwvb.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.blog.fehbvm.com/Article/details/ghtilolzy.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mobile.zdbjq.cn/Article/details/gmebvdwxq.sHtML

TS:   /error/gim
来源：http://www.blog.fehbvm.com/Article/details/gooljonuc.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mobile.zdbjq.cn/Article/details/gcykdpyjy.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://m.share.hesvh.cn/Article/details/gyxnlwsiw.sHtML

Ruby: s.scan(/error/i)
来源：http://wap.fehbvm.com/Article/details/gmmqtctho.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://wap.hesvh.cn/Article/details/gousjwycm.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://blog.fehbvm.com/Article/details/ghzrvdkuh.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://blog.fehbvm.com/Article/details/gyiqygvbo.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://3g.fehbvm.com/Article/details/gedtkrpdy.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.hesvh.cn/Article/details/gwrqlgxkh.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.hesvh.cn/Article/details/gjqhcxlah.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://read.share.zdbjq.cn/Article/details/gcrcnobpm.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://blog.hesvh.cn/Article/details/gbrfnfqag.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wap.fehbvm.com/Article/details/gdtrgragd.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://blog.zdbjq.cn/Article/details/gwkpixcvd.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/grdhooglw.sHtML

J. 日期与时间
来源：http://wap.hesvh.cn/Article/details/gkojnqywr.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/giqdslykx.sHtML

[J01] 获取当前时间
来源：http://read.share.hesvh.cn/Article/details/getynkzqh.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://3g.zdbjq.cn/Article/details/gqvzgusta.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://wap.fehbvm.com/Article/details/gleevhcno.sHtML

JS:   new Date();  Date.now()
来源：http://mobile.hesvh.cn/Article/details/ghfqtuhqa.sHtML

TS:   new Date();  Date.now()
来源：http://baike.hesvh.cn/Article/details/gycrvqoer.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://mobile.hesvh.cn/Article/details/ggnbzsttn.sHtML

Go:   time.Now()
来源：http://3g.zdbjq.cn/Article/details/gfpnbifda.sHtML

Ruby: Time.now
来源：http://mobile.fehbvm.com/Article/details/gbpfklqiq.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.m.share.fehbvm.com/Article/details/gtxwlqgtb.sHtML

[J02] 格式化输出
来源：http://wap.fehbvm.com/Article/details/gvenilqqn.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.hesvh.cn/Article/details/gqabwvnac.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://baike.fehbvm.com/Article/details/gsiglcajz.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.m.share.hesvh.cn/Article/details/gooumblrz.sHtML

TS:   d.toISOString()
来源：http://wap.fehbvm.com/Article/details/gbcbqjjgp.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.share.hesvh.cn/Article/details/gtruhxshp.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.blog.hesvh.cn/Article/details/gfotauuwn.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.fehbvm.com/Article/details/giguwkusj.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://blog.fehbvm.com/Article/details/gtxqqppzx.sHtML

[J03] 字符串解析为日期
来源：http://blog.hesvh.cn/Article/details/grkldkgro.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.m.share.zdbjq.cn/Article/details/gyjncinwu.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wap.fehbvm.com/Article/details/ggcqbpyqe.sHtML

JS:   new Date("2024-01-02")
来源：http://read.share.fehbvm.com/Article/details/gbtslzcpn.sHtML

TS:   new Date("2024-01-02")
来源：http://www.m.share.hesvh.cn/Article/details/gysudglmn.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.share.zdbjq.cn/Article/details/ghqumhgnj.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.m.share.zdbjq.cn/Article/details/gslmhcelh.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://m.share.hesvh.cn/Article/details/gdjwrkkiu.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.share.zdbjq.cn/Article/details/gdwphntwh.sHtML

[J04] 时间戳与日期互转
来源：http://blog.hesvh.cn/Article/details/gvenytbno.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.m.share.hesvh.cn/Article/details/gyowjnvwq.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.blog.zdbjq.cn/Article/details/gowjisnik.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://3g.zdbjq.cn/Article/details/gojdmwcki.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.share.hesvh.cn/Article/details/gyxvoqivp.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://3g.zdbjq.cn/Article/details/gxgzxmzbb.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://m.share.fehbvm.com/Article/details/gxqrzhuyv.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://baike.hesvh.cn/Article/details/gddejotof.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://m.share.zdbjq.cn/Article/details/gzhvmiugq.sHtML

[J05] 时间加减（加 7 天）
来源：http://3g.fehbvm.com/Article/details/gjbopeeiy.sHtML

Py:   now + timedelta(days=7)
来源：http://www.blog.fehbvm.com/Article/details/gpljaahxd.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://3g.hesvh.cn/Article/details/gzzmpoyhk.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.hesvh.cn/Article/details/gzdohngub.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.zdbjq.cn/Article/details/gnekyicam.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://read.share.hesvh.cn/Article/details/gtdrmnpfk.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.m.share.zdbjq.cn/Article/details/gbcbyavpf.sHtML

Ruby: Time.now + 7 * 86400
来源：http://wap.fehbvm.com/Article/details/glojsabbk.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://3g.zdbjq.cn/Article/details/gmnuhibar.sHtML

[J06] 计算两时间之差
来源：http://m.share.fehbvm.com/Article/details/gpfuwffml.sHtML

Py:   (end - start).total_seconds()
来源：http://m.share.zdbjq.cn/Article/details/glteiljkk.sHtML

PHP:  $end->diff($start)->days;
来源：http://mobile.fehbvm.com/Article/details/gmltcuedi.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.share.hesvh.cn/Article/details/grtnbflhp.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mobile.fehbvm.com/Article/details/guehlpzcr.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://wap.zdbjq.cn/Article/details/gaowmwzna.sHtML

Go:   end.Sub(start).Hours()
来源：http://wap.hesvh.cn/Article/details/gpvmerknx.sHtML

Ruby: end - start                 # 返回秒数
来源：http://3g.fehbvm.com/Article/details/gmcrdhjzr.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.m.share.fehbvm.com/Article/details/gqtutlxmk.sHtML

[J07] 比较两个日期
来源：http://mobile.zdbjq.cn/Article/details/ghzzncldu.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://mobile.hesvh.cn/Article/details/gljsauidn.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.share.hesvh.cn/Article/details/gbdhhcusq.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://read.share.hesvh.cn/Article/details/gqxngoole.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.hesvh.cn/Article/details/gqexseszd.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.blog.hesvh.cn/Article/details/gkjpdpgzr.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://read.share.hesvh.cn/Article/details/gageaxqmy.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://m.share.zdbjq.cn/Article/details/gfgaoldoy.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://m.share.hesvh.cn/Article/details/gxuzcpgmk.sHtML

[J08] 提取年月日与星期
来源：http://www.m.share.fehbvm.com/Article/details/gjuubexub.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.share.fehbvm.com/Article/details/gfogiuqop.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wap.hesvh.cn/Article/details/grctloent.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://baike.fehbvm.com/Article/details/gycabfisv.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mobile.zdbjq.cn/Article/details/gwwpjqwcx.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://read.share.zdbjq.cn/Article/details/gxoeciqis.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://m.share.zdbjq.cn/Article/details/gwsmwddti.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.blog.hesvh.cn/Article/details/gafnjazuq.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://blog.hesvh.cn/Article/details/gifbhzswn.sHtML

[J09] 时区处理
来源：http://m.share.hesvh.cn/Article/details/ganvrljzs.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.share.hesvh.cn/Article/details/gxmvjoywr.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://3g.zdbjq.cn/Article/details/gqeazmmir.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.fehbvm.com/Article/details/gniohxeye.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.zdbjq.cn/Article/details/gehhnmfib.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://3g.hesvh.cn/Article/details/gyoswqtjw.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wap.fehbvm.com/Article/details/ggxzndtyp.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://3g.fehbvm.com/Article/details/gqmsievxi.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.blog.zdbjq.cn/Article/details/grqziqato.sHtML

[J10] 取今天 / 本月第一天
来源：http://baike.zdbjq.cn/Article/details/gigppclii.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://wap.zdbjq.cn/Article/details/gtcaqbals.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.blog.hesvh.cn/Article/details/gkxzsrzvu.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mobile.hesvh.cn/Article/details/gfjguycmi.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wap.hesvh.cn/Article/details/gsbvwvlxc.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.share.hesvh.cn/Article/details/gliionxpf.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://blog.zdbjq.cn/Article/details/gomkyrsit.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.m.share.hesvh.cn/Article/details/gyhxdpvlt.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://m.share.hesvh.cn/Article/details/gsheycodk.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gmpeptpqm.sHtML

K. JSON 与序列化
来源：http://mobile.hesvh.cn/Article/details/ggkxmecip.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gburbbskk.sHtML

[K01] 对象转 JSON 字符串
来源：http://wap.zdbjq.cn/Article/details/gbrrptopq.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wap.zdbjq.cn/Article/details/glafuptja.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://baike.zdbjq.cn/Article/details/gomlindul.sHtML

JS:   JSON.stringify(obj)
来源：http://www.blog.hesvh.cn/Article/details/gpggnwczn.sHtML

TS:   JSON.stringify(obj)
来源：http://blog.fehbvm.com/Article/details/gmninikix.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://blog.zdbjq.cn/Article/details/gaztucgys.sHtML

Go:   json.Marshal(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gfojmqeth.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://baike.hesvh.cn/Article/details/gqwmvsbzl.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gwjiopqbv.sHtML

[K02] JSON 字符串转对象
来源：http://mobile.zdbjq.cn/Article/details/gjborcele.sHtML

Py:   json.loads(s)
来源：http://m.share.zdbjq.cn/Article/details/gxdxjvtft.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.share.fehbvm.com/Article/details/gljwabzca.sHtML

JS:   JSON.parse(s)
来源：http://baike.fehbvm.com/Article/details/glysfociy.sHtML

TS:   JSON.parse(s)
来源：http://read.share.hesvh.cn/Article/details/glmtewigs.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.blog.zdbjq.cn/Article/details/ghlwypjgc.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://baike.fehbvm.com/Article/details/ggwpnbuhp.sHtML

Ruby: JSON.parse(s)
来源：http://read.share.hesvh.cn/Article/details/grjwnwsez.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://baike.hesvh.cn/Article/details/gylrthfde.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://m.share.zdbjq.cn/Article/details/gjrrajkyh.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.share.zdbjq.cn/Article/details/glfxsxmnl.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.share.fehbvm.com/Article/details/gsaatopnq.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.share.hesvh.cn/Article/details/gwvijiiyy.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.fehbvm.com/Article/details/gqxxznmrx.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://blog.hesvh.cn/Article/details/glgbqmcwm.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://baike.zdbjq.cn/Article/details/gkxxxpzsl.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://wap.fehbvm.com/Article/details/gbitkajxv.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.share.zdbjq.cn/Article/details/gyqcaunou.sHtML

[K04] 读取 JSON 文件
来源：http://read.share.zdbjq.cn/Article/details/gtxlhjiiq.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.m.share.zdbjq.cn/Article/details/grxmbyoud.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://blog.fehbvm.com/Article/details/gyhagomgx.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.zdbjq.cn/Article/details/gsuhzgnay.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.hesvh.cn/Article/details/glyxyheqa.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mobile.fehbvm.com/Article/details/gditaujyd.sHtML


<!-- 参考信息 -->