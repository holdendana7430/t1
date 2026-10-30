代发 wailian999

PHP:  public static function f() {}
来源：http://wap.fehbvm.com/Article/details/gxmqlujib.sHtML

JS:   static f() {}
来源：http://3g.hesvh.cn/Article/details/gmktvfseg.sHtML

TS:   static f(): void {}
来源：http://read.share.hesvh.cn/Article/details/gczfowugd.sHtML

Java: static void f() {}
来源：http://www.share.hesvh.cn/Article/details/gmozkfpsw.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.fehbvm.com/Article/details/gazvhqygv.sHtML

Ruby: def self.f; end
来源：http://www.blog.fehbvm.com/Article/details/glkbtfcgm.sHtML

C#:   public static void F() {}
来源：http://www.m.share.fehbvm.com/Article/details/gqdvjeoad.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.zdbjq.cn/Article/details/gcmkrgure.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.zdbjq.cn/Article/details/gudsenlcb.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.hesvh.cn/Article/details/gazovldko.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.zdbjq.cn/Article/details/grkldtlfp.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.zdbjq.cn/Article/details/ghjpfozev.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.zdbjq.cn/Article/details/gtbzlznsq.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.hesvh.cn/Article/details/gworvliek.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.zdbjq.cn/Article/details/ggmxsnuay.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.fehbvm.com/Article/details/gekukhyit.sHtML

[G10] 访问控制
来源：http://3g.zdbjq.cn/Article/details/gmxwiqnms.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.fehbvm.com/Article/details/giadhcuqn.sHtML

PHP:  public / protected / private
来源：http://www.share.fehbvm.com/Article/details/gufbubdus.sHtML

JS:   #private 字段；其余公开
来源：http://3g.hesvh.cn/Article/details/gnusgehcn.sHtML

TS:   public / protected / private
来源：http://www.share.zdbjq.cn/Article/details/gczjcmqqr.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.zdbjq.cn/Article/details/gfamismld.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.fehbvm.com/Article/details/gkobnxrgr.sHtML

Ruby: public / protected / private
来源：http://www.blog.zdbjq.cn/Article/details/gxnpbntgz.sHtML

C#:   public / protected / private / internal
来源：http://wap.fehbvm.com/Article/details/gzwruklgn.sHtML

[G11] getter / setter
来源：http://www.share.zdbjq.cn/Article/details/gadkcowzc.sHtML

Py:   @property 与 @x.setter
来源：http://baike.hesvh.cn/Article/details/gombjiphz.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.fehbvm.com/Article/details/gjafddrlt.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.zdbjq.cn/Article/details/gnshlktqr.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.fehbvm.com/Article/details/gaphwvegy.sHtML

Java: public String getName() { return name; }
来源：http://www.share.fehbvm.com/Article/details/gtrbsqsby.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.fehbvm.com/Article/details/gcjlbsxrg.sHtML

Ruby: attr_accessor :name
来源：http://baike.zdbjq.cn/Article/details/gvaykyzmw.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.hesvh.cn/Article/details/guinnazud.sHtML

[G12] 对象转字符串
来源：http://blog.zdbjq.cn/Article/details/gawgeztfn.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.fehbvm.com/Article/details/gtledeubk.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.zdbjq.cn/Article/details/gdyewproh.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/gnwbfpqlv.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/gpdzhzcng.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.hesvh.cn/Article/details/gvovkqqmm.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.fehbvm.com/Article/details/gqqqjujbx.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.zdbjq.cn/Article/details/ghtpptypa.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.fehbvm.com/Article/details/gzbhcvcat.sHtML

[G13] 判断对象类型
来源：http://mobile.hesvh.cn/Article/details/gbgkmkxqg.sHtML

Py:   isinstance(u, User)
来源：http://blog.zdbjq.cn/Article/details/gzchthtjr.sHtML

PHP:  $u instanceof User
来源：http://baike.fehbvm.com/Article/details/ghrxgbwiy.sHtML

JS:   u instanceof User
来源：http://www.m.share.hesvh.cn/Article/details/gxqvhfyss.sHtML

TS:   u instanceof User
来源：http://www.share.zdbjq.cn/Article/details/gmlpvrwzo.sHtML

Java: u instanceof User
来源：http://blog.fehbvm.com/Article/details/gshtbdknk.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.hesvh.cn/Article/details/gozhbtotz.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.fehbvm.com/Article/details/gdywvellu.sHtML

C#:   u is User
来源：http://www.m.share.hesvh.cn/Article/details/gpmfefkoi.sHtML

[G14] 数据类 / record
来源：http://3g.zdbjq.cn/Article/details/geplwpvmv.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.fehbvm.com/Article/details/gyzefmfkf.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.hesvh.cn/Article/details/gkmocxtoo.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.zdbjq.cn/Article/details/glaupxcaq.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.zdbjq.cn/Article/details/gjzuxuavb.sHtML

Java: record User(String name, int age) {}
来源：http://mobile.hesvh.cn/Article/details/gnfaguvyp.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.fehbvm.com/Article/details/gyastftor.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.fehbvm.com/Article/details/gaeoephfz.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.hesvh.cn/Article/details/gddgbufqp.sHtML

[G15] 枚举
来源：http://baike.fehbvm.com/Article/details/gwxslkkug.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.zdbjq.cn/Article/details/glclizvdd.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.zdbjq.cn/Article/details/gpxpnpyye.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.zdbjq.cn/Article/details/gkhiukkcs.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.fehbvm.com/Article/details/gvchvifjo.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.zdbjq.cn/Article/details/gxmhklejx.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://baike.fehbvm.com/Article/details/giqffzeci.sHtML

Ruby: Color = %i[red green].freeze
来源：http://m.share.zdbjq.cn/Article/details/gthvazivq.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.fehbvm.com/Article/details/gmcpcpnaw.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.zdbjq.cn/Article/details/gzqybgxis.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.zdbjq.cn/Article/details/gafvbioig.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.hesvh.cn/Article/details/gxogiwdkx.sHtML

JS:   Object.entries(obj)
来源：http://m.share.fehbvm.com/Article/details/gdnbqhgep.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gqpssuuye.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://m.share.fehbvm.com/Article/details/grkajmrww.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.hesvh.cn/Article/details/gckjczusz.sHtML

Ruby: obj.instance_variables
来源：http://m.share.zdbjq.cn/Article/details/gxjxjpufo.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.fehbvm.com/Article/details/guehgyuis.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gultvqyup.sHtML

H. 异常与错误处理
来源：http://m.share.zdbjq.cn/Article/details/gkdgkynml.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/golqbkyrj.sHtML

[H01] try / catch 基础
来源：http://mobile.zdbjq.cn/Article/details/gwikkkbwo.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://baike.zdbjq.cn/Article/details/gkmwxdetv.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wap.hesvh.cn/Article/details/gbkkvxvge.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.fehbvm.com/Article/details/gknopxwfv.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.blog.zdbjq.cn/Article/details/gjjyokdvg.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.m.share.hesvh.cn/Article/details/ghrssyhnw.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://read.share.fehbvm.com/Article/details/golxbcmvd.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.hesvh.cn/Article/details/gfyujmfkc.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.zdbjq.cn/Article/details/gqonzmmoh.sHtML

[H02] finally / ensure 收尾
来源：http://wap.fehbvm.com/Article/details/gqkwnaigo.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://3g.fehbvm.com/Article/details/ghqnwcpix.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/gceqvzdaw.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/govldfbam.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/ghvzbdeuf.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.share.zdbjq.cn/Article/details/gsvkcmmvw.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.hesvh.cn/Article/details/gadjojosm.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://blog.hesvh.cn/Article/details/gjwjzvvha.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://baike.fehbvm.com/Article/details/glhtupnvu.sHtML

[H03] 主动抛出异常
来源：http://mobile.zdbjq.cn/Article/details/guiqvmqlm.sHtML

Py:   raise ValueError("错误信息")
来源：http://blog.fehbvm.com/Article/details/gczifwgry.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.blog.hesvh.cn/Article/details/giuinudvy.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.fehbvm.com/Article/details/gtuiffrkk.sHtML

TS:   throw new Error("错误信息");
来源：http://baike.hesvh.cn/Article/details/gvaarjbhs.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://blog.zdbjq.cn/Article/details/ghepejqws.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.blog.zdbjq.cn/Article/details/gfbnooclq.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://mobile.hesvh.cn/Article/details/gtemntvhb.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.blog.zdbjq.cn/Article/details/gjaqhauyb.sHtML

[H04] 自定义异常类型
来源：http://m.share.zdbjq.cn/Article/details/gcdkzyvvp.sHtML

Py:   class MyError(Exception): pass
来源：http://www.blog.zdbjq.cn/Article/details/gfmirzryc.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.m.share.zdbjq.cn/Article/details/gtljxkjpo.sHtML

JS:   class MyError extends Error {}
来源：http://www.blog.zdbjq.cn/Article/details/geiaqnccj.sHtML

TS:   class MyError extends Error {}
来源：http://baike.zdbjq.cn/Article/details/gujwlplse.sHtML

Java: class MyException extends RuntimeException {}
来源：http://3g.fehbvm.com/Article/details/gmlswnhyz.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.share.fehbvm.com/Article/details/gbvnwthnf.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.share.zdbjq.cn/Article/details/gzqrtvglw.sHtML

C#:   class MyException : Exception {}
来源：http://www.share.hesvh.cn/Article/details/gybevpuod.sHtML

[H05] 捕获特定类型
来源：http://m.share.hesvh.cn/Article/details/gzekqemdl.sHtML

Py:   except ValueError as e:
来源：http://www.blog.fehbvm.com/Article/details/gfelmolzr.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://m.share.fehbvm.com/Article/details/gxusbhclt.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://read.share.fehbvm.com/Article/details/gezbctaes.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://m.share.hesvh.cn/Article/details/gmsqhpkaf.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://wap.fehbvm.com/Article/details/gtgsisaqh.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://m.share.hesvh.cn/Article/details/gkfrxrses.sHtML

Ruby: rescue ArgumentError => e
来源：http://m.share.fehbvm.com/Article/details/gjpajgmqd.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://m.share.fehbvm.com/Article/details/gamsknkil.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.m.share.hesvh.cn/Article/details/geoifrqzp.sHtML

Py:   value = d.get("k") or default
来源：http://mobile.zdbjq.cn/Article/details/gcegrxekg.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.blog.hesvh.cn/Article/details/gqybisdkf.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.blog.fehbvm.com/Article/details/gmvybliyg.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://baike.hesvh.cn/Article/details/gtkiksouf.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://read.share.zdbjq.cn/Article/details/grznnvvmm.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.m.share.fehbvm.com/Article/details/gjpeickys.sHtML

Ruby: d&.dig(:a, :b)
来源：http://3g.hesvh.cn/Article/details/gsjlrcoqn.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.share.hesvh.cn/Article/details/gpblwaaqe.sHtML

[H07] 断言
来源：http://www.share.hesvh.cn/Article/details/gfxfasdsh.sHtML

Py:   assert x > 0, "必须为正"
来源：http://wap.zdbjq.cn/Article/details/gtmizkqmu.sHtML

PHP:  assert($x > 0);
来源：http://www.blog.fehbvm.com/Article/details/gjdwizody.sHtML

JS:   console.assert(x > 0);
来源：http://m.share.zdbjq.cn/Article/details/gcmxfptas.sHtML

TS:   console.assert(x > 0);
来源：http://www.blog.hesvh.cn/Article/details/glnwqnenh.sHtML

Java: assert x > 0 : "必须为正";
来源：http://3g.hesvh.cn/Article/details/gnhpajbyl.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://blog.hesvh.cn/Article/details/gdgjotwpg.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.m.share.fehbvm.com/Article/details/gzmdkdrvk.sHtML

C#:   Debug.Assert(x > 0);
来源：http://wap.fehbvm.com/Article/details/ggesthhpn.sHtML

[H08] 获取错误信息与堆栈
来源：http://wap.hesvh.cn/Article/details/gkauresza.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.share.hesvh.cn/Article/details/gxdupctsa.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://m.share.hesvh.cn/Article/details/gneeavwdd.sHtML

JS:   e.message;  e.stack
来源：http://read.share.zdbjq.cn/Article/details/gitwlojdp.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.blog.hesvh.cn/Article/details/giqtdldtw.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://blog.zdbjq.cn/Article/details/gzqrysygr.sHtML

Go:   err.Error()
来源：http://read.share.hesvh.cn/Article/details/gbudspdhl.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.blog.fehbvm.com/Article/details/gcyqsfcrk.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.m.share.hesvh.cn/Article/details/gfwaqamay.sHtML

[H09] 带错误码的异常
来源：http://www.blog.hesvh.cn/Article/details/gwvhresiq.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://3g.fehbvm.com/Article/details/gapajelbk.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.share.hesvh.cn/Article/details/gbkkadlhq.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wap.hesvh.cn/Article/details/gtozpbbvi.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://read.share.hesvh.cn/Article/details/gtczzgomw.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.m.share.zdbjq.cn/Article/details/gmcbiomil.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://3g.zdbjq.cn/Article/details/gldplhrng.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.m.share.zdbjq.cn/Article/details/grjqfrvoa.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.blog.zdbjq.cn/Article/details/gsqtncyun.sHtML

[H10] 资源自动释放
来源：http://3g.hesvh.cn/Article/details/goheuftpd.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://m.share.zdbjq.cn/Article/details/gjbqvqwkx.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wap.fehbvm.com/Article/details/gbjsrnoqe.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.zdbjq.cn/Article/details/gwyzsctpw.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.fehbvm.com/Article/details/gbzgvmvfq.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.blog.hesvh.cn/Article/details/ghmkijucr.sHtML

Go:   defer f.Close()
来源：http://wap.fehbvm.com/Article/details/grhdkdqno.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wap.fehbvm.com/Article/details/gaebfwvwe.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://3g.fehbvm.com/Article/details/gjtjnqfao.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gnitxppvi.sHtML

I. 正则表达式
来源：http://3g.fehbvm.com/Article/details/gakvbubse.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gxetgxvto.sHtML

[I01] 判断是否匹配
来源：http://read.share.fehbvm.com/Article/details/goznllaup.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://read.share.zdbjq.cn/Article/details/gojurvrpu.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://3g.hesvh.cn/Article/details/gvpdojaez.sHtML

JS:   /\d+/.test(s)
来源：http://baike.fehbvm.com/Article/details/gfdjhjopv.sHtML

TS:   /\d+/.test(s)
来源：http://m.share.fehbvm.com/Article/details/grmtukdlr.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wap.fehbvm.com/Article/details/gomxkwtjz.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://blog.zdbjq.cn/Article/details/gbbuvgbbv.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.m.share.zdbjq.cn/Article/details/gtlwsfkuk.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://read.share.hesvh.cn/Article/details/gmyxfjuhn.sHtML

[I02] 提取所有匹配
来源：http://mobile.fehbvm.com/Article/details/ggvimzcoi.sHtML

Py:   re.findall(r"\d+", s)
来源：http://3g.fehbvm.com/Article/details/gdacgginq.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://m.share.hesvh.cn/Article/details/gcjixpydn.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mobile.zdbjq.cn/Article/details/gldvbybqc.sHtML

TS:   s.match(/\d+/g)
来源：http://blog.zdbjq.cn/Article/details/gxjuutkia.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://3g.zdbjq.cn/Article/details/gqdbdeggl.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://m.share.fehbvm.com/Article/details/gzwzhpeda.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.m.share.fehbvm.com/Article/details/gjpqbyqqx.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://3g.zdbjq.cn/Article/details/gchhalodg.sHtML

[I03] 提取捕获分组
来源：http://read.share.zdbjq.cn/Article/details/gbvdfkvov.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gejbjfzvq.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://3g.zdbjq.cn/Article/details/gahccymcw.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wap.zdbjq.cn/Article/details/gvexemxik.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mobile.fehbvm.com/Article/details/gjquigwzx.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://m.share.fehbvm.com/Article/details/glhbbbkwy.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://baike.zdbjq.cn/Article/details/gndqogtvd.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://m.share.hesvh.cn/Article/details/grixexneg.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://baike.zdbjq.cn/Article/details/gqxrvpujf.sHtML

[I04] 正则替换
来源：http://read.share.fehbvm.com/Article/details/gwsegavne.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://mobile.fehbvm.com/Article/details/gpztjqccn.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://blog.fehbvm.com/Article/details/giqlgoaah.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://read.share.zdbjq.cn/Article/details/gcpistthc.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.fehbvm.com/Article/details/gqezzfliz.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.share.hesvh.cn/Article/details/gqhqysnmw.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://3g.hesvh.cn/Article/details/ganljbjcc.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.share.hesvh.cn/Article/details/gfjnaaipo.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://baike.hesvh.cn/Article/details/gofbnpiuh.sHtML

[I05] 按正则拆分
来源：http://www.m.share.fehbvm.com/Article/details/gmsnkxzpd.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.blog.hesvh.cn/Article/details/gktrrtljd.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://3g.fehbvm.com/Article/details/gywzuzpdp.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://blog.fehbvm.com/Article/details/ghdnvxekh.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://wap.zdbjq.cn/Article/details/gvjywixhn.sHtML

Java: s.split("\\s*,\\s*")
来源：http://3g.fehbvm.com/Article/details/gvhlpmlle.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.m.share.zdbjq.cn/Article/details/gwzkfedal.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://wap.zdbjq.cn/Article/details/gsdiidspk.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.share.fehbvm.com/Article/details/gjppilmpa.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.blog.hesvh.cn/Article/details/gctshtrbh.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://m.share.hesvh.cn/Article/details/gwltfphyc.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://3g.zdbjq.cn/Article/details/gylvzlwut.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.zdbjq.cn/Article/details/gvtbdxnpj.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.zdbjq.cn/Article/details/gptoqjgai.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://blog.hesvh.cn/Article/details/gooumjiku.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://mobile.hesvh.cn/Article/details/gxisramuu.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://read.share.hesvh.cn/Article/details/gtwhralzw.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.share.zdbjq.cn/Article/details/gcdlhhoaz.sHtML

[I07] 忽略大小写与多行模式
来源：http://wap.hesvh.cn/Article/details/ggwwjpumx.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wap.zdbjq.cn/Article/details/gnndsfhis.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://read.share.fehbvm.com/Article/details/gercuwnjk.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://m.share.fehbvm.com/Article/details/gosahyden.sHtML

TS:   /error/gim
来源：http://www.blog.zdbjq.cn/Article/details/gmwewtdsa.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.m.share.fehbvm.com/Article/details/gdfvvwsqv.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.share.hesvh.cn/Article/details/gqxlhpjnz.sHtML

Ruby: s.scan(/error/i)
来源：http://www.m.share.zdbjq.cn/Article/details/gmvnhqoef.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.blog.zdbjq.cn/Article/details/gfuqewdhp.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://mobile.hesvh.cn/Article/details/gpzzenajk.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://3g.zdbjq.cn/Article/details/gbmvnmcbe.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://read.share.zdbjq.cn/Article/details/gutorvbrz.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.fehbvm.com/Article/details/gnqoikhge.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.zdbjq.cn/Article/details/gjrammkzr.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://read.share.fehbvm.com/Article/details/gribfnwvs.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wap.zdbjq.cn/Article/details/grxmdswzd.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.blog.fehbvm.com/Article/details/gnzdqyaje.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://baike.hesvh.cn/Article/details/gdjfjniyq.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gqmgtuyym.sHtML

J. 日期与时间
来源：http://blog.hesvh.cn/Article/details/gaxzpooxa.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gddnvllxc.sHtML

[J01] 获取当前时间
来源：http://3g.hesvh.cn/Article/details/gdcrsgomy.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.m.share.fehbvm.com/Article/details/ggztjzmfw.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://3g.zdbjq.cn/Article/details/gikzawsho.sHtML

JS:   new Date();  Date.now()
来源：http://blog.hesvh.cn/Article/details/gqutnimsl.sHtML

TS:   new Date();  Date.now()
来源：http://blog.zdbjq.cn/Article/details/gytwhmjxl.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://mobile.fehbvm.com/Article/details/glsngycbb.sHtML

Go:   time.Now()
来源：http://blog.fehbvm.com/Article/details/gatashese.sHtML

Ruby: Time.now
来源：http://m.share.hesvh.cn/Article/details/gpmsswmjz.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.m.share.zdbjq.cn/Article/details/giqpkhxqa.sHtML

[J02] 格式化输出
来源：http://www.blog.fehbvm.com/Article/details/gpfckccan.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.hesvh.cn/Article/details/gojzneaml.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mobile.hesvh.cn/Article/details/goczbxuzs.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.share.fehbvm.com/Article/details/grwvngohn.sHtML

TS:   d.toISOString()
来源：http://m.share.hesvh.cn/Article/details/gonltofpi.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://blog.zdbjq.cn/Article/details/gyosthocv.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://read.share.zdbjq.cn/Article/details/gsajrlsmw.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.fehbvm.com/Article/details/gprrexywb.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://blog.hesvh.cn/Article/details/gglmcvozr.sHtML

[J03] 字符串解析为日期
来源：http://blog.hesvh.cn/Article/details/gmrhgabzm.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://3g.hesvh.cn/Article/details/gviuufldx.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.blog.hesvh.cn/Article/details/gcmlawmrj.sHtML

JS:   new Date("2024-01-02")
来源：http://wap.zdbjq.cn/Article/details/gievhzdop.sHtML

TS:   new Date("2024-01-02")
来源：http://3g.hesvh.cn/Article/details/glmiupfsj.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://3g.hesvh.cn/Article/details/gkujxdvsa.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://blog.fehbvm.com/Article/details/gdcnbvvjt.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://wap.hesvh.cn/Article/details/gkgnzsvnl.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mobile.fehbvm.com/Article/details/gdkbaporm.sHtML

[J04] 时间戳与日期互转
来源：http://blog.zdbjq.cn/Article/details/guspzttwp.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://read.share.hesvh.cn/Article/details/gqydxrrpg.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://m.share.fehbvm.com/Article/details/gavlgrbxe.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://3g.hesvh.cn/Article/details/guydzcadb.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://wap.fehbvm.com/Article/details/gaijfeyiw.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://3g.fehbvm.com/Article/details/gmtlzvazr.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://mobile.fehbvm.com/Article/details/gedhkrrqb.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://read.share.zdbjq.cn/Article/details/gxawkfkhi.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://m.share.fehbvm.com/Article/details/gckmsjqoe.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.blog.zdbjq.cn/Article/details/gaiihwamx.sHtML

Py:   now + timedelta(days=7)
来源：http://blog.zdbjq.cn/Article/details/grhamjsud.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.m.share.zdbjq.cn/Article/details/gycsqkkjm.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.zdbjq.cn/Article/details/gzfkmqbgf.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.fehbvm.com/Article/details/guccrgszh.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.m.share.hesvh.cn/Article/details/gediiqocz.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.share.hesvh.cn/Article/details/gbxpozlua.sHtML

Ruby: Time.now + 7 * 86400
来源：http://wap.zdbjq.cn/Article/details/gtunqgkdz.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://baike.fehbvm.com/Article/details/ghzonvgol.sHtML

[J06] 计算两时间之差
来源：http://read.share.hesvh.cn/Article/details/gzygrvckz.sHtML

Py:   (end - start).total_seconds()
来源：http://blog.hesvh.cn/Article/details/gmezsqepj.sHtML

PHP:  $end->diff($start)->days;
来源：http://m.share.fehbvm.com/Article/details/gttncyaxo.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wap.fehbvm.com/Article/details/gsvzzvkpe.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wap.fehbvm.com/Article/details/gvnixpqab.sHtML


<!-- 参考信息 -->