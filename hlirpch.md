代发 wailian999

Ruby: Color = %i[red green].freeze
来源：http://mobile.fanxiaobao.xyz/Article/details/gycluvtwp.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.fanxiaobao.xyz/Article/details/gqlladrbk.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.fanxiaobao.xyz/Article/details/gyrgcxjsu.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzoihfbag.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.fanxiaobao.xyz/Article/details/gmvmepyks.sHtML

JS:   Object.entries(obj)
来源：http://3g.fanxiaobao.xyz/Article/details/gavhmaehf.sHtML

TS:   Object.entries(obj)
来源：http://mobile.fanxiaobao.xyz/Article/details/gubjyygcp.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.fanxiaobao.xyz/Article/details/gqpvcxwgz.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.fanxiaobao.xyz/Article/details/gfbwcqylt.sHtML

Ruby: obj.instance_variables
来源：http://read.share.fanxiaobao.xyz/Article/details/gmrnepdrm.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gumgneebe.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbgovhbgc.sHtML

H. 异常与错误处理
来源：http://mobile.fanxiaobao.xyz/Article/details/gimvowmfy.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gepbryfdj.sHtML

[H01] try / catch 基础
来源：http://m.share.fanxiaobao.xyz/Article/details/gwtqjthsj.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gapymbnzw.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gxpmyszth.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gyfhaohew.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcowofyni.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gwkobiwco.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.fanxiaobao.xyz/Article/details/genqsobbc.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxbddduak.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.fanxiaobao.xyz/Article/details/gevoswxas.sHtML

[H02] finally / ensure 收尾
来源：http://3g.fanxiaobao.xyz/Article/details/gpxvqkmdu.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://baike.fanxiaobao.xyz/Article/details/gcwgjsdjh.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/guzvjcuuu.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://3g.fanxiaobao.xyz/Article/details/gzomzxyly.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gcaeymzno.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqvrwjlwo.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.share.fanxiaobao.xyz/Article/details/gdlvldwbg.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.fanxiaobao.xyz/Article/details/gwhrldnbd.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gqegfsdrs.sHtML

[H03] 主动抛出异常
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkmyrtula.sHtML

Py:   raise ValueError("错误信息")
来源：http://baike.fanxiaobao.xyz/Article/details/gubskmyfm.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdawqpxec.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.fanxiaobao.xyz/Article/details/gmzaiyqfb.sHtML

TS:   throw new Error("错误信息");
来源：http://mobile.fanxiaobao.xyz/Article/details/gspwczcij.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.fanxiaobao.xyz/Article/details/ghiblukdx.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnfmeupjk.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfmdlvohp.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://wap.fanxiaobao.xyz/Article/details/gslacihno.sHtML

[H04] 自定义异常类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnybwcuwa.sHtML

Py:   class MyError(Exception): pass
来源：http://www.share.fanxiaobao.xyz/Article/details/gbejfhkdh.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gkbphffsd.sHtML

JS:   class MyError extends Error {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkdcxjjls.sHtML

TS:   class MyError extends Error {}
来源：http://blog.fanxiaobao.xyz/Article/details/ggbkanlvj.sHtML

Java: class MyException extends RuntimeException {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gcfysqstf.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://read.share.fanxiaobao.xyz/Article/details/gbkojbvnb.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.fanxiaobao.xyz/Article/details/gsocwnmmf.sHtML

C#:   class MyException : Exception {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvxvvwtha.sHtML

[H05] 捕获特定类型
来源：http://mobile.fanxiaobao.xyz/Article/details/gwkypkyli.sHtML

Py:   except ValueError as e:
来源：http://m.share.fanxiaobao.xyz/Article/details/glbtlcbyc.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.fanxiaobao.xyz/Article/details/gjlnvrmhk.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://baike.fanxiaobao.xyz/Article/details/gjnjagzfq.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzxlriyys.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://blog.fanxiaobao.xyz/Article/details/gyhaeyous.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wap.fanxiaobao.xyz/Article/details/gistdsgqi.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.fanxiaobao.xyz/Article/details/gzhlfqmfu.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wap.fanxiaobao.xyz/Article/details/gsnyyoddo.sHtML

[H06] 可选值 / 空值安全访问
来源：http://wap.fanxiaobao.xyz/Article/details/ghevspptk.sHtML

Py:   value = d.get("k") or default
来源：http://www.share.fanxiaobao.xyz/Article/details/gtqhgdnhd.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://3g.fanxiaobao.xyz/Article/details/gkogyyeox.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxxcfaeui.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://mobile.fanxiaobao.xyz/Article/details/ggslrymcp.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://baike.fanxiaobao.xyz/Article/details/gfjpjhwtm.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsdnzxfex.sHtML

Ruby: d&.dig(:a, :b)
来源：http://m.share.fanxiaobao.xyz/Article/details/ggddqakaf.sHtML

C#:   obj?.A?.B ?? default
来源：http://mobile.fanxiaobao.xyz/Article/details/gprshnpxc.sHtML

[H07] 断言
来源：http://m.share.fanxiaobao.xyz/Article/details/gybqssxbb.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.share.fanxiaobao.xyz/Article/details/gmybvsvlg.sHtML

PHP:  assert($x > 0);
来源：http://wap.fanxiaobao.xyz/Article/details/gyuckadvl.sHtML

JS:   console.assert(x > 0);
来源：http://blog.fanxiaobao.xyz/Article/details/gcjrprcag.sHtML

TS:   console.assert(x > 0);
来源：http://3g.fanxiaobao.xyz/Article/details/gmizgofzf.sHtML

Java: assert x > 0 : "必须为正";
来源：http://baike.fanxiaobao.xyz/Article/details/gseuhkaga.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://m.share.fanxiaobao.xyz/Article/details/grmfshdcw.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.share.fanxiaobao.xyz/Article/details/gtksuuano.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geezghzmf.sHtML

[H08] 获取错误信息与堆栈
来源：http://baike.fanxiaobao.xyz/Article/details/gurzwggyz.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://mobile.fanxiaobao.xyz/Article/details/gomdnxuvo.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://blog.fanxiaobao.xyz/Article/details/gwnbevssb.sHtML

JS:   e.message;  e.stack
来源：http://read.share.fanxiaobao.xyz/Article/details/gtmjffggv.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://wap.fanxiaobao.xyz/Article/details/grqqnpjoq.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://m.share.fanxiaobao.xyz/Article/details/ggsggnnoa.sHtML

Go:   err.Error()
来源：http://blog.fanxiaobao.xyz/Article/details/giqtbgnna.sHtML

Ruby: e.message;  e.backtrace
来源：http://m.share.fanxiaobao.xyz/Article/details/gumpufira.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.blog.fanxiaobao.xyz/Article/details/gesaqzljz.sHtML

[H09] 带错误码的异常
来源：http://wap.fanxiaobao.xyz/Article/details/guqorhqpl.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.share.fanxiaobao.xyz/Article/details/gbhjalojq.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://blog.fanxiaobao.xyz/Article/details/gxruezjez.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gufxpafgl.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://read.share.fanxiaobao.xyz/Article/details/gkmoyiyec.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghkutoddn.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://3g.fanxiaobao.xyz/Article/details/gdymfrhvn.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://m.share.fanxiaobao.xyz/Article/details/gwdqtnjzf.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://baike.fanxiaobao.xyz/Article/details/ggqjatvij.sHtML

[H10] 资源自动释放
来源：http://blog.fanxiaobao.xyz/Article/details/gqeeoyrsj.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.share.fanxiaobao.xyz/Article/details/gfrehgqlj.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.share.fanxiaobao.xyz/Article/details/gxjxjjezp.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbvaglwzp.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.fanxiaobao.xyz/Article/details/gdqzzsspm.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://blog.fanxiaobao.xyz/Article/details/gaaobkudv.sHtML

Go:   defer f.Close()
来源：http://m.share.fanxiaobao.xyz/Article/details/gyhfqstmb.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://read.share.fanxiaobao.xyz/Article/details/griazchqm.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gafkdrmie.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gtfpchtqz.sHtML

I. 正则表达式
来源：http://3g.fanxiaobao.xyz/Article/details/gdqdmwhqg.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/geyyndduu.sHtML

[I01] 判断是否匹配
来源：http://mobile.fanxiaobao.xyz/Article/details/gmrphsstx.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gehcvwmha.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://mobile.fanxiaobao.xyz/Article/details/ghmmwnrbx.sHtML

JS:   /\d+/.test(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gctqggqxk.sHtML

TS:   /\d+/.test(s)
来源：http://blog.fanxiaobao.xyz/Article/details/goguqduml.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://baike.fanxiaobao.xyz/Article/details/giangjfsl.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wap.fanxiaobao.xyz/Article/details/gjholfxcq.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.share.fanxiaobao.xyz/Article/details/gkjmxcsmh.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://m.share.fanxiaobao.xyz/Article/details/gcbsispsi.sHtML

[I02] 提取所有匹配
来源：http://mobile.fanxiaobao.xyz/Article/details/geyljtbhx.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzvkhfeqp.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://3g.fanxiaobao.xyz/Article/details/gbidgepsu.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.share.fanxiaobao.xyz/Article/details/ggcbehljc.sHtML

TS:   s.match(/\d+/g)
来源：http://read.share.fanxiaobao.xyz/Article/details/gkfgsxvyg.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://3g.fanxiaobao.xyz/Article/details/gxidedybo.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghjbmbjsn.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gguouukdu.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://blog.fanxiaobao.xyz/Article/details/gqywsivcq.sHtML

[I03] 提取捕获分组
来源：http://www.share.fanxiaobao.xyz/Article/details/gpzekcjrd.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gbxctrwte.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://blog.fanxiaobao.xyz/Article/details/gbkmogydk.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wap.fanxiaobao.xyz/Article/details/gwhitfyob.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://3g.fanxiaobao.xyz/Article/details/gdctvwxfk.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://3g.fanxiaobao.xyz/Article/details/gtnalalvy.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://blog.fanxiaobao.xyz/Article/details/guzjuokce.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.share.fanxiaobao.xyz/Article/details/gagwjrctl.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://baike.fanxiaobao.xyz/Article/details/griodfpac.sHtML

[I04] 正则替换
来源：http://3g.fanxiaobao.xyz/Article/details/gjqekfurr.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfgagbemq.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://baike.fanxiaobao.xyz/Article/details/gcpjisvar.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbacuxzha.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://mobile.fanxiaobao.xyz/Article/details/gpjyguumn.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://read.share.fanxiaobao.xyz/Article/details/gmestpynn.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://mobile.fanxiaobao.xyz/Article/details/gjvjynjpc.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://blog.fanxiaobao.xyz/Article/details/gnbytnusc.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://3g.fanxiaobao.xyz/Article/details/grykzirwe.sHtML

[I05] 按正则拆分
来源：http://baike.fanxiaobao.xyz/Article/details/gifcnlmpc.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://baike.fanxiaobao.xyz/Article/details/gxapceqmf.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://3g.fanxiaobao.xyz/Article/details/gfkscrxqd.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsduyrwqi.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://3g.fanxiaobao.xyz/Article/details/gyhwdkgvi.sHtML

Java: s.split("\\s*,\\s*")
来源：http://mobile.fanxiaobao.xyz/Article/details/gzssusibj.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://blog.fanxiaobao.xyz/Article/details/gpwitalef.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gogkdepfr.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wap.fanxiaobao.xyz/Article/details/gduktkmog.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mobile.fanxiaobao.xyz/Article/details/ggdzkbqze.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://read.share.fanxiaobao.xyz/Article/details/gimsfslnl.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghlouiobg.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.fanxiaobao.xyz/Article/details/gncgtrlux.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcelioalr.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.share.fanxiaobao.xyz/Article/details/gysdbhgrr.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbpalnqlq.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://baike.fanxiaobao.xyz/Article/details/gxxkzgbqk.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gepikcgdh.sHtML

[I07] 忽略大小写与多行模式
来源：http://blog.fanxiaobao.xyz/Article/details/ggknrjbyr.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzptwaukg.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wap.fanxiaobao.xyz/Article/details/gbvtoyyqg.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://3g.fanxiaobao.xyz/Article/details/gccllcphd.sHtML

TS:   /error/gim
来源：http://www.share.fanxiaobao.xyz/Article/details/gdhuwklnh.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mobile.fanxiaobao.xyz/Article/details/gxhqqbgza.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mobile.fanxiaobao.xyz/Article/details/gfyzjzcqo.sHtML

Ruby: s.scan(/error/i)
来源：http://3g.fanxiaobao.xyz/Article/details/gslrdygjv.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mobile.fanxiaobao.xyz/Article/details/gamdwaofd.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://3g.fanxiaobao.xyz/Article/details/gsutsjysf.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://3g.fanxiaobao.xyz/Article/details/gwzpyqxkj.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxtcnjeew.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.fanxiaobao.xyz/Article/details/gqtmqucua.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnbjjoocp.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.share.fanxiaobao.xyz/Article/details/gpgyfmjeq.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvvbyjrov.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.share.fanxiaobao.xyz/Article/details/gsmjrkvow.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://read.share.fanxiaobao.xyz/Article/details/ggdvosnvf.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gmwklmhtm.sHtML

J. 日期与时间
来源：http://blog.fanxiaobao.xyz/Article/details/ggjrxhxlj.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gbqvuqpmy.sHtML

[J01] 获取当前时间
来源：http://read.share.fanxiaobao.xyz/Article/details/gtvfcroil.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://mobile.fanxiaobao.xyz/Article/details/gaxlkmpta.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://wap.fanxiaobao.xyz/Article/details/gyisigmkp.sHtML

JS:   new Date();  Date.now()
来源：http://m.share.fanxiaobao.xyz/Article/details/gvmqoeezm.sHtML

TS:   new Date();  Date.now()
来源：http://baike.fanxiaobao.xyz/Article/details/gciljsslp.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.share.fanxiaobao.xyz/Article/details/gyavkrpwv.sHtML

Go:   time.Now()
来源：http://mobile.fanxiaobao.xyz/Article/details/gkofrikmh.sHtML

Ruby: Time.now
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmkvpoxoc.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://read.share.fanxiaobao.xyz/Article/details/ghjpgtmuw.sHtML

[J02] 格式化输出
来源：http://3g.fanxiaobao.xyz/Article/details/gzwzrhjki.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdzrcdjxs.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://m.share.fanxiaobao.xyz/Article/details/gzhldowtq.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://blog.fanxiaobao.xyz/Article/details/gvqzmjkln.sHtML

TS:   d.toISOString()
来源：http://mobile.fanxiaobao.xyz/Article/details/grxcazvvz.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mobile.fanxiaobao.xyz/Article/details/gpdjfggia.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.blog.fanxiaobao.xyz/Article/details/gexhxzclj.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqohacmro.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://m.share.fanxiaobao.xyz/Article/details/gocfvkjhe.sHtML

[J03] 字符串解析为日期
来源：http://www.share.fanxiaobao.xyz/Article/details/grtjlkydt.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://baike.fanxiaobao.xyz/Article/details/gfuxhomrr.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbofedske.sHtML

JS:   new Date("2024-01-02")
来源：http://baike.fanxiaobao.xyz/Article/details/gtrxezuhu.sHtML

TS:   new Date("2024-01-02")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkjleheqt.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://wap.fanxiaobao.xyz/Article/details/gonkzkalb.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmqpommij.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://baike.fanxiaobao.xyz/Article/details/gsmkybnvs.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.share.fanxiaobao.xyz/Article/details/gilulaiad.sHtML

[J04] 时间戳与日期互转
来源：http://www.share.fanxiaobao.xyz/Article/details/gfhngnjxz.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://m.share.fanxiaobao.xyz/Article/details/gdwxbyihq.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://read.share.fanxiaobao.xyz/Article/details/gvoxlwrqt.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfrdcjplr.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gczoukdts.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.share.fanxiaobao.xyz/Article/details/gwbnhiiyj.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.share.fanxiaobao.xyz/Article/details/gbwdukyya.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://3g.fanxiaobao.xyz/Article/details/gzymwohur.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://m.share.fanxiaobao.xyz/Article/details/ggzbrrpwa.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.share.fanxiaobao.xyz/Article/details/gpycpoctp.sHtML

Py:   now + timedelta(days=7)
来源：http://mobile.fanxiaobao.xyz/Article/details/gakqkmdai.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://blog.fanxiaobao.xyz/Article/details/gqweuzioa.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.fanxiaobao.xyz/Article/details/gveygzbdy.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.fanxiaobao.xyz/Article/details/gmulazopx.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://mobile.fanxiaobao.xyz/Article/details/gmwakbnnv.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mobile.fanxiaobao.xyz/Article/details/gmzlrgtev.sHtML

Ruby: Time.now + 7 * 86400
来源：http://baike.fanxiaobao.xyz/Article/details/ganyjeeeh.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://wap.fanxiaobao.xyz/Article/details/gafmnkyqp.sHtML

[J06] 计算两时间之差
来源：http://m.share.fanxiaobao.xyz/Article/details/glohxscth.sHtML

Py:   (end - start).total_seconds()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxhcxkzcg.sHtML

PHP:  $end->diff($start)->days;
来源：http://mobile.fanxiaobao.xyz/Article/details/gqqvqxihq.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mobile.fanxiaobao.xyz/Article/details/gsxhxkkmy.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.share.fanxiaobao.xyz/Article/details/gkblhqilv.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://3g.fanxiaobao.xyz/Article/details/glengpbbw.sHtML

Go:   end.Sub(start).Hours()
来源：http://3g.fanxiaobao.xyz/Article/details/gsezzpvyy.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.share.fanxiaobao.xyz/Article/details/gcpcldsaf.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.share.fanxiaobao.xyz/Article/details/gzupoakkz.sHtML

[J07] 比较两个日期
来源：http://m.share.fanxiaobao.xyz/Article/details/gzkzcvmxm.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://blog.fanxiaobao.xyz/Article/details/gxdtrlfnt.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.share.fanxiaobao.xyz/Article/details/garkwglfm.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://read.share.fanxiaobao.xyz/Article/details/ggiyanodn.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.share.fanxiaobao.xyz/Article/details/gjugozvqr.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gphienrse.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcveyanap.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://blog.fanxiaobao.xyz/Article/details/gjzvscujl.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.share.fanxiaobao.xyz/Article/details/gefncdoux.sHtML

[J08] 提取年月日与星期
来源：http://3g.fanxiaobao.xyz/Article/details/gnxyaosfd.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjevijbko.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqzgphrhw.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://blog.fanxiaobao.xyz/Article/details/gprkcfqqm.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://m.share.fanxiaobao.xyz/Article/details/gfbdpdbme.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://blog.fanxiaobao.xyz/Article/details/gymrbpqds.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.blog.fanxiaobao.xyz/Article/details/guwmcujuk.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://blog.fanxiaobao.xyz/Article/details/gbtlqrpsx.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://baike.fanxiaobao.xyz/Article/details/gmoimfuos.sHtML

[J09] 时区处理
来源：http://blog.fanxiaobao.xyz/Article/details/gjctfavlj.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.share.fanxiaobao.xyz/Article/details/gxlwkkagt.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://m.share.fanxiaobao.xyz/Article/details/guwkljhon.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.fanxiaobao.xyz/Article/details/gntxxdyno.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.fanxiaobao.xyz/Article/details/gyvxglozy.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mobile.fanxiaobao.xyz/Article/details/gcsnczafh.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnyjqmsrx.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://m.share.fanxiaobao.xyz/Article/details/gnvvtnmko.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvqylfkbb.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.share.fanxiaobao.xyz/Article/details/gkoyjpeno.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://blog.fanxiaobao.xyz/Article/details/glpohwhny.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://blog.fanxiaobao.xyz/Article/details/gsfzljbhv.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gqkulwile.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://blog.fanxiaobao.xyz/Article/details/gysrosdwv.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gqnnlfcaw.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.share.fanxiaobao.xyz/Article/details/gpidkzotd.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://read.share.fanxiaobao.xyz/Article/details/gkibtxdgw.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gozmvztfq.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gzlzkfsqx.sHtML

K. JSON 与序列化
来源：http://baike.fanxiaobao.xyz/Article/details/gdogjtqkj.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gxirlhhao.sHtML

[K01] 对象转 JSON 字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gjvflmcwk.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://3g.fanxiaobao.xyz/Article/details/gvavsuhao.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wap.fanxiaobao.xyz/Article/details/gdcmibtoe.sHtML

JS:   JSON.stringify(obj)
来源：http://blog.fanxiaobao.xyz/Article/details/gkfwcxfff.sHtML

TS:   JSON.stringify(obj)
来源：http://mobile.fanxiaobao.xyz/Article/details/gawoacsph.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.share.fanxiaobao.xyz/Article/details/ggjtsuxrb.sHtML

Go:   json.Marshal(obj)
来源：http://m.share.fanxiaobao.xyz/Article/details/gmylvfxsd.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcgewkbsp.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gplzzyswc.sHtML

[K02] JSON 字符串转对象
来源：http://read.share.fanxiaobao.xyz/Article/details/guhaihdhs.sHtML

Py:   json.loads(s)
来源：http://blog.fanxiaobao.xyz/Article/details/gulsdpcwa.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://blog.fanxiaobao.xyz/Article/details/ghmaklaig.sHtML

JS:   JSON.parse(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/grgdrykdo.sHtML

TS:   JSON.parse(s)
来源：http://baike.fanxiaobao.xyz/Article/details/gktezthlj.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://read.share.fanxiaobao.xyz/Article/details/ggiwpswuq.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://3g.fanxiaobao.xyz/Article/details/gugihqkpe.sHtML

Ruby: JSON.parse(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gdoufmwuo.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gexrunyog.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://blog.fanxiaobao.xyz/Article/details/gunqbaggx.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://read.share.fanxiaobao.xyz/Article/details/gvbdvbkfo.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://m.share.fanxiaobao.xyz/Article/details/gkqjgimqh.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://baike.fanxiaobao.xyz/Article/details/gtcdirbbg.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/giesdlyqb.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.share.fanxiaobao.xyz/Article/details/gwmjzqepv.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.share.fanxiaobao.xyz/Article/details/glzeepwge.sHtML


<!-- 参考信息 -->