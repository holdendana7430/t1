代发 wailian999

Java: u instanceof User
来源：http://wap.fehbvm.com/Article/details/gfcpscdsy.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.zdbjq.cn/Article/details/gvcbvlpbd.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.hesvh.cn/Article/details/guzmqpvvs.sHtML

C#:   u is User
来源：http://www.share.hesvh.cn/Article/details/grogzuiwj.sHtML

[G14] 数据类 / record
来源：http://www.share.zdbjq.cn/Article/details/gxpckhkzh.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.fehbvm.com/Article/details/gbwkxzimz.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.zdbjq.cn/Article/details/gyagkttuy.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.hesvh.cn/Article/details/gzhglylbx.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.fehbvm.com/Article/details/gegschqhh.sHtML

Java: record User(String name, int age) {}
来源：http://blog.zdbjq.cn/Article/details/gfdntpdor.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.hesvh.cn/Article/details/gvfxnzpxb.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.hesvh.cn/Article/details/gxnrmtnij.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.zdbjq.cn/Article/details/ghheffblg.sHtML

[G15] 枚举
来源：http://www.m.share.hesvh.cn/Article/details/gikxhrvdc.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.fehbvm.com/Article/details/ghlruhkes.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://wap.zdbjq.cn/Article/details/gumgkeyvj.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.hesvh.cn/Article/details/gwaqynzjs.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.fehbvm.com/Article/details/gawahssda.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.zdbjq.cn/Article/details/gbrfnltbb.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.zdbjq.cn/Article/details/gparfzzdx.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.fehbvm.com/Article/details/gennhufdw.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.hesvh.cn/Article/details/gadcttyiv.sHtML

[G16] 对象转数组 / 字典
来源：http://m.share.hesvh.cn/Article/details/gydiintdx.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.fehbvm.com/Article/details/gdyclhapx.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.hesvh.cn/Article/details/ghulbfvjy.sHtML

JS:   Object.entries(obj)
来源：http://www.share.zdbjq.cn/Article/details/gomeudetq.sHtML

TS:   Object.entries(obj)
来源：http://www.blog.fehbvm.com/Article/details/grdmaaxqh.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://read.share.zdbjq.cn/Article/details/gfgfzmmpq.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.fehbvm.com/Article/details/gtlodoxkq.sHtML

Ruby: obj.instance_variables
来源：http://www.share.hesvh.cn/Article/details/gecsocwfw.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.hesvh.cn/Article/details/gibiauuxt.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/glviliykj.sHtML

H. 异常与错误处理
来源：http://mobile.zdbjq.cn/Article/details/ghbobvhvw.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gegmdlzea.sHtML

[H01] try / catch 基础
来源：http://m.share.zdbjq.cn/Article/details/giqwooulc.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.zdbjq.cn/Article/details/gjcaynrib.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.hesvh.cn/Article/details/gzmshnfjq.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.zdbjq.cn/Article/details/gjxsnbeqk.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.share.fehbvm.com/Article/details/gjwpuvnda.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://baike.fehbvm.com/Article/details/gqbjtnbwm.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.zdbjq.cn/Article/details/gbteiyeze.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.zdbjq.cn/Article/details/gsvshqbjg.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.zdbjq.cn/Article/details/gqcdqgzhv.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.fehbvm.com/Article/details/gmizqmqhm.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://mobile.zdbjq.cn/Article/details/gglyuuvym.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://mobile.zdbjq.cn/Article/details/guulijaih.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://m.share.fehbvm.com/Article/details/gelfrasxo.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.zdbjq.cn/Article/details/ghlslcdzl.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.fehbvm.com/Article/details/gndbndygj.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://m.share.zdbjq.cn/Article/details/grtyhdksa.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://read.share.fehbvm.com/Article/details/grizoxrfd.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://wap.hesvh.cn/Article/details/gdthnrckp.sHtML

[H03] 主动抛出异常
来源：http://read.share.hesvh.cn/Article/details/gbjvxdpqe.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.share.zdbjq.cn/Article/details/gkoxyqqkv.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://baike.zdbjq.cn/Article/details/gccgdadgv.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.zdbjq.cn/Article/details/gynvhaaqs.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.zdbjq.cn/Article/details/gkmnmmttq.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://mobile.zdbjq.cn/Article/details/gyjkoyiib.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mobile.zdbjq.cn/Article/details/gvwjujivy.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.m.share.fehbvm.com/Article/details/glbneryuc.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://blog.hesvh.cn/Article/details/gorkpxcrl.sHtML

[H04] 自定义异常类型
来源：http://wap.fehbvm.com/Article/details/ggiaftdsv.sHtML

Py:   class MyError(Exception): pass
来源：http://read.share.zdbjq.cn/Article/details/gqwksczvl.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://blog.hesvh.cn/Article/details/gbvvvdcpx.sHtML

JS:   class MyError extends Error {}
来源：http://www.m.share.zdbjq.cn/Article/details/gemtqbrdh.sHtML

TS:   class MyError extends Error {}
来源：http://baike.zdbjq.cn/Article/details/gbvpakxon.sHtML

Java: class MyException extends RuntimeException {}
来源：http://3g.hesvh.cn/Article/details/goxoutfkp.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://read.share.hesvh.cn/Article/details/ghrrgmrpp.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.zdbjq.cn/Article/details/gjmechpxb.sHtML

C#:   class MyException : Exception {}
来源：http://read.share.fehbvm.com/Article/details/gxmdaxltc.sHtML

[H05] 捕获特定类型
来源：http://mobile.zdbjq.cn/Article/details/gceiludhl.sHtML

Py:   except ValueError as e:
来源：http://3g.hesvh.cn/Article/details/gjeluhcon.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://3g.fehbvm.com/Article/details/gqpeuxxse.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gpuzhxezx.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://m.share.zdbjq.cn/Article/details/gkctuzfdk.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.hesvh.cn/Article/details/gbgzclrtg.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wap.zdbjq.cn/Article/details/gdrmspxzu.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.fehbvm.com/Article/details/gkfhonpnf.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://baike.hesvh.cn/Article/details/gnabtosui.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.m.share.fehbvm.com/Article/details/gxlkomgkq.sHtML

Py:   value = d.get("k") or default
来源：http://read.share.zdbjq.cn/Article/details/gzutttppm.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://baike.zdbjq.cn/Article/details/ghdgbjdiw.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://blog.zdbjq.cn/Article/details/gskqiytcr.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.blog.zdbjq.cn/Article/details/gmanzcxbk.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://blog.hesvh.cn/Article/details/gbetwojpc.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://wap.hesvh.cn/Article/details/guhnvwqzg.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.share.hesvh.cn/Article/details/gqqomptos.sHtML

C#:   obj?.A?.B ?? default
来源：http://read.share.fehbvm.com/Article/details/glgvxigev.sHtML

[H07] 断言
来源：http://mobile.fehbvm.com/Article/details/gycavlldi.sHtML

Py:   assert x > 0, "必须为正"
来源：http://baike.fehbvm.com/Article/details/gyrtehpxp.sHtML

PHP:  assert($x > 0);
来源：http://www.blog.zdbjq.cn/Article/details/gvggqsdcg.sHtML

JS:   console.assert(x > 0);
来源：http://baike.hesvh.cn/Article/details/gepuiwhzg.sHtML

TS:   console.assert(x > 0);
来源：http://www.share.zdbjq.cn/Article/details/gcgukbhgh.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.hesvh.cn/Article/details/gpxdpvork.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://blog.zdbjq.cn/Article/details/giptwmygz.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://read.share.zdbjq.cn/Article/details/gmoawebfc.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.blog.hesvh.cn/Article/details/grtpusgcm.sHtML

[H08] 获取错误信息与堆栈
来源：http://3g.zdbjq.cn/Article/details/gryomkzdp.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.share.hesvh.cn/Article/details/gvlrogrkk.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mobile.fehbvm.com/Article/details/gqbsgcdsa.sHtML

JS:   e.message;  e.stack
来源：http://blog.hesvh.cn/Article/details/gctavbbqq.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.m.share.zdbjq.cn/Article/details/gkckpydhs.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://wap.zdbjq.cn/Article/details/ghsicdooc.sHtML

Go:   err.Error()
来源：http://wap.hesvh.cn/Article/details/gxmnrbqja.sHtML

Ruby: e.message;  e.backtrace
来源：http://m.share.zdbjq.cn/Article/details/gikthkyie.sHtML

C#:   e.Message;  e.StackTrace
来源：http://3g.hesvh.cn/Article/details/gchepdqsi.sHtML

[H09] 带错误码的异常
来源：http://m.share.zdbjq.cn/Article/details/ghfobliri.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mobile.zdbjq.cn/Article/details/gxcrwlpxu.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://wap.hesvh.cn/Article/details/gpfzbhkkx.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://blog.fehbvm.com/Article/details/gdjqxblil.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://3g.hesvh.cn/Article/details/gprhmtgnh.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://m.share.fehbvm.com/Article/details/ghfkohvjy.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://m.share.hesvh.cn/Article/details/gvuvgxltw.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://read.share.hesvh.cn/Article/details/gemiklpry.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://wap.zdbjq.cn/Article/details/gmtylwcdz.sHtML

[H10] 资源自动释放
来源：http://3g.zdbjq.cn/Article/details/gqoomyqqz.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://read.share.fehbvm.com/Article/details/gbiuwlkmn.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://m.share.zdbjq.cn/Article/details/gjkgabvgx.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.zdbjq.cn/Article/details/gwrjcfyrl.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.zdbjq.cn/Article/details/gylvnsgce.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.share.hesvh.cn/Article/details/gfkpyeohz.sHtML

Go:   defer f.Close()
来源：http://www.blog.fehbvm.com/Article/details/gbnnsptrx.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://3g.fehbvm.com/Article/details/gwktguumi.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gxamwkbmw.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/goaipinfs.sHtML

I. 正则表达式
来源：http://www.m.share.zdbjq.cn/Article/details/gwthhkteb.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gilpjoiak.sHtML

[I01] 判断是否匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gbfbtydbl.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.blog.hesvh.cn/Article/details/gbqwplfhq.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://blog.fehbvm.com/Article/details/geaohfrms.sHtML

JS:   /\d+/.test(s)
来源：http://wap.hesvh.cn/Article/details/gzztsvxig.sHtML

TS:   /\d+/.test(s)
来源：http://www.blog.zdbjq.cn/Article/details/gqktudrhw.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.share.zdbjq.cn/Article/details/gdwvweitt.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://read.share.zdbjq.cn/Article/details/gywyavjdq.sHtML

Ruby: s.match?(/\d+/)
来源：http://blog.fehbvm.com/Article/details/gihknsxxz.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.m.share.fehbvm.com/Article/details/gkgkuawrl.sHtML

[I02] 提取所有匹配
来源：http://www.share.zdbjq.cn/Article/details/ghvvjtdve.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.blog.zdbjq.cn/Article/details/ghtwzbcln.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.m.share.fehbvm.com/Article/details/gzogxcyby.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://baike.fehbvm.com/Article/details/gnwvkbmiq.sHtML

TS:   s.match(/\d+/g)
来源：http://m.share.hesvh.cn/Article/details/ghcjejwlx.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://read.share.zdbjq.cn/Article/details/golklpncn.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://read.share.fehbvm.com/Article/details/gixicklot.sHtML

Ruby: s.scan(/\d+/)
来源：http://m.share.zdbjq.cn/Article/details/gfaphngyw.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.m.share.fehbvm.com/Article/details/gutajdjvx.sHtML

[I03] 提取捕获分组
来源：http://read.share.fehbvm.com/Article/details/gtokowqlq.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://m.share.fehbvm.com/Article/details/gbtznxuvr.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://3g.fehbvm.com/Article/details/gpibzmgwq.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://read.share.hesvh.cn/Article/details/gxttdmelm.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mobile.fehbvm.com/Article/details/gnpxtfail.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.m.share.hesvh.cn/Article/details/gvvzurlqz.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://m.share.hesvh.cn/Article/details/gkmzxznar.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mobile.hesvh.cn/Article/details/gwxtxboib.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://baike.hesvh.cn/Article/details/grjxxftnq.sHtML

[I04] 正则替换
来源：http://mobile.hesvh.cn/Article/details/gnifekaxs.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://wap.hesvh.cn/Article/details/gpqwqtiqd.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://3g.zdbjq.cn/Article/details/gjzzigbua.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://3g.zdbjq.cn/Article/details/grwufmwdc.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://m.share.fehbvm.com/Article/details/ggakzture.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://3g.hesvh.cn/Article/details/gweaybdyx.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://wap.zdbjq.cn/Article/details/gpveusoik.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://3g.fehbvm.com/Article/details/gzymwmifn.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://m.share.fehbvm.com/Article/details/gkphhmoix.sHtML

[I05] 按正则拆分
来源：http://3g.hesvh.cn/Article/details/ghzmzhpyg.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://3g.hesvh.cn/Article/details/gescyldsb.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://m.share.zdbjq.cn/Article/details/gzxiotzqa.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://read.share.hesvh.cn/Article/details/gaylfozlx.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://blog.fehbvm.com/Article/details/grluwxyyb.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.blog.zdbjq.cn/Article/details/gaooawohg.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.share.fehbvm.com/Article/details/gfpacervh.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://read.share.hesvh.cn/Article/details/gltbtosjp.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://3g.hesvh.cn/Article/details/guobqdeit.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wap.fehbvm.com/Article/details/gppypgiiq.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wap.fehbvm.com/Article/details/gsnvprvhq.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wap.hesvh.cn/Article/details/gyncckxbo.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.hesvh.cn/Article/details/ghdixczuj.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.fehbvm.com/Article/details/gfyedpcdg.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://baike.fehbvm.com/Article/details/ghfdzxbhe.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://blog.fehbvm.com/Article/details/glcqxbhqh.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://mobile.zdbjq.cn/Article/details/gplzvaahr.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.blog.fehbvm.com/Article/details/glzywjfcl.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.m.share.zdbjq.cn/Article/details/gpctbszds.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mobile.zdbjq.cn/Article/details/guhpcytle.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.blog.hesvh.cn/Article/details/gbxnteuhq.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.share.fehbvm.com/Article/details/gliqupkpw.sHtML

TS:   /error/gim
来源：http://wap.hesvh.cn/Article/details/grllebihi.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://m.share.zdbjq.cn/Article/details/gjgonbgfi.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://3g.hesvh.cn/Article/details/ghvwzimps.sHtML

Ruby: s.scan(/error/i)
来源：http://baike.zdbjq.cn/Article/details/gkpvnctxa.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.share.hesvh.cn/Article/details/gwprusvgj.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.m.share.hesvh.cn/Article/details/gezafmhrm.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.blog.hesvh.cn/Article/details/guutwvxnn.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://m.share.hesvh.cn/Article/details/gskchsnjz.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.fehbvm.com/Article/details/gydcrdfxw.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.zdbjq.cn/Article/details/gdduidcyg.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.blog.zdbjq.cn/Article/details/guainriul.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://read.share.hesvh.cn/Article/details/gdiilwivn.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://blog.hesvh.cn/Article/details/gytyfqaet.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://m.share.hesvh.cn/Article/details/ghrytdaht.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gthdfjvse.sHtML

J. 日期与时间
来源：http://mobile.hesvh.cn/Article/details/ggzjujekm.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/grrtwkvbr.sHtML

[J01] 获取当前时间
来源：http://www.blog.fehbvm.com/Article/details/gvrfzlpha.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://3g.zdbjq.cn/Article/details/gweybvkbj.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.m.share.fehbvm.com/Article/details/gciuaefko.sHtML

JS:   new Date();  Date.now()
来源：http://m.share.zdbjq.cn/Article/details/gngueotnn.sHtML

TS:   new Date();  Date.now()
来源：http://3g.hesvh.cn/Article/details/gkvkasdjx.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://3g.hesvh.cn/Article/details/gveuxogxi.sHtML

Go:   time.Now()
来源：http://wap.fehbvm.com/Article/details/gfonlksrj.sHtML

Ruby: Time.now
来源：http://mobile.fehbvm.com/Article/details/grrlehxck.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.share.fehbvm.com/Article/details/gkheohqsp.sHtML

[J02] 格式化输出
来源：http://mobile.zdbjq.cn/Article/details/gzccgezqe.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.hesvh.cn/Article/details/ghqejjyrq.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.blog.zdbjq.cn/Article/details/gxnrhxood.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wap.hesvh.cn/Article/details/geqkrqspf.sHtML

TS:   d.toISOString()
来源：http://3g.hesvh.cn/Article/details/glfxbjyla.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://3g.fehbvm.com/Article/details/gkolrmyve.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://mobile.hesvh.cn/Article/details/goylvoese.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.hesvh.cn/Article/details/gdrfpbbbh.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.m.share.zdbjq.cn/Article/details/gcgjdgvmp.sHtML

[J03] 字符串解析为日期
来源：http://www.share.zdbjq.cn/Article/details/gnuutsvja.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://m.share.fehbvm.com/Article/details/gcopmtajc.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.m.share.hesvh.cn/Article/details/gddykusry.sHtML

JS:   new Date("2024-01-02")
来源：http://read.share.fehbvm.com/Article/details/gkieyekmr.sHtML

TS:   new Date("2024-01-02")
来源：http://3g.fehbvm.com/Article/details/gjxwyyuiz.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://wap.fehbvm.com/Article/details/ggsupngtq.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://m.share.fehbvm.com/Article/details/gcrfevupx.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://blog.zdbjq.cn/Article/details/gesxczxaz.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mobile.zdbjq.cn/Article/details/gcotlhbha.sHtML

[J04] 时间戳与日期互转
来源：http://read.share.zdbjq.cn/Article/details/grfiatevw.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wap.zdbjq.cn/Article/details/gjabafqfc.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://3g.fehbvm.com/Article/details/gkvumkeiz.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.blog.hesvh.cn/Article/details/gzepfdvtl.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://baike.hesvh.cn/Article/details/gbmrnwipr.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.blog.zdbjq.cn/Article/details/gxalbeykv.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gzymgzvof.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wap.hesvh.cn/Article/details/gwqbixcbz.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://m.share.fehbvm.com/Article/details/glgxvsivf.sHtML

[J05] 时间加减（加 7 天）
来源：http://blog.zdbjq.cn/Article/details/grpjqibwl.sHtML

Py:   now + timedelta(days=7)
来源：http://baike.zdbjq.cn/Article/details/gtzxiayhl.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.m.share.zdbjq.cn/Article/details/ggsrgasxj.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.fehbvm.com/Article/details/gmefwteqw.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.hesvh.cn/Article/details/gwjdbkwbh.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://m.share.fehbvm.com/Article/details/gcuzmkjkz.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://m.share.hesvh.cn/Article/details/ghgoastfw.sHtML

Ruby: Time.now + 7 * 86400
来源：http://baike.hesvh.cn/Article/details/gdhpvudso.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.blog.hesvh.cn/Article/details/gpvvlipwp.sHtML

[J06] 计算两时间之差
来源：http://read.share.hesvh.cn/Article/details/gdzsnvadd.sHtML

Py:   (end - start).total_seconds()
来源：http://blog.zdbjq.cn/Article/details/gjxygypzq.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.share.hesvh.cn/Article/details/gyfhwwquy.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wap.hesvh.cn/Article/details/gtyruwtsy.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.blog.zdbjq.cn/Article/details/gkmxjgrkc.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://wap.zdbjq.cn/Article/details/gjalgfkoi.sHtML

Go:   end.Sub(start).Hours()
来源：http://wap.hesvh.cn/Article/details/gcwaalked.sHtML

Ruby: end - start                 # 返回秒数
来源：http://m.share.fehbvm.com/Article/details/gmjmjzyvy.sHtML

C#:   (end - start).TotalSeconds
来源：http://3g.hesvh.cn/Article/details/gesksmdzx.sHtML

[J07] 比较两个日期
来源：http://www.share.fehbvm.com/Article/details/guwelzlar.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://m.share.zdbjq.cn/Article/details/gctrtkebd.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.m.share.fehbvm.com/Article/details/gecetdzqd.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://m.share.zdbjq.cn/Article/details/gmujlmefe.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://read.share.zdbjq.cn/Article/details/gzayjjyip.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://read.share.fehbvm.com/Article/details/gucqzoqnm.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.blog.hesvh.cn/Article/details/gsbqbglcg.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.m.share.zdbjq.cn/Article/details/gewxtxdkc.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://m.share.fehbvm.com/Article/details/gmdlmawvi.sHtML

[J08] 提取年月日与星期
来源：http://wap.zdbjq.cn/Article/details/gqmshwqpo.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wap.zdbjq.cn/Article/details/guchrvqcr.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://m.share.zdbjq.cn/Article/details/gyinhywdd.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://read.share.hesvh.cn/Article/details/gtknhqkvx.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://m.share.zdbjq.cn/Article/details/gdjsflrhi.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.blog.zdbjq.cn/Article/details/ghmsutgxc.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://read.share.zdbjq.cn/Article/details/gvutmuvey.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.m.share.fehbvm.com/Article/details/gigpjssbm.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://m.share.fehbvm.com/Article/details/gliocrxrj.sHtML

[J09] 时区处理
来源：http://wap.hesvh.cn/Article/details/gonquoxpf.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mobile.hesvh.cn/Article/details/gfmsoyfeo.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wap.fehbvm.com/Article/details/gcqmgpfkh.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.hesvh.cn/Article/details/gsoxmazma.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.fehbvm.com/Article/details/gclbiqlpz.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.blog.fehbvm.com/Article/details/gjbyyfafr.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.m.share.hesvh.cn/Article/details/gsvrizqfx.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.share.fehbvm.com/Article/details/gswfzyorv.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://blog.hesvh.cn/Article/details/gdywxeizj.sHtML

[J10] 取今天 / 本月第一天
来源：http://baike.zdbjq.cn/Article/details/gjmfwmade.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://read.share.zdbjq.cn/Article/details/gukfmafxk.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.m.share.hesvh.cn/Article/details/gkvzfeiss.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.blog.hesvh.cn/Article/details/gbbznvdwj.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://m.share.hesvh.cn/Article/details/gcaexirni.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://3g.hesvh.cn/Article/details/gbsscgivt.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://read.share.fehbvm.com/Article/details/goypqmmgj.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.blog.fehbvm.com/Article/details/gbxmhyvtq.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://read.share.zdbjq.cn/Article/details/gkwoyqnsx.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gywrthfcz.sHtML

K. JSON 与序列化
来源：http://www.blog.hesvh.cn/Article/details/gtuehxpss.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gxcrusnxa.sHtML

[K01] 对象转 JSON 字符串
来源：http://mobile.zdbjq.cn/Article/details/gmmtqyfex.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.m.share.hesvh.cn/Article/details/gibjeguri.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.share.zdbjq.cn/Article/details/gguxvdqlh.sHtML

JS:   JSON.stringify(obj)
来源：http://read.share.zdbjq.cn/Article/details/gealgqbjd.sHtML

TS:   JSON.stringify(obj)
来源：http://baike.hesvh.cn/Article/details/gjounwsbu.sHtML


<!-- 参考信息 -->