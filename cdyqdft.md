代发 wailian999

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.fehbvm.com/Article/details/ggnqdilgq.sHtML

Ruby: def self.f; end
来源：http://mobile.zdbjq.cn/Article/details/gcmhxjyfe.sHtML

C#:   public static void F() {}
来源：http://3g.hesvh.cn/Article/details/guylymzps.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.fehbvm.com/Article/details/gtaxouarb.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.fehbvm.com/Article/details/gyapgczty.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.fehbvm.com/Article/details/gefaxgkzr.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.zdbjq.cn/Article/details/gmzjdxppt.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.hesvh.cn/Article/details/gcdrbwjcg.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.hesvh.cn/Article/details/gqbiaowle.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.zdbjq.cn/Article/details/gexjqzqyo.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.fehbvm.com/Article/details/gstahccng.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.fehbvm.com/Article/details/gnlzputgi.sHtML

[G10] 访问控制
来源：http://www.share.fehbvm.com/Article/details/gpnmnsqxx.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.zdbjq.cn/Article/details/gagtypony.sHtML

PHP:  public / protected / private
来源：http://read.share.fehbvm.com/Article/details/gwjyfvkgv.sHtML

JS:   #private 字段；其余公开
来源：http://baike.hesvh.cn/Article/details/glbybzacj.sHtML

TS:   public / protected / private
来源：http://mobile.zdbjq.cn/Article/details/gmwpydvts.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.hesvh.cn/Article/details/gfydknzwp.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.zdbjq.cn/Article/details/gfzhmrdkk.sHtML

Ruby: public / protected / private
来源：http://mobile.hesvh.cn/Article/details/geazzhpao.sHtML

C#:   public / protected / private / internal
来源：http://read.share.zdbjq.cn/Article/details/gclgvojlu.sHtML

[G11] getter / setter
来源：http://3g.zdbjq.cn/Article/details/gaqfzjqsm.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.hesvh.cn/Article/details/gxtaixzpo.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.zdbjq.cn/Article/details/gihhyardl.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.fehbvm.com/Article/details/gfyamgtwl.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.hesvh.cn/Article/details/gqynaodwo.sHtML

Java: public String getName() { return name; }
来源：http://baike.fehbvm.com/Article/details/gttwbdebp.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.fehbvm.com/Article/details/grqduvipr.sHtML

Ruby: attr_accessor :name
来源：http://wap.fehbvm.com/Article/details/gxkkdcsbp.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.hesvh.cn/Article/details/gqsrjimwz.sHtML

[G12] 对象转字符串
来源：http://3g.fehbvm.com/Article/details/gnhqhdmse.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.fehbvm.com/Article/details/getamxphc.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.hesvh.cn/Article/details/gkykcqkuh.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/gcusuaaqq.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/gpxtmcbaa.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.zdbjq.cn/Article/details/gecotsntf.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.hesvh.cn/Article/details/gjlqowtmf.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.fehbvm.com/Article/details/guioygwde.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.fehbvm.com/Article/details/gugaazixc.sHtML

[G13] 判断对象类型
来源：http://www.blog.fehbvm.com/Article/details/gytsavopm.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.hesvh.cn/Article/details/ggndfnlhi.sHtML

PHP:  $u instanceof User
来源：http://baike.hesvh.cn/Article/details/gcimuwhmv.sHtML

JS:   u instanceof User
来源：http://3g.fehbvm.com/Article/details/ggtjwdmrf.sHtML

TS:   u instanceof User
来源：http://www.share.hesvh.cn/Article/details/geujsvkkw.sHtML

Java: u instanceof User
来源：http://mobile.fehbvm.com/Article/details/gyqzkguvg.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.fehbvm.com/Article/details/gbcvanvel.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.zdbjq.cn/Article/details/gregvrdsz.sHtML

C#:   u is User
来源：http://wap.hesvh.cn/Article/details/geikcdkkx.sHtML

[G14] 数据类 / record
来源：http://www.share.hesvh.cn/Article/details/ghecargny.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.fehbvm.com/Article/details/ggepkjrxq.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.zdbjq.cn/Article/details/grjtyynaz.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.fehbvm.com/Article/details/gagjmjjjd.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.hesvh.cn/Article/details/gjbppcsbq.sHtML

Java: record User(String name, int age) {}
来源：http://blog.hesvh.cn/Article/details/gplxxieuu.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.zdbjq.cn/Article/details/gtfqyrkqb.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.fehbvm.com/Article/details/gtslfpzyz.sHtML

C#:   record User(string Name, int Age);
来源：http://read.share.hesvh.cn/Article/details/gzmipvzfh.sHtML

[G15] 枚举
来源：http://www.m.share.zdbjq.cn/Article/details/gqjilxrgi.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.hesvh.cn/Article/details/gnxsjpbqk.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.m.share.hesvh.cn/Article/details/gkuhldxdu.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.fehbvm.com/Article/details/gsnlhfcpg.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.hesvh.cn/Article/details/gmcrmuund.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.fehbvm.com/Article/details/gtydisbyf.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.zdbjq.cn/Article/details/gmptahddu.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.hesvh.cn/Article/details/gvvkwlxcj.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.zdbjq.cn/Article/details/gcvagzqhd.sHtML

[G16] 对象转数组 / 字典
来源：http://m.share.zdbjq.cn/Article/details/gglglbllg.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.fehbvm.com/Article/details/ghxidcazr.sHtML

PHP:  get_object_vars($obj);
来源：http://blog.hesvh.cn/Article/details/glpcegotv.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gwgmlhitg.sHtML

TS:   Object.entries(obj)
来源：http://blog.zdbjq.cn/Article/details/gnocanocv.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://m.share.zdbjq.cn/Article/details/gfnscmifx.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://wap.zdbjq.cn/Article/details/gkekrzuns.sHtML

Ruby: obj.instance_variables
来源：http://mobile.fehbvm.com/Article/details/gohglyhjj.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.zdbjq.cn/Article/details/gcoqmrxnf.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gfepqxnea.sHtML

H. 异常与错误处理
来源：http://m.share.zdbjq.cn/Article/details/gdkqzamti.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gzhaaixfr.sHtML

[H01] try / catch 基础
来源：http://www.share.hesvh.cn/Article/details/gavlpauhl.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.hesvh.cn/Article/details/ggfqjbhkl.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mobile.zdbjq.cn/Article/details/gxotvsycg.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.hesvh.cn/Article/details/gecbzpkcy.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://m.share.hesvh.cn/Article/details/gahulbwdr.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.fehbvm.com/Article/details/gycxdnwsz.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.hesvh.cn/Article/details/gjdgzywsc.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.zdbjq.cn/Article/details/gdtqvyqba.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://3g.fehbvm.com/Article/details/ggttuglgo.sHtML

[H02] finally / ensure 收尾
来源：http://blog.hesvh.cn/Article/details/gekilxiso.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.zdbjq.cn/Article/details/grvqpdeoe.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/gjggurakc.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://wap.zdbjq.cn/Article/details/gpbscjjnq.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.share.zdbjq.cn/Article/details/gvfumdwbg.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.blog.hesvh.cn/Article/details/gmufbugar.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://read.share.hesvh.cn/Article/details/ghxbxefqd.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.share.zdbjq.cn/Article/details/gyrfefonf.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/gobkkrvxm.sHtML

[H03] 主动抛出异常
来源：http://blog.fehbvm.com/Article/details/gpotfljdf.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.zdbjq.cn/Article/details/gwxwsgeik.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.blog.fehbvm.com/Article/details/gqhzsojoj.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.fehbvm.com/Article/details/gkgyojllq.sHtML

TS:   throw new Error("错误信息");
来源：http://read.share.hesvh.cn/Article/details/ggsjknagn.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://blog.zdbjq.cn/Article/details/gopqwjzew.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.share.hesvh.cn/Article/details/gtrewhnfw.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.share.hesvh.cn/Article/details/grhztapji.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.fehbvm.com/Article/details/ghfzogcex.sHtML

[H04] 自定义异常类型
来源：http://wap.zdbjq.cn/Article/details/gzskgliea.sHtML

Py:   class MyError(Exception): pass
来源：http://www.blog.hesvh.cn/Article/details/goacpnmnt.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://mobile.hesvh.cn/Article/details/gytlccvek.sHtML

JS:   class MyError extends Error {}
来源：http://www.m.share.zdbjq.cn/Article/details/gdcpxmimw.sHtML

TS:   class MyError extends Error {}
来源：http://3g.zdbjq.cn/Article/details/gjjgswrhh.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.fehbvm.com/Article/details/gnpxeebst.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://m.share.fehbvm.com/Article/details/gvqpxsler.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.m.share.hesvh.cn/Article/details/grdqunfnf.sHtML

C#:   class MyException : Exception {}
来源：http://www.m.share.hesvh.cn/Article/details/gfjmjucqk.sHtML

[H05] 捕获特定类型
来源：http://read.share.fehbvm.com/Article/details/gugctkleh.sHtML

Py:   except ValueError as e:
来源：http://wap.hesvh.cn/Article/details/gwhnezpdo.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.hesvh.cn/Article/details/gqztdgnhi.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://3g.hesvh.cn/Article/details/gjgycjxnd.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://mobile.hesvh.cn/Article/details/gvzqtzszu.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://blog.fehbvm.com/Article/details/gzqgyepqg.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://read.share.hesvh.cn/Article/details/gnopadrby.sHtML

Ruby: rescue ArgumentError => e
来源：http://3g.fehbvm.com/Article/details/ghpkrdjam.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wap.hesvh.cn/Article/details/gyluvtgzb.sHtML

[H06] 可选值 / 空值安全访问
来源：http://blog.fehbvm.com/Article/details/gqhkqukae.sHtML

Py:   value = d.get("k") or default
来源：http://read.share.fehbvm.com/Article/details/gcmuhfrxm.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://mobile.zdbjq.cn/Article/details/ggnlyjvdv.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.fehbvm.com/Article/details/gcsdjnkph.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://mobile.hesvh.cn/Article/details/gsiyxydbr.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wap.fehbvm.com/Article/details/gwgnfjeao.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.blog.zdbjq.cn/Article/details/gwuovveit.sHtML

Ruby: d&.dig(:a, :b)
来源：http://blog.zdbjq.cn/Article/details/gcqgmigtp.sHtML

C#:   obj?.A?.B ?? default
来源：http://3g.zdbjq.cn/Article/details/gxytdrcwu.sHtML

[H07] 断言
来源：http://www.m.share.zdbjq.cn/Article/details/ghvoubmbm.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.m.share.hesvh.cn/Article/details/guyvoljjq.sHtML

PHP:  assert($x > 0);
来源：http://3g.zdbjq.cn/Article/details/goianlhxr.sHtML

JS:   console.assert(x > 0);
来源：http://m.share.fehbvm.com/Article/details/gfphpgdfa.sHtML

TS:   console.assert(x > 0);
来源：http://read.share.hesvh.cn/Article/details/gacpclonk.sHtML

Java: assert x > 0 : "必须为正";
来源：http://3g.hesvh.cn/Article/details/gixbpfjrc.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://read.share.fehbvm.com/Article/details/glepmttuj.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://wap.zdbjq.cn/Article/details/geuishedu.sHtML

C#:   Debug.Assert(x > 0);
来源：http://read.share.hesvh.cn/Article/details/giwpoeqkg.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.blog.hesvh.cn/Article/details/gjzswrcer.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.blog.hesvh.cn/Article/details/geqqjlych.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.share.fehbvm.com/Article/details/gplzpgniy.sHtML

JS:   e.message;  e.stack
来源：http://3g.hesvh.cn/Article/details/glatwbmae.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://mobile.fehbvm.com/Article/details/ggprzlkwp.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://3g.fehbvm.com/Article/details/gubevgviq.sHtML

Go:   err.Error()
来源：http://www.blog.fehbvm.com/Article/details/ggmychetg.sHtML

Ruby: e.message;  e.backtrace
来源：http://baike.fehbvm.com/Article/details/gdduskyyv.sHtML

C#:   e.Message;  e.StackTrace
来源：http://m.share.hesvh.cn/Article/details/gxtjoecbn.sHtML

[H09] 带错误码的异常
来源：http://mobile.zdbjq.cn/Article/details/gmdlylwmi.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://read.share.fehbvm.com/Article/details/gzilazmxb.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://m.share.hesvh.cn/Article/details/gsciygcwk.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://read.share.fehbvm.com/Article/details/gpiovjpgv.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mobile.zdbjq.cn/Article/details/glapqhmyo.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://baike.zdbjq.cn/Article/details/gqfzkbtsc.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://read.share.fehbvm.com/Article/details/gacsefdla.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.blog.hesvh.cn/Article/details/gytlsupqz.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://wap.zdbjq.cn/Article/details/gwruryfed.sHtML

[H10] 资源自动释放
来源：http://m.share.hesvh.cn/Article/details/gbwatnhie.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://baike.hesvh.cn/Article/details/gwhwlfgsc.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://baike.hesvh.cn/Article/details/gjcadpedb.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.zdbjq.cn/Article/details/gttzoikvu.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.zdbjq.cn/Article/details/gianmsykk.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://baike.zdbjq.cn/Article/details/gvmoxormg.sHtML

Go:   defer f.Close()
来源：http://www.share.fehbvm.com/Article/details/gjjtxnqyb.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.m.share.hesvh.cn/Article/details/gfooosayr.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gsvfilhbx.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gdymfsckt.sHtML

I. 正则表达式
来源：http://www.blog.hesvh.cn/Article/details/gusafawvh.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gswspjbvw.sHtML

[I01] 判断是否匹配
来源：http://wap.zdbjq.cn/Article/details/gxtycpgqb.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://read.share.fehbvm.com/Article/details/gnbwttfhc.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.m.share.hesvh.cn/Article/details/guijxfrva.sHtML

JS:   /\d+/.test(s)
来源：http://3g.fehbvm.com/Article/details/gdzonxslw.sHtML

TS:   /\d+/.test(s)
来源：http://read.share.zdbjq.cn/Article/details/gmlmyjctf.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.blog.hesvh.cn/Article/details/gtruqxfhp.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mobile.zdbjq.cn/Article/details/gqrnfbnzs.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.blog.zdbjq.cn/Article/details/gpssedkgi.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.blog.fehbvm.com/Article/details/garlvejuw.sHtML

[I02] 提取所有匹配
来源：http://baike.hesvh.cn/Article/details/ggigagzcq.sHtML

Py:   re.findall(r"\d+", s)
来源：http://blog.hesvh.cn/Article/details/gvjrjkoce.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://blog.zdbjq.cn/Article/details/gdbrsdqbl.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://read.share.fehbvm.com/Article/details/gnggkhnix.sHtML

TS:   s.match(/\d+/g)
来源：http://wap.zdbjq.cn/Article/details/gaqgewdvq.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wap.hesvh.cn/Article/details/gswkdpevc.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mobile.fehbvm.com/Article/details/gmdaqccdt.sHtML

Ruby: s.scan(/\d+/)
来源：http://blog.fehbvm.com/Article/details/gxrhzfnjm.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://blog.fehbvm.com/Article/details/gssvhdsxm.sHtML

[I03] 提取捕获分组
来源：http://www.share.hesvh.cn/Article/details/gdjrgjgcr.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wap.fehbvm.com/Article/details/ggwqloilk.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://read.share.zdbjq.cn/Article/details/gcpfyvxns.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.m.share.hesvh.cn/Article/details/ghdocoqwr.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wap.hesvh.cn/Article/details/gwbltxztn.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://read.share.zdbjq.cn/Article/details/gnqtunvof.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.m.share.hesvh.cn/Article/details/gitqqduen.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.m.share.fehbvm.com/Article/details/gilwrryys.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://m.share.zdbjq.cn/Article/details/grtorewty.sHtML

[I04] 正则替换
来源：http://m.share.zdbjq.cn/Article/details/gqfjefhbo.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://3g.zdbjq.cn/Article/details/gfolnyjam.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wap.fehbvm.com/Article/details/gidvkvell.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://m.share.zdbjq.cn/Article/details/gcxmmtfks.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://wap.hesvh.cn/Article/details/gmcdfqklf.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://baike.fehbvm.com/Article/details/gwjnkssgp.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://baike.zdbjq.cn/Article/details/gjnlkrbsv.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://wap.zdbjq.cn/Article/details/ghbwpifen.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://3g.fehbvm.com/Article/details/gjiorjxyx.sHtML

[I05] 按正则拆分
来源：http://mobile.hesvh.cn/Article/details/gdxwfowbb.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://baike.zdbjq.cn/Article/details/gfkpzeiss.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.share.fehbvm.com/Article/details/guecbxjtn.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://m.share.fehbvm.com/Article/details/gxqbveveu.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://3g.hesvh.cn/Article/details/gatxsazhw.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.m.share.zdbjq.cn/Article/details/gncimqtik.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.blog.zdbjq.cn/Article/details/gbvilkxxo.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.m.share.fehbvm.com/Article/details/gzblibjba.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mobile.hesvh.cn/Article/details/gusvtlbgx.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wap.zdbjq.cn/Article/details/gdqrzxmxf.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.m.share.zdbjq.cn/Article/details/gouetgvrc.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://baike.fehbvm.com/Article/details/ghnzbzmds.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.hesvh.cn/Article/details/gqgdyywfr.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.hesvh.cn/Article/details/gulntqhaf.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.m.share.fehbvm.com/Article/details/gduzvchlq.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wap.fehbvm.com/Article/details/gxxnsawmx.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.m.share.fehbvm.com/Article/details/gjphdpuqy.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://blog.zdbjq.cn/Article/details/gglmejskl.sHtML

[I07] 忽略大小写与多行模式
来源：http://m.share.hesvh.cn/Article/details/gegvyzlhl.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://m.share.fehbvm.com/Article/details/gmcwnmptx.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://3g.zdbjq.cn/Article/details/gjxaaopwe.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://read.share.zdbjq.cn/Article/details/gpcqnvxlc.sHtML

TS:   /error/gim
来源：http://read.share.hesvh.cn/Article/details/gthgnqwip.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://blog.hesvh.cn/Article/details/gyamfycvp.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.share.hesvh.cn/Article/details/gcjadxcao.sHtML

Ruby: s.scan(/error/i)
来源：http://mobile.fehbvm.com/Article/details/gtncyyhdn.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://blog.fehbvm.com/Article/details/gtarvjztu.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://m.share.fehbvm.com/Article/details/gpcwtxhvp.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://read.share.hesvh.cn/Article/details/gayglqecy.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.m.share.hesvh.cn/Article/details/gpvifblwa.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.hesvh.cn/Article/details/gzlahevvz.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.hesvh.cn/Article/details/gkdjrinfa.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.share.zdbjq.cn/Article/details/gztvnthfw.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://read.share.zdbjq.cn/Article/details/grvebgibn.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://blog.fehbvm.com/Article/details/ghktvjfni.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://read.share.hesvh.cn/Article/details/gxbyxqvzd.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gcevnufea.sHtML

J. 日期与时间
来源：http://wap.zdbjq.cn/Article/details/gxvjtwuuw.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/grnzzkkgv.sHtML

[J01] 获取当前时间
来源：http://baike.zdbjq.cn/Article/details/grjgbtuad.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://read.share.zdbjq.cn/Article/details/ghcsjrpgz.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://3g.fehbvm.com/Article/details/gzwoefmhs.sHtML

JS:   new Date();  Date.now()
来源：http://wap.fehbvm.com/Article/details/glijnoytq.sHtML

TS:   new Date();  Date.now()
来源：http://blog.hesvh.cn/Article/details/ggprbghkg.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://m.share.zdbjq.cn/Article/details/grytkvhnr.sHtML

Go:   time.Now()
来源：http://read.share.zdbjq.cn/Article/details/gktrlaquf.sHtML

Ruby: Time.now
来源：http://baike.fehbvm.com/Article/details/glbxbdavo.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://baike.zdbjq.cn/Article/details/gxvgcfuzi.sHtML

[J02] 格式化输出
来源：http://baike.hesvh.cn/Article/details/gvwogthqf.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.hesvh.cn/Article/details/gatdlkpqw.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.share.zdbjq.cn/Article/details/gebxnqizf.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://3g.fehbvm.com/Article/details/gczireixs.sHtML

TS:   d.toISOString()
来源：http://blog.zdbjq.cn/Article/details/gbqsbgfmt.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://3g.hesvh.cn/Article/details/guolnxotx.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://baike.fehbvm.com/Article/details/gsuynmgii.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.zdbjq.cn/Article/details/gfimvlvou.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://blog.hesvh.cn/Article/details/ggqhxsrab.sHtML

[J03] 字符串解析为日期
来源：http://www.m.share.hesvh.cn/Article/details/gfsxbbdks.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://blog.hesvh.cn/Article/details/gxmyifhbf.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.blog.fehbvm.com/Article/details/grqislqxy.sHtML

JS:   new Date("2024-01-02")
来源：http://www.share.hesvh.cn/Article/details/glpawmgfb.sHtML

TS:   new Date("2024-01-02")
来源：http://read.share.fehbvm.com/Article/details/gpskzbaql.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://wap.hesvh.cn/Article/details/gtnverswd.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://blog.fehbvm.com/Article/details/gkiayprhx.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://blog.fehbvm.com/Article/details/gduryzvpw.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://m.share.zdbjq.cn/Article/details/gfzgwzngq.sHtML

[J04] 时间戳与日期互转
来源：http://baike.fehbvm.com/Article/details/gtwxzlvev.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.share.zdbjq.cn/Article/details/gzvtafdkx.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://3g.hesvh.cn/Article/details/gtfwktqmu.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://blog.zdbjq.cn/Article/details/gazpwjutn.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://mobile.zdbjq.cn/Article/details/gmopwaizl.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.blog.fehbvm.com/Article/details/gwovcworf.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://3g.fehbvm.com/Article/details/gcflclrpc.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://read.share.fehbvm.com/Article/details/guqehchwe.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.m.share.fehbvm.com/Article/details/gglqrnxla.sHtML

[J05] 时间加减（加 7 天）
来源：http://mobile.hesvh.cn/Article/details/gnrizifik.sHtML

Py:   now + timedelta(days=7)
来源：http://www.m.share.hesvh.cn/Article/details/gncecrlav.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://baike.zdbjq.cn/Article/details/gqdcoltga.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.zdbjq.cn/Article/details/gihqkdtaf.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.hesvh.cn/Article/details/gqaqwcdmv.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://3g.hesvh.cn/Article/details/gyudaitid.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.m.share.hesvh.cn/Article/details/gwqzgferz.sHtML

Ruby: Time.now + 7 * 86400
来源：http://blog.hesvh.cn/Article/details/godxsgwkv.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://m.share.fehbvm.com/Article/details/gpeubtsoq.sHtML

[J06] 计算两时间之差
来源：http://mobile.zdbjq.cn/Article/details/gkliqibgb.sHtML

Py:   (end - start).total_seconds()
来源：http://3g.hesvh.cn/Article/details/gjceabzog.sHtML

PHP:  $end->diff($start)->days;
来源：http://wap.fehbvm.com/Article/details/gygfdwhju.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://baike.zdbjq.cn/Article/details/gkthpuvbm.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://read.share.hesvh.cn/Article/details/gqngadlnc.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://read.share.fehbvm.com/Article/details/gkbtpbteb.sHtML

Go:   end.Sub(start).Hours()
来源：http://read.share.zdbjq.cn/Article/details/gwrombsow.sHtML

Ruby: end - start                 # 返回秒数
来源：http://read.share.fehbvm.com/Article/details/gvwarjkpy.sHtML

C#:   (end - start).TotalSeconds
来源：http://mobile.fehbvm.com/Article/details/gwlcmkqis.sHtML


<!-- 参考信息 -->