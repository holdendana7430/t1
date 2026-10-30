代发 wailian999

TS:   greet(): string { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/ghrwndcel.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/gfbkaakds.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.fehbvm.com/Article/details/ghftlhnpt.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.hesvh.cn/Article/details/grweizdjo.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.zdbjq.cn/Article/details/gcbhigshu.sHtML

[G07] 调用父类方法
来源：http://www.share.zdbjq.cn/Article/details/gdlkrpglz.sHtML

Py:   super().greet()
来源：http://wap.hesvh.cn/Article/details/gttjgqtui.sHtML

PHP:  parent::greet();
来源：http://3g.hesvh.cn/Article/details/gyfkszqjp.sHtML

JS:   super.greet();
来源：http://www.m.share.hesvh.cn/Article/details/gladxkbas.sHtML

TS:   super.greet();
来源：http://www.share.fehbvm.com/Article/details/gqkrvggja.sHtML

Java: super.greet();
来源：http://blog.hesvh.cn/Article/details/gafunkgot.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.hesvh.cn/Article/details/gtoigglso.sHtML

Ruby: super
来源：http://baike.hesvh.cn/Article/details/gxgidyfyk.sHtML

C#:   base.Greet();
来源：http://wap.zdbjq.cn/Article/details/gxoagdcsi.sHtML

[G08] 静态方法与属性
来源：http://baike.zdbjq.cn/Article/details/gvrewzksz.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.zdbjq.cn/Article/details/gczzgditp.sHtML

PHP:  public static function f() {}
来源：http://wap.fehbvm.com/Article/details/gkwguwjra.sHtML

JS:   static f() {}
来源：http://www.m.share.zdbjq.cn/Article/details/ggbubrpai.sHtML

TS:   static f(): void {}
来源：http://baike.zdbjq.cn/Article/details/gnddikoox.sHtML

Java: static void f() {}
来源：http://www.m.share.hesvh.cn/Article/details/ghbxwlprh.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.fehbvm.com/Article/details/gmcqfgmga.sHtML

Ruby: def self.f; end
来源：http://m.share.fehbvm.com/Article/details/gaqlvblgm.sHtML

C#:   public static void F() {}
来源：http://mobile.fehbvm.com/Article/details/geawtwxax.sHtML

[G09] 接口 / 抽象类
来源：http://wap.hesvh.cn/Article/details/gnfkdilnl.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.fehbvm.com/Article/details/godxhnvxc.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.zdbjq.cn/Article/details/gpkedgnjy.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.hesvh.cn/Article/details/gxpcqgfef.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.zdbjq.cn/Article/details/glmwfnkrh.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.zdbjq.cn/Article/details/grhkrvrlg.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.zdbjq.cn/Article/details/gfldxjjdi.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.zdbjq.cn/Article/details/gnmoktzwt.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.zdbjq.cn/Article/details/ggwqnqtgp.sHtML

[G10] 访问控制
来源：http://mobile.hesvh.cn/Article/details/glffktidl.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.zdbjq.cn/Article/details/gktyranrh.sHtML

PHP:  public / protected / private
来源：http://3g.zdbjq.cn/Article/details/grzeuxgwb.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.fehbvm.com/Article/details/gpyufqcnh.sHtML

TS:   public / protected / private
来源：http://www.share.zdbjq.cn/Article/details/gxygjuocg.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.hesvh.cn/Article/details/gehevqszg.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.fehbvm.com/Article/details/gsbqkhjny.sHtML

Ruby: public / protected / private
来源：http://blog.hesvh.cn/Article/details/gqpyuruxg.sHtML

C#:   public / protected / private / internal
来源：http://baike.fehbvm.com/Article/details/gojhvrjvh.sHtML

[G11] getter / setter
来源：http://blog.zdbjq.cn/Article/details/gnyzlvtyx.sHtML

Py:   @property 与 @x.setter
来源：http://blog.zdbjq.cn/Article/details/gzyebrhcv.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.hesvh.cn/Article/details/giivplecn.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.fehbvm.com/Article/details/geqodoxze.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.zdbjq.cn/Article/details/gpqjamstr.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gacfptgkh.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.fehbvm.com/Article/details/gnymowiae.sHtML

Ruby: attr_accessor :name
来源：http://m.share.zdbjq.cn/Article/details/gcyiugugd.sHtML

C#:   public string Name { get; set; }
来源：http://wap.fehbvm.com/Article/details/gtwxjpaxz.sHtML

[G12] 对象转字符串
来源：http://blog.fehbvm.com/Article/details/gjobwmekl.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.hesvh.cn/Article/details/gcqgcqshu.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.hesvh.cn/Article/details/gyvcwgbbh.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/gpcgdodyl.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.fehbvm.com/Article/details/gvkkaclmk.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.zdbjq.cn/Article/details/gfgnrvjvn.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.fehbvm.com/Article/details/gtzagwhbp.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.hesvh.cn/Article/details/gedfpradm.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.fehbvm.com/Article/details/gikunvwop.sHtML

[G13] 判断对象类型
来源：http://3g.fehbvm.com/Article/details/gdazjfnco.sHtML

Py:   isinstance(u, User)
来源：http://3g.zdbjq.cn/Article/details/glczcqeoe.sHtML

PHP:  $u instanceof User
来源：http://blog.hesvh.cn/Article/details/gzgrgzsip.sHtML

JS:   u instanceof User
来源：http://www.blog.fehbvm.com/Article/details/gshncfyie.sHtML

TS:   u instanceof User
来源：http://3g.fehbvm.com/Article/details/gwdlnwhis.sHtML

Java: u instanceof User
来源：http://baike.fehbvm.com/Article/details/gggmbcyhj.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.share.fehbvm.com/Article/details/goheebqyg.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.zdbjq.cn/Article/details/gninywxfl.sHtML

C#:   u is User
来源：http://baike.zdbjq.cn/Article/details/gwzrpamue.sHtML

[G14] 数据类 / record
来源：http://read.share.zdbjq.cn/Article/details/grvgtgcdu.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.zdbjq.cn/Article/details/guqcyymjm.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.zdbjq.cn/Article/details/glwddfhvb.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.hesvh.cn/Article/details/gbhxryvqw.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.hesvh.cn/Article/details/gqumazrko.sHtML

Java: record User(String name, int age) {}
来源：http://blog.zdbjq.cn/Article/details/gfnkodivm.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.fehbvm.com/Article/details/gvxmxjfva.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.fehbvm.com/Article/details/gnthtjxgd.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.zdbjq.cn/Article/details/ghtujtgyy.sHtML

[G15] 枚举
来源：http://www.m.share.zdbjq.cn/Article/details/ggftzlpko.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.hesvh.cn/Article/details/gvnxcibas.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.zdbjq.cn/Article/details/gcxhmavlg.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.zdbjq.cn/Article/details/gheeinhbj.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.fehbvm.com/Article/details/gmndjdmsm.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.fehbvm.com/Article/details/ggzbwebjc.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.hesvh.cn/Article/details/gjunfksra.sHtML

Ruby: Color = %i[red green].freeze
来源：http://read.share.fehbvm.com/Article/details/gyfccofra.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.fehbvm.com/Article/details/ghvpgunpx.sHtML

[G16] 对象转数组 / 字典
来源：http://www.blog.zdbjq.cn/Article/details/gxukamnzm.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://3g.zdbjq.cn/Article/details/golmkiehj.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.fehbvm.com/Article/details/gfriqesbk.sHtML

JS:   Object.entries(obj)
来源：http://mobile.zdbjq.cn/Article/details/gwdvdqdym.sHtML

TS:   Object.entries(obj)
来源：http://m.share.zdbjq.cn/Article/details/ggufwzdij.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.fehbvm.com/Article/details/gmhpkqxfp.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.hesvh.cn/Article/details/ghkdkgbxt.sHtML

Ruby: obj.instance_variables
来源：http://mobile.zdbjq.cn/Article/details/gptiwxkbk.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://blog.hesvh.cn/Article/details/gxnitvoxc.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gsldyvuem.sHtML

H. 异常与错误处理
来源：http://m.share.zdbjq.cn/Article/details/gturistvm.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/guqqrcbze.sHtML

[H01] try / catch 基础
来源：http://read.share.zdbjq.cn/Article/details/grrbfmhci.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.zdbjq.cn/Article/details/grkdiijjt.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wap.zdbjq.cn/Article/details/gnmpxclnq.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.fehbvm.com/Article/details/gmgqmtckp.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://m.share.fehbvm.com/Article/details/gfdzbizmn.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.fehbvm.com/Article/details/gwkutwrix.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.blog.zdbjq.cn/Article/details/gjtmczhgz.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.m.share.hesvh.cn/Article/details/gxgiqajqi.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://blog.zdbjq.cn/Article/details/gosmeqaeg.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.zdbjq.cn/Article/details/gpwlmrynn.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.m.share.fehbvm.com/Article/details/ggxuwnbzt.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/gemrjhmcd.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://read.share.zdbjq.cn/Article/details/gmgbzfgeb.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.fehbvm.com/Article/details/gozrzepkj.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.share.fehbvm.com/Article/details/gvfbzsccg.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.hesvh.cn/Article/details/gmxrrxage.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.m.share.hesvh.cn/Article/details/gflcivims.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://m.share.fehbvm.com/Article/details/gkngvqkrq.sHtML

[H03] 主动抛出异常
来源：http://www.m.share.hesvh.cn/Article/details/grfytzahj.sHtML

Py:   raise ValueError("错误信息")
来源：http://baike.zdbjq.cn/Article/details/gderzewba.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.fehbvm.com/Article/details/goiwvebjd.sHtML

JS:   throw new Error("错误信息");
来源：http://blog.zdbjq.cn/Article/details/ghccszstt.sHtML

TS:   throw new Error("错误信息");
来源：http://www.m.share.zdbjq.cn/Article/details/glvvwdice.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://baike.zdbjq.cn/Article/details/gtqltooub.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://read.share.zdbjq.cn/Article/details/gbesrikyg.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://mobile.hesvh.cn/Article/details/gtgchiotn.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/gnkzvqgvy.sHtML

[H04] 自定义异常类型
来源：http://baike.hesvh.cn/Article/details/gwwivtrgb.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.zdbjq.cn/Article/details/geytlymos.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://read.share.zdbjq.cn/Article/details/gycrhxshq.sHtML

JS:   class MyError extends Error {}
来源：http://wap.hesvh.cn/Article/details/gjbqnrmrn.sHtML

TS:   class MyError extends Error {}
来源：http://mobile.zdbjq.cn/Article/details/gfgeavuvm.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.hesvh.cn/Article/details/gowukbygk.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://baike.fehbvm.com/Article/details/gbntmcrpk.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.zdbjq.cn/Article/details/gcxxvduyt.sHtML

C#:   class MyException : Exception {}
来源：http://read.share.zdbjq.cn/Article/details/gynlrcppp.sHtML

[H05] 捕获特定类型
来源：http://www.m.share.hesvh.cn/Article/details/gnqwgecsh.sHtML

Py:   except ValueError as e:
来源：http://www.share.fehbvm.com/Article/details/gnwveczxc.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.blog.hesvh.cn/Article/details/gtbvgznaf.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://blog.fehbvm.com/Article/details/ggymaughc.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://mobile.zdbjq.cn/Article/details/ghxwpjgce.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://mobile.fehbvm.com/Article/details/gztfuxvwj.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://blog.zdbjq.cn/Article/details/gbushwfzz.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.m.share.hesvh.cn/Article/details/gwnwfcntk.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://baike.hesvh.cn/Article/details/ghxdwvhsc.sHtML

[H06] 可选值 / 空值安全访问
来源：http://baike.fehbvm.com/Article/details/gnhaboboz.sHtML

Py:   value = d.get("k") or default
来源：http://www.share.fehbvm.com/Article/details/gekmkjxsu.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://3g.hesvh.cn/Article/details/gwgijgrcg.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://mobile.zdbjq.cn/Article/details/gebyqcgzj.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://mobile.zdbjq.cn/Article/details/gqszjkgni.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://read.share.fehbvm.com/Article/details/gudstabyv.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://read.share.zdbjq.cn/Article/details/gkfblgrao.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.share.zdbjq.cn/Article/details/givtrkxfb.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.blog.fehbvm.com/Article/details/gnjycuzhl.sHtML

[H07] 断言
来源：http://mobile.hesvh.cn/Article/details/gdzywfwua.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.m.share.zdbjq.cn/Article/details/gyrtyleui.sHtML

PHP:  assert($x > 0);
来源：http://mobile.fehbvm.com/Article/details/goyixdoim.sHtML

JS:   console.assert(x > 0);
来源：http://www.share.fehbvm.com/Article/details/gdxeafcix.sHtML

TS:   console.assert(x > 0);
来源：http://3g.fehbvm.com/Article/details/gnvrgxswp.sHtML

Java: assert x > 0 : "必须为正";
来源：http://3g.zdbjq.cn/Article/details/guveqoppl.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://m.share.fehbvm.com/Article/details/ggrmyslqm.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://3g.fehbvm.com/Article/details/gevskfmvx.sHtML

C#:   Debug.Assert(x > 0);
来源：http://read.share.fehbvm.com/Article/details/glmaacxle.sHtML

[H08] 获取错误信息与堆栈
来源：http://m.share.fehbvm.com/Article/details/gpfynylys.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://mobile.hesvh.cn/Article/details/guzxnalcl.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.share.fehbvm.com/Article/details/ghcqrwhjp.sHtML

JS:   e.message;  e.stack
来源：http://www.share.hesvh.cn/Article/details/gzhmrdoui.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://read.share.zdbjq.cn/Article/details/gxwzdnkqe.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://wap.hesvh.cn/Article/details/gyitwbqlc.sHtML

Go:   err.Error()
来源：http://www.m.share.fehbvm.com/Article/details/gdeifswbg.sHtML

Ruby: e.message;  e.backtrace
来源：http://mobile.fehbvm.com/Article/details/gtjzxrttd.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.blog.zdbjq.cn/Article/details/gjazmnwgn.sHtML

[H09] 带错误码的异常
来源：http://www.m.share.zdbjq.cn/Article/details/gabzctgqq.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://3g.fehbvm.com/Article/details/gkmhmnwzp.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://read.share.fehbvm.com/Article/details/gvuvrhujg.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.blog.zdbjq.cn/Article/details/gxvpebnuo.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://3g.fehbvm.com/Article/details/gbamjuklr.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://read.share.zdbjq.cn/Article/details/gwjrlstmb.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://m.share.fehbvm.com/Article/details/gsdbnyvzz.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.blog.hesvh.cn/Article/details/gohkvwkdq.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://wap.zdbjq.cn/Article/details/gkrdslsib.sHtML

[H10] 资源自动释放
来源：http://m.share.hesvh.cn/Article/details/glurkyqhh.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://wap.hesvh.cn/Article/details/gsizveeso.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://baike.zdbjq.cn/Article/details/gvbrdhhuv.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.hesvh.cn/Article/details/gkcjtgbks.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.hesvh.cn/Article/details/gmemnnvsr.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.share.zdbjq.cn/Article/details/ggefsmvwi.sHtML

Go:   defer f.Close()
来源：http://mobile.hesvh.cn/Article/details/gtsqccjfy.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.share.hesvh.cn/Article/details/gpdfwcpqn.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gldsysuyt.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gvfioypeh.sHtML

I. 正则表达式
来源：http://3g.zdbjq.cn/Article/details/gulurhwjm.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gcaeduswy.sHtML

[I01] 判断是否匹配
来源：http://www.share.fehbvm.com/Article/details/giplggdez.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://m.share.fehbvm.com/Article/details/gyqxhkprq.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://read.share.fehbvm.com/Article/details/gchjslils.sHtML

JS:   /\d+/.test(s)
来源：http://read.share.zdbjq.cn/Article/details/garkhjqiv.sHtML

TS:   /\d+/.test(s)
来源：http://mobile.fehbvm.com/Article/details/glghnnyvb.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wap.zdbjq.cn/Article/details/gbeygpdpw.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://3g.hesvh.cn/Article/details/glaeiazrq.sHtML

Ruby: s.match?(/\d+/)
来源：http://read.share.zdbjq.cn/Article/details/gmelpivky.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://read.share.zdbjq.cn/Article/details/gpvsksknq.sHtML

[I02] 提取所有匹配
来源：http://www.share.hesvh.cn/Article/details/gvnojxmoc.sHtML

Py:   re.findall(r"\d+", s)
来源：http://blog.hesvh.cn/Article/details/gpnbopwde.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://3g.hesvh.cn/Article/details/gsvvfexvj.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://baike.zdbjq.cn/Article/details/gafdbiaxs.sHtML

TS:   s.match(/\d+/g)
来源：http://wap.hesvh.cn/Article/details/gibatwjqa.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mobile.fehbvm.com/Article/details/gzdmuyiqu.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://m.share.zdbjq.cn/Article/details/geiqbzvqb.sHtML

Ruby: s.scan(/\d+/)
来源：http://m.share.zdbjq.cn/Article/details/gzarkfuig.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/geahtvzjh.sHtML

[I03] 提取捕获分组
来源：http://mobile.fehbvm.com/Article/details/gxtxorqyv.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.share.hesvh.cn/Article/details/gwwnvknil.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://baike.fehbvm.com/Article/details/glltxdpmh.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.m.share.zdbjq.cn/Article/details/getvazjhz.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://read.share.hesvh.cn/Article/details/guasrqbdg.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://baike.zdbjq.cn/Article/details/gmrjeekcn.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://read.share.fehbvm.com/Article/details/gskpkklfj.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://m.share.fehbvm.com/Article/details/gckfjeqpq.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.share.fehbvm.com/Article/details/gxesgmjdb.sHtML

[I04] 正则替换
来源：http://www.share.hesvh.cn/Article/details/gqkggqams.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://mobile.zdbjq.cn/Article/details/glgiupowc.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://3g.hesvh.cn/Article/details/gredtrztx.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://baike.fehbvm.com/Article/details/gkkdclbmz.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://read.share.hesvh.cn/Article/details/gfhteirce.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://mobile.zdbjq.cn/Article/details/giqyaxvuq.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://m.share.fehbvm.com/Article/details/gfmstmprb.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://blog.hesvh.cn/Article/details/gjoggcbbr.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.m.share.hesvh.cn/Article/details/gwubgyucn.sHtML

[I05] 按正则拆分
来源：http://wap.fehbvm.com/Article/details/gkktbgujq.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.blog.hesvh.cn/Article/details/gqqmcrdey.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wap.hesvh.cn/Article/details/gwfngdzmw.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.blog.zdbjq.cn/Article/details/gykeeaiaq.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://m.share.zdbjq.cn/Article/details/gtfjlyhaf.sHtML

Java: s.split("\\s*,\\s*")
来源：http://baike.fehbvm.com/Article/details/gezktgmtd.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.blog.zdbjq.cn/Article/details/gwlhxwoih.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://blog.fehbvm.com/Article/details/gbctteggq.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://3g.zdbjq.cn/Article/details/gonkccaxe.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://3g.fehbvm.com/Article/details/gqqhbmkvj.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://3g.hesvh.cn/Article/details/gcrskgart.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.m.share.zdbjq.cn/Article/details/gdajlsqdb.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.fehbvm.com/Article/details/gnrtnoqzv.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.fehbvm.com/Article/details/gydwwengy.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://read.share.fehbvm.com/Article/details/gbexcprzp.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.m.share.hesvh.cn/Article/details/gbjrgtdyw.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.share.zdbjq.cn/Article/details/guhgplxkl.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.blog.zdbjq.cn/Article/details/gexbspipv.sHtML

[I07] 忽略大小写与多行模式
来源：http://baike.hesvh.cn/Article/details/gyinsacig.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://m.share.fehbvm.com/Article/details/glxdumooa.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.m.share.fehbvm.com/Article/details/gkjvxilid.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.blog.zdbjq.cn/Article/details/gjtwuugvz.sHtML

TS:   /error/gim
来源：http://read.share.fehbvm.com/Article/details/gqzkqyuse.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.blog.zdbjq.cn/Article/details/gsgwrqjad.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.blog.fehbvm.com/Article/details/geesyjddk.sHtML

Ruby: s.scan(/error/i)
来源：http://3g.hesvh.cn/Article/details/glhmfvgsf.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mobile.fehbvm.com/Article/details/gciiyjoyl.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://mobile.fehbvm.com/Article/details/gozmzqvlb.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://m.share.fehbvm.com/Article/details/gtkkoslal.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://3g.hesvh.cn/Article/details/ginkgztwy.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.zdbjq.cn/Article/details/gqowpfoaz.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.fehbvm.com/Article/details/gismcswvu.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.m.share.zdbjq.cn/Article/details/gwvdusses.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://m.share.zdbjq.cn/Article/details/goebgxesu.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wap.zdbjq.cn/Article/details/glkhvbfde.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://m.share.hesvh.cn/Article/details/gnilxxbxl.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/ggzulojpm.sHtML

J. 日期与时间
来源：http://m.share.fehbvm.com/Article/details/gmabaedsa.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gbbmoofux.sHtML

[J01] 获取当前时间
来源：http://m.share.zdbjq.cn/Article/details/gnnhkgoon.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://read.share.fehbvm.com/Article/details/ghcpkxrmz.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://baike.hesvh.cn/Article/details/glvhjudxx.sHtML

JS:   new Date();  Date.now()
来源：http://m.share.hesvh.cn/Article/details/gcqnyjlde.sHtML

TS:   new Date();  Date.now()
来源：http://m.share.zdbjq.cn/Article/details/gzatvgrjo.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://wap.hesvh.cn/Article/details/glodftxze.sHtML

Go:   time.Now()
来源：http://3g.hesvh.cn/Article/details/gklvjnybu.sHtML

Ruby: Time.now
来源：http://mobile.fehbvm.com/Article/details/gxpvoctny.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wap.fehbvm.com/Article/details/gtymvhofb.sHtML

[J02] 格式化输出
来源：http://blog.zdbjq.cn/Article/details/geiqqaili.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.fehbvm.com/Article/details/gouqmwdgo.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.share.fehbvm.com/Article/details/gfjshfgyx.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mobile.hesvh.cn/Article/details/gtoyykelo.sHtML

TS:   d.toISOString()
来源：http://mobile.fehbvm.com/Article/details/gjhoanzhd.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://3g.fehbvm.com/Article/details/ggovlusaa.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://baike.zdbjq.cn/Article/details/gqtamerak.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.hesvh.cn/Article/details/gwshwzkir.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.blog.zdbjq.cn/Article/details/gzfbpexmx.sHtML

[J03] 字符串解析为日期
来源：http://blog.hesvh.cn/Article/details/gvabefaxt.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://baike.fehbvm.com/Article/details/gqrcxcqxz.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.m.share.hesvh.cn/Article/details/gffzoyjyv.sHtML

JS:   new Date("2024-01-02")
来源：http://read.share.zdbjq.cn/Article/details/glnzppcad.sHtML

TS:   new Date("2024-01-02")
来源：http://www.share.fehbvm.com/Article/details/gyhyzkfwr.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://read.share.zdbjq.cn/Article/details/ghleqwtvo.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://read.share.zdbjq.cn/Article/details/gqrvlriva.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://read.share.hesvh.cn/Article/details/gazkumpmd.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wap.fehbvm.com/Article/details/gaiicmerk.sHtML

[J04] 时间戳与日期互转
来源：http://www.m.share.zdbjq.cn/Article/details/gjlufhtqj.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://3g.fehbvm.com/Article/details/ghuhkyfzt.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.blog.zdbjq.cn/Article/details/giuwdxukj.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.m.share.fehbvm.com/Article/details/gxmkahkoq.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.blog.zdbjq.cn/Article/details/gabkrtqrg.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.m.share.fehbvm.com/Article/details/gbgxeyevj.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wap.fehbvm.com/Article/details/gdffsjfjg.sHtML


<!-- 参考信息 -->