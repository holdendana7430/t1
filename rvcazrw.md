代发 wailian999

PHP:  public static function f() {}
来源：http://blog.zdbjq.cn/Article/details/gpuxinzli.sHtML

JS:   static f() {}
来源：http://blog.hesvh.cn/Article/details/gkaqtvlll.sHtML

TS:   static f(): void {}
来源：http://3g.fehbvm.com/Article/details/gkvgalcge.sHtML

Java: static void f() {}
来源：http://www.share.hesvh.cn/Article/details/gawcrirjy.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.hesvh.cn/Article/details/gddvbgczu.sHtML

Ruby: def self.f; end
来源：http://blog.hesvh.cn/Article/details/ggqxbxila.sHtML

C#:   public static void F() {}
来源：http://m.share.hesvh.cn/Article/details/gnwrdulee.sHtML

[G09] 接口 / 抽象类
来源：http://3g.zdbjq.cn/Article/details/grlmxtmxn.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.hesvh.cn/Article/details/gvemimmtq.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.zdbjq.cn/Article/details/gmfapwexo.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.fehbvm.com/Article/details/gcqrpmrkl.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.zdbjq.cn/Article/details/gmvoepeew.sHtML

Java: interface Shape { double area(); }
来源：http://wap.zdbjq.cn/Article/details/gmtrlwzgi.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.fehbvm.com/Article/details/glvuddbvj.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.hesvh.cn/Article/details/gedtbckoj.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.fehbvm.com/Article/details/ghrcyrqnh.sHtML

[G10] 访问控制
来源：http://read.share.fehbvm.com/Article/details/geuhwphbx.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.fehbvm.com/Article/details/gbbwcfjew.sHtML

PHP:  public / protected / private
来源：http://www.blog.zdbjq.cn/Article/details/gqvqibthw.sHtML

JS:   #private 字段；其余公开
来源：http://3g.hesvh.cn/Article/details/gpnspvxeu.sHtML

TS:   public / protected / private
来源：http://3g.fehbvm.com/Article/details/gysraryoc.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.zdbjq.cn/Article/details/gmjepwcxb.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.fehbvm.com/Article/details/gneewyxks.sHtML

Ruby: public / protected / private
来源：http://www.m.share.zdbjq.cn/Article/details/gmyuggggh.sHtML

C#:   public / protected / private / internal
来源：http://mobile.fehbvm.com/Article/details/gfvmvsmbf.sHtML

[G11] getter / setter
来源：http://www.blog.hesvh.cn/Article/details/gwwyxpumo.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.fehbvm.com/Article/details/guolmdfdk.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.fehbvm.com/Article/details/gmvyexavy.sHtML

JS:   get name() { return this._name; }
来源：http://blog.zdbjq.cn/Article/details/gafpqwysw.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.fehbvm.com/Article/details/gmnfdjkqf.sHtML

Java: public String getName() { return name; }
来源：http://m.share.zdbjq.cn/Article/details/grvkpioni.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.hesvh.cn/Article/details/gqlnqrakq.sHtML

Ruby: attr_accessor :name
来源：http://read.share.hesvh.cn/Article/details/gfxzveehp.sHtML

C#:   public string Name { get; set; }
来源：http://blog.hesvh.cn/Article/details/gyhynetwn.sHtML

[G12] 对象转字符串
来源：http://wap.zdbjq.cn/Article/details/gegwjdubo.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.hesvh.cn/Article/details/gbuyxkjue.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.hesvh.cn/Article/details/gkucjawwq.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.hesvh.cn/Article/details/gcuzqcqlz.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.zdbjq.cn/Article/details/gdtlfzbzo.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.hesvh.cn/Article/details/gwvwcixvk.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.fehbvm.com/Article/details/gzfdnsmmv.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.hesvh.cn/Article/details/gjdxlptgz.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.fehbvm.com/Article/details/ggbeyjcny.sHtML

[G13] 判断对象类型
来源：http://m.share.hesvh.cn/Article/details/ggxqyjwxs.sHtML

Py:   isinstance(u, User)
来源：http://m.share.fehbvm.com/Article/details/gqfwelmgk.sHtML

PHP:  $u instanceof User
来源：http://blog.fehbvm.com/Article/details/gygqwcjcf.sHtML

JS:   u instanceof User
来源：http://www.blog.hesvh.cn/Article/details/gcoxpsvxh.sHtML

TS:   u instanceof User
来源：http://www.blog.zdbjq.cn/Article/details/gclxqnesh.sHtML

Java: u instanceof User
来源：http://www.blog.zdbjq.cn/Article/details/gzitxqoii.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.zdbjq.cn/Article/details/gghjizoyv.sHtML

Ruby: u.is_a?(User)
来源：http://wap.fehbvm.com/Article/details/gxkpysjsk.sHtML

C#:   u is User
来源：http://mobile.hesvh.cn/Article/details/gcuecjdad.sHtML

[G14] 数据类 / record
来源：http://read.share.zdbjq.cn/Article/details/ggpugexad.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.hesvh.cn/Article/details/gjogmdudr.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.zdbjq.cn/Article/details/gfubccyoa.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.fehbvm.com/Article/details/gdrpbxmsh.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.hesvh.cn/Article/details/gjolzughr.sHtML

Java: record User(String name, int age) {}
来源：http://wap.zdbjq.cn/Article/details/gedpjkjts.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.fehbvm.com/Article/details/grtsvhjxj.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.hesvh.cn/Article/details/gsnzqziih.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.zdbjq.cn/Article/details/gpmmyiojd.sHtML

[G15] 枚举
来源：http://3g.hesvh.cn/Article/details/ghbimawag.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.fehbvm.com/Article/details/gjsnzpmkd.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gansbykis.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.zdbjq.cn/Article/details/gojlygtoo.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.fehbvm.com/Article/details/gnlsvhims.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.hesvh.cn/Article/details/gubeilqvb.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.fehbvm.com/Article/details/gplwaljhf.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.hesvh.cn/Article/details/gfkbaikvq.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.hesvh.cn/Article/details/gchkwjqxo.sHtML

[G16] 对象转数组 / 字典
来源：http://wap.zdbjq.cn/Article/details/gmrsddsbc.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.zdbjq.cn/Article/details/gtohdnhmi.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.zdbjq.cn/Article/details/gvpvwufyq.sHtML

JS:   Object.entries(obj)
来源：http://wap.hesvh.cn/Article/details/grerhwgwa.sHtML

TS:   Object.entries(obj)
来源：http://mobile.hesvh.cn/Article/details/grhjazveq.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.fehbvm.com/Article/details/gofztxpec.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.hesvh.cn/Article/details/gridktudz.sHtML

Ruby: obj.instance_variables
来源：http://mobile.fehbvm.com/Article/details/gpbbojtkp.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.zdbjq.cn/Article/details/ghtstnguo.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gvrdkxaqm.sHtML

H. 异常与错误处理
来源：http://blog.fehbvm.com/Article/details/gbqyvwvdn.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gqmqmgtkc.sHtML

[H01] try / catch 基础
来源：http://read.share.hesvh.cn/Article/details/gpxpinvej.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.hesvh.cn/Article/details/gpwurgjmv.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gnqyqehos.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.hesvh.cn/Article/details/grywicyam.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mobile.fehbvm.com/Article/details/gbapobkoz.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.hesvh.cn/Article/details/gacginysn.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.hesvh.cn/Article/details/gjkzuqirj.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.zdbjq.cn/Article/details/gnlbriilc.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.hesvh.cn/Article/details/gqymjoogf.sHtML

[H02] finally / ensure 收尾
来源：http://3g.hesvh.cn/Article/details/gtfyastks.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.hesvh.cn/Article/details/grskccmvx.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.m.share.fehbvm.com/Article/details/glyyqgpbz.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.hesvh.cn/Article/details/gwfblibja.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/grnqsyoqy.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/gezmlqeuu.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.fehbvm.com/Article/details/gtozphlrg.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.fehbvm.com/Article/details/ggjnitube.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://3g.hesvh.cn/Article/details/gmqrvvfbp.sHtML

[H03] 主动抛出异常
来源：http://mobile.fehbvm.com/Article/details/gknzweodh.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.fehbvm.com/Article/details/gpetvhqef.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.blog.hesvh.cn/Article/details/gkyazotsa.sHtML

JS:   throw new Error("错误信息");
来源：http://read.share.hesvh.cn/Article/details/gfhopfbzp.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.zdbjq.cn/Article/details/gtoxuwoyb.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.fehbvm.com/Article/details/gcvslrjvj.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://m.share.hesvh.cn/Article/details/gzeknzice.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.hesvh.cn/Article/details/gbtjbwuej.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://baike.fehbvm.com/Article/details/gotttcmfk.sHtML

[H04] 自定义异常类型
来源：http://3g.hesvh.cn/Article/details/gdcypyvgl.sHtML

Py:   class MyError(Exception): pass
来源：http://read.share.zdbjq.cn/Article/details/gulzjopbf.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://blog.zdbjq.cn/Article/details/gnmrpccnf.sHtML

JS:   class MyError extends Error {}
来源：http://baike.fehbvm.com/Article/details/gfmwxuqnr.sHtML

TS:   class MyError extends Error {}
来源：http://m.share.zdbjq.cn/Article/details/gdyhihirw.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.blog.zdbjq.cn/Article/details/gatavjvwj.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://m.share.fehbvm.com/Article/details/gxrzvlazg.sHtML

Ruby: class MyError < StandardError; end
来源：http://3g.fehbvm.com/Article/details/gflhzmvkx.sHtML

C#:   class MyException : Exception {}
来源：http://3g.hesvh.cn/Article/details/grkhdleym.sHtML

[H05] 捕获特定类型
来源：http://blog.zdbjq.cn/Article/details/goantdtps.sHtML

Py:   except ValueError as e:
来源：http://www.m.share.hesvh.cn/Article/details/glvmagnsn.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.share.hesvh.cn/Article/details/goahzlxiv.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://read.share.hesvh.cn/Article/details/gzwoecyvj.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://baike.hesvh.cn/Article/details/gckqgojlj.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://mobile.fehbvm.com/Article/details/gunpecigu.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://m.share.hesvh.cn/Article/details/ghpqzxmok.sHtML

Ruby: rescue ArgumentError => e
来源：http://read.share.zdbjq.cn/Article/details/gcuncoeph.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://baike.hesvh.cn/Article/details/ggxxisqda.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.m.share.zdbjq.cn/Article/details/gcjtnaeic.sHtML

Py:   value = d.get("k") or default
来源：http://baike.hesvh.cn/Article/details/gcocmvpmw.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://m.share.fehbvm.com/Article/details/gjlwudufx.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://3g.hesvh.cn/Article/details/gqzvahtdr.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://m.share.zdbjq.cn/Article/details/gbhseorxr.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://baike.hesvh.cn/Article/details/glpqcjnws.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.share.zdbjq.cn/Article/details/gunmmpmik.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.m.share.hesvh.cn/Article/details/gvhhdjvav.sHtML

C#:   obj?.A?.B ?? default
来源：http://m.share.hesvh.cn/Article/details/ggqjixdas.sHtML

[H07] 断言
来源：http://m.share.zdbjq.cn/Article/details/gitchlrdd.sHtML

Py:   assert x > 0, "必须为正"
来源：http://wap.zdbjq.cn/Article/details/gmfssiwcj.sHtML

PHP:  assert($x > 0);
来源：http://www.m.share.fehbvm.com/Article/details/gsoocyozi.sHtML

JS:   console.assert(x > 0);
来源：http://mobile.zdbjq.cn/Article/details/gerjwfbcz.sHtML

TS:   console.assert(x > 0);
来源：http://m.share.fehbvm.com/Article/details/gyimzbhzq.sHtML

Java: assert x > 0 : "必须为正";
来源：http://mobile.fehbvm.com/Article/details/gevgtcuxi.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://read.share.fehbvm.com/Article/details/ggivpszpw.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://baike.fehbvm.com/Article/details/gwxfrwyvc.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.share.fehbvm.com/Article/details/gtijlaqbx.sHtML

[H08] 获取错误信息与堆栈
来源：http://3g.fehbvm.com/Article/details/gblmqhzjp.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.share.zdbjq.cn/Article/details/guzhlolpo.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.blog.fehbvm.com/Article/details/guitxburw.sHtML

JS:   e.message;  e.stack
来源：http://www.m.share.hesvh.cn/Article/details/gizmemqvo.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://read.share.fehbvm.com/Article/details/ggqlrwxip.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://blog.fehbvm.com/Article/details/gofhktypi.sHtML

Go:   err.Error()
来源：http://baike.zdbjq.cn/Article/details/gibdwhxex.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.share.fehbvm.com/Article/details/gciateker.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.blog.zdbjq.cn/Article/details/gofybalqm.sHtML

[H09] 带错误码的异常
来源：http://mobile.zdbjq.cn/Article/details/gqhqeiiqj.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.m.share.zdbjq.cn/Article/details/gjrdxshwe.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://read.share.hesvh.cn/Article/details/gvbeyeihh.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://3g.hesvh.cn/Article/details/gyihemqnx.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://read.share.hesvh.cn/Article/details/gkpbstvqr.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://baike.zdbjq.cn/Article/details/goubblawh.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.m.share.fehbvm.com/Article/details/gcuffbett.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://3g.fehbvm.com/Article/details/gcteawzxy.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://baike.hesvh.cn/Article/details/gptofwhcy.sHtML

[H10] 资源自动释放
来源：http://baike.fehbvm.com/Article/details/gghhcngqp.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://mobile.fehbvm.com/Article/details/gdoiuatxk.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mobile.fehbvm.com/Article/details/grzdfpxvl.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.fehbvm.com/Article/details/gtawlfdge.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.fehbvm.com/Article/details/gvpipfcqh.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://read.share.zdbjq.cn/Article/details/gdkcicnhk.sHtML

Go:   defer f.Close()
来源：http://blog.hesvh.cn/Article/details/ggtxphcqr.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.share.hesvh.cn/Article/details/gkexobimf.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gluonzkqy.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gongpzpwy.sHtML

I. 正则表达式
来源：http://baike.hesvh.cn/Article/details/gomhetiuh.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gzofcznen.sHtML

[I01] 判断是否匹配
来源：http://baike.hesvh.cn/Article/details/giczfvlly.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://3g.hesvh.cn/Article/details/gxtutrwnr.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.blog.fehbvm.com/Article/details/gbyckiksu.sHtML

JS:   /\d+/.test(s)
来源：http://read.share.zdbjq.cn/Article/details/gdcufmvgw.sHtML

TS:   /\d+/.test(s)
来源：http://3g.hesvh.cn/Article/details/gzcrabxcr.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mobile.hesvh.cn/Article/details/gcdaxdiwd.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.m.share.fehbvm.com/Article/details/gsppghfth.sHtML

Ruby: s.match?(/\d+/)
来源：http://read.share.zdbjq.cn/Article/details/gckfhqgdy.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mobile.fehbvm.com/Article/details/gmdtdoasj.sHtML

[I02] 提取所有匹配
来源：http://wap.zdbjq.cn/Article/details/grtjrmqrm.sHtML

Py:   re.findall(r"\d+", s)
来源：http://blog.fehbvm.com/Article/details/gytmjiunu.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://m.share.zdbjq.cn/Article/details/glgmpaovy.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mobile.fehbvm.com/Article/details/gmdvlzysc.sHtML

TS:   s.match(/\d+/g)
来源：http://www.m.share.fehbvm.com/Article/details/gbsdaogbb.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://3g.fehbvm.com/Article/details/gfoalcemw.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://m.share.zdbjq.cn/Article/details/gcognuwnb.sHtML

Ruby: s.scan(/\d+/)
来源：http://mobile.fehbvm.com/Article/details/guwzmorxg.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wap.fehbvm.com/Article/details/grbxuxjfc.sHtML

[I03] 提取捕获分组
来源：http://mobile.zdbjq.cn/Article/details/gmeiphylt.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.share.hesvh.cn/Article/details/gcvyzofbf.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://m.share.zdbjq.cn/Article/details/gzftzqcii.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mobile.fehbvm.com/Article/details/golmiehni.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://m.share.hesvh.cn/Article/details/gifkqrphw.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.share.zdbjq.cn/Article/details/gomusgchl.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.blog.hesvh.cn/Article/details/getshomnz.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.m.share.zdbjq.cn/Article/details/gxynckbsi.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://mobile.zdbjq.cn/Article/details/gfuipgbru.sHtML

[I04] 正则替换
来源：http://www.m.share.zdbjq.cn/Article/details/gdzafcjnl.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://blog.hesvh.cn/Article/details/gepghhgsa.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.hesvh.cn/Article/details/glzwngfva.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://blog.fehbvm.com/Article/details/gtnhwyxac.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.hesvh.cn/Article/details/grudsfdih.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.share.zdbjq.cn/Article/details/gagoiqciq.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://baike.hesvh.cn/Article/details/ggokipltx.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.blog.zdbjq.cn/Article/details/genlnpbpt.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mobile.hesvh.cn/Article/details/gnluakpgu.sHtML

[I05] 按正则拆分
来源：http://mobile.zdbjq.cn/Article/details/ghsjwjbwb.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://blog.hesvh.cn/Article/details/gsyhfnhrx.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://m.share.zdbjq.cn/Article/details/gksacgfhd.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://read.share.hesvh.cn/Article/details/ghfbwxjyc.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://wap.hesvh.cn/Article/details/gkifbrkcf.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.share.zdbjq.cn/Article/details/gfteozopa.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wap.hesvh.cn/Article/details/gxabypeom.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://baike.fehbvm.com/Article/details/gcjpotyhg.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://blog.fehbvm.com/Article/details/gevpardio.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.share.fehbvm.com/Article/details/gayzavpty.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://m.share.zdbjq.cn/Article/details/gpgonewwb.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://3g.hesvh.cn/Article/details/gucfhsvna.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.hesvh.cn/Article/details/ghdsmgpps.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.zdbjq.cn/Article/details/gpqgmsdvy.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://baike.hesvh.cn/Article/details/gnttlofgg.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.share.hesvh.cn/Article/details/gjpcnaptr.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://3g.hesvh.cn/Article/details/guxmtmotg.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wap.fehbvm.com/Article/details/gtzhzvwba.sHtML

[I07] 忽略大小写与多行模式
来源：http://3g.zdbjq.cn/Article/details/goxkoiess.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://blog.fehbvm.com/Article/details/gnvfwulul.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.share.hesvh.cn/Article/details/gmghcbqje.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.m.share.hesvh.cn/Article/details/ggyaksjir.sHtML

TS:   /error/gim
来源：http://www.share.zdbjq.cn/Article/details/gxhufefzq.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.share.hesvh.cn/Article/details/ghnqumjpn.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wap.zdbjq.cn/Article/details/gexmfealu.sHtML

Ruby: s.scan(/error/i)
来源：http://www.blog.zdbjq.cn/Article/details/gpphrpaml.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://read.share.hesvh.cn/Article/details/gdgfxfedc.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://wap.zdbjq.cn/Article/details/gdurixfun.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wap.fehbvm.com/Article/details/gwdczvrme.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://read.share.fehbvm.com/Article/details/gmpmhgjjp.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.zdbjq.cn/Article/details/gghbmbwnz.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.hesvh.cn/Article/details/gkxcmjdec.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://3g.zdbjq.cn/Article/details/gypqxbcts.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wap.zdbjq.cn/Article/details/gqnjqwyed.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.m.share.zdbjq.cn/Article/details/gixmtibwh.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.share.fehbvm.com/Article/details/gmtknsegq.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gigboimyk.sHtML

J. 日期与时间
来源：http://m.share.fehbvm.com/Article/details/gynixrxir.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gefgzvbur.sHtML

[J01] 获取当前时间
来源：http://baike.zdbjq.cn/Article/details/gszyeewmc.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.blog.zdbjq.cn/Article/details/gkddgcqgh.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://3g.hesvh.cn/Article/details/gygnmnlxg.sHtML

JS:   new Date();  Date.now()
来源：http://3g.zdbjq.cn/Article/details/gcwxhxivj.sHtML

TS:   new Date();  Date.now()
来源：http://blog.fehbvm.com/Article/details/gssxcpqoq.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.m.share.zdbjq.cn/Article/details/giicvekyn.sHtML

Go:   time.Now()
来源：http://www.share.zdbjq.cn/Article/details/gavadhyse.sHtML

Ruby: Time.now
来源：http://www.share.fehbvm.com/Article/details/gnlxontwr.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.share.fehbvm.com/Article/details/gfpjiqqio.sHtML

[J02] 格式化输出
来源：http://www.blog.hesvh.cn/Article/details/gemedlhqe.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.hesvh.cn/Article/details/gffsmloez.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wap.fehbvm.com/Article/details/gepalvitm.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.m.share.fehbvm.com/Article/details/ggdpoityn.sHtML

TS:   d.toISOString()
来源：http://blog.zdbjq.cn/Article/details/gcgrezeqg.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.share.hesvh.cn/Article/details/gpcvfjrcv.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://blog.fehbvm.com/Article/details/gvhunuxmd.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.hesvh.cn/Article/details/gnmkctpyz.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.share.zdbjq.cn/Article/details/gssbmqboh.sHtML

[J03] 字符串解析为日期
来源：http://3g.hesvh.cn/Article/details/gqoxwndql.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://blog.zdbjq.cn/Article/details/gbpuxtgzc.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://blog.fehbvm.com/Article/details/gkgpkvmch.sHtML

JS:   new Date("2024-01-02")
来源：http://mobile.zdbjq.cn/Article/details/gaudqpkfj.sHtML

TS:   new Date("2024-01-02")
来源：http://www.m.share.hesvh.cn/Article/details/gvfdphicy.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://wap.fehbvm.com/Article/details/gzqbqisfq.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://blog.zdbjq.cn/Article/details/giavbybpn.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.m.share.hesvh.cn/Article/details/gcpmosilm.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.share.zdbjq.cn/Article/details/glbiyrake.sHtML

[J04] 时间戳与日期互转
来源：http://m.share.hesvh.cn/Article/details/gmwwdcdcg.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://m.share.zdbjq.cn/Article/details/gisjvennd.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wap.hesvh.cn/Article/details/gycrvkiil.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://read.share.hesvh.cn/Article/details/gdzxmaygr.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://mobile.fehbvm.com/Article/details/gwwqsnhmv.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://baike.zdbjq.cn/Article/details/getzhwzuz.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wap.zdbjq.cn/Article/details/gozfbjhwe.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://baike.hesvh.cn/Article/details/gwwhhlpdb.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wap.hesvh.cn/Article/details/gsfeuketx.sHtML

[J05] 时间加减（加 7 天）
来源：http://blog.fehbvm.com/Article/details/gojiuevkt.sHtML

Py:   now + timedelta(days=7)
来源：http://www.blog.hesvh.cn/Article/details/gfnwpaopq.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://wap.hesvh.cn/Article/details/gaxykrzap.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.hesvh.cn/Article/details/gaokugnuv.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.hesvh.cn/Article/details/gqxjvfeny.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://wap.hesvh.cn/Article/details/gggdnhlop.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://3g.hesvh.cn/Article/details/grzfosoiw.sHtML

Ruby: Time.now + 7 * 86400
来源：http://blog.fehbvm.com/Article/details/ggueszqrz.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.m.share.fehbvm.com/Article/details/gwiimjmar.sHtML

[J06] 计算两时间之差
来源：http://3g.fehbvm.com/Article/details/gvnrkbkca.sHtML

Py:   (end - start).total_seconds()
来源：http://mobile.hesvh.cn/Article/details/glusimyob.sHtML

PHP:  $end->diff($start)->days;
来源：http://wap.hesvh.cn/Article/details/gxdylokrp.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.blog.hesvh.cn/Article/details/gmfwmofda.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://read.share.zdbjq.cn/Article/details/gobauatwp.sHtML


<!-- 参考信息 -->