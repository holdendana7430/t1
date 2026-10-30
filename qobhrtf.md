代发 wailian999

Py:   isinstance(u, User)
来源：http://m.share.fehbvm.com/Article/details/gpvlgorld.sHtML

PHP:  $u instanceof User
来源：http://blog.hesvh.cn/Article/details/gvpgvsuin.sHtML

JS:   u instanceof User
来源：http://www.m.share.fehbvm.com/Article/details/gazujymsf.sHtML

TS:   u instanceof User
来源：http://wap.hesvh.cn/Article/details/gemsluoir.sHtML

Java: u instanceof User
来源：http://www.blog.fehbvm.com/Article/details/ghgbodxpk.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.hesvh.cn/Article/details/gvmjdehqp.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.zdbjq.cn/Article/details/gxutpzodj.sHtML

C#:   u is User
来源：http://www.share.zdbjq.cn/Article/details/gvxvymnlx.sHtML

[G14] 数据类 / record
来源：http://read.share.fehbvm.com/Article/details/gvcyyzpuf.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.hesvh.cn/Article/details/gwphcqpxi.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.hesvh.cn/Article/details/gkzdpxjmw.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.hesvh.cn/Article/details/ghawejmcn.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.fehbvm.com/Article/details/gzbzspfzp.sHtML

Java: record User(String name, int age) {}
来源：http://wap.fehbvm.com/Article/details/gkdoqvlvh.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.hesvh.cn/Article/details/ghsjyoquc.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.hesvh.cn/Article/details/gotwizjbm.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.hesvh.cn/Article/details/gydjfqovi.sHtML

[G15] 枚举
来源：http://mobile.hesvh.cn/Article/details/gsfxuzuox.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://read.share.zdbjq.cn/Article/details/gnedaevlw.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.fehbvm.com/Article/details/gtdtbfpvl.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.zdbjq.cn/Article/details/gywhsxfhe.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.fehbvm.com/Article/details/gxafueafx.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.fehbvm.com/Article/details/gwfzptxtm.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.fehbvm.com/Article/details/gzskogfoy.sHtML

Ruby: Color = %i[red green].freeze
来源：http://read.share.hesvh.cn/Article/details/gnrqvjfmq.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.zdbjq.cn/Article/details/gwyqjuaet.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.fehbvm.com/Article/details/gfzwxdtyg.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.fehbvm.com/Article/details/gtbkzdkoc.sHtML

PHP:  get_object_vars($obj);
来源：http://3g.zdbjq.cn/Article/details/gdprvcuer.sHtML

JS:   Object.entries(obj)
来源：http://blog.hesvh.cn/Article/details/gzfxzrhmr.sHtML

TS:   Object.entries(obj)
来源：http://read.share.zdbjq.cn/Article/details/glrmrcrnh.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.hesvh.cn/Article/details/gkhnilcxh.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.hesvh.cn/Article/details/gczmeiabp.sHtML

Ruby: obj.instance_variables
来源：http://baike.zdbjq.cn/Article/details/gqnxjhojy.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.blog.fehbvm.com/Article/details/gnslsoqia.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gvfilftzh.sHtML

H. 异常与错误处理
来源：http://m.share.hesvh.cn/Article/details/gcdbicbsg.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gsfntkxbw.sHtML

[H01] try / catch 基础
来源：http://www.blog.zdbjq.cn/Article/details/gisbpmhsb.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.zdbjq.cn/Article/details/gvsioecvd.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.blog.zdbjq.cn/Article/details/glbacxiez.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.fehbvm.com/Article/details/gurhzavzo.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.share.fehbvm.com/Article/details/gracyfxgb.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.fehbvm.com/Article/details/gbpyksxeu.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.zdbjq.cn/Article/details/gfyibbgzb.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.m.share.hesvh.cn/Article/details/grintqnpw.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mobile.zdbjq.cn/Article/details/gdlfuwans.sHtML

[H02] finally / ensure 收尾
来源：http://wap.fehbvm.com/Article/details/gfhpnockt.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.hesvh.cn/Article/details/gyaajjzin.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.zdbjq.cn/Article/details/glquiypxz.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/ggidxkfxc.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.zdbjq.cn/Article/details/grhgqiaqm.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.zdbjq.cn/Article/details/gkxjscfgw.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://3g.zdbjq.cn/Article/details/gvbqkihnj.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.fehbvm.com/Article/details/goaospego.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://m.share.hesvh.cn/Article/details/gqotiggit.sHtML

[H03] 主动抛出异常
来源：http://3g.hesvh.cn/Article/details/gajewtaba.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.zdbjq.cn/Article/details/gvmjlsnox.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.m.share.hesvh.cn/Article/details/gxaljmclx.sHtML

JS:   throw new Error("错误信息");
来源：http://baike.fehbvm.com/Article/details/gffjlafne.sHtML

TS:   throw new Error("错误信息");
来源：http://www.blog.zdbjq.cn/Article/details/gsslqrjlb.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.fehbvm.com/Article/details/glwegxcnx.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wap.zdbjq.cn/Article/details/gwivhxkvv.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.hesvh.cn/Article/details/goepkbzxs.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.fehbvm.com/Article/details/gyozheahz.sHtML

[H04] 自定义异常类型
来源：http://mobile.zdbjq.cn/Article/details/gmeaykplf.sHtML

Py:   class MyError(Exception): pass
来源：http://baike.fehbvm.com/Article/details/gojrwpxmo.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://baike.fehbvm.com/Article/details/gtlbzpumi.sHtML

JS:   class MyError extends Error {}
来源：http://blog.zdbjq.cn/Article/details/gekxjscmh.sHtML

TS:   class MyError extends Error {}
来源：http://mobile.zdbjq.cn/Article/details/gqdlmtaox.sHtML

Java: class MyException extends RuntimeException {}
来源：http://baike.fehbvm.com/Article/details/glazylcda.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.m.share.zdbjq.cn/Article/details/gkuqaqgnr.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.zdbjq.cn/Article/details/gebwrqpyl.sHtML

C#:   class MyException : Exception {}
来源：http://www.share.hesvh.cn/Article/details/gwvssszbu.sHtML

[H05] 捕获特定类型
来源：http://blog.zdbjq.cn/Article/details/gnpuwzwqp.sHtML

Py:   except ValueError as e:
来源：http://m.share.fehbvm.com/Article/details/gkipplkzu.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://baike.zdbjq.cn/Article/details/gxlzoocbd.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://mobile.hesvh.cn/Article/details/gzesfowlh.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://read.share.hesvh.cn/Article/details/gtabuwtme.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://m.share.zdbjq.cn/Article/details/gqityctdo.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://3g.hesvh.cn/Article/details/gscbsfxja.sHtML

Ruby: rescue ArgumentError => e
来源：http://read.share.zdbjq.cn/Article/details/gjuxaqeia.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://blog.fehbvm.com/Article/details/gvusfpwfq.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.m.share.hesvh.cn/Article/details/gbnbsbhiz.sHtML

Py:   value = d.get("k") or default
来源：http://www.blog.fehbvm.com/Article/details/gjkxpgqcn.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://wap.zdbjq.cn/Article/details/gjnxouhyr.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.fehbvm.com/Article/details/gbgjrzcct.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://wap.zdbjq.cn/Article/details/gojbcsmyn.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://blog.fehbvm.com/Article/details/gjdzxikno.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.blog.zdbjq.cn/Article/details/gosrudlze.sHtML

Ruby: d&.dig(:a, :b)
来源：http://baike.hesvh.cn/Article/details/gvbtduahq.sHtML

C#:   obj?.A?.B ?? default
来源：http://baike.fehbvm.com/Article/details/gsfkxwxws.sHtML

[H07] 断言
来源：http://www.blog.fehbvm.com/Article/details/gpjiyofkh.sHtML

Py:   assert x > 0, "必须为正"
来源：http://read.share.fehbvm.com/Article/details/ghzurrjdc.sHtML

PHP:  assert($x > 0);
来源：http://www.share.hesvh.cn/Article/details/gfswtxoll.sHtML

JS:   console.assert(x > 0);
来源：http://mobile.fehbvm.com/Article/details/gxggqaqje.sHtML

TS:   console.assert(x > 0);
来源：http://3g.fehbvm.com/Article/details/gdgcjuffp.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.blog.zdbjq.cn/Article/details/gethrgviv.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wap.zdbjq.cn/Article/details/gfnobamvn.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.blog.fehbvm.com/Article/details/ghqxhsart.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.blog.hesvh.cn/Article/details/gqzxxmbho.sHtML

[H08] 获取错误信息与堆栈
来源：http://read.share.fehbvm.com/Article/details/ghazbiopu.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://read.share.zdbjq.cn/Article/details/gkdaakycm.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mobile.fehbvm.com/Article/details/gooomjbgy.sHtML

JS:   e.message;  e.stack
来源：http://read.share.hesvh.cn/Article/details/ghqctgbbb.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.blog.hesvh.cn/Article/details/gjzmkklwy.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://m.share.hesvh.cn/Article/details/gmdwmdbkf.sHtML

Go:   err.Error()
来源：http://baike.zdbjq.cn/Article/details/ggbydmbas.sHtML

Ruby: e.message;  e.backtrace
来源：http://mobile.hesvh.cn/Article/details/gpatjsbgv.sHtML

C#:   e.Message;  e.StackTrace
来源：http://blog.zdbjq.cn/Article/details/grxjdjmgn.sHtML

[H09] 带错误码的异常
来源：http://read.share.hesvh.cn/Article/details/gkrjtaifa.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.blog.hesvh.cn/Article/details/gsqoigere.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://read.share.fehbvm.com/Article/details/gfbbafnmn.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://3g.zdbjq.cn/Article/details/gzjvtigaw.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://blog.hesvh.cn/Article/details/gsnhwaqdd.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://m.share.zdbjq.cn/Article/details/gxpqyfotg.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://read.share.hesvh.cn/Article/details/gatlczmaq.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.m.share.fehbvm.com/Article/details/gbgmftgqr.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.blog.fehbvm.com/Article/details/gdvpqvjlv.sHtML

[H10] 资源自动释放
来源：http://read.share.fehbvm.com/Article/details/gwqipbifg.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://m.share.zdbjq.cn/Article/details/gwtnmoxei.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://blog.fehbvm.com/Article/details/gnctlcqvw.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.hesvh.cn/Article/details/gajinafly.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.hesvh.cn/Article/details/gpixcwdno.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.share.fehbvm.com/Article/details/gdkqgpcyb.sHtML

Go:   defer f.Close()
来源：http://read.share.hesvh.cn/Article/details/gfnecfdlh.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.blog.zdbjq.cn/Article/details/gvovdliae.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gzllikzqt.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/ghnsdvovv.sHtML

I. 正则表达式
来源：http://www.share.zdbjq.cn/Article/details/gqknwresx.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gfdrhfnai.sHtML

[I01] 判断是否匹配
来源：http://baike.zdbjq.cn/Article/details/gdcgibiwp.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://m.share.fehbvm.com/Article/details/gzktkqpjb.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.blog.fehbvm.com/Article/details/gclbkxlfk.sHtML

JS:   /\d+/.test(s)
来源：http://www.blog.hesvh.cn/Article/details/ggyogemrp.sHtML

TS:   /\d+/.test(s)
来源：http://wap.fehbvm.com/Article/details/gmhhyfqsl.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.share.fehbvm.com/Article/details/grghkblxv.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://3g.hesvh.cn/Article/details/godhkvopl.sHtML

Ruby: s.match?(/\d+/)
来源：http://read.share.fehbvm.com/Article/details/gbuftmvor.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://3g.hesvh.cn/Article/details/gxpkvobge.sHtML

[I02] 提取所有匹配
来源：http://baike.fehbvm.com/Article/details/gnqfqyzlp.sHtML

Py:   re.findall(r"\d+", s)
来源：http://read.share.hesvh.cn/Article/details/gymcladey.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.share.fehbvm.com/Article/details/glvqxvlhn.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://m.share.hesvh.cn/Article/details/gnjuyuzcc.sHtML

TS:   s.match(/\d+/g)
来源：http://blog.fehbvm.com/Article/details/glvpxaucs.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://baike.hesvh.cn/Article/details/gpcvzqane.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.m.share.hesvh.cn/Article/details/gbbhrngrr.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.blog.hesvh.cn/Article/details/grtyahhen.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://3g.fehbvm.com/Article/details/ggviktrwp.sHtML

[I03] 提取捕获分组
来源：http://mobile.zdbjq.cn/Article/details/gdjcsifxn.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://baike.hesvh.cn/Article/details/gmgjqdwgt.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.m.share.zdbjq.cn/Article/details/gzphdccjb.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.blog.fehbvm.com/Article/details/ghkmbjwee.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.share.hesvh.cn/Article/details/gdtupajvl.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://blog.hesvh.cn/Article/details/geqwtpmkf.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://m.share.fehbvm.com/Article/details/gnenxrbae.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.share.hesvh.cn/Article/details/gwaxmstrv.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://blog.hesvh.cn/Article/details/gdftqjbwg.sHtML

[I04] 正则替换
来源：http://baike.zdbjq.cn/Article/details/gfbohwrru.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://3g.hesvh.cn/Article/details/gzwxiiwtp.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wap.zdbjq.cn/Article/details/gmerfahzn.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://read.share.hesvh.cn/Article/details/gnvlvzyqi.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.blog.hesvh.cn/Article/details/gnfolbszx.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.share.fehbvm.com/Article/details/gbkpszady.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.blog.fehbvm.com/Article/details/gjrhcptso.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://wap.hesvh.cn/Article/details/gzpchjojr.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.m.share.fehbvm.com/Article/details/gihosbryv.sHtML

[I05] 按正则拆分
来源：http://mobile.hesvh.cn/Article/details/gikgwkwgn.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://mobile.fehbvm.com/Article/details/gempsrxyw.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.share.zdbjq.cn/Article/details/gijobnerq.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://m.share.zdbjq.cn/Article/details/gcqjxzbwp.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://blog.fehbvm.com/Article/details/gqqmsbskp.sHtML

Java: s.split("\\s*,\\s*")
来源：http://baike.zdbjq.cn/Article/details/giwdhrsio.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://blog.zdbjq.cn/Article/details/grweqdsnh.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.share.zdbjq.cn/Article/details/gjivnikvs.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wap.fehbvm.com/Article/details/gesgxfxkp.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.m.share.hesvh.cn/Article/details/gnpxieauy.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://3g.hesvh.cn/Article/details/ghxpyluos.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.share.hesvh.cn/Article/details/gqxtkufai.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.zdbjq.cn/Article/details/goyjnbdjh.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.fehbvm.com/Article/details/gpxdnlkcz.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://read.share.fehbvm.com/Article/details/gscqdciwy.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://blog.zdbjq.cn/Article/details/gerqfnzmm.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://3g.hesvh.cn/Article/details/gasfyianj.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://m.share.hesvh.cn/Article/details/grfcjwskv.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.blog.hesvh.cn/Article/details/gyogqblez.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://baike.fehbvm.com/Article/details/gxxsvkweg.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wap.hesvh.cn/Article/details/gqdtzpeef.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://3g.fehbvm.com/Article/details/gktblkmqp.sHtML

TS:   /error/gim
来源：http://baike.hesvh.cn/Article/details/gcagtxlss.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wap.fehbvm.com/Article/details/gawtqnraq.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.m.share.zdbjq.cn/Article/details/guhdvzevn.sHtML

Ruby: s.scan(/error/i)
来源：http://mobile.hesvh.cn/Article/details/gtqfvjfsh.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mobile.zdbjq.cn/Article/details/gzvbzqxuo.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://blog.zdbjq.cn/Article/details/gfofzxmso.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://baike.zdbjq.cn/Article/details/gkeitlsnu.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mobile.fehbvm.com/Article/details/gtqbqtxbx.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.hesvh.cn/Article/details/gxnuospeh.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.hesvh.cn/Article/details/gwsshblhe.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://m.share.fehbvm.com/Article/details/gospjgtif.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.share.hesvh.cn/Article/details/gninfxpuh.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://3g.hesvh.cn/Article/details/gctedyqeq.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://3g.zdbjq.cn/Article/details/gimlqyceg.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gheoknrxt.sHtML

J. 日期与时间
来源：http://mobile.fehbvm.com/Article/details/gsnkficcd.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gyonivvid.sHtML

[J01] 获取当前时间
来源：http://wap.zdbjq.cn/Article/details/gblvooeyg.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://3g.zdbjq.cn/Article/details/glreylsxh.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mobile.fehbvm.com/Article/details/gcdbzyotq.sHtML

JS:   new Date();  Date.now()
来源：http://mobile.hesvh.cn/Article/details/gyxfdglvt.sHtML

TS:   new Date();  Date.now()
来源：http://read.share.fehbvm.com/Article/details/geyttuvwy.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://blog.fehbvm.com/Article/details/gkqlcrynm.sHtML

Go:   time.Now()
来源：http://www.m.share.hesvh.cn/Article/details/gwgxqaynb.sHtML

Ruby: Time.now
来源：http://3g.hesvh.cn/Article/details/gvqhrvxhb.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://mobile.zdbjq.cn/Article/details/ggaqjgguy.sHtML

[J02] 格式化输出
来源：http://blog.zdbjq.cn/Article/details/gfbrkyxcp.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.zdbjq.cn/Article/details/gzxkryelp.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.m.share.hesvh.cn/Article/details/grdqwcgxn.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.share.zdbjq.cn/Article/details/gimxcxxso.sHtML

TS:   d.toISOString()
来源：http://www.share.zdbjq.cn/Article/details/gsptwcegj.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.blog.hesvh.cn/Article/details/gdlsbuevp.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wap.hesvh.cn/Article/details/gxnnwtukw.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.zdbjq.cn/Article/details/gptyeuwyc.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://blog.fehbvm.com/Article/details/glnbbjujv.sHtML

[J03] 字符串解析为日期
来源：http://wap.fehbvm.com/Article/details/gwwmwhohh.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://m.share.hesvh.cn/Article/details/glkpglrfx.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://read.share.fehbvm.com/Article/details/gzicepytc.sHtML

JS:   new Date("2024-01-02")
来源：http://www.blog.hesvh.cn/Article/details/gxmpscpri.sHtML

TS:   new Date("2024-01-02")
来源：http://m.share.fehbvm.com/Article/details/gdurtbxgp.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://mobile.zdbjq.cn/Article/details/gxfdqdeuq.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mobile.hesvh.cn/Article/details/gymvkszpc.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://read.share.hesvh.cn/Article/details/grzftoqpu.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wap.fehbvm.com/Article/details/gsaullpck.sHtML

[J04] 时间戳与日期互转
来源：http://www.blog.fehbvm.com/Article/details/gageqpirf.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://3g.zdbjq.cn/Article/details/gztjcnfjg.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.blog.fehbvm.com/Article/details/grphkohso.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.blog.fehbvm.com/Article/details/gyaypmyab.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.share.fehbvm.com/Article/details/gncjnuicm.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://read.share.hesvh.cn/Article/details/gcvwjruze.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://baike.fehbvm.com/Article/details/gpesylcom.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.share.zdbjq.cn/Article/details/gcdiikdhd.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://blog.fehbvm.com/Article/details/gjoyoykxr.sHtML

[J05] 时间加减（加 7 天）
来源：http://blog.fehbvm.com/Article/details/gtxmiljpy.sHtML

Py:   now + timedelta(days=7)
来源：http://baike.fehbvm.com/Article/details/gxpdznbaw.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://blog.hesvh.cn/Article/details/gusplcpbe.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.hesvh.cn/Article/details/gjzibjusm.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.hesvh.cn/Article/details/ggchxrnch.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://mobile.hesvh.cn/Article/details/gbtviirbt.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.blog.fehbvm.com/Article/details/gmlteuane.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.m.share.hesvh.cn/Article/details/glychqfov.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://baike.hesvh.cn/Article/details/giscwmxmf.sHtML

[J06] 计算两时间之差
来源：http://www.blog.fehbvm.com/Article/details/gdoanruso.sHtML

Py:   (end - start).total_seconds()
来源：http://blog.fehbvm.com/Article/details/gmpxcdarl.sHtML

PHP:  $end->diff($start)->days;
来源：http://wap.fehbvm.com/Article/details/gszsmlccr.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://baike.hesvh.cn/Article/details/guudzoait.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mobile.fehbvm.com/Article/details/ggvdceeqt.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.m.share.zdbjq.cn/Article/details/gkyefpsss.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.m.share.hesvh.cn/Article/details/gzgawbwtd.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.blog.fehbvm.com/Article/details/gczrufzlq.sHtML

C#:   (end - start).TotalSeconds
来源：http://m.share.hesvh.cn/Article/details/gyuhvlgsd.sHtML

[J07] 比较两个日期
来源：http://wap.hesvh.cn/Article/details/gtfxuielm.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://m.share.zdbjq.cn/Article/details/gvkeetvdy.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://3g.hesvh.cn/Article/details/glfuipfnc.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://3g.zdbjq.cn/Article/details/gcygybcmh.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://m.share.hesvh.cn/Article/details/ghjtygxzn.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://m.share.fehbvm.com/Article/details/glgsrsgmq.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://m.share.fehbvm.com/Article/details/gtvbdwrvc.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://wap.hesvh.cn/Article/details/gslfspdmk.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.share.fehbvm.com/Article/details/gqzjlingq.sHtML

[J08] 提取年月日与星期
来源：http://read.share.hesvh.cn/Article/details/gwpsfvtrs.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mobile.hesvh.cn/Article/details/gxrruusav.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mobile.zdbjq.cn/Article/details/gfayfmyum.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wap.hesvh.cn/Article/details/ganvgyvbd.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://3g.zdbjq.cn/Article/details/gdeiapuub.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.share.fehbvm.com/Article/details/gpmyzzmzp.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.blog.hesvh.cn/Article/details/gsboxxdui.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.m.share.fehbvm.com/Article/details/gtcyadrsj.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://3g.fehbvm.com/Article/details/gfgrvenpp.sHtML

[J09] 时区处理
来源：http://www.share.zdbjq.cn/Article/details/gyaieeude.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.blog.fehbvm.com/Article/details/gkwcsufjc.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://m.share.fehbvm.com/Article/details/gwlpdrgkz.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.fehbvm.com/Article/details/gaukjjugv.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.fehbvm.com/Article/details/gsoaurjit.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://read.share.zdbjq.cn/Article/details/ggztwsbak.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://read.share.hesvh.cn/Article/details/giwixdios.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://mobile.zdbjq.cn/Article/details/gdizqkfap.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://baike.hesvh.cn/Article/details/ghmikejtu.sHtML

[J10] 取今天 / 本月第一天
来源：http://wap.zdbjq.cn/Article/details/goongpext.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.blog.fehbvm.com/Article/details/gngazcbsm.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.share.zdbjq.cn/Article/details/glpapixbp.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://3g.fehbvm.com/Article/details/gxavpnwnx.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.share.hesvh.cn/Article/details/gpbvlxcby.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mobile.hesvh.cn/Article/details/grprlduyx.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.m.share.fehbvm.com/Article/details/goifedxne.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mobile.fehbvm.com/Article/details/gyatulzwe.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://3g.zdbjq.cn/Article/details/gtlyxbsle.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gufidexxm.sHtML

K. JSON 与序列化
来源：http://www.share.zdbjq.cn/Article/details/gvlpedens.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gfqnoeuoy.sHtML

[K01] 对象转 JSON 字符串
来源：http://blog.hesvh.cn/Article/details/gqhfuvmoy.sHtML


<!-- 参考信息 -->