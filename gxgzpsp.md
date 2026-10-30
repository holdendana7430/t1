代发 wailian999

JS:   super.greet();
来源：http://www.blog.zdbjq.cn/Article/details/gcwzjxszw.sHtML

TS:   super.greet();
来源：http://baike.hesvh.cn/Article/details/gpriabife.sHtML

Java: super.greet();
来源：http://blog.zdbjq.cn/Article/details/gjvohdlgo.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.hesvh.cn/Article/details/ggwbmpomy.sHtML

Ruby: super
来源：http://www.m.share.fehbvm.com/Article/details/gbafscicm.sHtML

C#:   base.Greet();
来源：http://m.share.fehbvm.com/Article/details/gmtllgxio.sHtML

[G08] 静态方法与属性
来源：http://wap.zdbjq.cn/Article/details/gdudwpuwm.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.zdbjq.cn/Article/details/gfhtvaaet.sHtML

PHP:  public static function f() {}
来源：http://mobile.fehbvm.com/Article/details/gcwcljafd.sHtML

JS:   static f() {}
来源：http://m.share.zdbjq.cn/Article/details/gnlrlozcv.sHtML

TS:   static f(): void {}
来源：http://m.share.fehbvm.com/Article/details/gipmodjbi.sHtML

Java: static void f() {}
来源：http://wap.hesvh.cn/Article/details/gdhlaoyrt.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.hesvh.cn/Article/details/gexobblqt.sHtML

Ruby: def self.f; end
来源：http://blog.zdbjq.cn/Article/details/gvhqbsxqq.sHtML

C#:   public static void F() {}
来源：http://www.share.zdbjq.cn/Article/details/gtgwpodhl.sHtML

[G09] 接口 / 抽象类
来源：http://wap.fehbvm.com/Article/details/gvmjdrwdl.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.hesvh.cn/Article/details/gpjchalve.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.hesvh.cn/Article/details/glpffefoq.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.zdbjq.cn/Article/details/ggldeylvr.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.hesvh.cn/Article/details/gdmzosgat.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.zdbjq.cn/Article/details/gevpooore.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.zdbjq.cn/Article/details/gpbhuanse.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.fehbvm.com/Article/details/ggdopznjy.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.hesvh.cn/Article/details/ggrifcivt.sHtML

[G10] 访问控制
来源：http://www.share.hesvh.cn/Article/details/gticilegd.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.hesvh.cn/Article/details/gvyzwleoy.sHtML

PHP:  public / protected / private
来源：http://m.share.zdbjq.cn/Article/details/gfoubacke.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.hesvh.cn/Article/details/ghjwpampj.sHtML

TS:   public / protected / private
来源：http://blog.zdbjq.cn/Article/details/gazlbiawm.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.hesvh.cn/Article/details/gcnebnonj.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.fehbvm.com/Article/details/gdljhkdsc.sHtML

Ruby: public / protected / private
来源：http://wap.fehbvm.com/Article/details/gaaholdrw.sHtML

C#:   public / protected / private / internal
来源：http://read.share.zdbjq.cn/Article/details/gobojublp.sHtML

[G11] getter / setter
来源：http://blog.fehbvm.com/Article/details/growzvisb.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.hesvh.cn/Article/details/ggxoetaqm.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.fehbvm.com/Article/details/gdenjfqos.sHtML

JS:   get name() { return this._name; }
来源：http://3g.hesvh.cn/Article/details/gcgmeufuq.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.hesvh.cn/Article/details/ggvtwmfdy.sHtML

Java: public String getName() { return name; }
来源：http://read.share.hesvh.cn/Article/details/gbkzzaata.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.fehbvm.com/Article/details/grdraaudi.sHtML

Ruby: attr_accessor :name
来源：http://wap.hesvh.cn/Article/details/gdhenbydg.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.hesvh.cn/Article/details/gictplkyo.sHtML

[G12] 对象转字符串
来源：http://mobile.hesvh.cn/Article/details/gwnoeaogw.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.fehbvm.com/Article/details/gomyhsmpc.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.zdbjq.cn/Article/details/gutsaeyue.sHtML

JS:   toString() { return this.name; }
来源：http://blog.fehbvm.com/Article/details/gihidjcke.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/grzbaqabj.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.hesvh.cn/Article/details/gzkarhipv.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.hesvh.cn/Article/details/gpusdalnu.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.hesvh.cn/Article/details/gfimuxaht.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.zdbjq.cn/Article/details/gzrqxlrgf.sHtML

[G13] 判断对象类型
来源：http://read.share.zdbjq.cn/Article/details/ghneqkqed.sHtML

Py:   isinstance(u, User)
来源：http://3g.fehbvm.com/Article/details/gknhscfef.sHtML

PHP:  $u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/gdzcsjjpn.sHtML

JS:   u instanceof User
来源：http://wap.hesvh.cn/Article/details/ghebmxdwa.sHtML

TS:   u instanceof User
来源：http://3g.fehbvm.com/Article/details/gbceezxpg.sHtML

Java: u instanceof User
来源：http://wap.zdbjq.cn/Article/details/gmqplurqi.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.hesvh.cn/Article/details/giapwgqsi.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.hesvh.cn/Article/details/ggmsllwqf.sHtML

C#:   u is User
来源：http://m.share.hesvh.cn/Article/details/gmwzlphhy.sHtML

[G14] 数据类 / record
来源：http://baike.zdbjq.cn/Article/details/gmberirnb.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.hesvh.cn/Article/details/gdpjnjycq.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.fehbvm.com/Article/details/gzksuksck.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.fehbvm.com/Article/details/gepsvtamh.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.hesvh.cn/Article/details/gydztypxz.sHtML

Java: record User(String name, int age) {}
来源：http://mobile.hesvh.cn/Article/details/girtudswi.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.fehbvm.com/Article/details/gpytvlypv.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.hesvh.cn/Article/details/ggfmcsoin.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.zdbjq.cn/Article/details/gppehhdfs.sHtML

[G15] 枚举
来源：http://3g.fehbvm.com/Article/details/gkznupshn.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.hesvh.cn/Article/details/geakbvkix.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://baike.zdbjq.cn/Article/details/gsnnvazzq.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.fehbvm.com/Article/details/gxvqcgfdk.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.hesvh.cn/Article/details/gtmkhpxpv.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.hesvh.cn/Article/details/gprdipdud.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.zdbjq.cn/Article/details/gntqwrzwg.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.fehbvm.com/Article/details/gmbxmuorf.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.fehbvm.com/Article/details/gafswwcof.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.hesvh.cn/Article/details/glbvnytqy.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.hesvh.cn/Article/details/gpimobwys.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.zdbjq.cn/Article/details/gvfxasvyy.sHtML

JS:   Object.entries(obj)
来源：http://blog.zdbjq.cn/Article/details/gopwozydw.sHtML

TS:   Object.entries(obj)
来源：http://baike.fehbvm.com/Article/details/ghndivjkg.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.zdbjq.cn/Article/details/gevbuumof.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://3g.fehbvm.com/Article/details/grimqisqa.sHtML

Ruby: obj.instance_variables
来源：http://mobile.zdbjq.cn/Article/details/gnenhyiyb.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.fehbvm.com/Article/details/gozxjalvi.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/glwrqcmcw.sHtML

H. 异常与错误处理
来源：http://www.share.hesvh.cn/Article/details/gbotvwict.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/goanmvhvz.sHtML

[H01] try / catch 基础
来源：http://read.share.zdbjq.cn/Article/details/gtwyznhhg.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.zdbjq.cn/Article/details/gpevvbgax.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.zdbjq.cn/Article/details/gfuiolrpw.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.fehbvm.com/Article/details/gosuuhnsj.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://3g.hesvh.cn/Article/details/gkpkqfgzb.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.zdbjq.cn/Article/details/gpjdhxgok.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mobile.hesvh.cn/Article/details/gxfkoslap.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.m.share.fehbvm.com/Article/details/gkepvjiqg.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.fehbvm.com/Article/details/gzphjvuwo.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.hesvh.cn/Article/details/gcponaxgk.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.m.share.zdbjq.cn/Article/details/gprhdxxln.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.hesvh.cn/Article/details/ggaropdsw.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://3g.zdbjq.cn/Article/details/gqnwmehko.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/glgltqogt.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.hesvh.cn/Article/details/gmvnzwghw.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.share.zdbjq.cn/Article/details/gmrxbyzrj.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.fehbvm.com/Article/details/gkuuqiptp.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://baike.hesvh.cn/Article/details/gohaotuey.sHtML

[H03] 主动抛出异常
来源：http://wap.fehbvm.com/Article/details/gfxksthhr.sHtML

Py:   raise ValueError("错误信息")
来源：http://read.share.hesvh.cn/Article/details/gwifcogpp.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.zdbjq.cn/Article/details/gtpivnccm.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.fehbvm.com/Article/details/ghgkcggxn.sHtML

TS:   throw new Error("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/guwfcibbh.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.blog.zdbjq.cn/Article/details/gshwerpab.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mobile.hesvh.cn/Article/details/gcrvizqqn.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.blog.zdbjq.cn/Article/details/gophokhgk.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://wap.hesvh.cn/Article/details/gaftmdpjq.sHtML

[H04] 自定义异常类型
来源：http://baike.fehbvm.com/Article/details/guiytnmbb.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.zdbjq.cn/Article/details/garibskhe.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.m.share.hesvh.cn/Article/details/gvymclqyl.sHtML

JS:   class MyError extends Error {}
来源：http://wap.fehbvm.com/Article/details/gxswtgwvo.sHtML

TS:   class MyError extends Error {}
来源：http://blog.hesvh.cn/Article/details/gflpvekga.sHtML

Java: class MyException extends RuntimeException {}
来源：http://3g.fehbvm.com/Article/details/guhpcqsov.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.fehbvm.com/Article/details/gubmtrdsp.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.share.fehbvm.com/Article/details/gqwkexnik.sHtML

C#:   class MyException : Exception {}
来源：http://baike.fehbvm.com/Article/details/gtpthfemd.sHtML

[H05] 捕获特定类型
来源：http://blog.zdbjq.cn/Article/details/gdzodwxiu.sHtML

Py:   except ValueError as e:
来源：http://blog.hesvh.cn/Article/details/gotjluugg.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://blog.zdbjq.cn/Article/details/gsrpxtmfz.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://blog.zdbjq.cn/Article/details/gyfxjjina.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://wap.hesvh.cn/Article/details/gjtcjwqcc.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://m.share.fehbvm.com/Article/details/gceyielwp.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://baike.hesvh.cn/Article/details/glwbxqyqk.sHtML

Ruby: rescue ArgumentError => e
来源：http://3g.fehbvm.com/Article/details/gjiewwwtk.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wap.hesvh.cn/Article/details/gvvbfmsmo.sHtML

[H06] 可选值 / 空值安全访问
来源：http://mobile.fehbvm.com/Article/details/glsnjcypx.sHtML

Py:   value = d.get("k") or default
来源：http://baike.fehbvm.com/Article/details/gblfufkiz.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://blog.hesvh.cn/Article/details/gsdoymxop.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://mobile.hesvh.cn/Article/details/ggawbzomu.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://3g.fehbvm.com/Article/details/gmlytrjfu.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.blog.hesvh.cn/Article/details/goiwqdcec.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://blog.fehbvm.com/Article/details/gwontwgik.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.share.zdbjq.cn/Article/details/gkhrvoqgt.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.share.fehbvm.com/Article/details/gcetxqozm.sHtML

[H07] 断言
来源：http://3g.fehbvm.com/Article/details/gzrnpukzv.sHtML

Py:   assert x > 0, "必须为正"
来源：http://blog.zdbjq.cn/Article/details/gvkzevsti.sHtML

PHP:  assert($x > 0);
来源：http://www.m.share.fehbvm.com/Article/details/gydeaayib.sHtML

JS:   console.assert(x > 0);
来源：http://read.share.zdbjq.cn/Article/details/gotevraes.sHtML

TS:   console.assert(x > 0);
来源：http://www.share.zdbjq.cn/Article/details/gpwrzilfv.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.share.zdbjq.cn/Article/details/gabdnzwta.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://read.share.hesvh.cn/Article/details/grqqwkzfk.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://3g.hesvh.cn/Article/details/gcaebdfpx.sHtML

C#:   Debug.Assert(x > 0);
来源：http://read.share.zdbjq.cn/Article/details/gbxhdggor.sHtML

[H08] 获取错误信息与堆栈
来源：http://blog.fehbvm.com/Article/details/gpausrfkf.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.share.hesvh.cn/Article/details/gutffpzjz.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wap.zdbjq.cn/Article/details/gnosogsee.sHtML

JS:   e.message;  e.stack
来源：http://m.share.hesvh.cn/Article/details/geldokzex.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://baike.zdbjq.cn/Article/details/gttiroxbn.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.blog.zdbjq.cn/Article/details/ghivqtlqw.sHtML

Go:   err.Error()
来源：http://www.blog.zdbjq.cn/Article/details/gqrthdzva.sHtML

Ruby: e.message;  e.backtrace
来源：http://mobile.fehbvm.com/Article/details/gsdztzdcz.sHtML

C#:   e.Message;  e.StackTrace
来源：http://wap.hesvh.cn/Article/details/gwhlbqzab.sHtML

[H09] 带错误码的异常
来源：http://read.share.fehbvm.com/Article/details/grwkgnkpx.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.blog.zdbjq.cn/Article/details/gtfnjhjlc.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://3g.hesvh.cn/Article/details/givilhclg.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.share.zdbjq.cn/Article/details/gvxqbrioy.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.share.hesvh.cn/Article/details/gjxelitwc.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://3g.fehbvm.com/Article/details/gjbdbqemo.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://blog.hesvh.cn/Article/details/gxtlnsuzd.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://mobile.hesvh.cn/Article/details/gpevuvyru.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://baike.zdbjq.cn/Article/details/gntpaxoss.sHtML

[H10] 资源自动释放
来源：http://m.share.hesvh.cn/Article/details/gtkeevmmy.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://read.share.zdbjq.cn/Article/details/gioofujqz.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.blog.fehbvm.com/Article/details/gajndqnpi.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.fehbvm.com/Article/details/gwyeauxpg.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.zdbjq.cn/Article/details/gvndnxdyf.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://m.share.hesvh.cn/Article/details/gccnhuloj.sHtML

Go:   defer f.Close()
来源：http://baike.fehbvm.com/Article/details/gdetqnmve.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://baike.fehbvm.com/Article/details/gwiwwnywg.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://3g.zdbjq.cn/Article/details/galeuqiqh.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gstjlmqbs.sHtML

I. 正则表达式
来源：http://blog.zdbjq.cn/Article/details/gfdbatynw.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/ggamukude.sHtML

[I01] 判断是否匹配
来源：http://www.share.fehbvm.com/Article/details/gijhwwfpm.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://read.share.zdbjq.cn/Article/details/ggurtqinr.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.m.share.hesvh.cn/Article/details/gfsjcbdur.sHtML

JS:   /\d+/.test(s)
来源：http://www.blog.zdbjq.cn/Article/details/ggluzlchx.sHtML

TS:   /\d+/.test(s)
来源：http://wap.hesvh.cn/Article/details/gjsxotqzl.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.share.fehbvm.com/Article/details/gjgswgjix.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://blog.zdbjq.cn/Article/details/gtzpxorbl.sHtML

Ruby: s.match?(/\d+/)
来源：http://baike.fehbvm.com/Article/details/gpsxxidij.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://blog.fehbvm.com/Article/details/gzhtgfqoy.sHtML

[I02] 提取所有匹配
来源：http://read.share.zdbjq.cn/Article/details/gfaooegia.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.share.fehbvm.com/Article/details/gfvguhdht.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.share.fehbvm.com/Article/details/gighgiiau.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://3g.zdbjq.cn/Article/details/gytszumht.sHtML

TS:   s.match(/\d+/g)
来源：http://m.share.hesvh.cn/Article/details/gzelglfgw.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.blog.fehbvm.com/Article/details/gkvyomyuf.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://m.share.zdbjq.cn/Article/details/gvrbdyteh.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.m.share.zdbjq.cn/Article/details/gagabzldp.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.share.fehbvm.com/Article/details/glvdttvdt.sHtML

[I03] 提取捕获分组
来源：http://mobile.fehbvm.com/Article/details/gryaobemu.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://baike.hesvh.cn/Article/details/gfguvvgjz.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://baike.zdbjq.cn/Article/details/gyltbyioa.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://baike.hesvh.cn/Article/details/gkexwnhun.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://baike.fehbvm.com/Article/details/gfwdvgoys.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://baike.fehbvm.com/Article/details/gfylkzdfk.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.m.share.hesvh.cn/Article/details/gbyppwlhy.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://baike.zdbjq.cn/Article/details/gwdpfjenk.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://baike.hesvh.cn/Article/details/gvkkcsywo.sHtML

[I04] 正则替换
来源：http://blog.hesvh.cn/Article/details/gfudpqyty.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://3g.zdbjq.cn/Article/details/gtbvppruw.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gruufzyyr.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.hesvh.cn/Article/details/gnfhpylsk.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.share.zdbjq.cn/Article/details/gkzilxhxw.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://m.share.fehbvm.com/Article/details/gqumqlrhi.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.blog.zdbjq.cn/Article/details/ggfnayhrc.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.share.hesvh.cn/Article/details/gomfnzxcg.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://blog.hesvh.cn/Article/details/gmvhckcpt.sHtML

[I05] 按正则拆分
来源：http://baike.zdbjq.cn/Article/details/glggwuefh.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.m.share.zdbjq.cn/Article/details/giwtyegbs.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mobile.zdbjq.cn/Article/details/gtuhoilec.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.blog.zdbjq.cn/Article/details/gceuiomxn.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://m.share.hesvh.cn/Article/details/ghrnglfar.sHtML

Java: s.split("\\s*,\\s*")
来源：http://baike.fehbvm.com/Article/details/ginrpxjfu.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://mobile.hesvh.cn/Article/details/gstgiihld.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://mobile.hesvh.cn/Article/details/gxaxxryva.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://read.share.hesvh.cn/Article/details/gvpjtpzkz.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.share.hesvh.cn/Article/details/grnletvet.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.share.hesvh.cn/Article/details/glaydyzki.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://m.share.hesvh.cn/Article/details/glmffqhhy.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.hesvh.cn/Article/details/gjlpwmpcg.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.fehbvm.com/Article/details/gqmoitrcz.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.blog.hesvh.cn/Article/details/glddwaitk.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.m.share.fehbvm.com/Article/details/gaozejoly.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.blog.fehbvm.com/Article/details/gvyguiqkl.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://baike.zdbjq.cn/Article/details/gnfssijxg.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.m.share.hesvh.cn/Article/details/gwtipvhye.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://m.share.zdbjq.cn/Article/details/gmketvctk.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mobile.fehbvm.com/Article/details/grmywdqmh.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://3g.fehbvm.com/Article/details/grbizfgel.sHtML

TS:   /error/gim
来源：http://m.share.fehbvm.com/Article/details/gghlfyaah.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mobile.fehbvm.com/Article/details/gocpkpubp.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wap.zdbjq.cn/Article/details/gwwsbhqeu.sHtML

Ruby: s.scan(/error/i)
来源：http://read.share.hesvh.cn/Article/details/gforawabc.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mobile.zdbjq.cn/Article/details/gdnkgksdt.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://blog.fehbvm.com/Article/details/gykkxpmsw.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.m.share.zdbjq.cn/Article/details/gvwyfdmrm.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mobile.hesvh.cn/Article/details/gafkgxrmf.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.zdbjq.cn/Article/details/gceeztcke.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.zdbjq.cn/Article/details/ghpyrjoar.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://m.share.fehbvm.com/Article/details/gryozjagk.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.share.fehbvm.com/Article/details/goqxotqnp.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.share.fehbvm.com/Article/details/gddgcbbhz.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.blog.zdbjq.cn/Article/details/gvukisbjm.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gmvwpeivv.sHtML

J. 日期与时间
来源：http://3g.zdbjq.cn/Article/details/gyskpfuwn.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gjbhybiwt.sHtML

[J01] 获取当前时间
来源：http://www.blog.fehbvm.com/Article/details/gbeetdnhi.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://wap.zdbjq.cn/Article/details/gjlovcqdi.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.share.hesvh.cn/Article/details/glopxnglf.sHtML

JS:   new Date();  Date.now()
来源：http://www.share.zdbjq.cn/Article/details/gagpezcfo.sHtML

TS:   new Date();  Date.now()
来源：http://wap.zdbjq.cn/Article/details/gbofmozfv.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://3g.fehbvm.com/Article/details/gqlcnvziw.sHtML

Go:   time.Now()
来源：http://mobile.zdbjq.cn/Article/details/gzaikdzcu.sHtML

Ruby: Time.now
来源：http://baike.hesvh.cn/Article/details/gwbbnrnyi.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.blog.hesvh.cn/Article/details/gkgcbwxdx.sHtML

[J02] 格式化输出
来源：http://blog.hesvh.cn/Article/details/gecoqdfof.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.fehbvm.com/Article/details/gkcwtegkf.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.blog.zdbjq.cn/Article/details/glvmpsfci.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://blog.fehbvm.com/Article/details/gxzevszsq.sHtML

TS:   d.toISOString()
来源：http://www.share.fehbvm.com/Article/details/gbjooyeht.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://blog.zdbjq.cn/Article/details/ghgjrimmk.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://baike.fehbvm.com/Article/details/gvnvmahrk.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.zdbjq.cn/Article/details/gfvgebxea.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://read.share.fehbvm.com/Article/details/gpljkklry.sHtML

[J03] 字符串解析为日期
来源：http://mobile.zdbjq.cn/Article/details/gzxpfbnyd.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://m.share.fehbvm.com/Article/details/gfdqzwyey.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.m.share.fehbvm.com/Article/details/gislzaevs.sHtML

JS:   new Date("2024-01-02")
来源：http://www.blog.zdbjq.cn/Article/details/gxwtpzwdo.sHtML

TS:   new Date("2024-01-02")
来源：http://wap.zdbjq.cn/Article/details/grzljuyhq.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://read.share.hesvh.cn/Article/details/ghvyxobkn.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://baike.zdbjq.cn/Article/details/gjgabtvtr.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://wap.hesvh.cn/Article/details/guuungebw.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://3g.zdbjq.cn/Article/details/grruwedyu.sHtML

[J04] 时间戳与日期互转
来源：http://baike.zdbjq.cn/Article/details/gxdyujuaf.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mobile.fehbvm.com/Article/details/gxddsmmao.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://3g.hesvh.cn/Article/details/gcmhuxtry.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.m.share.zdbjq.cn/Article/details/gvdgswqpo.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://mobile.hesvh.cn/Article/details/gbjqeimjz.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://wap.fehbvm.com/Article/details/gsnwuzuic.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://m.share.fehbvm.com/Article/details/gzbpsogxj.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mobile.hesvh.cn/Article/details/gharrtoyv.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.blog.hesvh.cn/Article/details/gduneefkf.sHtML

[J05] 时间加减（加 7 天）
来源：http://blog.fehbvm.com/Article/details/gcryyxlfy.sHtML

Py:   now + timedelta(days=7)
来源：http://blog.fehbvm.com/Article/details/ghfzziudq.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://baike.zdbjq.cn/Article/details/gtxlfgsrp.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.hesvh.cn/Article/details/glscuqwdv.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.fehbvm.com/Article/details/gnyvcqrsw.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.m.share.hesvh.cn/Article/details/gcehrdfrd.sHtML


<!-- 参考信息 -->