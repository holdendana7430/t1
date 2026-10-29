代发 wailian999

JS:   super.greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gjvdcgerf.sHtML

TS:   super.greet();
来源：http://wap.zdbjq.cn/Article/details/gbshofvrk.sHtML

Java: super.greet();
来源：http://www.blog.hesvh.cn/Article/details/griiwaovz.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.zdbjq.cn/Article/details/gbufxnvee.sHtML

Ruby: super
来源：http://m.share.hesvh.cn/Article/details/gxqgytywu.sHtML

C#:   base.Greet();
来源：http://www.blog.hesvh.cn/Article/details/gtohzbcnw.sHtML

[G08] 静态方法与属性
来源：http://m.share.hesvh.cn/Article/details/ghbhlsyvq.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.zdbjq.cn/Article/details/gugjssbfn.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.zdbjq.cn/Article/details/gppuvialn.sHtML

JS:   static f() {}
来源：http://www.m.share.zdbjq.cn/Article/details/gohbzxrwf.sHtML

TS:   static f(): void {}
来源：http://m.share.fehbvm.com/Article/details/gbqavaqgo.sHtML

Java: static void f() {}
来源：http://blog.zdbjq.cn/Article/details/gjiqksdeq.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.zdbjq.cn/Article/details/gyflbnlvx.sHtML

Ruby: def self.f; end
来源：http://www.blog.fehbvm.com/Article/details/gpmlbafqz.sHtML

C#:   public static void F() {}
来源：http://www.blog.zdbjq.cn/Article/details/gqbbjkqpp.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.fehbvm.com/Article/details/gbickpand.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.zdbjq.cn/Article/details/gcpbdvekk.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.fehbvm.com/Article/details/gztxbrtsv.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.zdbjq.cn/Article/details/gahwnizxo.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.zdbjq.cn/Article/details/gfuklosnc.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.fehbvm.com/Article/details/ghcdttjzb.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.hesvh.cn/Article/details/grxadthrt.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.fehbvm.com/Article/details/gpxronzbq.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.hesvh.cn/Article/details/gjvlytsdy.sHtML

[G10] 访问控制
来源：http://wap.fehbvm.com/Article/details/gvuihmbtz.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.fehbvm.com/Article/details/gaykbxded.sHtML

PHP:  public / protected / private
来源：http://www.share.hesvh.cn/Article/details/gzdrjhtzp.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.hesvh.cn/Article/details/guikqzvhl.sHtML

TS:   public / protected / private
来源：http://blog.fehbvm.com/Article/details/gobjdhmne.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.zdbjq.cn/Article/details/gaxyxkmhn.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.zdbjq.cn/Article/details/givjxiygo.sHtML

Ruby: public / protected / private
来源：http://m.share.zdbjq.cn/Article/details/gxkiocwcj.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.fehbvm.com/Article/details/gurajdfwo.sHtML

[G11] getter / setter
来源：http://read.share.zdbjq.cn/Article/details/gavzarwje.sHtML

Py:   @property 与 @x.setter
来源：http://baike.fehbvm.com/Article/details/gfjqbbicm.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.fehbvm.com/Article/details/gdtrcvxjd.sHtML

JS:   get name() { return this._name; }
来源：http://baike.zdbjq.cn/Article/details/gpwgwzpbp.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.hesvh.cn/Article/details/gwgdgcqnp.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.fehbvm.com/Article/details/gjtojphek.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.zdbjq.cn/Article/details/gljaolzti.sHtML

Ruby: attr_accessor :name
来源：http://blog.fehbvm.com/Article/details/gnzqgelzz.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.fehbvm.com/Article/details/gapgdclxj.sHtML

[G12] 对象转字符串
来源：http://m.share.zdbjq.cn/Article/details/ghrowqxmt.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.zdbjq.cn/Article/details/ghyrbhnxw.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.fehbvm.com/Article/details/gtnvzzijn.sHtML

JS:   toString() { return this.name; }
来源：http://blog.hesvh.cn/Article/details/ghdeonhwl.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/gexmvsxvi.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.hesvh.cn/Article/details/ghwjekuze.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.fehbvm.com/Article/details/gsapvfmad.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.fehbvm.com/Article/details/gdsxlilhu.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.fehbvm.com/Article/details/gmufgvguv.sHtML

[G13] 判断对象类型
来源：http://baike.hesvh.cn/Article/details/gwraarorz.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.fehbvm.com/Article/details/gqcovhjaa.sHtML

PHP:  $u instanceof User
来源：http://read.share.hesvh.cn/Article/details/gyiuwwymv.sHtML

JS:   u instanceof User
来源：http://3g.fehbvm.com/Article/details/gbwchtrhn.sHtML

TS:   u instanceof User
来源：http://m.share.fehbvm.com/Article/details/gzfsnykks.sHtML

Java: u instanceof User
来源：http://3g.fehbvm.com/Article/details/gucgdmxsi.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.fehbvm.com/Article/details/gkbxsjsly.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.zdbjq.cn/Article/details/gdvojfpgz.sHtML

C#:   u is User
来源：http://baike.fehbvm.com/Article/details/gswwcqgbc.sHtML

[G14] 数据类 / record
来源：http://www.blog.fehbvm.com/Article/details/gumusbmsm.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.hesvh.cn/Article/details/gxwvwfsxe.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://read.share.zdbjq.cn/Article/details/gsrxhlerc.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.hesvh.cn/Article/details/gbclvdenb.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.fehbvm.com/Article/details/gghpvfgyu.sHtML

Java: record User(String name, int age) {}
来源：http://wap.fehbvm.com/Article/details/gradudlzw.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.fehbvm.com/Article/details/gqveeltic.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.fehbvm.com/Article/details/ggyjgxgxe.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.hesvh.cn/Article/details/gaskuaxtp.sHtML

[G15] 枚举
来源：http://www.m.share.zdbjq.cn/Article/details/gnurklucn.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.hesvh.cn/Article/details/gxxruzdsx.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.hesvh.cn/Article/details/gxottdczj.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mobile.fehbvm.com/Article/details/gleiklzeu.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.fehbvm.com/Article/details/gohtfwhiw.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.fehbvm.com/Article/details/gonvsetrr.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.zdbjq.cn/Article/details/geuhdiecw.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.hesvh.cn/Article/details/goqegqeel.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.hesvh.cn/Article/details/gneznszmp.sHtML

[G16] 对象转数组 / 字典
来源：http://m.share.hesvh.cn/Article/details/getpimgvp.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.fehbvm.com/Article/details/gvxclpoyf.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.fehbvm.com/Article/details/gnobjpehu.sHtML

JS:   Object.entries(obj)
来源：http://www.share.hesvh.cn/Article/details/gthrazdnz.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gfrqewjlp.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.hesvh.cn/Article/details/gjkkxcmac.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.zdbjq.cn/Article/details/gigkydrfw.sHtML

Ruby: obj.instance_variables
来源：http://baike.fehbvm.com/Article/details/gzyznixli.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://blog.hesvh.cn/Article/details/gkinydgvr.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gtffzvxmv.sHtML

H. 异常与错误处理
来源：http://www.m.share.fehbvm.com/Article/details/guhoqjvfk.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gaorxprje.sHtML

[H01] try / catch 基础
来源：http://3g.zdbjq.cn/Article/details/geoyezpzu.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://read.share.hesvh.cn/Article/details/girujgjad.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mobile.fehbvm.com/Article/details/ggfcwltew.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.zdbjq.cn/Article/details/gsqytjwdr.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.share.zdbjq.cn/Article/details/giurbsagt.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.zdbjq.cn/Article/details/gszbhnpxe.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://blog.zdbjq.cn/Article/details/greqakrse.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.zdbjq.cn/Article/details/gasnhsqud.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.zdbjq.cn/Article/details/gbndxfvjr.sHtML

[H02] finally / ensure 收尾
来源：http://wap.fehbvm.com/Article/details/gvbaxfmxp.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.zdbjq.cn/Article/details/gmgspzkrd.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/gzvvmlcas.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://m.share.hesvh.cn/Article/details/gcupdiyey.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.hesvh.cn/Article/details/gkbahqevv.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.zdbjq.cn/Article/details/gzemzewmh.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.fehbvm.com/Article/details/gxwamahqh.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.blog.hesvh.cn/Article/details/gwlpammdb.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.blog.zdbjq.cn/Article/details/gectiewvk.sHtML

[H03] 主动抛出异常
来源：http://blog.hesvh.cn/Article/details/ggfopbqrc.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.fehbvm.com/Article/details/gjatnirfo.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.m.share.zdbjq.cn/Article/details/gbljymbng.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.hesvh.cn/Article/details/glnvbozef.sHtML

TS:   throw new Error("错误信息");
来源：http://blog.zdbjq.cn/Article/details/gfyjjiqtw.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.zdbjq.cn/Article/details/gkpctltvr.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mobile.zdbjq.cn/Article/details/gccycehau.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://baike.fehbvm.com/Article/details/ggvvofgqb.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.zdbjq.cn/Article/details/gdctflnls.sHtML

[H04] 自定义异常类型
来源：http://mobile.hesvh.cn/Article/details/gauimdlct.sHtML

Py:   class MyError(Exception): pass
来源：http://blog.zdbjq.cn/Article/details/gzxxtchua.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://blog.zdbjq.cn/Article/details/gzqxzwksj.sHtML

JS:   class MyError extends Error {}
来源：http://3g.hesvh.cn/Article/details/gnxlnexvx.sHtML

TS:   class MyError extends Error {}
来源：http://www.share.zdbjq.cn/Article/details/gxxyjtalo.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.fehbvm.com/Article/details/gdugilwee.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://read.share.fehbvm.com/Article/details/gorbqvwau.sHtML

Ruby: class MyError < StandardError; end
来源：http://read.share.zdbjq.cn/Article/details/gwxqtnpzv.sHtML

C#:   class MyException : Exception {}
来源：http://baike.zdbjq.cn/Article/details/gxzdvknvp.sHtML

[H05] 捕获特定类型
来源：http://m.share.zdbjq.cn/Article/details/gldlfxvoh.sHtML

Py:   except ValueError as e:
来源：http://mobile.hesvh.cn/Article/details/gtzmftznr.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.m.share.fehbvm.com/Article/details/gsrjcmvpy.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://3g.zdbjq.cn/Article/details/gxuyfoqtl.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.m.share.fehbvm.com/Article/details/gyjbernxa.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://m.share.zdbjq.cn/Article/details/glqtbrkbr.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wap.fehbvm.com/Article/details/gdwuhuxes.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.share.fehbvm.com/Article/details/gespogwwi.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.share.zdbjq.cn/Article/details/gfhanibay.sHtML

[H06] 可选值 / 空值安全访问
来源：http://read.share.zdbjq.cn/Article/details/gllkjfjwk.sHtML

Py:   value = d.get("k") or default
来源：http://3g.hesvh.cn/Article/details/geyeufwmr.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.hesvh.cn/Article/details/gzaviiupe.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://blog.zdbjq.cn/Article/details/gpspillwy.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.share.hesvh.cn/Article/details/gawdzhiyx.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://m.share.zdbjq.cn/Article/details/gokjicgfy.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://read.share.zdbjq.cn/Article/details/gfrbujagv.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.m.share.hesvh.cn/Article/details/gtsynhkze.sHtML

C#:   obj?.A?.B ?? default
来源：http://3g.fehbvm.com/Article/details/gotkopvqw.sHtML

[H07] 断言
来源：http://3g.zdbjq.cn/Article/details/guzpcgfjf.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.m.share.hesvh.cn/Article/details/grgnoljwn.sHtML

PHP:  assert($x > 0);
来源：http://read.share.zdbjq.cn/Article/details/glvotrbdt.sHtML

JS:   console.assert(x > 0);
来源：http://www.share.fehbvm.com/Article/details/gwkxsudrh.sHtML

TS:   console.assert(x > 0);
来源：http://read.share.zdbjq.cn/Article/details/gpizhmsxo.sHtML

Java: assert x > 0 : "必须为正";
来源：http://wap.hesvh.cn/Article/details/gjzmospqx.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.blog.hesvh.cn/Article/details/gkohyvbcc.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://3g.zdbjq.cn/Article/details/gsckqkqtp.sHtML

C#:   Debug.Assert(x > 0);
来源：http://wap.hesvh.cn/Article/details/gatcczunn.sHtML

[H08] 获取错误信息与堆栈
来源：http://read.share.hesvh.cn/Article/details/grnxcopsn.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://3g.zdbjq.cn/Article/details/gkzmkntam.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://baike.fehbvm.com/Article/details/gztatjzte.sHtML

JS:   e.message;  e.stack
来源：http://blog.fehbvm.com/Article/details/ghtcuyvdp.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://read.share.zdbjq.cn/Article/details/gnqkhgfxf.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://blog.zdbjq.cn/Article/details/gfuzpwnii.sHtML

Go:   err.Error()
来源：http://www.m.share.fehbvm.com/Article/details/gghkdehgy.sHtML

Ruby: e.message;  e.backtrace
来源：http://mobile.hesvh.cn/Article/details/gqyrlvlpb.sHtML

C#:   e.Message;  e.StackTrace
来源：http://baike.hesvh.cn/Article/details/guetvnsvg.sHtML

[H09] 带错误码的异常
来源：http://www.m.share.fehbvm.com/Article/details/givtjqvgz.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.share.hesvh.cn/Article/details/gqkarutvz.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.m.share.fehbvm.com/Article/details/gdqgloqfb.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://m.share.zdbjq.cn/Article/details/gurtnknsu.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.m.share.zdbjq.cn/Article/details/goseuzxso.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://blog.fehbvm.com/Article/details/gpuhhfqyj.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://m.share.zdbjq.cn/Article/details/gqugtyxxr.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://m.share.fehbvm.com/Article/details/gzhpeoyge.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://read.share.fehbvm.com/Article/details/gskmazzog.sHtML

[H10] 资源自动释放
来源：http://www.m.share.hesvh.cn/Article/details/gimuubgho.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://baike.hesvh.cn/Article/details/gzaoxpwtr.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wap.zdbjq.cn/Article/details/gvvoltptz.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.zdbjq.cn/Article/details/gbxhnizhs.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.fehbvm.com/Article/details/gatllucqm.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.blog.fehbvm.com/Article/details/gisbsdypt.sHtML

Go:   defer f.Close()
来源：http://m.share.zdbjq.cn/Article/details/gybpjtoiw.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://read.share.fehbvm.com/Article/details/gunrvawkc.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gnrxteukj.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gewakgaov.sHtML

I. 正则表达式
来源：http://wap.fehbvm.com/Article/details/gbjgvkenq.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gwvivnofh.sHtML

[I01] 判断是否匹配
来源：http://baike.fehbvm.com/Article/details/gediftqbu.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://blog.zdbjq.cn/Article/details/gamkshejz.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://wap.fehbvm.com/Article/details/ggpllqhnv.sHtML

JS:   /\d+/.test(s)
来源：http://3g.fehbvm.com/Article/details/gzmozjezo.sHtML

TS:   /\d+/.test(s)
来源：http://mobile.hesvh.cn/Article/details/glwmgwdlk.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.blog.zdbjq.cn/Article/details/gmkadgsxw.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://baike.fehbvm.com/Article/details/gfkymlzbb.sHtML

Ruby: s.match?(/\d+/)
来源：http://m.share.hesvh.cn/Article/details/gkbchwqsx.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wap.fehbvm.com/Article/details/gwpjwdryl.sHtML

[I02] 提取所有匹配
来源：http://read.share.fehbvm.com/Article/details/gkeowxuyd.sHtML

Py:   re.findall(r"\d+", s)
来源：http://baike.hesvh.cn/Article/details/gctymhrcb.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wap.fehbvm.com/Article/details/gccfzgvsf.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.share.fehbvm.com/Article/details/gmhjgcqwo.sHtML

TS:   s.match(/\d+/g)
来源：http://www.m.share.hesvh.cn/Article/details/gnbjruray.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://m.share.zdbjq.cn/Article/details/gwqgqugub.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://m.share.fehbvm.com/Article/details/gpprlqxjk.sHtML

Ruby: s.scan(/\d+/)
来源：http://mobile.zdbjq.cn/Article/details/ghinjjvps.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://blog.hesvh.cn/Article/details/gcxelayiv.sHtML

[I03] 提取捕获分组
来源：http://read.share.hesvh.cn/Article/details/glifjaxjb.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.m.share.zdbjq.cn/Article/details/graopcahm.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wap.fehbvm.com/Article/details/gyrjrspng.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.m.share.fehbvm.com/Article/details/gulwxzwhf.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wap.zdbjq.cn/Article/details/gvpxijzcq.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.share.fehbvm.com/Article/details/glsvlqugs.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://baike.hesvh.cn/Article/details/gwqywlzic.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://3g.zdbjq.cn/Article/details/gclxwgafz.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://read.share.fehbvm.com/Article/details/gwinittbp.sHtML

[I04] 正则替换
来源：http://mobile.fehbvm.com/Article/details/glafbybbf.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://m.share.hesvh.cn/Article/details/gupmbswvf.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://blog.hesvh.cn/Article/details/gznvpzrpg.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.hesvh.cn/Article/details/gsfukjnnr.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://wap.hesvh.cn/Article/details/giqrqqhrp.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.blog.fehbvm.com/Article/details/gndnqfofx.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://read.share.hesvh.cn/Article/details/gtzkzozgd.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://blog.zdbjq.cn/Article/details/gszetmcvq.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.share.zdbjq.cn/Article/details/gripisrgi.sHtML

[I05] 按正则拆分
来源：http://www.blog.hesvh.cn/Article/details/gliiqkmja.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://3g.hesvh.cn/Article/details/gnjfgwxqf.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.blog.hesvh.cn/Article/details/gyfcpmhpt.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://baike.hesvh.cn/Article/details/gilxkqrws.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://baike.hesvh.cn/Article/details/guxhmgsit.sHtML

Java: s.split("\\s*,\\s*")
来源：http://m.share.hesvh.cn/Article/details/gojzysasj.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://m.share.fehbvm.com/Article/details/guvhmrnoq.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://wap.fehbvm.com/Article/details/gzdkaullh.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mobile.hesvh.cn/Article/details/gpeipbshs.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.blog.zdbjq.cn/Article/details/ghwxryngz.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.m.share.fehbvm.com/Article/details/ggstbediz.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://m.share.zdbjq.cn/Article/details/gtolgokic.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.fehbvm.com/Article/details/gqvnxzwdt.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.zdbjq.cn/Article/details/gechjvuxq.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mobile.hesvh.cn/Article/details/gunkrkhmz.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.blog.fehbvm.com/Article/details/ggimigmbw.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://blog.hesvh.cn/Article/details/gidwfypbu.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://m.share.fehbvm.com/Article/details/gmmmgorby.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.m.share.hesvh.cn/Article/details/gdyqmkpdm.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.m.share.zdbjq.cn/Article/details/gbcaotayy.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://baike.zdbjq.cn/Article/details/glmdzahrh.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://blog.fehbvm.com/Article/details/gmjawfixe.sHtML

TS:   /error/gim
来源：http://baike.hesvh.cn/Article/details/ggprvmgty.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.share.fehbvm.com/Article/details/grucmihzg.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.share.fehbvm.com/Article/details/ghsoujzbk.sHtML

Ruby: s.scan(/error/i)
来源：http://www.blog.hesvh.cn/Article/details/gepdgshug.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://blog.hesvh.cn/Article/details/gpdhkiqwl.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://mobile.zdbjq.cn/Article/details/gntxdoypv.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://read.share.zdbjq.cn/Article/details/gbdpywkuq.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://m.share.fehbvm.com/Article/details/giybmpmcn.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.hesvh.cn/Article/details/gvytufzcm.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.zdbjq.cn/Article/details/ghgnktowr.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://baike.hesvh.cn/Article/details/gmddabehs.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://mobile.hesvh.cn/Article/details/gzbuqrjyo.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.m.share.hesvh.cn/Article/details/gbkbdwvbp.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://3g.fehbvm.com/Article/details/gqwqysvfc.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/ggrccfdst.sHtML

J. 日期与时间
来源：http://www.share.fehbvm.com/Article/details/gyechhdpm.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gfbyobhmv.sHtML

[J01] 获取当前时间
来源：http://m.share.fehbvm.com/Article/details/gkjxtxals.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.blog.zdbjq.cn/Article/details/galsvmvre.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.blog.fehbvm.com/Article/details/gjhpfonsu.sHtML

JS:   new Date();  Date.now()
来源：http://3g.zdbjq.cn/Article/details/gquemobni.sHtML

TS:   new Date();  Date.now()
来源：http://www.m.share.zdbjq.cn/Article/details/gyaledqcn.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://read.share.hesvh.cn/Article/details/gfsasrlkj.sHtML

Go:   time.Now()
来源：http://wap.zdbjq.cn/Article/details/gbljzzhib.sHtML

Ruby: Time.now
来源：http://www.m.share.hesvh.cn/Article/details/gnmcmnmep.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://mobile.fehbvm.com/Article/details/grlchmvgn.sHtML

[J02] 格式化输出
来源：http://read.share.hesvh.cn/Article/details/gvyuayhaw.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.zdbjq.cn/Article/details/gyemxwjjh.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://baike.fehbvm.com/Article/details/gpkgagawc.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://read.share.fehbvm.com/Article/details/gldxfcvoc.sHtML

TS:   d.toISOString()
来源：http://mobile.zdbjq.cn/Article/details/grxexggua.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://m.share.zdbjq.cn/Article/details/gywuevbtx.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://blog.hesvh.cn/Article/details/gxjehkviw.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.fehbvm.com/Article/details/gipmangzn.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.m.share.zdbjq.cn/Article/details/gtuiigusa.sHtML

[J03] 字符串解析为日期
来源：http://mobile.hesvh.cn/Article/details/gbxxjknkg.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://3g.hesvh.cn/Article/details/gyrtcytvk.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wap.fehbvm.com/Article/details/gkfwbbdmq.sHtML

JS:   new Date("2024-01-02")
来源：http://www.share.zdbjq.cn/Article/details/gdbghkqai.sHtML

TS:   new Date("2024-01-02")
来源：http://m.share.hesvh.cn/Article/details/ghmbzgrsv.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://blog.zdbjq.cn/Article/details/gyotrdzwi.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.blog.hesvh.cn/Article/details/gfjvzjvia.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.m.share.hesvh.cn/Article/details/gxeapckcd.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://blog.zdbjq.cn/Article/details/gdtjmgjai.sHtML

[J04] 时间戳与日期互转
来源：http://www.m.share.zdbjq.cn/Article/details/gyieogeso.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.m.share.fehbvm.com/Article/details/gbtztrweb.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://baike.fehbvm.com/Article/details/gymraqnpv.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://3g.hesvh.cn/Article/details/gggtjowpr.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://3g.fehbvm.com/Article/details/gffwsajhb.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://read.share.zdbjq.cn/Article/details/gxugbadqv.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/grufjmmgr.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.blog.fehbvm.com/Article/details/gexxptqfx.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://read.share.hesvh.cn/Article/details/gnywlnltq.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.share.zdbjq.cn/Article/details/gvlmqudwh.sHtML

Py:   now + timedelta(days=7)
来源：http://m.share.hesvh.cn/Article/details/gzzojrhvv.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://mobile.hesvh.cn/Article/details/gqkpdtkxs.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.zdbjq.cn/Article/details/gbscoxngg.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.zdbjq.cn/Article/details/glkktspkh.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://baike.hesvh.cn/Article/details/gjdwxtdxe.sHtML


<!-- 参考信息 -->