代发 wailian999

TS:   public / protected / private
来源：http://www.share.fehbvm.com/Article/details/gtlgflvgj.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.hesvh.cn/Article/details/gjmraryuo.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.fehbvm.com/Article/details/gmqzxaeii.sHtML

Ruby: public / protected / private
来源：http://m.share.hesvh.cn/Article/details/gbrcfhlau.sHtML

C#:   public / protected / private / internal
来源：http://www.share.hesvh.cn/Article/details/gmjcccncr.sHtML

[G11] getter / setter
来源：http://blog.zdbjq.cn/Article/details/gpxooarub.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.zdbjq.cn/Article/details/glysvnvtl.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.hesvh.cn/Article/details/gngkbkwvd.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.zdbjq.cn/Article/details/gxuvzgqqe.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.zdbjq.cn/Article/details/giabxeptl.sHtML

Java: public String getName() { return name; }
来源：http://read.share.fehbvm.com/Article/details/gfugvvnvn.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.zdbjq.cn/Article/details/glzhnfavp.sHtML

Ruby: attr_accessor :name
来源：http://wap.fehbvm.com/Article/details/gqicdiypr.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.hesvh.cn/Article/details/guffntprx.sHtML

[G12] 对象转字符串
来源：http://read.share.zdbjq.cn/Article/details/gvlgipjer.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.hesvh.cn/Article/details/gbfybmiqo.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gidnpbidx.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/gylugzjch.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/geclfkpco.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.zdbjq.cn/Article/details/gxnqbklwb.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.hesvh.cn/Article/details/gjfonmxxq.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.hesvh.cn/Article/details/ggwfttojf.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.zdbjq.cn/Article/details/gtgqirini.sHtML

[G13] 判断对象类型
来源：http://m.share.hesvh.cn/Article/details/gugxgnnxo.sHtML

Py:   isinstance(u, User)
来源：http://mobile.hesvh.cn/Article/details/glsyyihbh.sHtML

PHP:  $u instanceof User
来源：http://blog.fehbvm.com/Article/details/gwsmkaycs.sHtML

JS:   u instanceof User
来源：http://www.share.fehbvm.com/Article/details/gcuqzoqjw.sHtML

TS:   u instanceof User
来源：http://www.m.share.fehbvm.com/Article/details/gvisesdsk.sHtML

Java: u instanceof User
来源：http://www.share.zdbjq.cn/Article/details/gpoghffqd.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.zdbjq.cn/Article/details/gxoncfsii.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.hesvh.cn/Article/details/ghcwoffpd.sHtML

C#:   u is User
来源：http://read.share.fehbvm.com/Article/details/gwmqfaqsr.sHtML

[G14] 数据类 / record
来源：http://mobile.fehbvm.com/Article/details/ghjzplpzg.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://3g.hesvh.cn/Article/details/gvnrkwhxx.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.fehbvm.com/Article/details/grsefnuen.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.fehbvm.com/Article/details/gkdxglpxw.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.fehbvm.com/Article/details/gtqsmtpnm.sHtML

Java: record User(String name, int age) {}
来源：http://blog.zdbjq.cn/Article/details/geyrnlgso.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.fehbvm.com/Article/details/gsxgomjaa.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.hesvh.cn/Article/details/griemtcpv.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.hesvh.cn/Article/details/gkjbkqare.sHtML

[G15] 枚举
来源：http://baike.fehbvm.com/Article/details/gabocedmf.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.hesvh.cn/Article/details/gwiykrvnk.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.fehbvm.com/Article/details/gddzwqygi.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mobile.hesvh.cn/Article/details/gbuyrzhwv.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.zdbjq.cn/Article/details/gwrujwwvv.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.zdbjq.cn/Article/details/gaxwcxxrr.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.zdbjq.cn/Article/details/gqufqifee.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.zdbjq.cn/Article/details/ghzwbyawv.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.zdbjq.cn/Article/details/gwwujpnxe.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.zdbjq.cn/Article/details/gbyqxjljl.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.zdbjq.cn/Article/details/gevkkoira.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.hesvh.cn/Article/details/gpaythefn.sHtML

JS:   Object.entries(obj)
来源：http://baike.zdbjq.cn/Article/details/gdfdnrjkk.sHtML

TS:   Object.entries(obj)
来源：http://www.share.fehbvm.com/Article/details/gbwtifpll.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.hesvh.cn/Article/details/gisagsklv.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.zdbjq.cn/Article/details/gaktrqtpp.sHtML

Ruby: obj.instance_variables
来源：http://www.share.hesvh.cn/Article/details/ghysczkcd.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.blog.zdbjq.cn/Article/details/gnysqfblc.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gweywzlit.sHtML

H. 异常与错误处理
来源：http://3g.fehbvm.com/Article/details/gbzzlrvsh.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gjpnmuuhy.sHtML

[H01] try / catch 基础
来源：http://read.share.zdbjq.cn/Article/details/grpdrfewi.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.zdbjq.cn/Article/details/glqqxxkuu.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mobile.hesvh.cn/Article/details/gykcesbbv.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.hesvh.cn/Article/details/gbmxstock.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.fehbvm.com/Article/details/ghavsjtjt.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://baike.hesvh.cn/Article/details/gohxifaag.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://baike.hesvh.cn/Article/details/gjqtaoaio.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.fehbvm.com/Article/details/gxktqjmjr.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://baike.hesvh.cn/Article/details/gtcaxieqr.sHtML

[H02] finally / ensure 收尾
来源：http://blog.hesvh.cn/Article/details/gkoyzaxte.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://baike.zdbjq.cn/Article/details/gbxqrpdsq.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://3g.zdbjq.cn/Article/details/gzcgfurbp.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://3g.zdbjq.cn/Article/details/gkriuolrm.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.hesvh.cn/Article/details/glhacruzn.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.blog.zdbjq.cn/Article/details/gvdwxjhge.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://3g.hesvh.cn/Article/details/gpguapgxr.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.zdbjq.cn/Article/details/gkfyvbwyl.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.share.fehbvm.com/Article/details/gyhegqvcn.sHtML

[H03] 主动抛出异常
来源：http://www.share.hesvh.cn/Article/details/gwxfyhbze.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.m.share.zdbjq.cn/Article/details/gxieazivf.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.hesvh.cn/Article/details/gwtlqdokf.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.zdbjq.cn/Article/details/gafzjtnwb.sHtML

TS:   throw new Error("错误信息");
来源：http://www.blog.fehbvm.com/Article/details/gfycrydxx.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://read.share.fehbvm.com/Article/details/grurywufm.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.hesvh.cn/Article/details/gvukhbmst.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://3g.zdbjq.cn/Article/details/gfvakepgz.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.zdbjq.cn/Article/details/gavonbidv.sHtML

[H04] 自定义异常类型
来源：http://mobile.hesvh.cn/Article/details/gyeykinhv.sHtML

Py:   class MyError(Exception): pass
来源：http://www.m.share.fehbvm.com/Article/details/guqyppdep.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://3g.fehbvm.com/Article/details/gexvgqbug.sHtML

JS:   class MyError extends Error {}
来源：http://blog.zdbjq.cn/Article/details/ghqkimgwc.sHtML

TS:   class MyError extends Error {}
来源：http://wap.fehbvm.com/Article/details/grcokpoux.sHtML

Java: class MyException extends RuntimeException {}
来源：http://wap.zdbjq.cn/Article/details/gabguuzfy.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://baike.hesvh.cn/Article/details/gvxyqhugy.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.hesvh.cn/Article/details/gcaxcbbxt.sHtML

C#:   class MyException : Exception {}
来源：http://m.share.fehbvm.com/Article/details/glfefjjuz.sHtML

[H05] 捕获特定类型
来源：http://m.share.zdbjq.cn/Article/details/gjzxhgwxm.sHtML

Py:   except ValueError as e:
来源：http://mobile.hesvh.cn/Article/details/gmjtzgdte.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://read.share.hesvh.cn/Article/details/gjdemmagt.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://m.share.hesvh.cn/Article/details/gbzmwcval.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.share.fehbvm.com/Article/details/gwnnhtzbn.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.blog.zdbjq.cn/Article/details/gyajneyad.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.share.hesvh.cn/Article/details/gdexftbdj.sHtML

Ruby: rescue ArgumentError => e
来源：http://wap.fehbvm.com/Article/details/gqhvtbpvq.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.blog.hesvh.cn/Article/details/gsvbafvaw.sHtML

[H06] 可选值 / 空值安全访问
来源：http://3g.fehbvm.com/Article/details/gxrmxfvka.sHtML

Py:   value = d.get("k") or default
来源：http://www.m.share.hesvh.cn/Article/details/gfekhrnwn.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.share.hesvh.cn/Article/details/gnhafedyf.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.hesvh.cn/Article/details/gfwnekgnm.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.share.zdbjq.cn/Article/details/grwuvlcrj.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.share.zdbjq.cn/Article/details/golrmzsox.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.blog.fehbvm.com/Article/details/gqipdnraz.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.m.share.fehbvm.com/Article/details/gqwexnlrs.sHtML

C#:   obj?.A?.B ?? default
来源：http://blog.hesvh.cn/Article/details/gkgarpztr.sHtML

[H07] 断言
来源：http://www.share.hesvh.cn/Article/details/govuuxyhn.sHtML

Py:   assert x > 0, "必须为正"
来源：http://wap.hesvh.cn/Article/details/guztoansf.sHtML

PHP:  assert($x > 0);
来源：http://baike.hesvh.cn/Article/details/gzmjomncj.sHtML

JS:   console.assert(x > 0);
来源：http://blog.zdbjq.cn/Article/details/gzbexufjf.sHtML

TS:   console.assert(x > 0);
来源：http://blog.hesvh.cn/Article/details/gxaqngtfj.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.share.zdbjq.cn/Article/details/gavhpsuih.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://baike.hesvh.cn/Article/details/gtgbxczmx.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://wap.fehbvm.com/Article/details/gicdryqqp.sHtML

C#:   Debug.Assert(x > 0);
来源：http://read.share.zdbjq.cn/Article/details/ganmdugrh.sHtML

[H08] 获取错误信息与堆栈
来源：http://mobile.zdbjq.cn/Article/details/gbgnjqksc.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://m.share.fehbvm.com/Article/details/gldswlksa.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://read.share.zdbjq.cn/Article/details/gdxewltxd.sHtML

JS:   e.message;  e.stack
来源：http://wap.hesvh.cn/Article/details/gyxrsiynb.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.share.zdbjq.cn/Article/details/grjlubgxe.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.blog.hesvh.cn/Article/details/ghioonzsn.sHtML

Go:   err.Error()
来源：http://baike.hesvh.cn/Article/details/gogcwkmuq.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.blog.fehbvm.com/Article/details/grnmwxczi.sHtML

C#:   e.Message;  e.StackTrace
来源：http://3g.zdbjq.cn/Article/details/gzmpzmaan.sHtML

[H09] 带错误码的异常
来源：http://read.share.fehbvm.com/Article/details/gbkpipbuq.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.share.fehbvm.com/Article/details/gqluxjvju.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.blog.zdbjq.cn/Article/details/grhlljyis.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wap.fehbvm.com/Article/details/goaymfwxz.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.m.share.zdbjq.cn/Article/details/gintoochp.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.blog.hesvh.cn/Article/details/gcqtguqkc.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mobile.hesvh.cn/Article/details/gbbaefyfi.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://mobile.hesvh.cn/Article/details/giacghufd.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://read.share.hesvh.cn/Article/details/gafrifuun.sHtML

[H10] 资源自动释放
来源：http://blog.fehbvm.com/Article/details/ghpxyfsql.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://wap.fehbvm.com/Article/details/gfhshnaux.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://baike.hesvh.cn/Article/details/gzzpaufnl.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.fehbvm.com/Article/details/grvgxmvfb.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.fehbvm.com/Article/details/gqlqoedek.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wap.zdbjq.cn/Article/details/gfmhyqkpc.sHtML

Go:   defer f.Close()
来源：http://mobile.zdbjq.cn/Article/details/gwmitjcuv.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://read.share.hesvh.cn/Article/details/gzvgughoc.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gjgfqiova.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gkxszerpg.sHtML

I. 正则表达式
来源：http://www.share.zdbjq.cn/Article/details/gdvnrdpfe.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gdptohtgy.sHtML

[I01] 判断是否匹配
来源：http://wap.hesvh.cn/Article/details/gqxjygdpc.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://m.share.fehbvm.com/Article/details/gngykyfmh.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://mobile.fehbvm.com/Article/details/gjlrasnlw.sHtML

JS:   /\d+/.test(s)
来源：http://m.share.hesvh.cn/Article/details/gjyozcldg.sHtML

TS:   /\d+/.test(s)
来源：http://www.blog.fehbvm.com/Article/details/glnlabhwh.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://3g.fehbvm.com/Article/details/gaxtoydih.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://baike.fehbvm.com/Article/details/gxzkvfvjo.sHtML

Ruby: s.match?(/\d+/)
来源：http://wap.hesvh.cn/Article/details/geritielz.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://read.share.hesvh.cn/Article/details/ggbjfrvtm.sHtML

[I02] 提取所有匹配
来源：http://3g.fehbvm.com/Article/details/gsysanraq.sHtML

Py:   re.findall(r"\d+", s)
来源：http://baike.hesvh.cn/Article/details/gxufxvkte.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.share.fehbvm.com/Article/details/gtaqexzam.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://3g.zdbjq.cn/Article/details/gcbegelnh.sHtML

TS:   s.match(/\d+/g)
来源：http://blog.zdbjq.cn/Article/details/geoeusbaf.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.m.share.hesvh.cn/Article/details/giewbeyme.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://read.share.zdbjq.cn/Article/details/gsqtklhwm.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.share.zdbjq.cn/Article/details/gxoufgxok.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.share.fehbvm.com/Article/details/gscbkfvos.sHtML

[I03] 提取捕获分组
来源：http://wap.zdbjq.cn/Article/details/gqfwcsoby.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://m.share.hesvh.cn/Article/details/gwisunetw.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://blog.hesvh.cn/Article/details/gzlchrlro.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.m.share.zdbjq.cn/Article/details/gaykutjqi.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://m.share.zdbjq.cn/Article/details/grzmesqlf.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://3g.zdbjq.cn/Article/details/ggizspqez.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.blog.hesvh.cn/Article/details/gcfzugvqw.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wap.hesvh.cn/Article/details/gbqwyfwfi.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.blog.hesvh.cn/Article/details/glmffhoxa.sHtML

[I04] 正则替换
来源：http://blog.fehbvm.com/Article/details/gwsqgqhxq.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://3g.fehbvm.com/Article/details/grvnchlkb.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.hesvh.cn/Article/details/gjqenahjs.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.share.hesvh.cn/Article/details/gweaxovjs.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.share.hesvh.cn/Article/details/gqubtdhgk.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://m.share.fehbvm.com/Article/details/gtqjrzpda.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://mobile.zdbjq.cn/Article/details/gzjtbtfoo.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://m.share.hesvh.cn/Article/details/ggqsmwoft.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mobile.fehbvm.com/Article/details/gevmcsucr.sHtML

[I05] 按正则拆分
来源：http://3g.fehbvm.com/Article/details/gjdmuguwy.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://baike.hesvh.cn/Article/details/grcvxqpzz.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://read.share.hesvh.cn/Article/details/gabbwqmit.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.blog.zdbjq.cn/Article/details/gwdfleoxl.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.m.share.fehbvm.com/Article/details/gcpvjuyab.sHtML

Java: s.split("\\s*,\\s*")
来源：http://mobile.fehbvm.com/Article/details/geitwyvyd.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.m.share.zdbjq.cn/Article/details/gyzaqseaj.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://3g.zdbjq.cn/Article/details/ghlujzsky.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://m.share.fehbvm.com/Article/details/gjloflrnv.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.m.share.fehbvm.com/Article/details/gdqgakarv.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://read.share.fehbvm.com/Article/details/gpjgqkshe.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://baike.hesvh.cn/Article/details/gxuzbopsf.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.fehbvm.com/Article/details/ggldywvvp.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.fehbvm.com/Article/details/glmvvhvoc.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.blog.hesvh.cn/Article/details/gjzucutsy.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://3g.zdbjq.cn/Article/details/gesupcosm.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.m.share.zdbjq.cn/Article/details/gbiuhesns.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://read.share.hesvh.cn/Article/details/gkddrbfqj.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.m.share.zdbjq.cn/Article/details/gdjurvetr.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wap.fehbvm.com/Article/details/gbcachpvx.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://read.share.zdbjq.cn/Article/details/gbjeydmzd.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.m.share.fehbvm.com/Article/details/gfnrwwmeg.sHtML

TS:   /error/gim
来源：http://www.m.share.hesvh.cn/Article/details/gvnwhmlcb.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://read.share.zdbjq.cn/Article/details/gsovcxmis.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://baike.hesvh.cn/Article/details/gorhlhgez.sHtML

Ruby: s.scan(/error/i)
来源：http://wap.fehbvm.com/Article/details/gvtcvouwf.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.share.fehbvm.com/Article/details/gklnessov.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://3g.hesvh.cn/Article/details/gckiwiqch.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.blog.hesvh.cn/Article/details/gbnrwmxog.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://3g.hesvh.cn/Article/details/gqpzsiktw.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.zdbjq.cn/Article/details/gwipsuuum.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.zdbjq.cn/Article/details/gsymhfyci.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://blog.hesvh.cn/Article/details/gykzfqomv.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.share.hesvh.cn/Article/details/ggtiafgdk.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.share.fehbvm.com/Article/details/gbydldryx.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.blog.zdbjq.cn/Article/details/gkyusuchv.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gtpxxcjoh.sHtML

J. 日期与时间
来源：http://baike.hesvh.cn/Article/details/gfddwrfhn.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gbuaioquj.sHtML

[J01] 获取当前时间
来源：http://www.blog.zdbjq.cn/Article/details/gjfwthgje.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://baike.hesvh.cn/Article/details/gtdgoqeaw.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://blog.fehbvm.com/Article/details/glkmxqugl.sHtML

JS:   new Date();  Date.now()
来源：http://www.m.share.hesvh.cn/Article/details/gjcopumwn.sHtML

TS:   new Date();  Date.now()
来源：http://baike.hesvh.cn/Article/details/gpmdcvtxg.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://3g.zdbjq.cn/Article/details/glvipnukz.sHtML

Go:   time.Now()
来源：http://www.m.share.zdbjq.cn/Article/details/gmfbaoxna.sHtML

Ruby: Time.now
来源：http://www.blog.fehbvm.com/Article/details/gbqillmrf.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wap.hesvh.cn/Article/details/gtpasefpm.sHtML

[J02] 格式化输出
来源：http://baike.fehbvm.com/Article/details/gjubtyllp.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.fehbvm.com/Article/details/gtpnlgodm.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.m.share.hesvh.cn/Article/details/gkjomqcax.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wap.zdbjq.cn/Article/details/gpqhasaue.sHtML

TS:   d.toISOString()
来源：http://baike.zdbjq.cn/Article/details/gmphdkrzx.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://wap.zdbjq.cn/Article/details/gmygmwsuz.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.share.fehbvm.com/Article/details/gqttzdoux.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.zdbjq.cn/Article/details/gnszdtudc.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.blog.hesvh.cn/Article/details/gzygvmzlg.sHtML

[J03] 字符串解析为日期
来源：http://blog.zdbjq.cn/Article/details/goppgbsnf.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.share.zdbjq.cn/Article/details/gfkhbfsra.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.m.share.zdbjq.cn/Article/details/gzgamqkpn.sHtML

JS:   new Date("2024-01-02")
来源：http://blog.hesvh.cn/Article/details/ggntxormh.sHtML

TS:   new Date("2024-01-02")
来源：http://3g.hesvh.cn/Article/details/gfzmfgamd.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.m.share.zdbjq.cn/Article/details/gzbtezurn.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.m.share.hesvh.cn/Article/details/glhwuvxjx.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.blog.zdbjq.cn/Article/details/gkjooqtdt.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.blog.fehbvm.com/Article/details/gxlvtmsfv.sHtML

[J04] 时间戳与日期互转
来源：http://www.share.hesvh.cn/Article/details/gbajhqnvy.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wap.zdbjq.cn/Article/details/gpjfhjhou.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wap.fehbvm.com/Article/details/gaqvmlzlw.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.share.hesvh.cn/Article/details/gwhhkwats.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://blog.fehbvm.com/Article/details/ghdoifkny.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.share.fehbvm.com/Article/details/ggumwcwsj.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://blog.zdbjq.cn/Article/details/graecmedg.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wap.fehbvm.com/Article/details/gjuuffazl.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://read.share.hesvh.cn/Article/details/gujdvljvg.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.blog.fehbvm.com/Article/details/gbluliwyx.sHtML

Py:   now + timedelta(days=7)
来源：http://3g.hesvh.cn/Article/details/guepgnugo.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.blog.zdbjq.cn/Article/details/gkncffdgc.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.fehbvm.com/Article/details/gqdbmwgav.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.fehbvm.com/Article/details/gpqyhvqqn.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.share.zdbjq.cn/Article/details/gmbzljxak.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mobile.fehbvm.com/Article/details/gttavglwq.sHtML

Ruby: Time.now + 7 * 86400
来源：http://blog.hesvh.cn/Article/details/gezptoukc.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.m.share.zdbjq.cn/Article/details/gwysnixcl.sHtML

[J06] 计算两时间之差
来源：http://wap.hesvh.cn/Article/details/gckldzcwp.sHtML

Py:   (end - start).total_seconds()
来源：http://mobile.fehbvm.com/Article/details/glkovopyc.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.m.share.zdbjq.cn/Article/details/gmwkhpstb.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wap.hesvh.cn/Article/details/grhoprokr.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://baike.fehbvm.com/Article/details/gklwvpvda.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.blog.hesvh.cn/Article/details/gnofipedh.sHtML

Go:   end.Sub(start).Hours()
来源：http://baike.hesvh.cn/Article/details/gzjiuyeks.sHtML

Ruby: end - start                 # 返回秒数
来源：http://m.share.hesvh.cn/Article/details/gwnbdcfbb.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.blog.zdbjq.cn/Article/details/gxpaogzpz.sHtML

[J07] 比较两个日期
来源：http://m.share.zdbjq.cn/Article/details/gutjqjzys.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://wap.hesvh.cn/Article/details/gejjwplvd.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://wap.zdbjq.cn/Article/details/gbrnbzjbd.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://wap.fehbvm.com/Article/details/gehnpsgvd.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://baike.hesvh.cn/Article/details/gkvhywrlk.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.share.hesvh.cn/Article/details/geolgdqjq.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.blog.zdbjq.cn/Article/details/gapebceyv.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://blog.fehbvm.com/Article/details/gajmezfqc.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.m.share.hesvh.cn/Article/details/gwckwvcjk.sHtML

[J08] 提取年月日与星期
来源：http://baike.zdbjq.cn/Article/details/gfdokjxyq.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://blog.fehbvm.com/Article/details/gdrswhrve.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wap.hesvh.cn/Article/details/gkeervqhj.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.m.share.zdbjq.cn/Article/details/gvdfypgdu.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://blog.hesvh.cn/Article/details/geukhsuol.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://3g.zdbjq.cn/Article/details/gunddozro.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://blog.zdbjq.cn/Article/details/gpbjqvyak.sHtML


<!-- 参考信息 -->