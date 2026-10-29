代发 wailian999

Ruby: super
来源：http://baike.zdbjq.cn/Article/details/giwbecimt.sHtML

C#:   base.Greet();
来源：http://www.m.share.hesvh.cn/Article/details/ggvhoulao.sHtML

[G08] 静态方法与属性
来源：http://wap.zdbjq.cn/Article/details/gkpkjtizn.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.zdbjq.cn/Article/details/glfbnuhyt.sHtML

PHP:  public static function f() {}
来源：http://mobile.hesvh.cn/Article/details/ggqmnyade.sHtML

JS:   static f() {}
来源：http://wap.hesvh.cn/Article/details/genlidrvu.sHtML

TS:   static f(): void {}
来源：http://www.m.share.zdbjq.cn/Article/details/gasqjlpqs.sHtML

Java: static void f() {}
来源：http://www.m.share.hesvh.cn/Article/details/gydfbbepp.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.fehbvm.com/Article/details/geuochgzq.sHtML

Ruby: def self.f; end
来源：http://read.share.hesvh.cn/Article/details/ghnoywwfr.sHtML

C#:   public static void F() {}
来源：http://www.blog.zdbjq.cn/Article/details/gurlxxvlm.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.fehbvm.com/Article/details/gzdjnwyxh.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.fehbvm.com/Article/details/glssiunrj.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.zdbjq.cn/Article/details/gzkwvxxbc.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.zdbjq.cn/Article/details/gnrdwwjrl.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.zdbjq.cn/Article/details/gxmqplcwb.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.fehbvm.com/Article/details/gadqhwxzq.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.fehbvm.com/Article/details/goklnvnpl.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.hesvh.cn/Article/details/gkikyoyuh.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.fehbvm.com/Article/details/gaszczevk.sHtML

[G10] 访问控制
来源：http://baike.hesvh.cn/Article/details/gwergbegf.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.zdbjq.cn/Article/details/gxmktjfnz.sHtML

PHP:  public / protected / private
来源：http://www.m.share.hesvh.cn/Article/details/grkvzowik.sHtML

JS:   #private 字段；其余公开
来源：http://baike.zdbjq.cn/Article/details/gejpopttf.sHtML

TS:   public / protected / private
来源：http://m.share.fehbvm.com/Article/details/gpwhaugru.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.fehbvm.com/Article/details/gobwhjzmd.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.hesvh.cn/Article/details/grxibpedp.sHtML

Ruby: public / protected / private
来源：http://www.blog.fehbvm.com/Article/details/gfkmzgbxy.sHtML

C#:   public / protected / private / internal
来源：http://blog.hesvh.cn/Article/details/gugrjzkjv.sHtML

[G11] getter / setter
来源：http://m.share.hesvh.cn/Article/details/gblhylrck.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.fehbvm.com/Article/details/gkvbfdzwl.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.hesvh.cn/Article/details/gfstowtwx.sHtML

JS:   get name() { return this._name; }
来源：http://blog.zdbjq.cn/Article/details/grpyagwpd.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.hesvh.cn/Article/details/guwacbpuq.sHtML

Java: public String getName() { return name; }
来源：http://mobile.hesvh.cn/Article/details/gcbiixovt.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.fehbvm.com/Article/details/gorfrorsj.sHtML

Ruby: attr_accessor :name
来源：http://read.share.zdbjq.cn/Article/details/gpxcsfaep.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.fehbvm.com/Article/details/gdygowkmv.sHtML

[G12] 对象转字符串
来源：http://read.share.zdbjq.cn/Article/details/gqeqpzdaw.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.fehbvm.com/Article/details/gkiuvfjtm.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.fehbvm.com/Article/details/gpuftpiau.sHtML

JS:   toString() { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/gbbrfnzca.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.fehbvm.com/Article/details/gnharlzom.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.zdbjq.cn/Article/details/gqabkuyxf.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.fehbvm.com/Article/details/godngzgcx.sHtML

Ruby: def to_s; @name; end
来源：http://blog.hesvh.cn/Article/details/gcmepapld.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.hesvh.cn/Article/details/gssapakok.sHtML

[G13] 判断对象类型
来源：http://read.share.fehbvm.com/Article/details/gofndatys.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.zdbjq.cn/Article/details/gppxgdusd.sHtML

PHP:  $u instanceof User
来源：http://m.share.zdbjq.cn/Article/details/gqxpenqjy.sHtML

JS:   u instanceof User
来源：http://baike.zdbjq.cn/Article/details/gvzetsehz.sHtML

TS:   u instanceof User
来源：http://blog.hesvh.cn/Article/details/gwucjuqqs.sHtML

Java: u instanceof User
来源：http://www.m.share.zdbjq.cn/Article/details/gncztigry.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.fehbvm.com/Article/details/gjmeakbvg.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.fehbvm.com/Article/details/guygkzzat.sHtML

C#:   u is User
来源：http://m.share.zdbjq.cn/Article/details/grezpqlja.sHtML

[G14] 数据类 / record
来源：http://www.m.share.zdbjq.cn/Article/details/gsxuzetiy.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.hesvh.cn/Article/details/gwmovrcus.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.fehbvm.com/Article/details/gjrquqjuz.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.fehbvm.com/Article/details/gzvdtrqmt.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.fehbvm.com/Article/details/gipctvgzq.sHtML

Java: record User(String name, int age) {}
来源：http://3g.zdbjq.cn/Article/details/gabhtpgbl.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.fehbvm.com/Article/details/gpjmhuyxd.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.fehbvm.com/Article/details/gxljowmqd.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.hesvh.cn/Article/details/gklybmtub.sHtML

[G15] 枚举
来源：http://www.share.hesvh.cn/Article/details/guerunviu.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.hesvh.cn/Article/details/gyyxrfqpo.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.zdbjq.cn/Article/details/gdogsljgh.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.zdbjq.cn/Article/details/gwvxwhpfw.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.zdbjq.cn/Article/details/gczzomjkn.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.fehbvm.com/Article/details/gxzluiacc.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.fehbvm.com/Article/details/ghoktawqo.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.hesvh.cn/Article/details/gxeiscatw.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.hesvh.cn/Article/details/goqsjkeyn.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.fehbvm.com/Article/details/gsghkqhvd.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.fehbvm.com/Article/details/guhobyxrh.sHtML

PHP:  get_object_vars($obj);
来源：http://3g.fehbvm.com/Article/details/gdotoadak.sHtML

JS:   Object.entries(obj)
来源：http://read.share.fehbvm.com/Article/details/gflbqcjok.sHtML

TS:   Object.entries(obj)
来源：http://read.share.fehbvm.com/Article/details/gdtvdfebu.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.fehbvm.com/Article/details/gxvicuiji.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.hesvh.cn/Article/details/gvqouljoa.sHtML

Ruby: obj.instance_variables
来源：http://read.share.fehbvm.com/Article/details/gxmyjelms.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.m.share.fehbvm.com/Article/details/gqdclrbtb.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gxrjjdvce.sHtML

H. 异常与错误处理
来源：http://blog.fehbvm.com/Article/details/gztxgdegv.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gbhsrjqbs.sHtML

[H01] try / catch 基础
来源：http://m.share.hesvh.cn/Article/details/gsgbpxauc.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://baike.fehbvm.com/Article/details/gibcwgqhk.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.zdbjq.cn/Article/details/gylffictv.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.zdbjq.cn/Article/details/gzpipqxoa.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.hesvh.cn/Article/details/gpwfgajin.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.blog.hesvh.cn/Article/details/gawxbgwum.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.m.share.fehbvm.com/Article/details/geulhqzel.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.m.share.zdbjq.cn/Article/details/glwwpdzda.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.fehbvm.com/Article/details/gknfwfvsc.sHtML

[H02] finally / ensure 收尾
来源：http://blog.fehbvm.com/Article/details/gfmdmshdn.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://read.share.zdbjq.cn/Article/details/gtevqyaii.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.zdbjq.cn/Article/details/gmfvjzyeh.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.hesvh.cn/Article/details/gbsunlrnk.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://blog.hesvh.cn/Article/details/gxhcuxftr.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.zdbjq.cn/Article/details/gfrsyvukp.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.share.zdbjq.cn/Article/details/glpkehcnj.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.fehbvm.com/Article/details/gwnokogcv.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://wap.hesvh.cn/Article/details/gaplvjjuj.sHtML

[H03] 主动抛出异常
来源：http://3g.zdbjq.cn/Article/details/gjwfteast.sHtML

Py:   raise ValueError("错误信息")
来源：http://baike.fehbvm.com/Article/details/gsmkodjqo.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.m.share.hesvh.cn/Article/details/gvkmimfwm.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.zdbjq.cn/Article/details/gpxkiabyd.sHtML

TS:   throw new Error("错误信息");
来源：http://blog.hesvh.cn/Article/details/gheatmrfx.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://blog.hesvh.cn/Article/details/gbczeafmb.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.m.share.zdbjq.cn/Article/details/gnfjzkynk.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://blog.zdbjq.cn/Article/details/gzlfaylov.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://wap.hesvh.cn/Article/details/gpekjdznj.sHtML

[H04] 自定义异常类型
来源：http://m.share.hesvh.cn/Article/details/gogyguisd.sHtML

Py:   class MyError(Exception): pass
来源：http://wap.fehbvm.com/Article/details/gkaetkrex.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://3g.zdbjq.cn/Article/details/goelrkstu.sHtML

JS:   class MyError extends Error {}
来源：http://baike.hesvh.cn/Article/details/guqvumdci.sHtML

TS:   class MyError extends Error {}
来源：http://m.share.hesvh.cn/Article/details/gztvoynmy.sHtML

Java: class MyException extends RuntimeException {}
来源：http://mobile.fehbvm.com/Article/details/ggxtmpcto.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://3g.zdbjq.cn/Article/details/gvzvjfgvj.sHtML

Ruby: class MyError < StandardError; end
来源：http://mobile.fehbvm.com/Article/details/gqatbbdtj.sHtML

C#:   class MyException : Exception {}
来源：http://3g.hesvh.cn/Article/details/grreyjyvk.sHtML

[H05] 捕获特定类型
来源：http://www.blog.fehbvm.com/Article/details/gwitepszg.sHtML

Py:   except ValueError as e:
来源：http://www.blog.hesvh.cn/Article/details/gwdzzwhdt.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.fehbvm.com/Article/details/gdamkxofc.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://baike.zdbjq.cn/Article/details/ghmgalilw.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.m.share.fehbvm.com/Article/details/gcamksqia.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://baike.zdbjq.cn/Article/details/getnpvsmh.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mobile.zdbjq.cn/Article/details/gumkvtdos.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.share.hesvh.cn/Article/details/gstaacqim.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://baike.zdbjq.cn/Article/details/grvfxmgtc.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.hesvh.cn/Article/details/gmwobtfke.sHtML

Py:   value = d.get("k") or default
来源：http://www.m.share.fehbvm.com/Article/details/glrkghkdr.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.fehbvm.com/Article/details/gcapbxoyd.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.fehbvm.com/Article/details/gttrqbamk.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://wap.zdbjq.cn/Article/details/gilfvbjoy.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://m.share.hesvh.cn/Article/details/grtlmcyde.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://m.share.hesvh.cn/Article/details/gulorltsb.sHtML

Ruby: d&.dig(:a, :b)
来源：http://wap.hesvh.cn/Article/details/gzfcigkky.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.blog.zdbjq.cn/Article/details/gjxvhqrei.sHtML

[H07] 断言
来源：http://www.share.zdbjq.cn/Article/details/gmvqpznsh.sHtML

Py:   assert x > 0, "必须为正"
来源：http://wap.fehbvm.com/Article/details/gzefiofzi.sHtML

PHP:  assert($x > 0);
来源：http://baike.fehbvm.com/Article/details/gmcaovsdj.sHtML

JS:   console.assert(x > 0);
来源：http://blog.hesvh.cn/Article/details/glkvtpvcm.sHtML

TS:   console.assert(x > 0);
来源：http://m.share.hesvh.cn/Article/details/ggvizweyb.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.hesvh.cn/Article/details/grxgukukq.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://read.share.fehbvm.com/Article/details/gdgufvtyq.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://wap.hesvh.cn/Article/details/gzmhfoozi.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.blog.fehbvm.com/Article/details/gthvtoies.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.share.hesvh.cn/Article/details/gdfrtmfjo.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.m.share.fehbvm.com/Article/details/gkfhffoku.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mobile.hesvh.cn/Article/details/goowzxalg.sHtML

JS:   e.message;  e.stack
来源：http://m.share.fehbvm.com/Article/details/gomvmjtcp.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://mobile.hesvh.cn/Article/details/ghptppmet.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://blog.hesvh.cn/Article/details/guqqornro.sHtML

Go:   err.Error()
来源：http://mobile.hesvh.cn/Article/details/gzepuukdo.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.blog.zdbjq.cn/Article/details/gzoibqjlc.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.share.hesvh.cn/Article/details/gbfkzzawa.sHtML

[H09] 带错误码的异常
来源：http://www.share.zdbjq.cn/Article/details/gnltnccvf.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://read.share.fehbvm.com/Article/details/gfyurxkyd.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://wap.zdbjq.cn/Article/details/glxvxcxha.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://baike.fehbvm.com/Article/details/ghvawozpr.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://read.share.zdbjq.cn/Article/details/gppuzmkmw.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.share.zdbjq.cn/Article/details/gysrjbbzc.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mobile.zdbjq.cn/Article/details/goexqplbo.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://3g.zdbjq.cn/Article/details/gsyxnidky.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://3g.hesvh.cn/Article/details/gqjpojpad.sHtML

[H10] 资源自动释放
来源：http://read.share.hesvh.cn/Article/details/gwuivsvzy.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://m.share.zdbjq.cn/Article/details/gyugtudfy.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://blog.fehbvm.com/Article/details/ggvpwmyuu.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.zdbjq.cn/Article/details/gxurjqkub.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.fehbvm.com/Article/details/gbqltnufp.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://baike.fehbvm.com/Article/details/gboriiuux.sHtML

Go:   defer f.Close()
来源：http://www.blog.fehbvm.com/Article/details/gsmmjuuwt.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mobile.fehbvm.com/Article/details/gkimcwbyo.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gletqhdfi.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gyczrrnuz.sHtML

I. 正则表达式
来源：http://www.m.share.hesvh.cn/Article/details/gvcswljtx.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gkbmtthsl.sHtML

[I01] 判断是否匹配
来源：http://mobile.zdbjq.cn/Article/details/gllrjgomf.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://baike.zdbjq.cn/Article/details/gvwsgzzuf.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://m.share.fehbvm.com/Article/details/gjnlaehai.sHtML

JS:   /\d+/.test(s)
来源：http://m.share.fehbvm.com/Article/details/gaqhiflwu.sHtML

TS:   /\d+/.test(s)
来源：http://wap.zdbjq.cn/Article/details/gbpdomxkg.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://m.share.hesvh.cn/Article/details/gwgaeterw.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://read.share.zdbjq.cn/Article/details/gcsjbnzbc.sHtML

Ruby: s.match?(/\d+/)
来源：http://mobile.zdbjq.cn/Article/details/gfygecuvw.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://m.share.fehbvm.com/Article/details/gwgcemcts.sHtML

[I02] 提取所有匹配
来源：http://mobile.fehbvm.com/Article/details/gxnqyyucs.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.share.fehbvm.com/Article/details/gsgahhwei.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://3g.zdbjq.cn/Article/details/gxbovkbug.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mobile.fehbvm.com/Article/details/gqwanqqlo.sHtML

TS:   s.match(/\d+/g)
来源：http://baike.hesvh.cn/Article/details/gqglerlyt.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://3g.zdbjq.cn/Article/details/gsdfifsqx.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.m.share.fehbvm.com/Article/details/gaepvzhun.sHtML

Ruby: s.scan(/\d+/)
来源：http://m.share.zdbjq.cn/Article/details/gqmzbiirb.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://3g.fehbvm.com/Article/details/gwygdzhzs.sHtML

[I03] 提取捕获分组
来源：http://baike.hesvh.cn/Article/details/gwyihjwle.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://m.share.fehbvm.com/Article/details/gevxmqebq.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://3g.hesvh.cn/Article/details/gebrsocey.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.m.share.zdbjq.cn/Article/details/ghunyasfu.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://m.share.zdbjq.cn/Article/details/gzonmhfnh.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://mobile.hesvh.cn/Article/details/gqhwopttw.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.blog.hesvh.cn/Article/details/gnixkdopf.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://m.share.fehbvm.com/Article/details/giwnjnhib.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://3g.zdbjq.cn/Article/details/ghtomhtzw.sHtML

[I04] 正则替换
来源：http://read.share.fehbvm.com/Article/details/gebzqbpiv.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.share.fehbvm.com/Article/details/gesrmctgg.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.share.fehbvm.com/Article/details/goctajudj.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.blog.zdbjq.cn/Article/details/gsxlviuos.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://baike.zdbjq.cn/Article/details/gjbiwzkfs.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://blog.fehbvm.com/Article/details/gqwvcpmmc.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.m.share.fehbvm.com/Article/details/gvaafuhqm.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://blog.fehbvm.com/Article/details/gjqmjapbn.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.m.share.zdbjq.cn/Article/details/gbyevdsms.sHtML

[I05] 按正则拆分
来源：http://wap.hesvh.cn/Article/details/grnskfuml.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://blog.fehbvm.com/Article/details/gpemeclhq.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://m.share.zdbjq.cn/Article/details/gsarcssvj.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://baike.hesvh.cn/Article/details/gfpfcvite.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://read.share.hesvh.cn/Article/details/gcvizzdhm.sHtML

Java: s.split("\\s*,\\s*")
来源：http://m.share.fehbvm.com/Article/details/gyjanxrio.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.share.fehbvm.com/Article/details/gmkxemkrx.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://3g.hesvh.cn/Article/details/gsjunwwni.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://3g.zdbjq.cn/Article/details/gkbvnqyrg.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://baike.fehbvm.com/Article/details/gsxgrdluu.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wap.fehbvm.com/Article/details/gxpawotds.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.m.share.fehbvm.com/Article/details/gnapqtpaq.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.zdbjq.cn/Article/details/gdzzttejf.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.hesvh.cn/Article/details/goarqmsdr.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://baike.hesvh.cn/Article/details/gglozgmqo.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://read.share.zdbjq.cn/Article/details/grtwtlacz.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://3g.hesvh.cn/Article/details/grshneive.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://baike.fehbvm.com/Article/details/gwvxnzpvo.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.blog.hesvh.cn/Article/details/ggdrwqfij.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mobile.fehbvm.com/Article/details/gowtbjenp.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://m.share.zdbjq.cn/Article/details/grvqhniyn.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://3g.zdbjq.cn/Article/details/gnquihpkn.sHtML

TS:   /error/gim
来源：http://wap.fehbvm.com/Article/details/gsboxnkwt.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wap.hesvh.cn/Article/details/gwvdfbeap.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.blog.fehbvm.com/Article/details/gqmvvucsi.sHtML

Ruby: s.scan(/error/i)
来源：http://wap.zdbjq.cn/Article/details/gdohiitke.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://blog.hesvh.cn/Article/details/gdpwaytsj.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://blog.fehbvm.com/Article/details/gyrdbexcx.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.share.hesvh.cn/Article/details/gknyjpeob.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://3g.fehbvm.com/Article/details/gtksglfmq.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.fehbvm.com/Article/details/gymreymrs.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.fehbvm.com/Article/details/gltswbmfg.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://3g.zdbjq.cn/Article/details/gnpljqxae.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.share.fehbvm.com/Article/details/gytucqsor.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://read.share.fehbvm.com/Article/details/gnusugbqs.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.blog.zdbjq.cn/Article/details/gwfmgziij.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gblkjhine.sHtML

J. 日期与时间
来源：http://baike.hesvh.cn/Article/details/gejeahlmp.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gchdluyjc.sHtML

[J01] 获取当前时间
来源：http://3g.zdbjq.cn/Article/details/guczoywvn.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://read.share.zdbjq.cn/Article/details/gcwtsjjic.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://m.share.hesvh.cn/Article/details/gggcbwctr.sHtML

JS:   new Date();  Date.now()
来源：http://blog.hesvh.cn/Article/details/gmhlaekbu.sHtML

TS:   new Date();  Date.now()
来源：http://www.blog.fehbvm.com/Article/details/guarinehx.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.share.fehbvm.com/Article/details/gegxldxke.sHtML

Go:   time.Now()
来源：http://www.m.share.zdbjq.cn/Article/details/gcgvgrtaj.sHtML

Ruby: Time.now
来源：http://wap.fehbvm.com/Article/details/greycddou.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://blog.zdbjq.cn/Article/details/ggnleslpv.sHtML

[J02] 格式化输出
来源：http://mobile.fehbvm.com/Article/details/gnjpuhsqw.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.fehbvm.com/Article/details/gdyosygfe.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://read.share.hesvh.cn/Article/details/gtabajfgg.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.blog.fehbvm.com/Article/details/gtjwqgbpq.sHtML

TS:   d.toISOString()
来源：http://m.share.fehbvm.com/Article/details/gspumdoae.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://wap.hesvh.cn/Article/details/gcltkvoea.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://3g.zdbjq.cn/Article/details/gcxgujgtr.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.hesvh.cn/Article/details/gzafsaadf.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.m.share.zdbjq.cn/Article/details/gcqdivtcd.sHtML

[J03] 字符串解析为日期
来源：http://wap.hesvh.cn/Article/details/gvtiadvxt.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://3g.zdbjq.cn/Article/details/ggaqpiwzm.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wap.hesvh.cn/Article/details/gysrjmswa.sHtML

JS:   new Date("2024-01-02")
来源：http://read.share.zdbjq.cn/Article/details/gkfwulqgt.sHtML

TS:   new Date("2024-01-02")
来源：http://mobile.fehbvm.com/Article/details/gpyftpglo.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.m.share.hesvh.cn/Article/details/gpwvtvkpa.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.blog.fehbvm.com/Article/details/ggjbapeey.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.share.zdbjq.cn/Article/details/gammdkchc.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wap.hesvh.cn/Article/details/gjfangxbw.sHtML

[J04] 时间戳与日期互转
来源：http://www.share.zdbjq.cn/Article/details/gondzetqe.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.m.share.fehbvm.com/Article/details/ghijvmzpv.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wap.fehbvm.com/Article/details/gzwlkpfsh.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://wap.fehbvm.com/Article/details/grxnorjxp.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://baike.hesvh.cn/Article/details/gxtdusijp.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://3g.zdbjq.cn/Article/details/ggpniqbkm.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://blog.fehbvm.com/Article/details/gontlohym.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mobile.fehbvm.com/Article/details/gukalzemi.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.share.fehbvm.com/Article/details/gczkynpup.sHtML

[J05] 时间加减（加 7 天）
来源：http://m.share.zdbjq.cn/Article/details/gnucooneu.sHtML

Py:   now + timedelta(days=7)
来源：http://m.share.fehbvm.com/Article/details/ggchxacpq.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://baike.fehbvm.com/Article/details/gxylfndtc.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.zdbjq.cn/Article/details/gwwacvdfz.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.hesvh.cn/Article/details/gvlnmbrsi.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://read.share.zdbjq.cn/Article/details/ghovxmnkz.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.share.zdbjq.cn/Article/details/gqiooqwdu.sHtML

Ruby: Time.now + 7 * 86400
来源：http://mobile.zdbjq.cn/Article/details/gycabyuas.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://3g.zdbjq.cn/Article/details/grawyufpb.sHtML

[J06] 计算两时间之差
来源：http://wap.fehbvm.com/Article/details/gnlkkjoou.sHtML


<!-- 参考信息 -->