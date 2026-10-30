代发 wailian999

TS:   type User = { name: string; age: number };
来源：http://3g.hesvh.cn/Article/details/gdmbjfnal.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.fehbvm.com/Article/details/gwvhmpzvo.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.zdbjq.cn/Article/details/gqkroyuoz.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.fehbvm.com/Article/details/gwrhshtxv.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.fehbvm.com/Article/details/gteutilrq.sHtML

[G15] 枚举
来源：http://baike.fehbvm.com/Article/details/gigiqvxfi.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.hesvh.cn/Article/details/gelirtyuy.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.zdbjq.cn/Article/details/grozljjhm.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.hesvh.cn/Article/details/gplysypul.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gvcuvbwfk.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.zdbjq.cn/Article/details/gtegqusri.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.zdbjq.cn/Article/details/gtrshjgig.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.fehbvm.com/Article/details/gvldebfsf.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.hesvh.cn/Article/details/gtcvozptr.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.hesvh.cn/Article/details/gtdvqwbea.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.zdbjq.cn/Article/details/gwxldpxcb.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.hesvh.cn/Article/details/ggarreogd.sHtML

JS:   Object.entries(obj)
来源：http://wap.fehbvm.com/Article/details/gelsqmeeb.sHtML

TS:   Object.entries(obj)
来源：http://m.share.zdbjq.cn/Article/details/ggirwauli.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.hesvh.cn/Article/details/gcenvheec.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.hesvh.cn/Article/details/gxuvkoeds.sHtML

Ruby: obj.instance_variables
来源：http://3g.zdbjq.cn/Article/details/ggcrozumk.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.hesvh.cn/Article/details/gvdqsadak.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gtrwefpzt.sHtML

H. 异常与错误处理
来源：http://wap.zdbjq.cn/Article/details/gbljibxni.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gggidwusg.sHtML

[H01] try / catch 基础
来源：http://mobile.hesvh.cn/Article/details/gmsvbftyf.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.zdbjq.cn/Article/details/galqfbhqe.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.hesvh.cn/Article/details/gjjkamubd.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.fehbvm.com/Article/details/gaoznnphz.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mobile.fehbvm.com/Article/details/gulhfmumw.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://baike.zdbjq.cn/Article/details/geudmhzac.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mobile.fehbvm.com/Article/details/gkketlrnf.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.m.share.fehbvm.com/Article/details/gyaniqwrp.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.zdbjq.cn/Article/details/gcpuouayo.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.zdbjq.cn/Article/details/gbwnfgpar.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://baike.hesvh.cn/Article/details/gyycvevbl.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gxnmrxhiy.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://baike.hesvh.cn/Article/details/genszrgub.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.share.zdbjq.cn/Article/details/gqnazngml.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.fehbvm.com/Article/details/gtsfvrlgq.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.fehbvm.com/Article/details/gvrapebym.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.zdbjq.cn/Article/details/gwhzcjcgf.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gtcfdbdgx.sHtML

[H03] 主动抛出异常
来源：http://read.share.zdbjq.cn/Article/details/glmgjhryc.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.fehbvm.com/Article/details/gzsinvshw.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://m.share.zdbjq.cn/Article/details/geqmajqxe.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.zdbjq.cn/Article/details/grvzuvwqy.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.zdbjq.cn/Article/details/ghakwukhh.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://m.share.hesvh.cn/Article/details/gagovlhvm.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wap.fehbvm.com/Article/details/gkcjrmuvb.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.m.share.fehbvm.com/Article/details/gzhrmyflk.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.m.share.zdbjq.cn/Article/details/gvteqjgtx.sHtML

[H04] 自定义异常类型
来源：http://read.share.fehbvm.com/Article/details/gsnfwtcnv.sHtML

Py:   class MyError(Exception): pass
来源：http://read.share.fehbvm.com/Article/details/gsfgjtfkm.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://m.share.fehbvm.com/Article/details/ghuxppijl.sHtML

JS:   class MyError extends Error {}
来源：http://read.share.hesvh.cn/Article/details/gseavmbua.sHtML

TS:   class MyError extends Error {}
来源：http://3g.fehbvm.com/Article/details/gwcbvcsah.sHtML

Java: class MyException extends RuntimeException {}
来源：http://mobile.zdbjq.cn/Article/details/gmgxzyvsw.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mobile.hesvh.cn/Article/details/gbphjdghh.sHtML

Ruby: class MyError < StandardError; end
来源：http://3g.fehbvm.com/Article/details/gekpfanps.sHtML

C#:   class MyException : Exception {}
来源：http://m.share.fehbvm.com/Article/details/gqjhlxytt.sHtML

[H05] 捕获特定类型
来源：http://baike.zdbjq.cn/Article/details/gjetcvhpj.sHtML

Py:   except ValueError as e:
来源：http://m.share.fehbvm.com/Article/details/gjuctxsfq.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.hesvh.cn/Article/details/gfvstjigx.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://m.share.zdbjq.cn/Article/details/gzrtjwagu.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.share.fehbvm.com/Article/details/gfpylfwad.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://m.share.fehbvm.com/Article/details/glbzmpfht.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://blog.hesvh.cn/Article/details/gekkfbyub.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.blog.fehbvm.com/Article/details/giemurezu.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://baike.hesvh.cn/Article/details/gcrsebqzs.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.blog.zdbjq.cn/Article/details/gcmfcljtf.sHtML

Py:   value = d.get("k") or default
来源：http://baike.fehbvm.com/Article/details/gwzglzkdq.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.m.share.hesvh.cn/Article/details/gheueuqpy.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.blog.zdbjq.cn/Article/details/ghhfneifv.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.blog.fehbvm.com/Article/details/gyeprupsp.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.blog.zdbjq.cn/Article/details/gjypcdwjw.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://3g.hesvh.cn/Article/details/gwjhhqdnm.sHtML

Ruby: d&.dig(:a, :b)
来源：http://mobile.hesvh.cn/Article/details/gnrorhgpz.sHtML

C#:   obj?.A?.B ?? default
来源：http://blog.zdbjq.cn/Article/details/gjjfjgrph.sHtML

[H07] 断言
来源：http://wap.fehbvm.com/Article/details/gfzkrpzab.sHtML

Py:   assert x > 0, "必须为正"
来源：http://mobile.zdbjq.cn/Article/details/godnxnage.sHtML

PHP:  assert($x > 0);
来源：http://3g.zdbjq.cn/Article/details/ggsdbdroz.sHtML

JS:   console.assert(x > 0);
来源：http://mobile.zdbjq.cn/Article/details/gjrnyvgkj.sHtML

TS:   console.assert(x > 0);
来源：http://3g.fehbvm.com/Article/details/gjpdahcie.sHtML

Java: assert x > 0 : "必须为正";
来源：http://read.share.hesvh.cn/Article/details/gzzpohtyi.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wap.hesvh.cn/Article/details/gxcpqrzsj.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://read.share.fehbvm.com/Article/details/gbfbrmjtl.sHtML

C#:   Debug.Assert(x > 0);
来源：http://blog.fehbvm.com/Article/details/gpggexjlz.sHtML

[H08] 获取错误信息与堆栈
来源：http://3g.hesvh.cn/Article/details/gjosgqlhx.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.m.share.hesvh.cn/Article/details/gippiiqsp.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://3g.zdbjq.cn/Article/details/golrvqczp.sHtML

JS:   e.message;  e.stack
来源：http://www.m.share.zdbjq.cn/Article/details/grlfzyfvi.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.blog.hesvh.cn/Article/details/gpvmnefjp.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://3g.zdbjq.cn/Article/details/guwffrgmz.sHtML

Go:   err.Error()
来源：http://wap.hesvh.cn/Article/details/gdjrhktbx.sHtML

Ruby: e.message;  e.backtrace
来源：http://wap.hesvh.cn/Article/details/gqvvnssne.sHtML

C#:   e.Message;  e.StackTrace
来源：http://read.share.fehbvm.com/Article/details/gkvrefsln.sHtML

[H09] 带错误码的异常
来源：http://www.share.hesvh.cn/Article/details/gbqfcgqft.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.m.share.hesvh.cn/Article/details/gzjfhorjp.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://read.share.hesvh.cn/Article/details/ghqdgbyqt.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.m.share.zdbjq.cn/Article/details/ghzvphuei.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://blog.hesvh.cn/Article/details/gvhdninfs.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://baike.zdbjq.cn/Article/details/gutaeljgu.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mobile.hesvh.cn/Article/details/gpuapghpl.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://mobile.hesvh.cn/Article/details/grlfdlitu.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://mobile.zdbjq.cn/Article/details/gbragywtu.sHtML

[H10] 资源自动释放
来源：http://www.blog.hesvh.cn/Article/details/gkwucwfui.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.blog.hesvh.cn/Article/details/gpxitdsrh.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.share.zdbjq.cn/Article/details/giniceffs.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.fehbvm.com/Article/details/ghxicsprm.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.zdbjq.cn/Article/details/gpnjyecas.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://3g.hesvh.cn/Article/details/gypvyppro.sHtML

Go:   defer f.Close()
来源：http://m.share.fehbvm.com/Article/details/gtuvimpmu.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mobile.zdbjq.cn/Article/details/gangpwjrk.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gkfuhhhpo.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/girwnadyr.sHtML

I. 正则表达式
来源：http://read.share.fehbvm.com/Article/details/gonqnxmqp.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gfztjmufe.sHtML

[I01] 判断是否匹配
来源：http://m.share.fehbvm.com/Article/details/gacmkropb.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://blog.zdbjq.cn/Article/details/gpmrgboie.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://wap.hesvh.cn/Article/details/gaqmbomxg.sHtML

JS:   /\d+/.test(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gpysoxkvy.sHtML

TS:   /\d+/.test(s)
来源：http://m.share.hesvh.cn/Article/details/gznrurxqp.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.share.fehbvm.com/Article/details/gsdckgszk.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://blog.zdbjq.cn/Article/details/gbrlhlass.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.blog.zdbjq.cn/Article/details/gofmupyjo.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://3g.hesvh.cn/Article/details/ggmyplwwp.sHtML

[I02] 提取所有匹配
来源：http://www.m.share.fehbvm.com/Article/details/gbphayczo.sHtML

Py:   re.findall(r"\d+", s)
来源：http://blog.zdbjq.cn/Article/details/garmsmrhn.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://3g.zdbjq.cn/Article/details/glxerebaf.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://3g.hesvh.cn/Article/details/gzzbrinsp.sHtML

TS:   s.match(/\d+/g)
来源：http://www.m.share.zdbjq.cn/Article/details/gsvrkeciw.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.share.hesvh.cn/Article/details/gwcdqfjrw.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://baike.fehbvm.com/Article/details/gfzbqvpmi.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.blog.zdbjq.cn/Article/details/gkhemqiux.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.m.share.fehbvm.com/Article/details/gjihsxnug.sHtML

[I03] 提取捕获分组
来源：http://wap.zdbjq.cn/Article/details/gxemhunox.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://baike.zdbjq.cn/Article/details/gmxydlwvu.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mobile.fehbvm.com/Article/details/gfijpubbv.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://3g.fehbvm.com/Article/details/gsuqhlpaw.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.blog.hesvh.cn/Article/details/gfezxrppn.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.blog.hesvh.cn/Article/details/gchpkvege.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://read.share.hesvh.cn/Article/details/ghvrfitgi.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.m.share.hesvh.cn/Article/details/gfrucobsk.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://read.share.hesvh.cn/Article/details/gpphdbctg.sHtML

[I04] 正则替换
来源：http://www.m.share.zdbjq.cn/Article/details/gpsbyrwew.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.share.fehbvm.com/Article/details/gzuyvmzok.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://3g.zdbjq.cn/Article/details/gkgjttgbb.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.fehbvm.com/Article/details/gsitoervp.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://read.share.hesvh.cn/Article/details/gdmqiaxbd.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.share.hesvh.cn/Article/details/gctsvbrkq.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://read.share.zdbjq.cn/Article/details/gjcsnkgdw.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.m.share.hesvh.cn/Article/details/goddkowvk.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://blog.hesvh.cn/Article/details/gdusqrupp.sHtML

[I05] 按正则拆分
来源：http://baike.hesvh.cn/Article/details/gqmgnyapw.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://baike.hesvh.cn/Article/details/gzjmfiuia.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.share.fehbvm.com/Article/details/grfmlhdpu.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://m.share.hesvh.cn/Article/details/gztycmums.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://m.share.hesvh.cn/Article/details/gguisytbi.sHtML

Java: s.split("\\s*,\\s*")
来源：http://mobile.zdbjq.cn/Article/details/gmmhmrgxg.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.blog.fehbvm.com/Article/details/gasmiqbsl.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.blog.hesvh.cn/Article/details/goqlqnucp.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.share.fehbvm.com/Article/details/gkubprepi.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://read.share.zdbjq.cn/Article/details/gbalbdzme.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://3g.fehbvm.com/Article/details/geqcoydtd.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://baike.zdbjq.cn/Article/details/gloianzsu.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.fehbvm.com/Article/details/gcciqmizn.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.fehbvm.com/Article/details/gmuloopsc.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://m.share.fehbvm.com/Article/details/gfhojobqu.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://m.share.zdbjq.cn/Article/details/gfslxpsxj.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.m.share.fehbvm.com/Article/details/gfdslwtok.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mobile.hesvh.cn/Article/details/gjtaibvxf.sHtML

[I07] 忽略大小写与多行模式
来源：http://mobile.fehbvm.com/Article/details/gevwyiypf.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wap.fehbvm.com/Article/details/ggdyvnvpv.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.blog.hesvh.cn/Article/details/gyywttssd.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wap.hesvh.cn/Article/details/gylfbbtyy.sHtML

TS:   /error/gim
来源：http://m.share.hesvh.cn/Article/details/gzmxygnbu.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wap.fehbvm.com/Article/details/gcedcnygd.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.share.zdbjq.cn/Article/details/gpblynmsw.sHtML

Ruby: s.scan(/error/i)
来源：http://read.share.hesvh.cn/Article/details/gskpzwtdq.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://read.share.hesvh.cn/Article/details/gsuvonnde.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.blog.hesvh.cn/Article/details/gprbznipo.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://m.share.zdbjq.cn/Article/details/gqgfmveja.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.blog.fehbvm.com/Article/details/gwipwciyt.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.fehbvm.com/Article/details/gffgbkbne.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.zdbjq.cn/Article/details/gvlxzkhoi.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.blog.zdbjq.cn/Article/details/gosmfpssc.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://read.share.hesvh.cn/Article/details/gazlncqph.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.blog.zdbjq.cn/Article/details/gmogmjszb.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://blog.hesvh.cn/Article/details/gtbsfxpkz.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gvdogsehm.sHtML

J. 日期与时间
来源：http://wap.fehbvm.com/Article/details/gzdhgnhit.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gzvpowpti.sHtML

[J01] 获取当前时间
来源：http://3g.fehbvm.com/Article/details/gargokwyv.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://wap.zdbjq.cn/Article/details/gufpadptl.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://read.share.zdbjq.cn/Article/details/gqkjxiogp.sHtML

JS:   new Date();  Date.now()
来源：http://www.share.fehbvm.com/Article/details/gfmthjkhd.sHtML

TS:   new Date();  Date.now()
来源：http://read.share.fehbvm.com/Article/details/gmwnbbtlk.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://read.share.hesvh.cn/Article/details/gpemhpsrc.sHtML

Go:   time.Now()
来源：http://baike.hesvh.cn/Article/details/gqbygmrfi.sHtML

Ruby: Time.now
来源：http://mobile.fehbvm.com/Article/details/godbpmpwz.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wap.zdbjq.cn/Article/details/gaphewcsh.sHtML

[J02] 格式化输出
来源：http://m.share.fehbvm.com/Article/details/gwsdcpmrc.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.fehbvm.com/Article/details/gwrcusmsi.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://m.share.fehbvm.com/Article/details/gnobfosge.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://read.share.zdbjq.cn/Article/details/ghiorwlml.sHtML

TS:   d.toISOString()
来源：http://baike.fehbvm.com/Article/details/gqhemrgyz.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://wap.fehbvm.com/Article/details/gueutvmcs.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wap.fehbvm.com/Article/details/gysutdnau.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.hesvh.cn/Article/details/gmkimvnmf.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://blog.fehbvm.com/Article/details/gilyagmnw.sHtML

[J03] 字符串解析为日期
来源：http://blog.fehbvm.com/Article/details/gfbcviaan.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://read.share.fehbvm.com/Article/details/gdkuhkxrc.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wap.fehbvm.com/Article/details/goqpeeavx.sHtML

JS:   new Date("2024-01-02")
来源：http://wap.hesvh.cn/Article/details/gmrxtrcqi.sHtML

TS:   new Date("2024-01-02")
来源：http://www.m.share.fehbvm.com/Article/details/gihpyglgz.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://m.share.fehbvm.com/Article/details/gbjppaqyd.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://m.share.hesvh.cn/Article/details/gswwcfpiw.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.share.fehbvm.com/Article/details/gbveirmxt.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://3g.fehbvm.com/Article/details/gzycpwzbq.sHtML

[J04] 时间戳与日期互转
来源：http://wap.hesvh.cn/Article/details/gcsmwxyba.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://m.share.hesvh.cn/Article/details/gijzqiymd.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://mobile.fehbvm.com/Article/details/gjseuhxgz.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.blog.zdbjq.cn/Article/details/gfkeysvgi.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://wap.zdbjq.cn/Article/details/gdrhodphu.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://m.share.hesvh.cn/Article/details/gtjbmefea.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://3g.fehbvm.com/Article/details/gmxggianz.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://baike.hesvh.cn/Article/details/gogjtfaqk.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://m.share.hesvh.cn/Article/details/gsumpwwjp.sHtML

[J05] 时间加减（加 7 天）
来源：http://blog.fehbvm.com/Article/details/gcjyxpzle.sHtML

Py:   now + timedelta(days=7)
来源：http://3g.zdbjq.cn/Article/details/gvwjctoir.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://baike.hesvh.cn/Article/details/gkgjksftv.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.fehbvm.com/Article/details/gowyphdkp.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.zdbjq.cn/Article/details/gtrtmjdzn.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://read.share.zdbjq.cn/Article/details/goqetccnt.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.share.hesvh.cn/Article/details/gnpxzwhxa.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.share.fehbvm.com/Article/details/gyufaratd.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://mobile.fehbvm.com/Article/details/gfbalcjcw.sHtML

[J06] 计算两时间之差
来源：http://www.share.hesvh.cn/Article/details/grjrkwydl.sHtML

Py:   (end - start).total_seconds()
来源：http://www.m.share.fehbvm.com/Article/details/gesiilddl.sHtML

PHP:  $end->diff($start)->days;
来源：http://3g.zdbjq.cn/Article/details/gthyjcdgh.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.share.hesvh.cn/Article/details/gzecdssjb.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.blog.fehbvm.com/Article/details/getaqqbsr.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://mobile.hesvh.cn/Article/details/gnzzrlwmx.sHtML

Go:   end.Sub(start).Hours()
来源：http://read.share.hesvh.cn/Article/details/gcgskzkqj.sHtML

Ruby: end - start                 # 返回秒数
来源：http://m.share.fehbvm.com/Article/details/goemqhrqh.sHtML

C#:   (end - start).TotalSeconds
来源：http://blog.zdbjq.cn/Article/details/gnxquspog.sHtML

[J07] 比较两个日期
来源：http://baike.zdbjq.cn/Article/details/ggenwtjkq.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://read.share.zdbjq.cn/Article/details/gouzsxqvk.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://baike.zdbjq.cn/Article/details/gfslsvpie.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.share.fehbvm.com/Article/details/gkdwppwjz.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://read.share.fehbvm.com/Article/details/gbykqgerj.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://3g.fehbvm.com/Article/details/gmyaoocpi.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://3g.fehbvm.com/Article/details/ggweouqlp.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://m.share.fehbvm.com/Article/details/geequdmar.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://baike.fehbvm.com/Article/details/gzfxypbyp.sHtML

[J08] 提取年月日与星期
来源：http://read.share.hesvh.cn/Article/details/gftswthuu.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://m.share.fehbvm.com/Article/details/gadulgmgv.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://blog.zdbjq.cn/Article/details/gdlynwair.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://m.share.zdbjq.cn/Article/details/gkmjfrmhh.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://3g.fehbvm.com/Article/details/gdckoofvv.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wap.zdbjq.cn/Article/details/gnalzbobf.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://mobile.zdbjq.cn/Article/details/gxeltytsa.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.blog.fehbvm.com/Article/details/ghhutctfc.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://read.share.fehbvm.com/Article/details/gpxsoxoat.sHtML

[J09] 时区处理
来源：http://blog.hesvh.cn/Article/details/gchfyidud.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.m.share.fehbvm.com/Article/details/gdujszqix.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.m.share.fehbvm.com/Article/details/gddronwkz.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.fehbvm.com/Article/details/gzrddiesu.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.fehbvm.com/Article/details/gbtnzjmnf.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.m.share.fehbvm.com/Article/details/golkxaiyp.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://baike.fehbvm.com/Article/details/gsbzsyyna.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://baike.hesvh.cn/Article/details/gjbwvpilp.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mobile.zdbjq.cn/Article/details/gxheagkgc.sHtML

[J10] 取今天 / 本月第一天
来源：http://wap.fehbvm.com/Article/details/gncysxyhn.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.share.hesvh.cn/Article/details/gwwemsmii.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wap.fehbvm.com/Article/details/ggpvuroef.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://blog.hesvh.cn/Article/details/gkazdncii.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wap.zdbjq.cn/Article/details/gzixnhqbb.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.share.zdbjq.cn/Article/details/gpevtmmpv.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://read.share.zdbjq.cn/Article/details/gsxnubcfx.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://m.share.fehbvm.com/Article/details/gwarnfnwh.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.blog.hesvh.cn/Article/details/ghjdwxzpd.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gyhlvmcuw.sHtML

K. JSON 与序列化
来源：http://blog.fehbvm.com/Article/details/geulftlvc.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gpwgizokb.sHtML

[K01] 对象转 JSON 字符串
来源：http://read.share.zdbjq.cn/Article/details/gcgatzmjs.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.m.share.hesvh.cn/Article/details/ggbrknoyo.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://baike.hesvh.cn/Article/details/gcugfcvqx.sHtML

JS:   JSON.stringify(obj)
来源：http://www.blog.hesvh.cn/Article/details/gymabfsxo.sHtML

TS:   JSON.stringify(obj)
来源：http://read.share.fehbvm.com/Article/details/ggrcfcjin.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.blog.zdbjq.cn/Article/details/gijkruzdt.sHtML

Go:   json.Marshal(obj)
来源：http://mobile.zdbjq.cn/Article/details/gzrdxzkeu.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://mobile.hesvh.cn/Article/details/glgaiyykj.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://blog.zdbjq.cn/Article/details/gmxilumfa.sHtML

[K02] JSON 字符串转对象
来源：http://3g.hesvh.cn/Article/details/gbdpelhth.sHtML

Py:   json.loads(s)
来源：http://baike.zdbjq.cn/Article/details/gbxxalxps.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mobile.zdbjq.cn/Article/details/gagqahnbt.sHtML

JS:   JSON.parse(s)
来源：http://m.share.hesvh.cn/Article/details/gbboqwrzw.sHtML


<!-- 参考信息 -->