代发 wailian999

Py:   isinstance(u, User)
来源：http://www.share.fehbvm.com/Article/details/gkatkldap.sHtML

PHP:  $u instanceof User
来源：http://www.blog.hesvh.cn/Article/details/gybzxlaeu.sHtML

JS:   u instanceof User
来源：http://www.m.share.hesvh.cn/Article/details/gfprqxbsy.sHtML

TS:   u instanceof User
来源：http://mobile.fehbvm.com/Article/details/gxgqgoxhk.sHtML

Java: u instanceof User
来源：http://read.share.fehbvm.com/Article/details/glhlbrlvr.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.fehbvm.com/Article/details/gwrfcitlb.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.hesvh.cn/Article/details/gyjoslfgv.sHtML

C#:   u is User
来源：http://wap.hesvh.cn/Article/details/gppoztoec.sHtML

[G14] 数据类 / record
来源：http://mobile.hesvh.cn/Article/details/gtovhegjd.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://baike.fehbvm.com/Article/details/gaowgxovq.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://read.share.fehbvm.com/Article/details/grsesndxs.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.hesvh.cn/Article/details/gvxbngoms.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.hesvh.cn/Article/details/grpmmnrud.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.zdbjq.cn/Article/details/gmmtdcnif.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.hesvh.cn/Article/details/gjoaudwjt.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://baike.hesvh.cn/Article/details/gcnibbtay.sHtML

C#:   record User(string Name, int Age);
来源：http://read.share.fehbvm.com/Article/details/gvuemlnxx.sHtML

[G15] 枚举
来源：http://www.blog.fehbvm.com/Article/details/gmanqapqb.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.zdbjq.cn/Article/details/gjwbzsbsn.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.fehbvm.com/Article/details/gyrdjkdre.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.zdbjq.cn/Article/details/gmmjbraol.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.fehbvm.com/Article/details/guljptxmr.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.zdbjq.cn/Article/details/gjmglogan.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.fehbvm.com/Article/details/genzfjacq.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.hesvh.cn/Article/details/gcmsouxwe.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.hesvh.cn/Article/details/gvmgognpu.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.zdbjq.cn/Article/details/gqywmafvk.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.fehbvm.com/Article/details/geceqatic.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.hesvh.cn/Article/details/ggsuntopl.sHtML

JS:   Object.entries(obj)
来源：http://3g.hesvh.cn/Article/details/gkferehln.sHtML

TS:   Object.entries(obj)
来源：http://3g.zdbjq.cn/Article/details/gebqfkwlf.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.hesvh.cn/Article/details/gmhixiean.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.zdbjq.cn/Article/details/geiejmmem.sHtML

Ruby: obj.instance_variables
来源：http://www.m.share.fehbvm.com/Article/details/grjfkpbzu.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://blog.fehbvm.com/Article/details/gbykyoqnz.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/giajkmivs.sHtML

H. 异常与错误处理
来源：http://baike.zdbjq.cn/Article/details/gpglzkamn.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gtfnsyhui.sHtML

[H01] try / catch 基础
来源：http://wap.fehbvm.com/Article/details/giifbnyka.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://read.share.zdbjq.cn/Article/details/gzkczztuh.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.blog.zdbjq.cn/Article/details/gjjzxcaoi.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://blog.zdbjq.cn/Article/details/glaixdobn.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.m.share.hesvh.cn/Article/details/grrbtoahc.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.zdbjq.cn/Article/details/ghiilpwan.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.zdbjq.cn/Article/details/gfqfwgzus.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.hesvh.cn/Article/details/gtqualwdu.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mobile.zdbjq.cn/Article/details/gcdxxpfro.sHtML

[H02] finally / ensure 收尾
来源：http://blog.hesvh.cn/Article/details/gradbadyb.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://read.share.fehbvm.com/Article/details/grjbdfmov.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/gwhwtlyva.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/gavetadfd.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://m.share.hesvh.cn/Article/details/gbisxbfbm.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://wap.hesvh.cn/Article/details/gkivracbq.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.hesvh.cn/Article/details/grspebbjj.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.fehbvm.com/Article/details/glezyvdee.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://m.share.fehbvm.com/Article/details/gndjaciin.sHtML

[H03] 主动抛出异常
来源：http://3g.zdbjq.cn/Article/details/gppakfhbv.sHtML

Py:   raise ValueError("错误信息")
来源：http://blog.fehbvm.com/Article/details/gbxsjuuim.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://m.share.zdbjq.cn/Article/details/glnbdvuya.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.hesvh.cn/Article/details/ghtemexqu.sHtML

TS:   throw new Error("错误信息");
来源：http://baike.hesvh.cn/Article/details/gxylbfpah.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.hesvh.cn/Article/details/gygbtvqos.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mobile.fehbvm.com/Article/details/gmtnvmlms.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.m.share.fehbvm.com/Article/details/gdecrxuiu.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.blog.hesvh.cn/Article/details/gqfxnuqgx.sHtML

[H04] 自定义异常类型
来源：http://www.share.hesvh.cn/Article/details/geacijqxl.sHtML

Py:   class MyError(Exception): pass
来源：http://read.share.hesvh.cn/Article/details/ggthxhrdk.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://mobile.fehbvm.com/Article/details/gkargduua.sHtML

JS:   class MyError extends Error {}
来源：http://m.share.hesvh.cn/Article/details/gujrpxvtp.sHtML

TS:   class MyError extends Error {}
来源：http://3g.zdbjq.cn/Article/details/glooeivbi.sHtML

Java: class MyException extends RuntimeException {}
来源：http://3g.zdbjq.cn/Article/details/gibfvpmep.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.share.zdbjq.cn/Article/details/grklegwpc.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.zdbjq.cn/Article/details/gdlvtmfdp.sHtML

C#:   class MyException : Exception {}
来源：http://mobile.hesvh.cn/Article/details/gzavhvlhr.sHtML

[H05] 捕获特定类型
来源：http://mobile.fehbvm.com/Article/details/gzdvkdjwq.sHtML

Py:   except ValueError as e:
来源：http://read.share.fehbvm.com/Article/details/gdkylivfh.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.blog.zdbjq.cn/Article/details/gocguylwd.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.share.fehbvm.com/Article/details/grwdrioec.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://blog.fehbvm.com/Article/details/gwxnudieq.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://baike.hesvh.cn/Article/details/gdagufwje.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://baike.zdbjq.cn/Article/details/gvozhayyg.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.blog.fehbvm.com/Article/details/ggidazqhq.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mobile.zdbjq.cn/Article/details/grlalsahy.sHtML

[H06] 可选值 / 空值安全访问
来源：http://3g.fehbvm.com/Article/details/gngzdixfa.sHtML

Py:   value = d.get("k") or default
来源：http://read.share.zdbjq.cn/Article/details/ggvofzklm.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://blog.hesvh.cn/Article/details/gftkjqyuv.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://3g.fehbvm.com/Article/details/gvgoebikt.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://blog.fehbvm.com/Article/details/guduygbox.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://m.share.fehbvm.com/Article/details/gmsfdjyqk.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.m.share.fehbvm.com/Article/details/gsenxltru.sHtML

Ruby: d&.dig(:a, :b)
来源：http://read.share.hesvh.cn/Article/details/gcwpynklp.sHtML

C#:   obj?.A?.B ?? default
来源：http://read.share.fehbvm.com/Article/details/gpcfuoevc.sHtML

[H07] 断言
来源：http://baike.zdbjq.cn/Article/details/gtyacdhpz.sHtML

Py:   assert x > 0, "必须为正"
来源：http://m.share.fehbvm.com/Article/details/gsbplkitk.sHtML

PHP:  assert($x > 0);
来源：http://baike.hesvh.cn/Article/details/gmsasrxbt.sHtML

JS:   console.assert(x > 0);
来源：http://3g.hesvh.cn/Article/details/gakuxrlkm.sHtML

TS:   console.assert(x > 0);
来源：http://baike.zdbjq.cn/Article/details/gdilqhbhw.sHtML

Java: assert x > 0 : "必须为正";
来源：http://baike.zdbjq.cn/Article/details/glpgltykd.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mobile.hesvh.cn/Article/details/gfmudkiio.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://3g.fehbvm.com/Article/details/gcnaxqrel.sHtML

C#:   Debug.Assert(x > 0);
来源：http://wap.fehbvm.com/Article/details/gjipsrrcb.sHtML

[H08] 获取错误信息与堆栈
来源：http://read.share.fehbvm.com/Article/details/gmnnovumg.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://read.share.fehbvm.com/Article/details/gbqqywovf.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mobile.zdbjq.cn/Article/details/gymmijmvs.sHtML

JS:   e.message;  e.stack
来源：http://blog.zdbjq.cn/Article/details/gxsfdkfim.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.blog.zdbjq.cn/Article/details/gsucicbhf.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://m.share.fehbvm.com/Article/details/gvqgyblso.sHtML

Go:   err.Error()
来源：http://www.m.share.hesvh.cn/Article/details/gykateven.sHtML

Ruby: e.message;  e.backtrace
来源：http://blog.hesvh.cn/Article/details/glsnjosoc.sHtML

C#:   e.Message;  e.StackTrace
来源：http://baike.fehbvm.com/Article/details/gqcweuqai.sHtML

[H09] 带错误码的异常
来源：http://3g.fehbvm.com/Article/details/ggomkdanl.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.blog.hesvh.cn/Article/details/ghzilatsa.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://m.share.hesvh.cn/Article/details/gdfsmwhkp.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.share.fehbvm.com/Article/details/gzqqeywju.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://baike.zdbjq.cn/Article/details/giragmlsr.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://3g.hesvh.cn/Article/details/gmytxwppt.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wap.fehbvm.com/Article/details/gsvbafgxt.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://wap.zdbjq.cn/Article/details/glpnfeebg.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://baike.fehbvm.com/Article/details/gurkpwapk.sHtML

[H10] 资源自动释放
来源：http://www.share.fehbvm.com/Article/details/gnflxhjoj.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://m.share.fehbvm.com/Article/details/ghmjisxeq.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://3g.hesvh.cn/Article/details/gnpzqddrw.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.hesvh.cn/Article/details/gvovikujx.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.fehbvm.com/Article/details/gpyemnzpx.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://blog.fehbvm.com/Article/details/gwjoyxxsu.sHtML

Go:   defer f.Close()
来源：http://mobile.zdbjq.cn/Article/details/gelsyodsa.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://read.share.hesvh.cn/Article/details/ghkdlkrgm.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gbqcmaayt.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/ghydygnzi.sHtML

I. 正则表达式
来源：http://wap.hesvh.cn/Article/details/gricosfvh.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gdvpecgnh.sHtML

[I01] 判断是否匹配
来源：http://www.blog.zdbjq.cn/Article/details/gxldzkzvv.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.blog.zdbjq.cn/Article/details/gdoczrthb.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.blog.fehbvm.com/Article/details/gvpeyrmbp.sHtML

JS:   /\d+/.test(s)
来源：http://baike.hesvh.cn/Article/details/gzfiygvrn.sHtML

TS:   /\d+/.test(s)
来源：http://3g.zdbjq.cn/Article/details/ghkrskqas.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://m.share.fehbvm.com/Article/details/grmjzhexp.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.blog.fehbvm.com/Article/details/gcujxbtwt.sHtML

Ruby: s.match?(/\d+/)
来源：http://blog.hesvh.cn/Article/details/gsjhhspyc.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://baike.fehbvm.com/Article/details/gdlvumemb.sHtML

[I02] 提取所有匹配
来源：http://baike.fehbvm.com/Article/details/geevjaera.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.blog.hesvh.cn/Article/details/gqhxjzhmc.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://blog.hesvh.cn/Article/details/gukwlhjsq.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.share.zdbjq.cn/Article/details/gcxcrcdhd.sHtML

TS:   s.match(/\d+/g)
来源：http://www.share.zdbjq.cn/Article/details/gqaaxlqsh.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.blog.zdbjq.cn/Article/details/gwqhxvqeb.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://blog.hesvh.cn/Article/details/gdmdpvnkj.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.share.zdbjq.cn/Article/details/gutzuroxo.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.share.zdbjq.cn/Article/details/guyxfwqix.sHtML

[I03] 提取捕获分组
来源：http://wap.hesvh.cn/Article/details/gberhbsyi.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.share.zdbjq.cn/Article/details/gtqoqdnhc.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.share.hesvh.cn/Article/details/gwhlifjtz.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.blog.fehbvm.com/Article/details/giqckncfs.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.m.share.zdbjq.cn/Article/details/gtqwcpkip.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.m.share.fehbvm.com/Article/details/glapftsia.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://read.share.zdbjq.cn/Article/details/gnugzkbfp.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wap.fehbvm.com/Article/details/gvplmekfy.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://3g.hesvh.cn/Article/details/gnmjmieif.sHtML

[I04] 正则替换
来源：http://baike.hesvh.cn/Article/details/gggpabmcz.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.m.share.zdbjq.cn/Article/details/gyolgnxoj.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://read.share.zdbjq.cn/Article/details/gxgcdhnfy.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://wap.hesvh.cn/Article/details/goauigyvv.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.zdbjq.cn/Article/details/gthjmjmnt.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.blog.zdbjq.cn/Article/details/gcrkxjeho.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://read.share.fehbvm.com/Article/details/gkgyfyazx.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.blog.hesvh.cn/Article/details/gemaehmgf.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://baike.zdbjq.cn/Article/details/grlemhdpb.sHtML

[I05] 按正则拆分
来源：http://www.share.hesvh.cn/Article/details/gtcvvjuyn.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.m.share.hesvh.cn/Article/details/gcxyrmmgr.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.share.hesvh.cn/Article/details/grnzlsgek.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://wap.hesvh.cn/Article/details/gdlfufmbg.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://blog.fehbvm.com/Article/details/gfaomyzgd.sHtML

Java: s.split("\\s*,\\s*")
来源：http://3g.zdbjq.cn/Article/details/gafhcfsgc.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.share.zdbjq.cn/Article/details/gfleiivdb.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://mobile.hesvh.cn/Article/details/gdzrwlaia.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.blog.fehbvm.com/Article/details/gosjwfizr.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://m.share.zdbjq.cn/Article/details/gbqjsnfhw.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.share.zdbjq.cn/Article/details/gshelnbox.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://blog.zdbjq.cn/Article/details/gwyfugkii.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.zdbjq.cn/Article/details/gydzesdwd.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.zdbjq.cn/Article/details/gsgwzzuit.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.m.share.fehbvm.com/Article/details/gcyeikpqi.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wap.hesvh.cn/Article/details/gbpykupfg.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.share.hesvh.cn/Article/details/goqnnfpuu.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://m.share.hesvh.cn/Article/details/gisqhucff.sHtML

[I07] 忽略大小写与多行模式
来源：http://mobile.zdbjq.cn/Article/details/gmmarlzoy.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.m.share.hesvh.cn/Article/details/gcuasrguo.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mobile.fehbvm.com/Article/details/grvptlypc.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.m.share.zdbjq.cn/Article/details/gjskibiho.sHtML

TS:   /error/gim
来源：http://baike.zdbjq.cn/Article/details/gxsruqxjt.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.m.share.hesvh.cn/Article/details/gxnqvcnby.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://m.share.zdbjq.cn/Article/details/gnzailmen.sHtML

Ruby: s.scan(/error/i)
来源：http://www.share.hesvh.cn/Article/details/gvrrgdefd.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.m.share.hesvh.cn/Article/details/gpjwnpncq.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.blog.zdbjq.cn/Article/details/gwnfuzqse.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://read.share.fehbvm.com/Article/details/gvbslpkwv.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://baike.fehbvm.com/Article/details/gobfkkqsn.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.zdbjq.cn/Article/details/glivyapek.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.hesvh.cn/Article/details/gkrfcxind.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.m.share.fehbvm.com/Article/details/gbxilyszm.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.share.fehbvm.com/Article/details/gclgmtosu.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.m.share.hesvh.cn/Article/details/gnkcbavic.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://m.share.zdbjq.cn/Article/details/grrwlmnex.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gtuzsepym.sHtML

J. 日期与时间
来源：http://www.m.share.zdbjq.cn/Article/details/gpdridgzc.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gcflsmcqi.sHtML

[J01] 获取当前时间
来源：http://wap.hesvh.cn/Article/details/gftegxaab.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://mobile.zdbjq.cn/Article/details/gazxrinav.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.m.share.fehbvm.com/Article/details/goeouyciz.sHtML

JS:   new Date();  Date.now()
来源：http://3g.zdbjq.cn/Article/details/gafcfczbx.sHtML

TS:   new Date();  Date.now()
来源：http://www.blog.zdbjq.cn/Article/details/gjajcqkvi.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://3g.hesvh.cn/Article/details/grzuvakjr.sHtML

Go:   time.Now()
来源：http://www.blog.fehbvm.com/Article/details/gjfkvhiox.sHtML

Ruby: Time.now
来源：http://m.share.zdbjq.cn/Article/details/gpbpxbqze.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://mobile.hesvh.cn/Article/details/gmqqpmuuh.sHtML

[J02] 格式化输出
来源：http://blog.zdbjq.cn/Article/details/goeuyxzjk.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.zdbjq.cn/Article/details/goldjoknq.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://baike.fehbvm.com/Article/details/gjpxssevu.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://baike.hesvh.cn/Article/details/gdasyrdia.sHtML

TS:   d.toISOString()
来源：http://read.share.fehbvm.com/Article/details/gviqxzlie.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://m.share.hesvh.cn/Article/details/gihzwjkxn.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://read.share.hesvh.cn/Article/details/gldbdzyar.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.fehbvm.com/Article/details/gsnkdvuhx.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://mobile.fehbvm.com/Article/details/gpyghywnm.sHtML

[J03] 字符串解析为日期
来源：http://read.share.zdbjq.cn/Article/details/gzqhhnhcb.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://blog.hesvh.cn/Article/details/gexswceay.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://mobile.zdbjq.cn/Article/details/gwqkxptjs.sHtML

JS:   new Date("2024-01-02")
来源：http://baike.fehbvm.com/Article/details/gwwrurczj.sHtML

TS:   new Date("2024-01-02")
来源：http://m.share.fehbvm.com/Article/details/gllbblgif.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.m.share.fehbvm.com/Article/details/gppzfsajc.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://read.share.fehbvm.com/Article/details/gmolniiqt.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://baike.fehbvm.com/Article/details/gnvmhltcf.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://m.share.fehbvm.com/Article/details/gzqszcjbl.sHtML

[J04] 时间戳与日期互转
来源：http://baike.zdbjq.cn/Article/details/guyiqxukh.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wap.hesvh.cn/Article/details/glgnoqinl.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://baike.zdbjq.cn/Article/details/gdgjarsyk.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://3g.hesvh.cn/Article/details/gwqbquqdw.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://read.share.hesvh.cn/Article/details/gxgirvazg.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.blog.hesvh.cn/Article/details/gckxjdkdo.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://baike.zdbjq.cn/Article/details/gxafoctxm.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://3g.fehbvm.com/Article/details/gyypzzmzf.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wap.zdbjq.cn/Article/details/gjsbparbg.sHtML

[J05] 时间加减（加 7 天）
来源：http://blog.hesvh.cn/Article/details/gbdpxrvcd.sHtML

Py:   now + timedelta(days=7)
来源：http://blog.zdbjq.cn/Article/details/gdgdewlaj.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.m.share.hesvh.cn/Article/details/gvkvoxngp.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.zdbjq.cn/Article/details/gvmzyouzo.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.fehbvm.com/Article/details/gbwdanrtx.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.blog.zdbjq.cn/Article/details/gkhqvydwc.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://3g.zdbjq.cn/Article/details/gbbexhonm.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.m.share.fehbvm.com/Article/details/ggjnxrxbb.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.m.share.zdbjq.cn/Article/details/gdbjrbhdi.sHtML

[J06] 计算两时间之差
来源：http://m.share.hesvh.cn/Article/details/gurxopzfo.sHtML

Py:   (end - start).total_seconds()
来源：http://m.share.hesvh.cn/Article/details/gqpgkoibl.sHtML

PHP:  $end->diff($start)->days;
来源：http://3g.fehbvm.com/Article/details/guwgsxiwj.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.m.share.fehbvm.com/Article/details/glgqyjdip.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.blog.zdbjq.cn/Article/details/gyvdoowos.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://wap.fehbvm.com/Article/details/gziumzbgs.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.blog.zdbjq.cn/Article/details/gzhuackmc.sHtML

Ruby: end - start                 # 返回秒数
来源：http://m.share.hesvh.cn/Article/details/gmfxogkxi.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.m.share.hesvh.cn/Article/details/guxckbsyz.sHtML

[J07] 比较两个日期
来源：http://3g.hesvh.cn/Article/details/gsffflcdk.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://wap.zdbjq.cn/Article/details/ghhtspnee.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://blog.hesvh.cn/Article/details/gbdbsbdkw.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://read.share.zdbjq.cn/Article/details/gnivkxwmk.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://read.share.hesvh.cn/Article/details/glgmdlpxv.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.m.share.hesvh.cn/Article/details/guqszlfwd.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://mobile.fehbvm.com/Article/details/gpqljydbe.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.blog.fehbvm.com/Article/details/gcndswwzb.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.share.hesvh.cn/Article/details/gyjtidcqt.sHtML

[J08] 提取年月日与星期
来源：http://baike.hesvh.cn/Article/details/gwpzjrozo.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.blog.zdbjq.cn/Article/details/gslcdcklf.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.blog.zdbjq.cn/Article/details/gkdwuslag.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.blog.fehbvm.com/Article/details/gizshktnb.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://3g.fehbvm.com/Article/details/gdkqdicfz.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://3g.hesvh.cn/Article/details/gzuqbapfb.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://baike.fehbvm.com/Article/details/gqigmvcgc.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.blog.fehbvm.com/Article/details/gwdbokmos.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://read.share.fehbvm.com/Article/details/gfgfsmoxq.sHtML

[J09] 时区处理
来源：http://3g.zdbjq.cn/Article/details/gasovbzkf.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://m.share.hesvh.cn/Article/details/galnmkflj.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://3g.hesvh.cn/Article/details/grwnwxzpd.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.fehbvm.com/Article/details/gjqhbsabb.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.fehbvm.com/Article/details/gsplxtdyr.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wap.fehbvm.com/Article/details/gswjcvyzk.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://3g.fehbvm.com/Article/details/grcpljhvy.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://mobile.hesvh.cn/Article/details/gxldrjzdb.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://baike.hesvh.cn/Article/details/gwbqgcmlc.sHtML

[J10] 取今天 / 本月第一天
来源：http://mobile.hesvh.cn/Article/details/gmvbdpspr.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.m.share.zdbjq.cn/Article/details/grnjnpkbo.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://m.share.zdbjq.cn/Article/details/gyrzuteun.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://blog.zdbjq.cn/Article/details/gidlcpnsi.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://3g.hesvh.cn/Article/details/galtgfpaj.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://m.share.hesvh.cn/Article/details/ggsretlys.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://3g.fehbvm.com/Article/details/ggtfaoutz.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.blog.zdbjq.cn/Article/details/gcpdsaqcj.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://blog.zdbjq.cn/Article/details/gfxtohtez.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gbikkuprd.sHtML

K. JSON 与序列化
来源：http://mobile.hesvh.cn/Article/details/gfppjiyjh.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gutryjswa.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.m.share.hesvh.cn/Article/details/gaiqxhbth.sHtML


<!-- 参考信息 -->