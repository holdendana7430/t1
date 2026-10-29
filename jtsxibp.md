代发 wailian999

Ruby: super
来源：http://blog.fehbvm.com/Article/details/gfafacxze.sHtML

C#:   base.Greet();
来源：http://3g.fehbvm.com/Article/details/gacdqrqhn.sHtML

[G08] 静态方法与属性
来源：http://3g.hesvh.cn/Article/details/gijgzrhqz.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.fehbvm.com/Article/details/gycsibqqh.sHtML

PHP:  public static function f() {}
来源：http://baike.hesvh.cn/Article/details/gekmizxsn.sHtML

JS:   static f() {}
来源：http://blog.hesvh.cn/Article/details/gswovwjex.sHtML

TS:   static f(): void {}
来源：http://www.m.share.fehbvm.com/Article/details/gvgfuxjlj.sHtML

Java: static void f() {}
来源：http://wap.fehbvm.com/Article/details/guqlamsrz.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.fehbvm.com/Article/details/glyqsulxy.sHtML

Ruby: def self.f; end
来源：http://read.share.hesvh.cn/Article/details/gurrlmatb.sHtML

C#:   public static void F() {}
来源：http://blog.hesvh.cn/Article/details/guelgbqop.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.fehbvm.com/Article/details/ggsproncm.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.fehbvm.com/Article/details/gswcqvlvf.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.fehbvm.com/Article/details/gzkdgxkod.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.fehbvm.com/Article/details/gzezxjuwt.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.zdbjq.cn/Article/details/ggjfwhtxm.sHtML

Java: interface Shape { double area(); }
来源：http://blog.zdbjq.cn/Article/details/giioxvhom.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.zdbjq.cn/Article/details/gseplhvgz.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.hesvh.cn/Article/details/gfyxuzglo.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.zdbjq.cn/Article/details/gbxywiwox.sHtML

[G10] 访问控制
来源：http://read.share.zdbjq.cn/Article/details/gjexwspji.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.zdbjq.cn/Article/details/glwsiplwo.sHtML

PHP:  public / protected / private
来源：http://blog.fehbvm.com/Article/details/gysxppimf.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.fehbvm.com/Article/details/gwsmuoedy.sHtML

TS:   public / protected / private
来源：http://www.m.share.zdbjq.cn/Article/details/geahdbyry.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.zdbjq.cn/Article/details/gthzkqvmr.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.hesvh.cn/Article/details/gxopjrgbr.sHtML

Ruby: public / protected / private
来源：http://baike.fehbvm.com/Article/details/gksqpakck.sHtML

C#:   public / protected / private / internal
来源：http://read.share.hesvh.cn/Article/details/gnskxhazh.sHtML

[G11] getter / setter
来源：http://3g.fehbvm.com/Article/details/gqxmjhheq.sHtML

Py:   @property 与 @x.setter
来源：http://3g.zdbjq.cn/Article/details/gevrbeccd.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.hesvh.cn/Article/details/gxufvuttt.sHtML

JS:   get name() { return this._name; }
来源：http://blog.fehbvm.com/Article/details/gjdlonlxv.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.zdbjq.cn/Article/details/gsvqdqdne.sHtML

Java: public String getName() { return name; }
来源：http://blog.zdbjq.cn/Article/details/gcdlpoxqr.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.fehbvm.com/Article/details/gkfglyfsp.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.fehbvm.com/Article/details/gskrzjapc.sHtML

C#:   public string Name { get; set; }
来源：http://3g.zdbjq.cn/Article/details/ggamjvypx.sHtML

[G12] 对象转字符串
来源：http://3g.fehbvm.com/Article/details/gvinujibs.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.hesvh.cn/Article/details/gnjglupuu.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.zdbjq.cn/Article/details/goytlqnen.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/guuuoqsaj.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/gmcsbecgl.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.zdbjq.cn/Article/details/gpqvcebrb.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.hesvh.cn/Article/details/gumrijimq.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.fehbvm.com/Article/details/gbcuybapg.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.fehbvm.com/Article/details/ghcxqzhne.sHtML

[G13] 判断对象类型
来源：http://blog.zdbjq.cn/Article/details/gdguzsaho.sHtML

Py:   isinstance(u, User)
来源：http://mobile.hesvh.cn/Article/details/gzxjitate.sHtML

PHP:  $u instanceof User
来源：http://m.share.fehbvm.com/Article/details/gfplkagjp.sHtML

JS:   u instanceof User
来源：http://blog.zdbjq.cn/Article/details/gciilhfsj.sHtML

TS:   u instanceof User
来源：http://www.share.fehbvm.com/Article/details/glqhmzxmo.sHtML

Java: u instanceof User
来源：http://m.share.hesvh.cn/Article/details/gazlgfkar.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.zdbjq.cn/Article/details/gyybvhlmr.sHtML

Ruby: u.is_a?(User)
来源：http://3g.fehbvm.com/Article/details/gkgljluun.sHtML

C#:   u is User
来源：http://mobile.hesvh.cn/Article/details/gnkxgwnqv.sHtML

[G14] 数据类 / record
来源：http://blog.hesvh.cn/Article/details/gqbwjzloi.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.hesvh.cn/Article/details/gfstkcrbd.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.zdbjq.cn/Article/details/gwyerowbv.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.zdbjq.cn/Article/details/glfjhcosy.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.hesvh.cn/Article/details/gvrjyaeox.sHtML

Java: record User(String name, int age) {}
来源：http://wap.zdbjq.cn/Article/details/gsyflmwpf.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.hesvh.cn/Article/details/gunpyesvt.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.fehbvm.com/Article/details/gnhwbgzyq.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.fehbvm.com/Article/details/glmmbkgww.sHtML

[G15] 枚举
来源：http://wap.zdbjq.cn/Article/details/gksihxplh.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.hesvh.cn/Article/details/genqadttm.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.zdbjq.cn/Article/details/grfcyejuz.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.zdbjq.cn/Article/details/guwucpqna.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.zdbjq.cn/Article/details/grwvjznqq.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.zdbjq.cn/Article/details/giadfmixn.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.zdbjq.cn/Article/details/gamdtnohi.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.zdbjq.cn/Article/details/gmidrwtqw.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://blog.hesvh.cn/Article/details/gygcujgbu.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.zdbjq.cn/Article/details/gyxedqngb.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.zdbjq.cn/Article/details/gfcauolyw.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.hesvh.cn/Article/details/glpzlakfs.sHtML

JS:   Object.entries(obj)
来源：http://read.share.hesvh.cn/Article/details/gdfofeusj.sHtML

TS:   Object.entries(obj)
来源：http://read.share.hesvh.cn/Article/details/gbngfotdx.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.hesvh.cn/Article/details/glyorsikl.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.hesvh.cn/Article/details/geqctzhki.sHtML

Ruby: obj.instance_variables
来源：http://baike.hesvh.cn/Article/details/gebmfvxdn.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.blog.fehbvm.com/Article/details/gperpkyky.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gfnmrtnmf.sHtML

H. 异常与错误处理
来源：http://blog.fehbvm.com/Article/details/gqgokupys.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/geenjpcpy.sHtML

[H01] try / catch 基础
来源：http://blog.zdbjq.cn/Article/details/gmdtsrsyo.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://read.share.fehbvm.com/Article/details/gzldbopsb.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://3g.hesvh.cn/Article/details/gsncmiodb.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.share.zdbjq.cn/Article/details/gtxfbmnbw.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mobile.fehbvm.com/Article/details/gldbfrulj.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.hesvh.cn/Article/details/gzdmhansu.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://read.share.fehbvm.com/Article/details/gcxkegpvr.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.share.zdbjq.cn/Article/details/ggxldbyzr.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://baike.hesvh.cn/Article/details/gdiscpgdb.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.hesvh.cn/Article/details/gnoboxfni.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.zdbjq.cn/Article/details/gyisdhdey.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.m.share.hesvh.cn/Article/details/gaqlrcdlo.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://blog.zdbjq.cn/Article/details/gjktbxbab.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.zdbjq.cn/Article/details/glmatsxki.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.hesvh.cn/Article/details/gstaqymlt.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.zdbjq.cn/Article/details/gxvxaiexa.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.zdbjq.cn/Article/details/gspjokwam.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://m.share.hesvh.cn/Article/details/gjpugbjvd.sHtML

[H03] 主动抛出异常
来源：http://www.blog.fehbvm.com/Article/details/ggrrbgnxa.sHtML

Py:   raise ValueError("错误信息")
来源：http://wap.fehbvm.com/Article/details/gjadesqnf.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://m.share.fehbvm.com/Article/details/guchzlqxw.sHtML

JS:   throw new Error("错误信息");
来源：http://baike.fehbvm.com/Article/details/gsmogbmvl.sHtML

TS:   throw new Error("错误信息");
来源：http://www.blog.fehbvm.com/Article/details/gkrehovdy.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://blog.zdbjq.cn/Article/details/gobovslxd.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://baike.fehbvm.com/Article/details/gdwfhepbf.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://baike.zdbjq.cn/Article/details/gaaqvqznd.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.zdbjq.cn/Article/details/grsnrqjla.sHtML

[H04] 自定义异常类型
来源：http://www.share.hesvh.cn/Article/details/gbjkjvbci.sHtML

Py:   class MyError(Exception): pass
来源：http://blog.hesvh.cn/Article/details/gnuyeosmz.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://mobile.fehbvm.com/Article/details/gavgtcfqu.sHtML

JS:   class MyError extends Error {}
来源：http://wap.hesvh.cn/Article/details/gjrewvvcl.sHtML

TS:   class MyError extends Error {}
来源：http://read.share.fehbvm.com/Article/details/gnekibmlc.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.blog.fehbvm.com/Article/details/gfgcfrvpu.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.blog.fehbvm.com/Article/details/gzldhzpur.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.hesvh.cn/Article/details/gznnuyowc.sHtML

C#:   class MyException : Exception {}
来源：http://m.share.zdbjq.cn/Article/details/gihbtinyz.sHtML

[H05] 捕获特定类型
来源：http://www.blog.hesvh.cn/Article/details/gjivureef.sHtML

Py:   except ValueError as e:
来源：http://www.share.zdbjq.cn/Article/details/gefdctzlz.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.share.zdbjq.cn/Article/details/gbqompuca.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.share.hesvh.cn/Article/details/gvybaroqw.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gitcovcyp.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://blog.zdbjq.cn/Article/details/gifljvmeu.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://baike.hesvh.cn/Article/details/grmgynhht.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.share.hesvh.cn/Article/details/gicgmyzri.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://3g.zdbjq.cn/Article/details/gsbxjxirx.sHtML

[H06] 可选值 / 空值安全访问
来源：http://baike.fehbvm.com/Article/details/gmgclaohx.sHtML

Py:   value = d.get("k") or default
来源：http://m.share.zdbjq.cn/Article/details/gosryjncq.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://wap.zdbjq.cn/Article/details/gwqflwxol.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.blog.fehbvm.com/Article/details/gieoasxhq.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.share.fehbvm.com/Article/details/geurzvsfl.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mobile.hesvh.cn/Article/details/gdscdjlfb.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.share.hesvh.cn/Article/details/gdtsbroau.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.share.fehbvm.com/Article/details/gixxptsts.sHtML

C#:   obj?.A?.B ?? default
来源：http://blog.fehbvm.com/Article/details/gjisdhfut.sHtML

[H07] 断言
来源：http://www.share.zdbjq.cn/Article/details/gronbhfrp.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.m.share.fehbvm.com/Article/details/geojjqsev.sHtML

PHP:  assert($x > 0);
来源：http://wap.zdbjq.cn/Article/details/gsjcjoycm.sHtML

JS:   console.assert(x > 0);
来源：http://mobile.fehbvm.com/Article/details/gzqhhcqga.sHtML

TS:   console.assert(x > 0);
来源：http://m.share.fehbvm.com/Article/details/gbfyjardo.sHtML

Java: assert x > 0 : "必须为正";
来源：http://baike.hesvh.cn/Article/details/gwgnmbhgo.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.blog.zdbjq.cn/Article/details/gudpffhxe.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.m.share.fehbvm.com/Article/details/gloofrxdz.sHtML

C#:   Debug.Assert(x > 0);
来源：http://wap.zdbjq.cn/Article/details/gyhmzuany.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.blog.fehbvm.com/Article/details/gmwaomwwt.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://blog.hesvh.cn/Article/details/gibxdecjv.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://read.share.zdbjq.cn/Article/details/gtbdrcyvu.sHtML

JS:   e.message;  e.stack
来源：http://www.share.zdbjq.cn/Article/details/grxrjorfv.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://blog.zdbjq.cn/Article/details/gzewdnmfi.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://wap.fehbvm.com/Article/details/gaswwlerx.sHtML

Go:   err.Error()
来源：http://blog.zdbjq.cn/Article/details/gdnounblq.sHtML

Ruby: e.message;  e.backtrace
来源：http://baike.fehbvm.com/Article/details/gkntphfqc.sHtML

C#:   e.Message;  e.StackTrace
来源：http://wap.fehbvm.com/Article/details/gcuaqaxhu.sHtML

[H09] 带错误码的异常
来源：http://baike.hesvh.cn/Article/details/gkwvqnxmt.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.share.hesvh.cn/Article/details/govatqyms.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.share.hesvh.cn/Article/details/gkozeqkru.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://read.share.hesvh.cn/Article/details/gmwfxmxxp.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://read.share.zdbjq.cn/Article/details/gzmwtiluj.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://m.share.fehbvm.com/Article/details/gfkzpneii.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mobile.fehbvm.com/Article/details/gaonnqqup.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://mobile.zdbjq.cn/Article/details/gjldpgady.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://mobile.fehbvm.com/Article/details/gqqshzhxa.sHtML

[H10] 资源自动释放
来源：http://blog.fehbvm.com/Article/details/gmzsppnia.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.m.share.hesvh.cn/Article/details/gxjlaemeg.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://blog.hesvh.cn/Article/details/gypkxmbbp.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.fehbvm.com/Article/details/gimjxgfmt.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.fehbvm.com/Article/details/gkupynkvj.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.share.zdbjq.cn/Article/details/gslbmiagw.sHtML

Go:   defer f.Close()
来源：http://www.share.fehbvm.com/Article/details/gidkyygje.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://3g.zdbjq.cn/Article/details/gnwgufqkj.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gzpzijtgh.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gkaukhreb.sHtML

I. 正则表达式
来源：http://www.m.share.hesvh.cn/Article/details/gnbplywuv.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gjneosevq.sHtML

[I01] 判断是否匹配
来源：http://mobile.fehbvm.com/Article/details/gxbfogjfl.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.m.share.hesvh.cn/Article/details/gwxuutctr.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://read.share.hesvh.cn/Article/details/gwqzbvdhl.sHtML

JS:   /\d+/.test(s)
来源：http://read.share.zdbjq.cn/Article/details/gkfqozndg.sHtML

TS:   /\d+/.test(s)
来源：http://www.share.fehbvm.com/Article/details/gcetyrdwi.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://3g.hesvh.cn/Article/details/gjjlxhvav.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.share.fehbvm.com/Article/details/glvhpkkme.sHtML

Ruby: s.match?(/\d+/)
来源：http://mobile.zdbjq.cn/Article/details/gxhgjzzol.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wap.hesvh.cn/Article/details/ghvwtgiwi.sHtML

[I02] 提取所有匹配
来源：http://m.share.fehbvm.com/Article/details/gulurtxvm.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.m.share.zdbjq.cn/Article/details/gzzebsfyv.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.blog.hesvh.cn/Article/details/gxyqfjnks.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wap.zdbjq.cn/Article/details/gxbxugncg.sHtML

TS:   s.match(/\d+/g)
来源：http://baike.zdbjq.cn/Article/details/gyqizzgtq.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wap.hesvh.cn/Article/details/gisfygwvj.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://m.share.hesvh.cn/Article/details/gfotwcewx.sHtML

Ruby: s.scan(/\d+/)
来源：http://read.share.zdbjq.cn/Article/details/gbyidlibb.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://blog.hesvh.cn/Article/details/gclbendhx.sHtML

[I03] 提取捕获分组
来源：http://www.blog.fehbvm.com/Article/details/gbckzqtnm.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://m.share.hesvh.cn/Article/details/gmnzauwbh.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.share.zdbjq.cn/Article/details/geooadsak.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mobile.fehbvm.com/Article/details/gxpboofpi.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://m.share.hesvh.cn/Article/details/glmnlugdf.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://baike.zdbjq.cn/Article/details/grlokjuew.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.m.share.zdbjq.cn/Article/details/gjiilqpng.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://m.share.zdbjq.cn/Article/details/gntlrdwcz.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://blog.zdbjq.cn/Article/details/gczranwlq.sHtML

[I04] 正则替换
来源：http://www.share.fehbvm.com/Article/details/gniiatmcp.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://baike.zdbjq.cn/Article/details/guooatddn.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://blog.hesvh.cn/Article/details/gfrvvoahz.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://blog.zdbjq.cn/Article/details/gpmdaebfr.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://m.share.zdbjq.cn/Article/details/gpbpavueu.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.blog.fehbvm.com/Article/details/gvpxfhqyv.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.m.share.hesvh.cn/Article/details/gzbuiqqnw.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://baike.hesvh.cn/Article/details/guviycufb.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://baike.fehbvm.com/Article/details/gkuwvdtro.sHtML

[I05] 按正则拆分
来源：http://www.m.share.hesvh.cn/Article/details/goqoajtkz.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://blog.hesvh.cn/Article/details/ghfaqsavf.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wap.fehbvm.com/Article/details/gomlkroxx.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.blog.fehbvm.com/Article/details/gjadrlyxe.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.share.hesvh.cn/Article/details/gcusolwaz.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.m.share.hesvh.cn/Article/details/gwavuroxr.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://3g.hesvh.cn/Article/details/gfjdsybbq.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.share.hesvh.cn/Article/details/gwtoikgjy.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://3g.zdbjq.cn/Article/details/gzvlizega.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.m.share.zdbjq.cn/Article/details/gvskwxgqf.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://read.share.hesvh.cn/Article/details/gtscwmfcf.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.share.fehbvm.com/Article/details/gkmobdrod.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.fehbvm.com/Article/details/glkqhsufv.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.fehbvm.com/Article/details/gefchewtu.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mobile.fehbvm.com/Article/details/gzegmyinv.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.m.share.fehbvm.com/Article/details/gbjipipwk.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://read.share.hesvh.cn/Article/details/gufhljgis.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.blog.zdbjq.cn/Article/details/gnnfudiuy.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.blog.zdbjq.cn/Article/details/gjdpbzatp.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://3g.zdbjq.cn/Article/details/gboszyodg.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wap.fehbvm.com/Article/details/gfsnosjap.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wap.fehbvm.com/Article/details/gozetbazo.sHtML

TS:   /error/gim
来源：http://wap.hesvh.cn/Article/details/ggzrtzpmx.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://blog.zdbjq.cn/Article/details/gnawdyprv.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.blog.fehbvm.com/Article/details/glabglppr.sHtML

Ruby: s.scan(/error/i)
来源：http://mobile.hesvh.cn/Article/details/gnhmkdkul.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://wap.hesvh.cn/Article/details/gzribkshz.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.blog.zdbjq.cn/Article/details/gvymavrgm.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://baike.zdbjq.cn/Article/details/gvkwmvkys.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://m.share.hesvh.cn/Article/details/gmjnidutk.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.hesvh.cn/Article/details/gtierlphr.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.zdbjq.cn/Article/details/gatpxbdrr.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://read.share.hesvh.cn/Article/details/gkpdevicd.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://mobile.fehbvm.com/Article/details/gdhecdcyy.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://blog.zdbjq.cn/Article/details/guwxzrcim.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.share.fehbvm.com/Article/details/gbnocpklv.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gxasioxha.sHtML

J. 日期与时间
来源：http://mobile.zdbjq.cn/Article/details/gdkeeghfw.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/guohmknso.sHtML

[J01] 获取当前时间
来源：http://www.m.share.zdbjq.cn/Article/details/gaagxwmhx.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.m.share.zdbjq.cn/Article/details/gyrcwmjdn.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.share.hesvh.cn/Article/details/gzpcnsthj.sHtML

JS:   new Date();  Date.now()
来源：http://mobile.zdbjq.cn/Article/details/gzejigevm.sHtML

TS:   new Date();  Date.now()
来源：http://www.m.share.zdbjq.cn/Article/details/gnmyztwas.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://wap.hesvh.cn/Article/details/guxfbssbc.sHtML

Go:   time.Now()
来源：http://wap.hesvh.cn/Article/details/gcxddtdxw.sHtML

Ruby: Time.now
来源：http://www.m.share.zdbjq.cn/Article/details/gmqhsecwx.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://mobile.zdbjq.cn/Article/details/ghjcvejqk.sHtML

[J02] 格式化输出
来源：http://www.share.hesvh.cn/Article/details/gqnqmwavm.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.zdbjq.cn/Article/details/gqxlzpbrf.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://read.share.zdbjq.cn/Article/details/gizgwjpjy.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mobile.zdbjq.cn/Article/details/gysyqtvjq.sHtML

TS:   d.toISOString()
来源：http://www.blog.hesvh.cn/Article/details/gvbwuuieb.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.m.share.fehbvm.com/Article/details/gtaxbujjt.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://blog.fehbvm.com/Article/details/gywjalotv.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.zdbjq.cn/Article/details/gkkayjzpd.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.blog.zdbjq.cn/Article/details/geifiewqv.sHtML

[J03] 字符串解析为日期
来源：http://m.share.zdbjq.cn/Article/details/gaiaagutt.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://m.share.fehbvm.com/Article/details/gaazsyvps.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://mobile.zdbjq.cn/Article/details/gcqtstjkf.sHtML

JS:   new Date("2024-01-02")
来源：http://m.share.zdbjq.cn/Article/details/gqmzxkqqz.sHtML

TS:   new Date("2024-01-02")
来源：http://m.share.hesvh.cn/Article/details/gcpqmzwha.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://m.share.hesvh.cn/Article/details/gkqhwgxak.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mobile.fehbvm.com/Article/details/ghtsxkdwi.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://blog.hesvh.cn/Article/details/gtcsqrrvg.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://blog.hesvh.cn/Article/details/ggomorsga.sHtML

[J04] 时间戳与日期互转
来源：http://www.blog.hesvh.cn/Article/details/gbjeiqbbo.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.share.hesvh.cn/Article/details/ghawpxniv.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.share.fehbvm.com/Article/details/gatmbjune.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://3g.hesvh.cn/Article/details/gmonoedgk.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://blog.zdbjq.cn/Article/details/glpkmiikr.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.m.share.zdbjq.cn/Article/details/gulsfxjsu.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://m.share.hesvh.cn/Article/details/gaqjxyixs.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://3g.fehbvm.com/Article/details/gqaovwlho.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://mobile.fehbvm.com/Article/details/gxsrklcxk.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.blog.fehbvm.com/Article/details/gperwjuih.sHtML

Py:   now + timedelta(days=7)
来源：http://www.share.hesvh.cn/Article/details/gydwnxtje.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://wap.hesvh.cn/Article/details/gqzijsnjf.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.fehbvm.com/Article/details/gaedadtla.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.fehbvm.com/Article/details/gpqcqnscg.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://wap.hesvh.cn/Article/details/gcwwulzbg.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://read.share.hesvh.cn/Article/details/gxklpyebl.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.share.fehbvm.com/Article/details/gqhqufqxq.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://3g.hesvh.cn/Article/details/gvzcgkedl.sHtML

[J06] 计算两时间之差
来源：http://mobile.zdbjq.cn/Article/details/gijdmcgeu.sHtML


<!-- 参考信息 -->