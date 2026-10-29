代发 wailian999

PHP:  get_object_vars($obj);
来源：http://read.share.fehbvm.com/Article/details/gnlfztcjw.sHtML

JS:   Object.entries(obj)
来源：http://m.share.hesvh.cn/Article/details/gxbqjujhc.sHtML

TS:   Object.entries(obj)
来源：http://read.share.zdbjq.cn/Article/details/gpssrurqm.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://m.share.hesvh.cn/Article/details/gbelufeqv.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.hesvh.cn/Article/details/goejmdbmx.sHtML

Ruby: obj.instance_variables
来源：http://www.share.hesvh.cn/Article/details/gtqtsoyiw.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.zdbjq.cn/Article/details/giblafqld.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/giezwgjwg.sHtML

H. 异常与错误处理
来源：http://www.blog.zdbjq.cn/Article/details/gqetqsvvx.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/grmuphrhf.sHtML

[H01] try / catch 基础
来源：http://mobile.hesvh.cn/Article/details/gdnwnduha.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.zdbjq.cn/Article/details/gjjvtjton.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.fehbvm.com/Article/details/gxayklftm.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.share.fehbvm.com/Article/details/gxftfktju.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mobile.fehbvm.com/Article/details/ggpolpptd.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mobile.fehbvm.com/Article/details/gmfdzbgep.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://read.share.hesvh.cn/Article/details/gzpoxpmtj.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.m.share.zdbjq.cn/Article/details/gamhsijmm.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.m.share.fehbvm.com/Article/details/gptxyphbz.sHtML

[H02] finally / ensure 收尾
来源：http://mobile.zdbjq.cn/Article/details/giooizayi.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://3g.zdbjq.cn/Article/details/guhzfervz.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.hesvh.cn/Article/details/gnliszfdq.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/gsfwhthvy.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.share.zdbjq.cn/Article/details/geqpzrdnr.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.zdbjq.cn/Article/details/gxrraxali.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.zdbjq.cn/Article/details/gfxligvoa.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://3g.hesvh.cn/Article/details/gfbcglrvk.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://3g.hesvh.cn/Article/details/gzlpdcgmn.sHtML

[H03] 主动抛出异常
来源：http://mobile.zdbjq.cn/Article/details/glidqlxeu.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.fehbvm.com/Article/details/gpfojawkl.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mobile.zdbjq.cn/Article/details/gqjbkrgya.sHtML

JS:   throw new Error("错误信息");
来源：http://www.share.zdbjq.cn/Article/details/grrntbzve.sHtML

TS:   throw new Error("错误信息");
来源：http://mobile.fehbvm.com/Article/details/gecaswgnr.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.fehbvm.com/Article/details/gjbarpqdk.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.share.fehbvm.com/Article/details/gpdssrerf.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://baike.fehbvm.com/Article/details/gzzifaway.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://blog.zdbjq.cn/Article/details/gsncvthwz.sHtML

[H04] 自定义异常类型
来源：http://m.share.zdbjq.cn/Article/details/gohgwdmqv.sHtML

Py:   class MyError(Exception): pass
来源：http://www.blog.zdbjq.cn/Article/details/gictcprbc.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://mobile.hesvh.cn/Article/details/ghxafjwpt.sHtML

JS:   class MyError extends Error {}
来源：http://m.share.zdbjq.cn/Article/details/gkbdxiupg.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.fehbvm.com/Article/details/guudgiqfc.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.blog.fehbvm.com/Article/details/gvplegyld.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.blog.hesvh.cn/Article/details/gcudcxzek.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.fehbvm.com/Article/details/gowtyojbr.sHtML

C#:   class MyException : Exception {}
来源：http://3g.zdbjq.cn/Article/details/gteghsnnx.sHtML

[H05] 捕获特定类型
来源：http://blog.fehbvm.com/Article/details/gejiawhrk.sHtML

Py:   except ValueError as e:
来源：http://www.share.zdbjq.cn/Article/details/gkljmukdv.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.blog.zdbjq.cn/Article/details/gxkeqylgf.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.blog.fehbvm.com/Article/details/gluvqvxgf.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://mobile.fehbvm.com/Article/details/gitdnnhjp.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://blog.fehbvm.com/Article/details/gllnvbpnx.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.blog.zdbjq.cn/Article/details/girfhmzvm.sHtML

Ruby: rescue ArgumentError => e
来源：http://wap.hesvh.cn/Article/details/gzdspjjia.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://baike.fehbvm.com/Article/details/gytgljzhc.sHtML

[H06] 可选值 / 空值安全访问
来源：http://wap.fehbvm.com/Article/details/gxjybxagr.sHtML

Py:   value = d.get("k") or default
来源：http://wap.zdbjq.cn/Article/details/gisagbfhh.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.share.zdbjq.cn/Article/details/gxjwlhipb.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://3g.hesvh.cn/Article/details/gzcmdwesr.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://m.share.hesvh.cn/Article/details/gitpqjdpu.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://read.share.zdbjq.cn/Article/details/gcanydzak.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://read.share.hesvh.cn/Article/details/goeupgovp.sHtML

Ruby: d&.dig(:a, :b)
来源：http://baike.zdbjq.cn/Article/details/gvvhugarn.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.blog.hesvh.cn/Article/details/guryrztmk.sHtML

[H07] 断言
来源：http://m.share.zdbjq.cn/Article/details/gjhxvksgr.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.blog.hesvh.cn/Article/details/gbifcuqpg.sHtML

PHP:  assert($x > 0);
来源：http://blog.hesvh.cn/Article/details/gqqmjrbsn.sHtML

JS:   console.assert(x > 0);
来源：http://mobile.zdbjq.cn/Article/details/gcfoxonrq.sHtML

TS:   console.assert(x > 0);
来源：http://read.share.fehbvm.com/Article/details/gmdevnvvd.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.zdbjq.cn/Article/details/gcwcebhim.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://3g.fehbvm.com/Article/details/glcdbkqie.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://m.share.hesvh.cn/Article/details/gfeoenxoe.sHtML

C#:   Debug.Assert(x > 0);
来源：http://blog.zdbjq.cn/Article/details/gtrwhmrrt.sHtML

[H08] 获取错误信息与堆栈
来源：http://wap.hesvh.cn/Article/details/glohycrkc.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://read.share.zdbjq.cn/Article/details/ghiyrzpsl.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.share.fehbvm.com/Article/details/glfbmtolh.sHtML

JS:   e.message;  e.stack
来源：http://www.blog.fehbvm.com/Article/details/gnltjksfr.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://baike.zdbjq.cn/Article/details/gxcjujdix.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://blog.fehbvm.com/Article/details/gpizyjeaa.sHtML

Go:   err.Error()
来源：http://read.share.hesvh.cn/Article/details/gzrxepgbw.sHtML

Ruby: e.message;  e.backtrace
来源：http://m.share.fehbvm.com/Article/details/giogqrell.sHtML

C#:   e.Message;  e.StackTrace
来源：http://wap.zdbjq.cn/Article/details/gfeuxjhsy.sHtML

[H09] 带错误码的异常
来源：http://wap.zdbjq.cn/Article/details/gmbultfwu.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://3g.hesvh.cn/Article/details/gbgozdviz.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://blog.zdbjq.cn/Article/details/gmnunigbi.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.m.share.zdbjq.cn/Article/details/gyeibptll.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://blog.hesvh.cn/Article/details/gukyosyzk.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://3g.zdbjq.cn/Article/details/ggtbioaac.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.m.share.zdbjq.cn/Article/details/giiocylcc.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://mobile.hesvh.cn/Article/details/gjkdorsvr.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://baike.hesvh.cn/Article/details/gjrinmadf.sHtML

[H10] 资源自动释放
来源：http://3g.fehbvm.com/Article/details/gdpbxyilz.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://mobile.hesvh.cn/Article/details/gnkrkqnwb.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://3g.zdbjq.cn/Article/details/gvkqolhcs.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.zdbjq.cn/Article/details/gkodurneh.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.hesvh.cn/Article/details/gzoqspqim.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wap.zdbjq.cn/Article/details/gadndldsl.sHtML

Go:   defer f.Close()
来源：http://wap.zdbjq.cn/Article/details/guwawdvkp.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://blog.fehbvm.com/Article/details/gipbgqixe.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gpwraiihi.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gvaeyhuih.sHtML

I. 正则表达式
来源：http://www.share.fehbvm.com/Article/details/gqxlpbxpv.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gdolmzxaq.sHtML

[I01] 判断是否匹配
来源：http://wap.hesvh.cn/Article/details/gvjqcnion.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://m.share.fehbvm.com/Article/details/gakdlzoti.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://blog.hesvh.cn/Article/details/gqybucqsy.sHtML

JS:   /\d+/.test(s)
来源：http://www.share.zdbjq.cn/Article/details/gwlkrlter.sHtML

TS:   /\d+/.test(s)
来源：http://m.share.hesvh.cn/Article/details/grbleyimy.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.m.share.fehbvm.com/Article/details/gbcerhvbu.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.blog.hesvh.cn/Article/details/gdcdtrdar.sHtML

Ruby: s.match?(/\d+/)
来源：http://blog.hesvh.cn/Article/details/gmfhsvmbn.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.share.zdbjq.cn/Article/details/gudgpubos.sHtML

[I02] 提取所有匹配
来源：http://baike.zdbjq.cn/Article/details/gkhgsyafy.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.blog.hesvh.cn/Article/details/gribedjek.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://read.share.zdbjq.cn/Article/details/gcwshpduj.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://read.share.fehbvm.com/Article/details/ggbtxpyqx.sHtML

TS:   s.match(/\d+/g)
来源：http://baike.fehbvm.com/Article/details/goytdydqj.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://m.share.fehbvm.com/Article/details/grylaxnvq.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://3g.fehbvm.com/Article/details/glrezmdml.sHtML

Ruby: s.scan(/\d+/)
来源：http://m.share.hesvh.cn/Article/details/gtbxqpvmk.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://m.share.fehbvm.com/Article/details/glocvunmh.sHtML

[I03] 提取捕获分组
来源：http://3g.zdbjq.cn/Article/details/gjhdzqvuf.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.share.fehbvm.com/Article/details/gzknvhhhr.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://3g.hesvh.cn/Article/details/gmjuerybz.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.m.share.fehbvm.com/Article/details/gnaunzhci.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.blog.zdbjq.cn/Article/details/gpfnidwpu.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.m.share.hesvh.cn/Article/details/gmornjhns.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://m.share.zdbjq.cn/Article/details/glmdidwaq.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mobile.fehbvm.com/Article/details/gosdslpkr.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.share.hesvh.cn/Article/details/glyxabijh.sHtML

[I04] 正则替换
来源：http://mobile.zdbjq.cn/Article/details/grcxshyee.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.blog.zdbjq.cn/Article/details/glbojuogo.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://3g.hesvh.cn/Article/details/glecarvdx.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://read.share.hesvh.cn/Article/details/gmwnnulmb.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.share.fehbvm.com/Article/details/gumrhnorr.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://3g.hesvh.cn/Article/details/gwovqftaz.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://m.share.fehbvm.com/Article/details/gmqsmidvf.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.share.hesvh.cn/Article/details/gtkxlfueh.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.blog.zdbjq.cn/Article/details/gpytrewpo.sHtML

[I05] 按正则拆分
来源：http://baike.hesvh.cn/Article/details/gseqcevus.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.blog.fehbvm.com/Article/details/gsapcdiwe.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://baike.zdbjq.cn/Article/details/gfcorfgri.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://wap.hesvh.cn/Article/details/givxhcyme.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://wap.hesvh.cn/Article/details/gqbhzjjoh.sHtML

Java: s.split("\\s*,\\s*")
来源：http://3g.hesvh.cn/Article/details/gcjdxuhni.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://mobile.hesvh.cn/Article/details/gymbsxthj.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://blog.hesvh.cn/Article/details/ghqgbzuwy.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://read.share.zdbjq.cn/Article/details/gtibhyijy.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.share.fehbvm.com/Article/details/gvwfjwtif.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.blog.fehbvm.com/Article/details/giwbgiitq.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://blog.hesvh.cn/Article/details/gpwbywgrk.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.hesvh.cn/Article/details/gxlqrbjmh.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.zdbjq.cn/Article/details/gxfhgyyis.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.blog.zdbjq.cn/Article/details/ghsgagdsj.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.m.share.fehbvm.com/Article/details/gjyelcuhc.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://mobile.hesvh.cn/Article/details/gpyvucnwq.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wap.fehbvm.com/Article/details/gqdrrcavi.sHtML

[I07] 忽略大小写与多行模式
来源：http://3g.hesvh.cn/Article/details/gnzbkhzrd.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.blog.zdbjq.cn/Article/details/gadqqcwsy.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.blog.fehbvm.com/Article/details/gnfgwllkv.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://read.share.hesvh.cn/Article/details/gewohizrq.sHtML

TS:   /error/gim
来源：http://www.m.share.fehbvm.com/Article/details/gcqxjvfhv.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://m.share.zdbjq.cn/Article/details/gjdrajnbr.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wap.fehbvm.com/Article/details/gaiahzzqu.sHtML

Ruby: s.scan(/error/i)
来源：http://baike.fehbvm.com/Article/details/gjcbbljla.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://baike.zdbjq.cn/Article/details/grpjlkoth.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://wap.hesvh.cn/Article/details/gwnpannmk.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://blog.fehbvm.com/Article/details/gmczihcsh.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.share.zdbjq.cn/Article/details/gvvnicmoo.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.zdbjq.cn/Article/details/gorwqqaus.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.hesvh.cn/Article/details/gtgjkylan.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://blog.hesvh.cn/Article/details/geowgvpql.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://read.share.hesvh.cn/Article/details/gpjqctnrj.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.m.share.hesvh.cn/Article/details/gsnqkwtgb.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://read.share.hesvh.cn/Article/details/gfuphvdxg.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gyqbbezmk.sHtML

J. 日期与时间
来源：http://wap.zdbjq.cn/Article/details/gruxsvldp.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gxsvkuzil.sHtML

[J01] 获取当前时间
来源：http://read.share.zdbjq.cn/Article/details/gfqedbhen.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.m.share.zdbjq.cn/Article/details/gvqxbxdpv.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://m.share.fehbvm.com/Article/details/gsvtnbjsa.sHtML

JS:   new Date();  Date.now()
来源：http://3g.zdbjq.cn/Article/details/gmchdodhw.sHtML

TS:   new Date();  Date.now()
来源：http://mobile.zdbjq.cn/Article/details/gckdwifix.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://blog.fehbvm.com/Article/details/gbecrcazo.sHtML

Go:   time.Now()
来源：http://www.blog.fehbvm.com/Article/details/glwlkbvtg.sHtML

Ruby: Time.now
来源：http://wap.zdbjq.cn/Article/details/gklvbvjak.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.share.hesvh.cn/Article/details/gibnhxwxq.sHtML

[J02] 格式化输出
来源：http://blog.hesvh.cn/Article/details/gepjcqdha.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.fehbvm.com/Article/details/gcfoctwib.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mobile.zdbjq.cn/Article/details/gxobomcyr.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://m.share.zdbjq.cn/Article/details/gwprkgxcm.sHtML

TS:   d.toISOString()
来源：http://wap.fehbvm.com/Article/details/gkfjaujib.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://m.share.hesvh.cn/Article/details/ggnndndel.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://read.share.fehbvm.com/Article/details/goifjyspt.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.hesvh.cn/Article/details/gnerwexoy.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://mobile.zdbjq.cn/Article/details/gbmkabamt.sHtML

[J03] 字符串解析为日期
来源：http://wap.zdbjq.cn/Article/details/gyjqaogcm.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://baike.hesvh.cn/Article/details/goasdmuva.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.m.share.hesvh.cn/Article/details/gbwoovknq.sHtML

JS:   new Date("2024-01-02")
来源：http://baike.fehbvm.com/Article/details/glliveuqp.sHtML

TS:   new Date("2024-01-02")
来源：http://www.m.share.hesvh.cn/Article/details/gpyarzxks.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.blog.hesvh.cn/Article/details/gdtbtihzj.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.blog.fehbvm.com/Article/details/gzzkeqsly.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.m.share.fehbvm.com/Article/details/gqopmvrtx.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://baike.hesvh.cn/Article/details/gaxwreiux.sHtML

[J04] 时间戳与日期互转
来源：http://mobile.zdbjq.cn/Article/details/gbucsxxzt.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://read.share.fehbvm.com/Article/details/gzpnujdzy.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://read.share.hesvh.cn/Article/details/gahsqxjef.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://m.share.zdbjq.cn/Article/details/ganrzehjr.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://baike.fehbvm.com/Article/details/gdjgxrxaa.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.blog.hesvh.cn/Article/details/gxekwbcrb.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://3g.fehbvm.com/Article/details/goecilhjm.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://blog.hesvh.cn/Article/details/gvzskifih.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wap.fehbvm.com/Article/details/ghnnrwoid.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.m.share.hesvh.cn/Article/details/gdpjmgbku.sHtML

Py:   now + timedelta(days=7)
来源：http://wap.hesvh.cn/Article/details/gsgchnqqb.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://baike.hesvh.cn/Article/details/ggvsnpmgh.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.fehbvm.com/Article/details/gpaiqlhqm.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.zdbjq.cn/Article/details/gfdevtavn.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://mobile.fehbvm.com/Article/details/gmzkwfzyg.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://blog.zdbjq.cn/Article/details/gyknkqfie.sHtML

Ruby: Time.now + 7 * 86400
来源：http://m.share.zdbjq.cn/Article/details/gfhujakiu.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://m.share.fehbvm.com/Article/details/grsaacxoz.sHtML

[J06] 计算两时间之差
来源：http://blog.fehbvm.com/Article/details/gfaqnseoe.sHtML

Py:   (end - start).total_seconds()
来源：http://www.m.share.zdbjq.cn/Article/details/gbfhcznwv.sHtML

PHP:  $end->diff($start)->days;
来源：http://3g.fehbvm.com/Article/details/gnkaquaum.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://m.share.fehbvm.com/Article/details/gvpmtwflv.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.share.hesvh.cn/Article/details/gsoxhqskl.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://wap.zdbjq.cn/Article/details/govokarko.sHtML

Go:   end.Sub(start).Hours()
来源：http://baike.zdbjq.cn/Article/details/gqxfwpnsw.sHtML

Ruby: end - start                 # 返回秒数
来源：http://3g.hesvh.cn/Article/details/glltodndb.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.share.fehbvm.com/Article/details/gxkxoelli.sHtML

[J07] 比较两个日期
来源：http://mobile.zdbjq.cn/Article/details/gyrminscx.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.share.fehbvm.com/Article/details/gjgeoxqid.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://blog.zdbjq.cn/Article/details/gwxfatmvc.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://3g.fehbvm.com/Article/details/gukrumdwm.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.share.hesvh.cn/Article/details/glyvadawh.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.share.fehbvm.com/Article/details/geewmtlkk.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://mobile.hesvh.cn/Article/details/gzogsrtom.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://blog.hesvh.cn/Article/details/gyfdyhglg.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.share.fehbvm.com/Article/details/gtoeixqzo.sHtML

[J08] 提取年月日与星期
来源：http://3g.hesvh.cn/Article/details/guwflkqco.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.m.share.fehbvm.com/Article/details/glhwarcye.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://3g.zdbjq.cn/Article/details/grwlzcmlc.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mobile.hesvh.cn/Article/details/garrkglxs.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mobile.zdbjq.cn/Article/details/gxcssxtvl.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://3g.fehbvm.com/Article/details/gdecejjwv.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://blog.zdbjq.cn/Article/details/gyubdnvvw.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://blog.zdbjq.cn/Article/details/gwuivdoac.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://3g.fehbvm.com/Article/details/gpuoybrjb.sHtML

[J09] 时区处理
来源：http://baike.fehbvm.com/Article/details/goqptxlvh.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://blog.zdbjq.cn/Article/details/gsjymbmkq.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wap.hesvh.cn/Article/details/gfmzhuhfp.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.zdbjq.cn/Article/details/gbolxovwv.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.fehbvm.com/Article/details/gsjotwzqv.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.m.share.zdbjq.cn/Article/details/gubpnwblv.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wap.fehbvm.com/Article/details/glpbqufng.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://mobile.hesvh.cn/Article/details/gpadfqwoi.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.m.share.zdbjq.cn/Article/details/gsrxzjiba.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.m.share.zdbjq.cn/Article/details/gsjocqnwi.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://baike.hesvh.cn/Article/details/gesjzoggh.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://m.share.fehbvm.com/Article/details/gsjvrxjmc.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://blog.zdbjq.cn/Article/details/gxffdtmjg.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mobile.zdbjq.cn/Article/details/gxadalcwp.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.share.hesvh.cn/Article/details/godcrcoqf.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.blog.hesvh.cn/Article/details/gpjotnzay.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://m.share.hesvh.cn/Article/details/gqvudxssy.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://blog.zdbjq.cn/Article/details/grmuytukm.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/guhcsmdsg.sHtML

K. JSON 与序列化
来源：http://www.share.hesvh.cn/Article/details/gmkshatja.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gorrwyucc.sHtML

[K01] 对象转 JSON 字符串
来源：http://m.share.fehbvm.com/Article/details/gxagemuyr.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://baike.hesvh.cn/Article/details/gziivzrqr.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://baike.hesvh.cn/Article/details/goywdebge.sHtML

JS:   JSON.stringify(obj)
来源：http://wap.fehbvm.com/Article/details/gxxgdvxlw.sHtML

TS:   JSON.stringify(obj)
来源：http://baike.zdbjq.cn/Article/details/glbfipdvz.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://3g.hesvh.cn/Article/details/gwxkrrpzg.sHtML

Go:   json.Marshal(obj)
来源：http://mobile.zdbjq.cn/Article/details/gmqlcyykc.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.blog.zdbjq.cn/Article/details/gwjmqsifl.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://blog.fehbvm.com/Article/details/gljpvoumd.sHtML

[K02] JSON 字符串转对象
来源：http://www.blog.fehbvm.com/Article/details/gaasnbpif.sHtML

Py:   json.loads(s)
来源：http://www.blog.fehbvm.com/Article/details/gbkdakwtt.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://read.share.zdbjq.cn/Article/details/gncqaljdq.sHtML

JS:   JSON.parse(s)
来源：http://www.blog.fehbvm.com/Article/details/grgutrqrn.sHtML

TS:   JSON.parse(s)
来源：http://www.blog.hesvh.cn/Article/details/gbzhvtofp.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://blog.hesvh.cn/Article/details/glrbyjqiv.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://3g.zdbjq.cn/Article/details/gvhlqnyro.sHtML

Ruby: JSON.parse(s)
来源：http://3g.fehbvm.com/Article/details/gbceagqvv.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://read.share.fehbvm.com/Article/details/gdalmzchc.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.share.zdbjq.cn/Article/details/ggciqkyne.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.m.share.hesvh.cn/Article/details/ggsfrbelw.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://read.share.hesvh.cn/Article/details/gblpemtni.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://mobile.zdbjq.cn/Article/details/glwasblxz.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://read.share.fehbvm.com/Article/details/gltgnrddh.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://3g.hesvh.cn/Article/details/gpgaohoiu.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://read.share.hesvh.cn/Article/details/ghvloszxi.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://wap.fehbvm.com/Article/details/gbqyemmab.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://3g.fehbvm.com/Article/details/geciiprnh.sHtML

[K04] 读取 JSON 文件
来源：http://3g.zdbjq.cn/Article/details/gznnhjayw.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.blog.fehbvm.com/Article/details/gotrebqrt.sHtML


<!-- 参考信息 -->