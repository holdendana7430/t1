代发 wailian999

TS:   type User = { name: string; age: number };
来源：http://blog.hesvh.cn/Article/details/gckvnorbc.sHtML

Java: record User(String name, int age) {}
来源：http://blog.zdbjq.cn/Article/details/gwcjwfrwq.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.zdbjq.cn/Article/details/gxkbgvkei.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.zdbjq.cn/Article/details/gyxcdpors.sHtML

C#:   record User(string Name, int Age);
来源：http://blog.zdbjq.cn/Article/details/gunhrbnsa.sHtML

[G15] 枚举
来源：http://blog.zdbjq.cn/Article/details/gkqncynrw.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.fehbvm.com/Article/details/gpklhlxdp.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://wap.zdbjq.cn/Article/details/guybqkfkk.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.zdbjq.cn/Article/details/gerktuehu.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.hesvh.cn/Article/details/gdnhgohen.sHtML

Java: enum Color { RED, GREEN }
来源：http://m.share.hesvh.cn/Article/details/girdgtoyp.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://baike.fehbvm.com/Article/details/gzuejvqms.sHtML

Ruby: Color = %i[red green].freeze
来源：http://read.share.hesvh.cn/Article/details/ggjwppijc.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.hesvh.cn/Article/details/gltduadsu.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.hesvh.cn/Article/details/gffasqdtn.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.zdbjq.cn/Article/details/gbbmfecsh.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.zdbjq.cn/Article/details/glnsastzw.sHtML

JS:   Object.entries(obj)
来源：http://m.share.hesvh.cn/Article/details/ggbqzjicr.sHtML

TS:   Object.entries(obj)
来源：http://blog.hesvh.cn/Article/details/gcxcaorxy.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://blog.fehbvm.com/Article/details/gcgtnvcyo.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.zdbjq.cn/Article/details/gfsugqzdp.sHtML

Ruby: obj.instance_variables
来源：http://read.share.zdbjq.cn/Article/details/gqdmeuyqc.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.fehbvm.com/Article/details/gfwydapzn.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gqhihcxfy.sHtML

H. 异常与错误处理
来源：http://mobile.zdbjq.cn/Article/details/gpcqkcdvp.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gwteogyxe.sHtML

[H01] try / catch 基础
来源：http://www.share.zdbjq.cn/Article/details/geyxemkxn.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.zdbjq.cn/Article/details/gmllaedhr.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wap.fehbvm.com/Article/details/gttdqrwhu.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.blog.hesvh.cn/Article/details/gfztcjsqa.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.zdbjq.cn/Article/details/grcoatsaj.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.fehbvm.com/Article/details/glavqilpk.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.fehbvm.com/Article/details/ghzkeykyb.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.m.share.zdbjq.cn/Article/details/gpehkzykw.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.fehbvm.com/Article/details/gtmixmqms.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.hesvh.cn/Article/details/gylptlpjp.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.fehbvm.com/Article/details/gebbjiluu.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/gamlyvuul.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://wap.zdbjq.cn/Article/details/gabtqgoff.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.hesvh.cn/Article/details/gnbtawelp.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/guiyycdua.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.hesvh.cn/Article/details/gfvtjjfxn.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://blog.hesvh.cn/Article/details/gbbrwmuxs.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/grnremqgi.sHtML

[H03] 主动抛出异常
来源：http://blog.hesvh.cn/Article/details/gxqriqdkv.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.m.share.hesvh.cn/Article/details/gkfcfbbmd.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mobile.fehbvm.com/Article/details/gqhieplzr.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.hesvh.cn/Article/details/gubsglsfw.sHtML

TS:   throw new Error("错误信息");
来源：http://mobile.fehbvm.com/Article/details/gprfuakbl.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.m.share.fehbvm.com/Article/details/gjnphgxwz.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.m.share.zdbjq.cn/Article/details/gqwnsemix.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.hesvh.cn/Article/details/gqkkdwxcf.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.m.share.zdbjq.cn/Article/details/gsobabfak.sHtML

[H04] 自定义异常类型
来源：http://3g.fehbvm.com/Article/details/gxrdsofmj.sHtML

Py:   class MyError(Exception): pass
来源：http://baike.fehbvm.com/Article/details/gvufwrqat.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.m.share.zdbjq.cn/Article/details/guxdaknue.sHtML

JS:   class MyError extends Error {}
来源：http://baike.zdbjq.cn/Article/details/gunoialdf.sHtML

TS:   class MyError extends Error {}
来源：http://3g.zdbjq.cn/Article/details/gkhihtygt.sHtML

Java: class MyException extends RuntimeException {}
来源：http://wap.hesvh.cn/Article/details/gaezejwqz.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.blog.zdbjq.cn/Article/details/glqnhsvcr.sHtML

Ruby: class MyError < StandardError; end
来源：http://blog.zdbjq.cn/Article/details/gqorkykyn.sHtML

C#:   class MyException : Exception {}
来源：http://baike.hesvh.cn/Article/details/ghbwjbgdf.sHtML

[H05] 捕获特定类型
来源：http://read.share.fehbvm.com/Article/details/guzhppypr.sHtML

Py:   except ValueError as e:
来源：http://mobile.zdbjq.cn/Article/details/gmaqxljpm.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.share.hesvh.cn/Article/details/gtkbvxowd.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.blog.hesvh.cn/Article/details/gzhvskvei.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://mobile.zdbjq.cn/Article/details/gcgpatnnn.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://blog.fehbvm.com/Article/details/ghmzhfevb.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mobile.hesvh.cn/Article/details/gudzdhttn.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.m.share.hesvh.cn/Article/details/gjhsdtizn.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://read.share.fehbvm.com/Article/details/gfweysbax.sHtML

[H06] 可选值 / 空值安全访问
来源：http://mobile.fehbvm.com/Article/details/gbcjkwitn.sHtML

Py:   value = d.get("k") or default
来源：http://3g.zdbjq.cn/Article/details/gnjkpejim.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.fehbvm.com/Article/details/gxvrxjkat.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://blog.hesvh.cn/Article/details/gdcwdlmyh.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.share.zdbjq.cn/Article/details/gcmtalcgj.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://blog.fehbvm.com/Article/details/gxlsetpry.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://3g.hesvh.cn/Article/details/gxbkmytml.sHtML

Ruby: d&.dig(:a, :b)
来源：http://baike.zdbjq.cn/Article/details/gqianbyza.sHtML

C#:   obj?.A?.B ?? default
来源：http://read.share.hesvh.cn/Article/details/gtkfdftoa.sHtML

[H07] 断言
来源：http://baike.zdbjq.cn/Article/details/gigfiedkj.sHtML

Py:   assert x > 0, "必须为正"
来源：http://m.share.zdbjq.cn/Article/details/gdjebjrfe.sHtML

PHP:  assert($x > 0);
来源：http://m.share.zdbjq.cn/Article/details/gheippzoz.sHtML

JS:   console.assert(x > 0);
来源：http://www.m.share.fehbvm.com/Article/details/gnwmfmdad.sHtML

TS:   console.assert(x > 0);
来源：http://m.share.zdbjq.cn/Article/details/gpjnoaqut.sHtML

Java: assert x > 0 : "必须为正";
来源：http://blog.hesvh.cn/Article/details/gmqwgmuut.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.share.fehbvm.com/Article/details/goqnptkdd.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.share.zdbjq.cn/Article/details/gfpngrlsx.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.share.hesvh.cn/Article/details/gieswunrw.sHtML

[H08] 获取错误信息与堆栈
来源：http://blog.zdbjq.cn/Article/details/guzkvjqot.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://wap.hesvh.cn/Article/details/garsappsu.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.blog.zdbjq.cn/Article/details/gvazrnsgc.sHtML

JS:   e.message;  e.stack
来源：http://www.m.share.fehbvm.com/Article/details/gdwrchsdt.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://mobile.zdbjq.cn/Article/details/gnvxuqpzg.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.blog.fehbvm.com/Article/details/gnasmwmmj.sHtML

Go:   err.Error()
来源：http://www.share.hesvh.cn/Article/details/gxqjgfmkl.sHtML

Ruby: e.message;  e.backtrace
来源：http://blog.fehbvm.com/Article/details/glvnzuxuu.sHtML

C#:   e.Message;  e.StackTrace
来源：http://wap.fehbvm.com/Article/details/gsadgaveo.sHtML

[H09] 带错误码的异常
来源：http://www.m.share.zdbjq.cn/Article/details/gbjzkzbwm.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://blog.hesvh.cn/Article/details/gwumkypzd.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://wap.zdbjq.cn/Article/details/gvbkbywmr.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.blog.zdbjq.cn/Article/details/gumvykncr.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://read.share.fehbvm.com/Article/details/ghqbfvgze.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://baike.fehbvm.com/Article/details/gybqypknf.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://read.share.zdbjq.cn/Article/details/gmbssvjas.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://blog.zdbjq.cn/Article/details/gjhqmblwd.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://3g.fehbvm.com/Article/details/ggcwvxplu.sHtML

[H10] 资源自动释放
来源：http://baike.hesvh.cn/Article/details/grzriwwxr.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://blog.zdbjq.cn/Article/details/gddippvpb.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.blog.fehbvm.com/Article/details/gfyouemkh.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.fehbvm.com/Article/details/gwthukowq.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.fehbvm.com/Article/details/gjfyrjsei.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://3g.hesvh.cn/Article/details/gbeduiqww.sHtML

Go:   defer f.Close()
来源：http://www.blog.zdbjq.cn/Article/details/gioojfyzt.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://read.share.hesvh.cn/Article/details/gffjykslj.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://3g.fehbvm.com/Article/details/ghxudjkay.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gepxfzeti.sHtML

I. 正则表达式
来源：http://wap.fehbvm.com/Article/details/gpdhwfvif.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gugfewfhs.sHtML

[I01] 判断是否匹配
来源：http://read.share.fehbvm.com/Article/details/gtajixevd.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://read.share.zdbjq.cn/Article/details/gzsyyrycd.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://mobile.hesvh.cn/Article/details/glzfzgptq.sHtML

JS:   /\d+/.test(s)
来源：http://mobile.fehbvm.com/Article/details/glkxdjnbj.sHtML

TS:   /\d+/.test(s)
来源：http://mobile.fehbvm.com/Article/details/gzqqyczbi.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://3g.zdbjq.cn/Article/details/gunanfxqa.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://3g.hesvh.cn/Article/details/gslsjpyfl.sHtML

Ruby: s.match?(/\d+/)
来源：http://blog.zdbjq.cn/Article/details/glbsqrbee.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.share.zdbjq.cn/Article/details/gchsihhyk.sHtML

[I02] 提取所有匹配
来源：http://mobile.fehbvm.com/Article/details/guuziaplk.sHtML

Py:   re.findall(r"\d+", s)
来源：http://3g.fehbvm.com/Article/details/ghzcldckv.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://baike.hesvh.cn/Article/details/gbppnniee.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://read.share.hesvh.cn/Article/details/grlszvncd.sHtML

TS:   s.match(/\d+/g)
来源：http://blog.hesvh.cn/Article/details/gvcesoikw.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://blog.zdbjq.cn/Article/details/glziwmyha.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://blog.fehbvm.com/Article/details/gjonbdflw.sHtML

Ruby: s.scan(/\d+/)
来源：http://mobile.hesvh.cn/Article/details/gtnhzwtcu.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wap.hesvh.cn/Article/details/gcbxdxqjt.sHtML

[I03] 提取捕获分组
来源：http://blog.zdbjq.cn/Article/details/gewqpnjya.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mobile.hesvh.cn/Article/details/gpvzqukmf.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.share.hesvh.cn/Article/details/gsvtnhest.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://blog.hesvh.cn/Article/details/gelxnbltz.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.m.share.fehbvm.com/Article/details/gfaosrshj.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://blog.zdbjq.cn/Article/details/gsqfposjc.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mobile.hesvh.cn/Article/details/gqyxyxjus.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://m.share.hesvh.cn/Article/details/ghhjoumkh.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://m.share.hesvh.cn/Article/details/gmrbgjwjo.sHtML

[I04] 正则替换
来源：http://www.m.share.hesvh.cn/Article/details/gaetgxenv.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://baike.hesvh.cn/Article/details/gjnhdsglv.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mobile.hesvh.cn/Article/details/gaksvblzf.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://blog.zdbjq.cn/Article/details/gbjrpemyj.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://mobile.hesvh.cn/Article/details/gbjrsaemw.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.m.share.fehbvm.com/Article/details/gwhqqrzip.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://mobile.fehbvm.com/Article/details/gpfvelckh.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://baike.zdbjq.cn/Article/details/ggbiidetx.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.blog.hesvh.cn/Article/details/gxywhxlyg.sHtML

[I05] 按正则拆分
来源：http://wap.zdbjq.cn/Article/details/gyunasvxt.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.m.share.zdbjq.cn/Article/details/gqartwfah.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://baike.hesvh.cn/Article/details/gaurmoxnh.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://mobile.zdbjq.cn/Article/details/gbtyrdkyj.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://m.share.hesvh.cn/Article/details/gzaefrpcr.sHtML

Java: s.split("\\s*,\\s*")
来源：http://blog.fehbvm.com/Article/details/gtuqarmfm.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://mobile.fehbvm.com/Article/details/gtumjlsrv.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://baike.fehbvm.com/Article/details/gbhqrrmfs.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://m.share.fehbvm.com/Article/details/gkyniuech.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://m.share.zdbjq.cn/Article/details/gjzfieqfe.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://blog.hesvh.cn/Article/details/ghndgiugg.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.m.share.zdbjq.cn/Article/details/gvncsccti.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.hesvh.cn/Article/details/ggjtjlztw.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.hesvh.cn/Article/details/gkamllfyd.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://m.share.zdbjq.cn/Article/details/gmvqbkloz.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://read.share.fehbvm.com/Article/details/gtunjgyqr.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.share.fehbvm.com/Article/details/gazdumujb.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mobile.hesvh.cn/Article/details/gbhbhxubn.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.blog.zdbjq.cn/Article/details/ghpouxiec.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://read.share.hesvh.cn/Article/details/gimlevfek.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.blog.hesvh.cn/Article/details/guhbaylui.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://baike.zdbjq.cn/Article/details/gnqynjkww.sHtML

TS:   /error/gim
来源：http://www.m.share.fehbvm.com/Article/details/gnvhxwyua.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://read.share.fehbvm.com/Article/details/gychncmki.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.blog.hesvh.cn/Article/details/gtjicixwi.sHtML

Ruby: s.scan(/error/i)
来源：http://baike.zdbjq.cn/Article/details/ggjaqqhrf.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://read.share.zdbjq.cn/Article/details/gdyfahzjh.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://baike.zdbjq.cn/Article/details/gmyzocqyo.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.m.share.fehbvm.com/Article/details/gsoqilewb.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://blog.fehbvm.com/Article/details/gxyveelho.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.hesvh.cn/Article/details/gvnxpzsjp.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.hesvh.cn/Article/details/gllzrqvut.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://3g.hesvh.cn/Article/details/gzpbbewoq.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://3g.fehbvm.com/Article/details/ggucgfuco.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.m.share.zdbjq.cn/Article/details/gpxopnscn.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://baike.fehbvm.com/Article/details/gspdalvhh.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/geumiexbf.sHtML

J. 日期与时间
来源：http://blog.hesvh.cn/Article/details/gbusatysx.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gsktacqnv.sHtML

[J01] 获取当前时间
来源：http://m.share.zdbjq.cn/Article/details/gazomxsqc.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://baike.hesvh.cn/Article/details/gnsxoodtm.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.share.hesvh.cn/Article/details/gsoupnguz.sHtML

JS:   new Date();  Date.now()
来源：http://m.share.hesvh.cn/Article/details/gxakcrjxx.sHtML

TS:   new Date();  Date.now()
来源：http://wap.hesvh.cn/Article/details/gmrdzrynx.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.blog.hesvh.cn/Article/details/gzvemwyhf.sHtML

Go:   time.Now()
来源：http://www.m.share.hesvh.cn/Article/details/gnvmyrwlp.sHtML

Ruby: Time.now
来源：http://www.m.share.zdbjq.cn/Article/details/guqlrmacr.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.m.share.fehbvm.com/Article/details/gttvymyrl.sHtML

[J02] 格式化输出
来源：http://www.m.share.zdbjq.cn/Article/details/gfopuvxbb.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.zdbjq.cn/Article/details/gwpkgwrhd.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://3g.fehbvm.com/Article/details/gqkshnrca.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.blog.fehbvm.com/Article/details/gqxqcyroh.sHtML

TS:   d.toISOString()
来源：http://read.share.zdbjq.cn/Article/details/guiqbvhoe.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.m.share.fehbvm.com/Article/details/gyxxpekwy.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.m.share.hesvh.cn/Article/details/glwpuaxsy.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.zdbjq.cn/Article/details/grwcdqjhy.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://baike.hesvh.cn/Article/details/gdokgsdod.sHtML

[J03] 字符串解析为日期
来源：http://www.blog.fehbvm.com/Article/details/gcbshocas.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://blog.hesvh.cn/Article/details/gplwopfiu.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://m.share.fehbvm.com/Article/details/gmjgiuxfu.sHtML

JS:   new Date("2024-01-02")
来源：http://baike.zdbjq.cn/Article/details/gzwunwtsz.sHtML

TS:   new Date("2024-01-02")
来源：http://read.share.fehbvm.com/Article/details/gilygeiml.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.m.share.hesvh.cn/Article/details/gamszgzfa.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.m.share.hesvh.cn/Article/details/guqlzctkq.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://baike.fehbvm.com/Article/details/gqbdlehky.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://baike.zdbjq.cn/Article/details/ghofkbzpn.sHtML

[J04] 时间戳与日期互转
来源：http://blog.fehbvm.com/Article/details/gjqnrgatr.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mobile.zdbjq.cn/Article/details/gwysguosz.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wap.hesvh.cn/Article/details/gxsbmwdqb.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mobile.hesvh.cn/Article/details/gkcmpmzyq.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://m.share.fehbvm.com/Article/details/grnoythua.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.blog.fehbvm.com/Article/details/gnrhryomj.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://baike.fehbvm.com/Article/details/gzzksrhpn.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.m.share.hesvh.cn/Article/details/gjcbchqce.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://mobile.zdbjq.cn/Article/details/ganakosup.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.share.hesvh.cn/Article/details/gxomxdkfe.sHtML

Py:   now + timedelta(days=7)
来源：http://3g.fehbvm.com/Article/details/gvzdjvwyk.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://read.share.hesvh.cn/Article/details/gkbpgyhgc.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.fehbvm.com/Article/details/gwkcxpmiq.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.zdbjq.cn/Article/details/gkvsmmwuz.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://wap.fehbvm.com/Article/details/gzybkpvcg.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.share.hesvh.cn/Article/details/gqkvgvszd.sHtML

Ruby: Time.now + 7 * 86400
来源：http://wap.zdbjq.cn/Article/details/gjivxpdge.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.m.share.hesvh.cn/Article/details/ghbmgldjg.sHtML

[J06] 计算两时间之差
来源：http://blog.zdbjq.cn/Article/details/gplejnnoz.sHtML

Py:   (end - start).total_seconds()
来源：http://baike.hesvh.cn/Article/details/gffktbyqi.sHtML

PHP:  $end->diff($start)->days;
来源：http://mobile.fehbvm.com/Article/details/gnntpfazg.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.blog.zdbjq.cn/Article/details/gpgvhvkfn.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mobile.zdbjq.cn/Article/details/gmlaijfax.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.blog.hesvh.cn/Article/details/glouzkmed.sHtML

Go:   end.Sub(start).Hours()
来源：http://read.share.zdbjq.cn/Article/details/ggmgldtln.sHtML

Ruby: end - start                 # 返回秒数
来源：http://read.share.zdbjq.cn/Article/details/gfzvilgur.sHtML

C#:   (end - start).TotalSeconds
来源：http://blog.fehbvm.com/Article/details/gxqkwnkqn.sHtML

[J07] 比较两个日期
来源：http://www.m.share.fehbvm.com/Article/details/gjajyprfk.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://blog.fehbvm.com/Article/details/gilgwpeub.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://3g.hesvh.cn/Article/details/gnvbavvmu.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.blog.fehbvm.com/Article/details/gfdfyjepf.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://baike.fehbvm.com/Article/details/gbimymxtd.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://m.share.zdbjq.cn/Article/details/gdoemqtvf.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://m.share.zdbjq.cn/Article/details/gsvnpxcgp.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://m.share.hesvh.cn/Article/details/gmqxjcdou.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.share.zdbjq.cn/Article/details/gjnknqtda.sHtML

[J08] 提取年月日与星期
来源：http://www.share.fehbvm.com/Article/details/gwrpffpjq.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.blog.hesvh.cn/Article/details/girrmcbth.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://3g.hesvh.cn/Article/details/gthhdfnqh.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.m.share.hesvh.cn/Article/details/gdunnxymk.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://wap.fehbvm.com/Article/details/gfshtybcm.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.share.hesvh.cn/Article/details/gdkudhzcu.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://blog.fehbvm.com/Article/details/gkhtvgyiv.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://blog.hesvh.cn/Article/details/gcwmkpngj.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://3g.hesvh.cn/Article/details/gqivmydlh.sHtML

[J09] 时区处理
来源：http://www.share.zdbjq.cn/Article/details/gvsjjmkig.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.share.zdbjq.cn/Article/details/gutgzsdvu.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wap.fehbvm.com/Article/details/goknniyfk.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.fehbvm.com/Article/details/gizddqyfh.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.hesvh.cn/Article/details/gxodusbjf.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.blog.zdbjq.cn/Article/details/gumqkbirx.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mobile.hesvh.cn/Article/details/gnrpmhqyo.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://baike.zdbjq.cn/Article/details/gzqxxaoxd.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.blog.zdbjq.cn/Article/details/ggmreyobq.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.share.hesvh.cn/Article/details/geeoilsbd.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://blog.fehbvm.com/Article/details/gxacoaqbm.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.m.share.fehbvm.com/Article/details/gnyswjhzk.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.share.fehbvm.com/Article/details/gkcaeqtyi.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mobile.fehbvm.com/Article/details/gffraoihg.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://baike.fehbvm.com/Article/details/gilxaxrfr.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://read.share.hesvh.cn/Article/details/gqvfmqggu.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://baike.hesvh.cn/Article/details/gxmdqalyc.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://blog.fehbvm.com/Article/details/gdsyknrfy.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gyyrkspex.sHtML

K. JSON 与序列化
来源：http://m.share.fehbvm.com/Article/details/gvenkfjlj.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gbzjjydgw.sHtML

[K01] 对象转 JSON 字符串
来源：http://mobile.fehbvm.com/Article/details/gvqyafqnt.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.share.fehbvm.com/Article/details/ghilcozhq.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://read.share.fehbvm.com/Article/details/gscgovurh.sHtML

JS:   JSON.stringify(obj)
来源：http://mobile.fehbvm.com/Article/details/gpdofwyeu.sHtML

TS:   JSON.stringify(obj)
来源：http://blog.fehbvm.com/Article/details/gsicaezqc.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://baike.hesvh.cn/Article/details/gquuwawuh.sHtML

Go:   json.Marshal(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gceuosfrb.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://baike.hesvh.cn/Article/details/ggjfjwlcb.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://blog.hesvh.cn/Article/details/gtuunghaw.sHtML

[K02] JSON 字符串转对象
来源：http://www.m.share.hesvh.cn/Article/details/gdurduhqg.sHtML

Py:   json.loads(s)
来源：http://3g.zdbjq.cn/Article/details/ggkfspmyp.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.m.share.zdbjq.cn/Article/details/grzypufwl.sHtML

JS:   JSON.parse(s)
来源：http://blog.zdbjq.cn/Article/details/ghudmrubi.sHtML


<!-- 参考信息 -->