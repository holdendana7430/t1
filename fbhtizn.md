代发 wailian999

H. 异常与错误处理
来源：http://mobile.fehbvm.com/Article/details/gctqzdada.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gymlhxcss.sHtML

[H01] try / catch 基础
来源：http://www.m.share.fehbvm.com/Article/details/gbaemjccn.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.hesvh.cn/Article/details/gwdyoefhs.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.fehbvm.com/Article/details/gflosgbqh.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.blog.fehbvm.com/Article/details/gnyctomeg.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.hesvh.cn/Article/details/gcuaycfsj.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.blog.zdbjq.cn/Article/details/gaisalbia.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mobile.hesvh.cn/Article/details/gpalfjmeu.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.zdbjq.cn/Article/details/gctjlfexo.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.m.share.fehbvm.com/Article/details/gasxviohx.sHtML

[H02] finally / ensure 收尾
来源：http://baike.hesvh.cn/Article/details/gjoqqnowz.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.hesvh.cn/Article/details/gbxyggpnz.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/guixlkgkw.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://blog.zdbjq.cn/Article/details/gtmjnfrqy.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.fehbvm.com/Article/details/ggsqvsskr.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://wap.fehbvm.com/Article/details/gwcvabjhj.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.hesvh.cn/Article/details/ghfnewich.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.hesvh.cn/Article/details/gqhliaaxj.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://read.share.zdbjq.cn/Article/details/gpgltlmgu.sHtML

[H03] 主动抛出异常
来源：http://3g.zdbjq.cn/Article/details/gtwbromph.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.fehbvm.com/Article/details/gvzoaufbn.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blog.hesvh.cn/Article/details/gmgvfxmpn.sHtML

JS:   throw new Error("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/grikqqlsx.sHtML

TS:   throw new Error("错误信息");
来源：http://read.share.hesvh.cn/Article/details/ggvegjolk.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://read.share.fehbvm.com/Article/details/gysiwuhjs.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://read.share.zdbjq.cn/Article/details/gwlsdlndr.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://m.share.zdbjq.cn/Article/details/gwqoryfrm.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.share.fehbvm.com/Article/details/grqqalvob.sHtML

[H04] 自定义异常类型
来源：http://m.share.fehbvm.com/Article/details/gzuqvdscl.sHtML

Py:   class MyError(Exception): pass
来源：http://3g.hesvh.cn/Article/details/gljhbzbnp.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://blog.fehbvm.com/Article/details/giaxwkjdw.sHtML

JS:   class MyError extends Error {}
来源：http://mobile.zdbjq.cn/Article/details/gypjnamje.sHtML

TS:   class MyError extends Error {}
来源：http://mobile.hesvh.cn/Article/details/glyuzgtzs.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.zdbjq.cn/Article/details/gwoslttxd.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.m.share.fehbvm.com/Article/details/ggnyaijnx.sHtML

Ruby: class MyError < StandardError; end
来源：http://mobile.zdbjq.cn/Article/details/ghofrxzey.sHtML

C#:   class MyException : Exception {}
来源：http://m.share.zdbjq.cn/Article/details/gqrzsbort.sHtML

[H05] 捕获特定类型
来源：http://mobile.zdbjq.cn/Article/details/giqbzemuj.sHtML

Py:   except ValueError as e:
来源：http://3g.zdbjq.cn/Article/details/gutyrfdbo.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.m.share.hesvh.cn/Article/details/ggociirxz.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://3g.hesvh.cn/Article/details/gajskkihj.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.m.share.hesvh.cn/Article/details/gwnevqgpl.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://3g.zdbjq.cn/Article/details/guotbiykc.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://baike.fehbvm.com/Article/details/glvisbpii.sHtML

Ruby: rescue ArgumentError => e
来源：http://mobile.zdbjq.cn/Article/details/gbpybuvpe.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://3g.hesvh.cn/Article/details/gyqcsbspa.sHtML

[H06] 可选值 / 空值安全访问
来源：http://wap.fehbvm.com/Article/details/gcgoaahzh.sHtML

Py:   value = d.get("k") or default
来源：http://www.share.fehbvm.com/Article/details/gvxinbkja.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://3g.hesvh.cn/Article/details/gzvpyjzll.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.share.fehbvm.com/Article/details/gnhtdxbgf.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.share.zdbjq.cn/Article/details/gfikrqhhq.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://blog.fehbvm.com/Article/details/gawbntxgo.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.m.share.fehbvm.com/Article/details/gtqocrzjb.sHtML

Ruby: d&.dig(:a, :b)
来源：http://wap.fehbvm.com/Article/details/gvtppedpl.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.m.share.hesvh.cn/Article/details/gmpjwnjjn.sHtML

[H07] 断言
来源：http://wap.fehbvm.com/Article/details/gdgxdjqmy.sHtML

Py:   assert x > 0, "必须为正"
来源：http://wap.fehbvm.com/Article/details/gjuftjimx.sHtML

PHP:  assert($x > 0);
来源：http://mobile.zdbjq.cn/Article/details/gnvpglncu.sHtML

JS:   console.assert(x > 0);
来源：http://blog.zdbjq.cn/Article/details/gbilrkkle.sHtML

TS:   console.assert(x > 0);
来源：http://www.blog.hesvh.cn/Article/details/gdyeghwnr.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.zdbjq.cn/Article/details/giegwfmfv.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.m.share.zdbjq.cn/Article/details/gqynkshxu.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.share.fehbvm.com/Article/details/geylcwijx.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.blog.hesvh.cn/Article/details/gjzilkenq.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.m.share.zdbjq.cn/Article/details/gtkhljomz.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.m.share.hesvh.cn/Article/details/ggxhwoftk.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.share.fehbvm.com/Article/details/gvoqgfylt.sHtML

JS:   e.message;  e.stack
来源：http://read.share.hesvh.cn/Article/details/gfsziqdip.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://m.share.hesvh.cn/Article/details/gvkiosdpv.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.m.share.fehbvm.com/Article/details/gfcgyrzld.sHtML

Go:   err.Error()
来源：http://read.share.zdbjq.cn/Article/details/gggwahaek.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.blog.hesvh.cn/Article/details/ghbmlgvuq.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.m.share.hesvh.cn/Article/details/gaemdvxqr.sHtML

[H09] 带错误码的异常
来源：http://blog.zdbjq.cn/Article/details/gprapimss.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://3g.hesvh.cn/Article/details/grzamlbkq.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.share.hesvh.cn/Article/details/gteqqaril.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.share.hesvh.cn/Article/details/glscnieaz.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.share.zdbjq.cn/Article/details/gvjyejvpn.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.m.share.hesvh.cn/Article/details/gjabhutzp.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://m.share.fehbvm.com/Article/details/genrrwixx.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.blog.hesvh.cn/Article/details/gkfdseige.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.m.share.hesvh.cn/Article/details/gehcssrsn.sHtML

[H10] 资源自动释放
来源：http://mobile.hesvh.cn/Article/details/gxpjcyzem.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.m.share.fehbvm.com/Article/details/gphndqajp.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.m.share.hesvh.cn/Article/details/gfkxckryz.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.zdbjq.cn/Article/details/gguxordlg.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.hesvh.cn/Article/details/gvjuuykcx.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wap.hesvh.cn/Article/details/gynuhonbk.sHtML

Go:   defer f.Close()
来源：http://www.blog.fehbvm.com/Article/details/gyugugnou.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://m.share.zdbjq.cn/Article/details/gmlmagkns.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gxlldheil.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gfxzsxfyi.sHtML

I. 正则表达式
来源：http://www.m.share.hesvh.cn/Article/details/gzohvetzp.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gajatxgdv.sHtML

[I01] 判断是否匹配
来源：http://m.share.hesvh.cn/Article/details/gpidupywd.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.blog.hesvh.cn/Article/details/gnkrvrppb.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://baike.zdbjq.cn/Article/details/ghvecbkrq.sHtML

JS:   /\d+/.test(s)
来源：http://read.share.zdbjq.cn/Article/details/gncviyrpc.sHtML

TS:   /\d+/.test(s)
来源：http://read.share.hesvh.cn/Article/details/gpbyglpoq.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://read.share.fehbvm.com/Article/details/gfrtaijsr.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://m.share.fehbvm.com/Article/details/gylzcbeij.sHtML

Ruby: s.match?(/\d+/)
来源：http://wap.zdbjq.cn/Article/details/gbkwtcyhb.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.m.share.zdbjq.cn/Article/details/gcpdpsqdc.sHtML

[I02] 提取所有匹配
来源：http://m.share.fehbvm.com/Article/details/gvojnisne.sHtML

Py:   re.findall(r"\d+", s)
来源：http://blog.hesvh.cn/Article/details/gfatqhfzj.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://read.share.fehbvm.com/Article/details/gxgqpboxh.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://blog.zdbjq.cn/Article/details/gsbgrucqv.sHtML

TS:   s.match(/\d+/g)
来源：http://www.m.share.hesvh.cn/Article/details/gfzsedazs.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://read.share.zdbjq.cn/Article/details/glpqadbpi.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://read.share.hesvh.cn/Article/details/gyrvynrsv.sHtML

Ruby: s.scan(/\d+/)
来源：http://mobile.fehbvm.com/Article/details/gidjdbrtu.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://baike.zdbjq.cn/Article/details/gencskacy.sHtML

[I03] 提取捕获分组
来源：http://www.m.share.zdbjq.cn/Article/details/gjiguhflb.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://3g.fehbvm.com/Article/details/gblhpwjqh.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://read.share.zdbjq.cn/Article/details/gyqxpxrrm.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://blog.hesvh.cn/Article/details/gmnrkcszz.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wap.hesvh.cn/Article/details/gjjctaatr.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://mobile.hesvh.cn/Article/details/gyedakiom.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.blog.fehbvm.com/Article/details/ggedlfzjn.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://m.share.hesvh.cn/Article/details/gcdprufxx.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://m.share.hesvh.cn/Article/details/gahapqwpj.sHtML

[I04] 正则替换
来源：http://www.m.share.hesvh.cn/Article/details/gfsvymxlp.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.m.share.zdbjq.cn/Article/details/gcjmfxodh.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mobile.hesvh.cn/Article/details/gqnassrpm.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.share.hesvh.cn/Article/details/gbjiukpea.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://mobile.fehbvm.com/Article/details/gcrfiolao.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://wap.zdbjq.cn/Article/details/ghqczflne.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://mobile.hesvh.cn/Article/details/gzkkrnbcw.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://3g.zdbjq.cn/Article/details/gedxhviwg.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.m.share.zdbjq.cn/Article/details/gowbfacyu.sHtML

[I05] 按正则拆分
来源：http://3g.zdbjq.cn/Article/details/gysntswld.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.blog.fehbvm.com/Article/details/gdfgeysbh.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.blog.fehbvm.com/Article/details/gcqwpimpu.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://wap.zdbjq.cn/Article/details/gdbyjqryq.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://read.share.hesvh.cn/Article/details/gwhkjxncf.sHtML

Java: s.split("\\s*,\\s*")
来源：http://baike.hesvh.cn/Article/details/ggwgqpvje.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://blog.hesvh.cn/Article/details/gtskwpmkp.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.m.share.fehbvm.com/Article/details/gskruaoyn.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.share.zdbjq.cn/Article/details/gsfsuojpa.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://baike.zdbjq.cn/Article/details/gcnywhbwf.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wap.hesvh.cn/Article/details/gydoizgod.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://mobile.hesvh.cn/Article/details/gxvaomesz.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.zdbjq.cn/Article/details/gfluakman.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.hesvh.cn/Article/details/gnfmaxsuc.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://blog.fehbvm.com/Article/details/gstdddaul.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://baike.hesvh.cn/Article/details/ghvhfyxfz.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://baike.fehbvm.com/Article/details/ggtmiriju.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://m.share.zdbjq.cn/Article/details/gumndxmke.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.m.share.zdbjq.cn/Article/details/gjuyocymb.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.m.share.zdbjq.cn/Article/details/gskawjcsc.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mobile.hesvh.cn/Article/details/ghthgkqko.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://m.share.hesvh.cn/Article/details/gnvushjbo.sHtML

TS:   /error/gim
来源：http://www.share.fehbvm.com/Article/details/gbqopflgw.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://baike.hesvh.cn/Article/details/gkuyebhgs.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://baike.hesvh.cn/Article/details/gszjzlokf.sHtML

Ruby: s.scan(/error/i)
来源：http://m.share.zdbjq.cn/Article/details/gustwdwpp.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://m.share.zdbjq.cn/Article/details/gtzzszyax.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://blog.fehbvm.com/Article/details/ginrimjrs.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://blog.hesvh.cn/Article/details/gwjvuqnwg.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://blog.zdbjq.cn/Article/details/gzibyzdsd.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.fehbvm.com/Article/details/gzdnhoxab.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.zdbjq.cn/Article/details/gzwshibhv.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.blog.fehbvm.com/Article/details/gefjpafnc.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://blog.hesvh.cn/Article/details/gpqvbvguk.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://read.share.fehbvm.com/Article/details/gdeyviolb.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://baike.fehbvm.com/Article/details/gwciyrwww.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gjftxbhjn.sHtML

J. 日期与时间
来源：http://read.share.fehbvm.com/Article/details/gsbavuoiq.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/grtxyfmym.sHtML

[J01] 获取当前时间
来源：http://www.m.share.zdbjq.cn/Article/details/gfgfcoifj.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://wap.zdbjq.cn/Article/details/gkmnreupc.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://blog.zdbjq.cn/Article/details/grexffbql.sHtML

JS:   new Date();  Date.now()
来源：http://3g.fehbvm.com/Article/details/gkjhnqwfu.sHtML

TS:   new Date();  Date.now()
来源：http://blog.fehbvm.com/Article/details/gkvncbhjj.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://mobile.zdbjq.cn/Article/details/gwedxdonu.sHtML

Go:   time.Now()
来源：http://m.share.zdbjq.cn/Article/details/gfrqyqetk.sHtML

Ruby: Time.now
来源：http://wap.zdbjq.cn/Article/details/gsknaiowf.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://m.share.fehbvm.com/Article/details/gfubtxann.sHtML

[J02] 格式化输出
来源：http://wap.hesvh.cn/Article/details/gkgtqupvg.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.fehbvm.com/Article/details/gcigiqwff.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.share.zdbjq.cn/Article/details/gqoaywxzi.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://3g.zdbjq.cn/Article/details/gmkjftcrt.sHtML

TS:   d.toISOString()
来源：http://www.share.fehbvm.com/Article/details/gxqhvsxoo.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://m.share.hesvh.cn/Article/details/gkzbindeo.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://3g.zdbjq.cn/Article/details/gitphmfmj.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.hesvh.cn/Article/details/giuzneaev.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://read.share.hesvh.cn/Article/details/gsejeeeqo.sHtML

[J03] 字符串解析为日期
来源：http://baike.zdbjq.cn/Article/details/gtfvfntht.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.blog.fehbvm.com/Article/details/gkvamtcee.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://3g.hesvh.cn/Article/details/gtdmrtokj.sHtML

JS:   new Date("2024-01-02")
来源：http://www.m.share.fehbvm.com/Article/details/gxixanceo.sHtML

TS:   new Date("2024-01-02")
来源：http://www.share.zdbjq.cn/Article/details/gpiepdhec.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://mobile.hesvh.cn/Article/details/gyadxtwvx.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://m.share.hesvh.cn/Article/details/gotmadodf.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://read.share.zdbjq.cn/Article/details/gzsbshilm.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://blog.hesvh.cn/Article/details/gmrqtiidv.sHtML

[J04] 时间戳与日期互转
来源：http://mobile.fehbvm.com/Article/details/gwtdbfjpj.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mobile.fehbvm.com/Article/details/guhtspufk.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.share.zdbjq.cn/Article/details/gzeolxsml.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://baike.fehbvm.com/Article/details/gznyojhdm.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://blog.zdbjq.cn/Article/details/gfiiggjbv.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.m.share.hesvh.cn/Article/details/gexrcxkqt.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://read.share.fehbvm.com/Article/details/gahvtzvrt.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://3g.hesvh.cn/Article/details/gsvchriwk.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://m.share.hesvh.cn/Article/details/ghypvkhre.sHtML

[J05] 时间加减（加 7 天）
来源：http://wap.zdbjq.cn/Article/details/gqomwcajg.sHtML

Py:   now + timedelta(days=7)
来源：http://www.m.share.fehbvm.com/Article/details/gcbsayczb.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://m.share.zdbjq.cn/Article/details/gigvueihx.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.fehbvm.com/Article/details/gyidfucbe.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.zdbjq.cn/Article/details/gdkfxdqap.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://wap.zdbjq.cn/Article/details/gteejkhrp.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://blog.zdbjq.cn/Article/details/gcsufcpne.sHtML

Ruby: Time.now + 7 * 86400
来源：http://blog.fehbvm.com/Article/details/gmbhnsgmy.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.share.fehbvm.com/Article/details/gpgzfjyry.sHtML

[J06] 计算两时间之差
来源：http://3g.fehbvm.com/Article/details/gropezsaq.sHtML

Py:   (end - start).total_seconds()
来源：http://www.blog.fehbvm.com/Article/details/giuugctjn.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.share.fehbvm.com/Article/details/gnhmuilcn.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://m.share.fehbvm.com/Article/details/gztcxfvvw.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mobile.zdbjq.cn/Article/details/gfowuisyt.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://wap.zdbjq.cn/Article/details/goemlgufx.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.m.share.fehbvm.com/Article/details/gzyiqkuay.sHtML

Ruby: end - start                 # 返回秒数
来源：http://baike.fehbvm.com/Article/details/gueuodmcb.sHtML

C#:   (end - start).TotalSeconds
来源：http://mobile.hesvh.cn/Article/details/gmaprukzu.sHtML

[J07] 比较两个日期
来源：http://mobile.fehbvm.com/Article/details/ghphllwmq.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://m.share.fehbvm.com/Article/details/gsafnvndr.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://wap.zdbjq.cn/Article/details/gfprtsbju.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://mobile.hesvh.cn/Article/details/gpebozcwk.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://blog.zdbjq.cn/Article/details/giasgwole.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.share.hesvh.cn/Article/details/gjosdrnnd.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://m.share.zdbjq.cn/Article/details/gbhcsfeah.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://wap.zdbjq.cn/Article/details/gamhlzxmt.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.blog.fehbvm.com/Article/details/gewpduabh.sHtML

[J08] 提取年月日与星期
来源：http://www.share.zdbjq.cn/Article/details/gwmyrdrtb.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wap.zdbjq.cn/Article/details/gbhiudztx.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://baike.zdbjq.cn/Article/details/gzeoacfdr.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wap.zdbjq.cn/Article/details/gysdmydkh.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://blog.zdbjq.cn/Article/details/grqvxbqzz.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.share.hesvh.cn/Article/details/getdxkigs.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.share.zdbjq.cn/Article/details/glxcoszga.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://read.share.zdbjq.cn/Article/details/gjqqueyoq.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://read.share.hesvh.cn/Article/details/gxgweigcv.sHtML

[J09] 时区处理
来源：http://wap.fehbvm.com/Article/details/gufkxiytk.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://read.share.hesvh.cn/Article/details/gukymrtaf.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://3g.zdbjq.cn/Article/details/gbevzxufv.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.zdbjq.cn/Article/details/guqzodvfz.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.fehbvm.com/Article/details/gwvqrkytx.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.blog.fehbvm.com/Article/details/gztedhowz.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.m.share.zdbjq.cn/Article/details/gkxwnozvb.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://blog.fehbvm.com/Article/details/guczzywzk.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mobile.hesvh.cn/Article/details/guskwfrrt.sHtML

[J10] 取今天 / 本月第一天
来源：http://blog.fehbvm.com/Article/details/glssaoxql.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.m.share.fehbvm.com/Article/details/ghneyxtrx.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.share.fehbvm.com/Article/details/gcnbsbioh.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://baike.zdbjq.cn/Article/details/goyojhdcn.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mobile.fehbvm.com/Article/details/gqfhkhqfl.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wap.hesvh.cn/Article/details/gpkidiukv.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mobile.hesvh.cn/Article/details/gqzoaybem.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mobile.fehbvm.com/Article/details/gzpffwfoe.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.m.share.hesvh.cn/Article/details/gaewydqzv.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gdgqihyer.sHtML

K. JSON 与序列化
来源：http://www.m.share.zdbjq.cn/Article/details/gdcjvhaob.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gzsrdxwpp.sHtML

[K01] 对象转 JSON 字符串
来源：http://blog.hesvh.cn/Article/details/gpqayanhe.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://3g.fehbvm.com/Article/details/glrnpufts.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mobile.zdbjq.cn/Article/details/gelfezkba.sHtML

JS:   JSON.stringify(obj)
来源：http://m.share.hesvh.cn/Article/details/gipjbtjyu.sHtML

TS:   JSON.stringify(obj)
来源：http://www.blog.hesvh.cn/Article/details/grxoxkxol.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://read.share.fehbvm.com/Article/details/gomywmsyc.sHtML

Go:   json.Marshal(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gsqicpsvf.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://m.share.zdbjq.cn/Article/details/gjqxnfgnp.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gzqpujzer.sHtML

[K02] JSON 字符串转对象
来源：http://www.m.share.hesvh.cn/Article/details/grdxxwflh.sHtML

Py:   json.loads(s)
来源：http://read.share.hesvh.cn/Article/details/gittclazr.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://m.share.hesvh.cn/Article/details/gxsuadnir.sHtML

JS:   JSON.parse(s)
来源：http://www.blog.fehbvm.com/Article/details/grdgwkurc.sHtML

TS:   JSON.parse(s)
来源：http://blog.hesvh.cn/Article/details/gxxdawqon.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://3g.hesvh.cn/Article/details/goqwklvle.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://wap.zdbjq.cn/Article/details/gqugfromo.sHtML

Ruby: JSON.parse(s)
来源：http://www.m.share.hesvh.cn/Article/details/gelpoavaa.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mobile.zdbjq.cn/Article/details/glaxvdodt.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://blog.hesvh.cn/Article/details/gyzftquld.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://baike.fehbvm.com/Article/details/gsssjpvfe.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mobile.fehbvm.com/Article/details/gdhxkkvan.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.hesvh.cn/Article/details/gknuvjhpm.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.fehbvm.com/Article/details/gmzyjcrre.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://3g.fehbvm.com/Article/details/gxzufcrtn.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.blog.hesvh.cn/Article/details/gcptvyszy.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://wap.zdbjq.cn/Article/details/goahvvroy.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://3g.fehbvm.com/Article/details/gwwgxlabw.sHtML

[K04] 读取 JSON 文件
来源：http://3g.zdbjq.cn/Article/details/gflgqpnds.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://blog.fehbvm.com/Article/details/gjfeaphqe.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://blog.zdbjq.cn/Article/details/gufvswseq.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.fehbvm.com/Article/details/giurqbynf.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.fehbvm.com/Article/details/gjjysnwav.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://baike.fehbvm.com/Article/details/gvuevmuxl.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://read.share.zdbjq.cn/Article/details/glusjjtme.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://baike.hesvh.cn/Article/details/gzeltskyb.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://read.share.zdbjq.cn/Article/details/gyyrxntup.sHtML

[K05] 深拷贝对象
来源：http://wap.fehbvm.com/Article/details/gaetfybtb.sHtML


<!-- 参考信息 -->