代发 wailian999

C#:   public override string Greet() => "admin";
来源：http://www.blog.zdbjq.cn/Article/details/geadruqob.sHtML

[G07] 调用父类方法
来源：http://read.share.hesvh.cn/Article/details/grjapwjic.sHtML

Py:   super().greet()
来源：http://baike.zdbjq.cn/Article/details/gqorfxkop.sHtML

PHP:  parent::greet();
来源：http://www.m.share.hesvh.cn/Article/details/ggvbcyqqo.sHtML

JS:   super.greet();
来源：http://www.m.share.fehbvm.com/Article/details/gfgrnuyfu.sHtML

TS:   super.greet();
来源：http://3g.fehbvm.com/Article/details/gyroixrtx.sHtML

Java: super.greet();
来源：http://wap.zdbjq.cn/Article/details/gvlnkwzca.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.hesvh.cn/Article/details/gbubjyilw.sHtML

Ruby: super
来源：http://baike.hesvh.cn/Article/details/gfhnophkf.sHtML

C#:   base.Greet();
来源：http://blog.fehbvm.com/Article/details/gkhcijzoz.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.zdbjq.cn/Article/details/gxkiomryi.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.fehbvm.com/Article/details/gskhgzjrz.sHtML

PHP:  public static function f() {}
来源：http://www.share.zdbjq.cn/Article/details/ghlngpbdx.sHtML

JS:   static f() {}
来源：http://www.share.hesvh.cn/Article/details/gdqlqdhoi.sHtML

TS:   static f(): void {}
来源：http://m.share.zdbjq.cn/Article/details/gdalrntnv.sHtML

Java: static void f() {}
来源：http://www.blog.hesvh.cn/Article/details/gvnmbpoza.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.hesvh.cn/Article/details/gjvgfgled.sHtML

Ruby: def self.f; end
来源：http://3g.zdbjq.cn/Article/details/girxctqga.sHtML

C#:   public static void F() {}
来源：http://blog.fehbvm.com/Article/details/ghrxopyjw.sHtML

[G09] 接口 / 抽象类
来源：http://blog.zdbjq.cn/Article/details/gohtfoxao.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.fehbvm.com/Article/details/gufqjrhwo.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.hesvh.cn/Article/details/gozshqhbz.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.fehbvm.com/Article/details/gaykwsbvl.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.hesvh.cn/Article/details/gopnghiig.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.fehbvm.com/Article/details/gllfbwswl.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.zdbjq.cn/Article/details/gyjjcjhqg.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.fehbvm.com/Article/details/gdifmmxbr.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.zdbjq.cn/Article/details/gbvpuyeef.sHtML

[G10] 访问控制
来源：http://www.m.share.hesvh.cn/Article/details/gkeddrlle.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.fehbvm.com/Article/details/gbztqwfdk.sHtML

PHP:  public / protected / private
来源：http://www.m.share.fehbvm.com/Article/details/gynujsalu.sHtML

JS:   #private 字段；其余公开
来源：http://3g.fehbvm.com/Article/details/gyvnlybba.sHtML

TS:   public / protected / private
来源：http://www.share.zdbjq.cn/Article/details/glpovzasn.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.hesvh.cn/Article/details/gvkxdbeia.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.zdbjq.cn/Article/details/greyplmle.sHtML

Ruby: public / protected / private
来源：http://www.share.fehbvm.com/Article/details/guruwdfzw.sHtML

C#:   public / protected / private / internal
来源：http://blog.zdbjq.cn/Article/details/ghsnzncsj.sHtML

[G11] getter / setter
来源：http://3g.zdbjq.cn/Article/details/gtvfuvxuu.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.zdbjq.cn/Article/details/gqualzmgj.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.hesvh.cn/Article/details/gqmovzyve.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.zdbjq.cn/Article/details/gwpqfbftj.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.zdbjq.cn/Article/details/gvgbzwqvd.sHtML

Java: public String getName() { return name; }
来源：http://read.share.fehbvm.com/Article/details/gfidopdth.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.zdbjq.cn/Article/details/gupdvpgry.sHtML

Ruby: attr_accessor :name
来源：http://mobile.zdbjq.cn/Article/details/gfcnthzmb.sHtML

C#:   public string Name { get; set; }
来源：http://wap.fehbvm.com/Article/details/gmowjmsry.sHtML

[G12] 对象转字符串
来源：http://mobile.zdbjq.cn/Article/details/gynrxvarp.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.zdbjq.cn/Article/details/gjpkpgzzh.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.zdbjq.cn/Article/details/gnwoboohr.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.zdbjq.cn/Article/details/gqkdupdvh.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.hesvh.cn/Article/details/gxjnyrzxe.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.fehbvm.com/Article/details/gowhodqgr.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.zdbjq.cn/Article/details/gszlcyihm.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.hesvh.cn/Article/details/gdojgqzfg.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.fehbvm.com/Article/details/gdwpgwtyt.sHtML

[G13] 判断对象类型
来源：http://www.share.zdbjq.cn/Article/details/gdezpsyvw.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.hesvh.cn/Article/details/gfzjytczc.sHtML

PHP:  $u instanceof User
来源：http://blog.zdbjq.cn/Article/details/gqohmtyoi.sHtML

JS:   u instanceof User
来源：http://www.m.share.fehbvm.com/Article/details/ghzjslann.sHtML

TS:   u instanceof User
来源：http://read.share.fehbvm.com/Article/details/garfseifg.sHtML

Java: u instanceof User
来源：http://3g.hesvh.cn/Article/details/gmwjwovdd.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.hesvh.cn/Article/details/gsrswgnfr.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.hesvh.cn/Article/details/gkllrzcut.sHtML

C#:   u is User
来源：http://blog.zdbjq.cn/Article/details/gbbqvkmos.sHtML

[G14] 数据类 / record
来源：http://3g.fehbvm.com/Article/details/gpawfiddc.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.hesvh.cn/Article/details/gxmavqwnr.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.zdbjq.cn/Article/details/gnbjzdbih.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.zdbjq.cn/Article/details/gthenlywv.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.zdbjq.cn/Article/details/gjlrgqcmj.sHtML

Java: record User(String name, int age) {}
来源：http://3g.hesvh.cn/Article/details/gdmdbkkng.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.zdbjq.cn/Article/details/gkiqtimvm.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.fehbvm.com/Article/details/gofbzrfws.sHtML

C#:   record User(string Name, int Age);
来源：http://wap.hesvh.cn/Article/details/guddbnfrv.sHtML

[G15] 枚举
来源：http://www.share.fehbvm.com/Article/details/gvinsdkws.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.fehbvm.com/Article/details/gxqtzxkge.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.fehbvm.com/Article/details/gnwsowequ.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mobile.zdbjq.cn/Article/details/ghwkwwzgh.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.fehbvm.com/Article/details/gnlpengyg.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.hesvh.cn/Article/details/gtsunomkg.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.hesvh.cn/Article/details/gsrxfjgua.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.fehbvm.com/Article/details/gkoucvzoy.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.zdbjq.cn/Article/details/gptesabto.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.zdbjq.cn/Article/details/gwxtahelt.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.hesvh.cn/Article/details/grqtshrfr.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.zdbjq.cn/Article/details/gzmnbjdxi.sHtML

JS:   Object.entries(obj)
来源：http://www.share.zdbjq.cn/Article/details/gdqefovra.sHtML

TS:   Object.entries(obj)
来源：http://baike.fehbvm.com/Article/details/gmsottvgg.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.fehbvm.com/Article/details/grokjpoiz.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.zdbjq.cn/Article/details/gsbetazot.sHtML

Ruby: obj.instance_variables
来源：http://m.share.zdbjq.cn/Article/details/gjuhuxwme.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.zdbjq.cn/Article/details/gtujvmadl.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gilhvibzp.sHtML

H. 异常与错误处理
来源：http://www.m.share.hesvh.cn/Article/details/gzvatcahb.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/grqbrdtfc.sHtML

[H01] try / catch 基础
来源：http://blog.hesvh.cn/Article/details/goquduobo.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.fehbvm.com/Article/details/gzswxpugp.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gfzkbipmj.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://blog.fehbvm.com/Article/details/gbjbqwlyv.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.fehbvm.com/Article/details/gmwouxmwx.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.fehbvm.com/Article/details/girbphwxn.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://read.share.hesvh.cn/Article/details/gobmmdebs.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://3g.hesvh.cn/Article/details/gngovyafj.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.m.share.fehbvm.com/Article/details/gxifguson.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.hesvh.cn/Article/details/gqjfpbzph.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.m.share.hesvh.cn/Article/details/gxvbbeyeq.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.zdbjq.cn/Article/details/gekduxdnv.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://wap.fehbvm.com/Article/details/gmnzcyjne.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/gvwgepxup.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.hesvh.cn/Article/details/gqcblzssd.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.fehbvm.com/Article/details/gfmpdehks.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.fehbvm.com/Article/details/ghvembmbx.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://3g.zdbjq.cn/Article/details/guybjjdmk.sHtML

[H03] 主动抛出异常
来源：http://www.m.share.fehbvm.com/Article/details/gphpnlnzi.sHtML

Py:   raise ValueError("错误信息")
来源：http://read.share.hesvh.cn/Article/details/glcebgvvs.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.blog.hesvh.cn/Article/details/gktedmkli.sHtML

JS:   throw new Error("错误信息");
来源：http://blog.fehbvm.com/Article/details/gljnqpcch.sHtML

TS:   throw new Error("错误信息");
来源：http://wap.zdbjq.cn/Article/details/gcinbbhzz.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.hesvh.cn/Article/details/gldujdqbx.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.zdbjq.cn/Article/details/gxuxqgkig.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://mobile.zdbjq.cn/Article/details/gaiiorkkz.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.share.fehbvm.com/Article/details/gmzoinmbz.sHtML

[H04] 自定义异常类型
来源：http://blog.fehbvm.com/Article/details/gogrwdqgv.sHtML

Py:   class MyError(Exception): pass
来源：http://www.m.share.hesvh.cn/Article/details/gflagjddk.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://3g.fehbvm.com/Article/details/gijmxwqjq.sHtML

JS:   class MyError extends Error {}
来源：http://mobile.hesvh.cn/Article/details/gjpahymtk.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.fehbvm.com/Article/details/gmtmlhzaw.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.m.share.fehbvm.com/Article/details/ghspqeuyp.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://3g.fehbvm.com/Article/details/grlzlsdoq.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.hesvh.cn/Article/details/gbuiiiext.sHtML

C#:   class MyException : Exception {}
来源：http://mobile.zdbjq.cn/Article/details/gjxurjutv.sHtML

[H05] 捕获特定类型
来源：http://3g.zdbjq.cn/Article/details/grfwnljix.sHtML

Py:   except ValueError as e:
来源：http://www.blog.hesvh.cn/Article/details/gioswgpss.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://m.share.fehbvm.com/Article/details/gewaihagz.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://blog.fehbvm.com/Article/details/gbkunaawi.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.m.share.zdbjq.cn/Article/details/glrvnwvap.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://3g.fehbvm.com/Article/details/gwpmjoasl.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.m.share.zdbjq.cn/Article/details/gruqvylhs.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.zdbjq.cn/Article/details/gmvskfjtp.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://baike.fehbvm.com/Article/details/gdjyrxxli.sHtML

[H06] 可选值 / 空值安全访问
来源：http://blog.zdbjq.cn/Article/details/gdnxltetu.sHtML

Py:   value = d.get("k") or default
来源：http://3g.zdbjq.cn/Article/details/grwwsfrsz.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.share.fehbvm.com/Article/details/gveingnwu.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://3g.hesvh.cn/Article/details/guuzgslnt.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://read.share.fehbvm.com/Article/details/gyrbcttxx.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://blog.fehbvm.com/Article/details/gjquuravl.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.blog.fehbvm.com/Article/details/gyaurmrev.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.blog.hesvh.cn/Article/details/gqajaldjb.sHtML

C#:   obj?.A?.B ?? default
来源：http://baike.fehbvm.com/Article/details/grqjvefbm.sHtML

[H07] 断言
来源：http://mobile.fehbvm.com/Article/details/gomkocist.sHtML

Py:   assert x > 0, "必须为正"
来源：http://baike.fehbvm.com/Article/details/gwanfywob.sHtML

PHP:  assert($x > 0);
来源：http://blog.fehbvm.com/Article/details/gkdgdokbw.sHtML

JS:   console.assert(x > 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gaqyoales.sHtML

TS:   console.assert(x > 0);
来源：http://blog.fehbvm.com/Article/details/gqzgxqrnm.sHtML

Java: assert x > 0 : "必须为正";
来源：http://read.share.fehbvm.com/Article/details/glpckixgx.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://read.share.fehbvm.com/Article/details/gthhdshlb.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://baike.zdbjq.cn/Article/details/gagurhwhr.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.share.fehbvm.com/Article/details/gbpyoadlk.sHtML

[H08] 获取错误信息与堆栈
来源：http://mobile.hesvh.cn/Article/details/gzagpqvft.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.share.fehbvm.com/Article/details/gzzofryfc.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://m.share.hesvh.cn/Article/details/gmlloubcs.sHtML

JS:   e.message;  e.stack
来源：http://baike.fehbvm.com/Article/details/ginpfppmh.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.blog.hesvh.cn/Article/details/gpmsbeeun.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://blog.hesvh.cn/Article/details/gnkvbmukk.sHtML

Go:   err.Error()
来源：http://read.share.fehbvm.com/Article/details/ghzoifbpu.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.blog.fehbvm.com/Article/details/gjvtreogj.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.blog.fehbvm.com/Article/details/gbteieovd.sHtML

[H09] 带错误码的异常
来源：http://read.share.hesvh.cn/Article/details/gcriakbbq.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://blog.fehbvm.com/Article/details/gzxppicjb.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.m.share.hesvh.cn/Article/details/grszwghid.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wap.fehbvm.com/Article/details/gbnwcfkaq.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.share.hesvh.cn/Article/details/gtihfuvsu.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.m.share.zdbjq.cn/Article/details/gsivwibag.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mobile.zdbjq.cn/Article/details/giibhtxug.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://3g.hesvh.cn/Article/details/gbeyjcqmn.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://blog.zdbjq.cn/Article/details/gkvaeyyip.sHtML

[H10] 资源自动释放
来源：http://3g.zdbjq.cn/Article/details/ghshwkpxe.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://blog.hesvh.cn/Article/details/gkpxagqfu.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://blog.zdbjq.cn/Article/details/gblpxsovb.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.zdbjq.cn/Article/details/gzsyfocsa.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.hesvh.cn/Article/details/gfgiogfyd.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.share.hesvh.cn/Article/details/gkyhmlgca.sHtML

Go:   defer f.Close()
来源：http://mobile.fehbvm.com/Article/details/gzpbcrrrz.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.blog.hesvh.cn/Article/details/gzanylqgc.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gfsohdsck.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gnymvpfjy.sHtML

I. 正则表达式
来源：http://www.blog.zdbjq.cn/Article/details/gesfifayi.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gnbhzciyy.sHtML

[I01] 判断是否匹配
来源：http://m.share.zdbjq.cn/Article/details/gfaxeuooo.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://read.share.zdbjq.cn/Article/details/gummvldzd.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.blog.zdbjq.cn/Article/details/gcaojokkm.sHtML

JS:   /\d+/.test(s)
来源：http://mobile.zdbjq.cn/Article/details/gmxhmxlgb.sHtML

TS:   /\d+/.test(s)
来源：http://read.share.zdbjq.cn/Article/details/grfcekwbq.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://3g.hesvh.cn/Article/details/gjqqjdikz.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wap.zdbjq.cn/Article/details/gljklvsiw.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.m.share.zdbjq.cn/Article/details/gwxsswxfe.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://m.share.fehbvm.com/Article/details/gqbgizzyv.sHtML

[I02] 提取所有匹配
来源：http://wap.hesvh.cn/Article/details/galhutiwm.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.m.share.zdbjq.cn/Article/details/gkzxvhvgl.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://blog.hesvh.cn/Article/details/gjrgascjt.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wap.fehbvm.com/Article/details/gypmurxtv.sHtML

TS:   s.match(/\d+/g)
来源：http://wap.zdbjq.cn/Article/details/goxcjfhbn.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wap.fehbvm.com/Article/details/gbidmuoge.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mobile.zdbjq.cn/Article/details/gosycbwpi.sHtML

Ruby: s.scan(/\d+/)
来源：http://wap.hesvh.cn/Article/details/guanoimzu.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.share.zdbjq.cn/Article/details/gitrddzvs.sHtML

[I03] 提取捕获分组
来源：http://www.m.share.zdbjq.cn/Article/details/ggiyndohv.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://read.share.fehbvm.com/Article/details/ghkotvmzw.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.m.share.hesvh.cn/Article/details/gejlvutpm.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://3g.zdbjq.cn/Article/details/gdczwthej.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://baike.fehbvm.com/Article/details/gfaczunhv.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://3g.fehbvm.com/Article/details/gbiqkezlm.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://read.share.hesvh.cn/Article/details/gocejqtpg.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.m.share.hesvh.cn/Article/details/gzjchqkne.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://mobile.hesvh.cn/Article/details/gmjuyegpj.sHtML

[I04] 正则替换
来源：http://baike.fehbvm.com/Article/details/gmwsamogs.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://3g.zdbjq.cn/Article/details/gmrpmgpav.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.share.fehbvm.com/Article/details/gmkxuuzrs.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://blog.hesvh.cn/Article/details/guefwmjgt.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.blog.hesvh.cn/Article/details/glmpnulol.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.share.fehbvm.com/Article/details/gwrfxrwgm.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://wap.hesvh.cn/Article/details/gdtwswnnm.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://3g.hesvh.cn/Article/details/gstkowtma.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://baike.zdbjq.cn/Article/details/gommrdqwv.sHtML

[I05] 按正则拆分
来源：http://www.m.share.fehbvm.com/Article/details/gvequhrwk.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://wap.hesvh.cn/Article/details/gatujpkzr.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://3g.fehbvm.com/Article/details/gqyycytao.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.blog.hesvh.cn/Article/details/gdzmrikka.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.blog.hesvh.cn/Article/details/gjipgpxca.sHtML

Java: s.split("\\s*,\\s*")
来源：http://m.share.fehbvm.com/Article/details/gsauznhtk.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://read.share.fehbvm.com/Article/details/gupyhseqg.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://wap.zdbjq.cn/Article/details/gdplwbgpn.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://baike.hesvh.cn/Article/details/gqtfivsqa.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.share.hesvh.cn/Article/details/gostccwah.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://mobile.hesvh.cn/Article/details/gqzygfgps.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.share.hesvh.cn/Article/details/ggmimyawr.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.hesvh.cn/Article/details/gclqnrenb.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.hesvh.cn/Article/details/gmrnvogii.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.share.hesvh.cn/Article/details/gkyptwhfi.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://baike.fehbvm.com/Article/details/gkhuueloo.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://mobile.hesvh.cn/Article/details/gidoozpjc.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mobile.zdbjq.cn/Article/details/gfnusdyap.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.m.share.fehbvm.com/Article/details/gbtgqznmw.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://baike.fehbvm.com/Article/details/gklhbxptg.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.blog.hesvh.cn/Article/details/gcoahcpvf.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.m.share.hesvh.cn/Article/details/gxtwncphm.sHtML

TS:   /error/gim
来源：http://wap.hesvh.cn/Article/details/glkiwiuav.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://m.share.hesvh.cn/Article/details/gvsocmzry.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.blog.hesvh.cn/Article/details/gmhoelkfi.sHtML

Ruby: s.scan(/error/i)
来源：http://blog.fehbvm.com/Article/details/goxbbgxsp.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://baike.zdbjq.cn/Article/details/gmxywxlmn.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://m.share.zdbjq.cn/Article/details/girzpmwnh.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.m.share.hesvh.cn/Article/details/gfcpuextd.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.m.share.fehbvm.com/Article/details/geyynimof.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.zdbjq.cn/Article/details/gfuubtnzi.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.zdbjq.cn/Article/details/gvwfgjaoq.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.share.zdbjq.cn/Article/details/gfsinmnex.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://mobile.zdbjq.cn/Article/details/gqzzqvlxz.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://3g.zdbjq.cn/Article/details/gswwolgfg.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.m.share.fehbvm.com/Article/details/gtpwkgamv.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gmiqnrlkn.sHtML

J. 日期与时间
来源：http://3g.fehbvm.com/Article/details/gqqarysyo.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/ggkbdvbkk.sHtML

[J01] 获取当前时间
来源：http://blog.zdbjq.cn/Article/details/gqwwdtzhr.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://mobile.zdbjq.cn/Article/details/gvnqiarny.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mobile.zdbjq.cn/Article/details/gmodftoty.sHtML

JS:   new Date();  Date.now()
来源：http://3g.fehbvm.com/Article/details/ghlkrjang.sHtML

TS:   new Date();  Date.now()
来源：http://3g.hesvh.cn/Article/details/gvncbfqxb.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://blog.hesvh.cn/Article/details/gqbjukmdf.sHtML

Go:   time.Now()
来源：http://baike.fehbvm.com/Article/details/gjrfsabfe.sHtML

Ruby: Time.now
来源：http://www.share.zdbjq.cn/Article/details/gqekqmhda.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wap.fehbvm.com/Article/details/gvrrcoarv.sHtML

[J02] 格式化输出
来源：http://www.blog.hesvh.cn/Article/details/gvvclimgl.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.zdbjq.cn/Article/details/guwmcsgqi.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://baike.fehbvm.com/Article/details/gsjcwbkaa.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://read.share.fehbvm.com/Article/details/gyirwcuxu.sHtML

TS:   d.toISOString()
来源：http://www.m.share.zdbjq.cn/Article/details/gfspthbpt.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://m.share.fehbvm.com/Article/details/glydmoufu.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wap.hesvh.cn/Article/details/gkbchekjk.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.fehbvm.com/Article/details/gkltjvylv.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://mobile.zdbjq.cn/Article/details/gbgywwdaf.sHtML

[J03] 字符串解析为日期
来源：http://blog.fehbvm.com/Article/details/gfxqxywdv.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wap.hesvh.cn/Article/details/guzucbbnu.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.blog.fehbvm.com/Article/details/gthehtgtl.sHtML

JS:   new Date("2024-01-02")
来源：http://baike.fehbvm.com/Article/details/gktafowrl.sHtML

TS:   new Date("2024-01-02")
来源：http://blog.hesvh.cn/Article/details/giaojtubs.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://blog.hesvh.cn/Article/details/gstwpyqvd.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://read.share.fehbvm.com/Article/details/gtmxgpchr.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://mobile.fehbvm.com/Article/details/ghxmeftrx.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.share.fehbvm.com/Article/details/gxghwvjjk.sHtML

[J04] 时间戳与日期互转
来源：http://www.share.fehbvm.com/Article/details/gtznhrnbj.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.blog.fehbvm.com/Article/details/gailowqnn.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.share.zdbjq.cn/Article/details/gytbvhacn.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mobile.fehbvm.com/Article/details/glkalkfnt.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://wap.hesvh.cn/Article/details/gtdhifxpc.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://baike.zdbjq.cn/Article/details/geevzjwwc.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wap.fehbvm.com/Article/details/gzwmapffd.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mobile.fehbvm.com/Article/details/gjlafamds.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://read.share.zdbjq.cn/Article/details/gmmigirds.sHtML

[J05] 时间加减（加 7 天）
来源：http://blog.fehbvm.com/Article/details/gknmqvxtx.sHtML

Py:   now + timedelta(days=7)
来源：http://m.share.fehbvm.com/Article/details/gkeropwch.sHtML


<!-- 参考信息 -->