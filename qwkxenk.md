代发 wailian999

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.hesvh.cn/Article/details/gajsckfbh.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.zdbjq.cn/Article/details/gsbfiuhor.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.zdbjq.cn/Article/details/gmsxxbgmt.sHtML

[G05] 继承
来源：http://blog.fehbvm.com/Article/details/guhlzyrsm.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.hesvh.cn/Article/details/gypylsztg.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gofjbdwmt.sHtML

JS:   class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/gtwpjcvuv.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/gsfjaquyn.sHtML

Java: class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/gqzalabyf.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://baike.fehbvm.com/Article/details/gphcbrzrl.sHtML

Ruby: class Admin < User; end
来源：http://www.share.zdbjq.cn/Article/details/gcysljnwu.sHtML

C#:   class Admin : User {}
来源：http://wap.fehbvm.com/Article/details/gmtudnrwd.sHtML

[G06] 重写方法
来源：http://www.share.fehbvm.com/Article/details/gkpjfdpcq.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.fehbvm.com/Article/details/gudrsfahx.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/ggadpdiaq.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/glnbtxjnr.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/gsxmvgusm.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/gsnxcpyrk.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.zdbjq.cn/Article/details/ghnyenmwp.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.zdbjq.cn/Article/details/gxovhqono.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.hesvh.cn/Article/details/gahiexilp.sHtML

[G07] 调用父类方法
来源：http://blog.fehbvm.com/Article/details/gogptnjug.sHtML

Py:   super().greet()
来源：http://mobile.fehbvm.com/Article/details/gyunhsooe.sHtML

PHP:  parent::greet();
来源：http://wap.zdbjq.cn/Article/details/gactohcgs.sHtML

JS:   super.greet();
来源：http://baike.zdbjq.cn/Article/details/gzlwxvffk.sHtML

TS:   super.greet();
来源：http://blog.fehbvm.com/Article/details/gyzajirbx.sHtML

Java: super.greet();
来源：http://3g.hesvh.cn/Article/details/gbkycowab.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.hesvh.cn/Article/details/gecchdrlq.sHtML

Ruby: super
来源：http://3g.zdbjq.cn/Article/details/gmgatzqlb.sHtML

C#:   base.Greet();
来源：http://blog.hesvh.cn/Article/details/gexlcjvvq.sHtML

[G08] 静态方法与属性
来源：http://m.share.fehbvm.com/Article/details/gidewnooa.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.fehbvm.com/Article/details/gnuvpkhgm.sHtML

PHP:  public static function f() {}
来源：http://wap.fehbvm.com/Article/details/gvimvnwdd.sHtML

JS:   static f() {}
来源：http://wap.hesvh.cn/Article/details/ghgmgwjzo.sHtML

TS:   static f(): void {}
来源：http://wap.fehbvm.com/Article/details/gjzshtacz.sHtML

Java: static void f() {}
来源：http://wap.hesvh.cn/Article/details/gcvncocvh.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.fehbvm.com/Article/details/gkjiusbjs.sHtML

Ruby: def self.f; end
来源：http://m.share.zdbjq.cn/Article/details/gtcpcewvx.sHtML

C#:   public static void F() {}
来源：http://www.share.zdbjq.cn/Article/details/gmeghtban.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.fehbvm.com/Article/details/gvckwmgzl.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.zdbjq.cn/Article/details/gefrixarp.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.zdbjq.cn/Article/details/gssghdzxx.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.zdbjq.cn/Article/details/gsigbrscp.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.hesvh.cn/Article/details/glxemgrul.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.zdbjq.cn/Article/details/gteqsxbbk.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.zdbjq.cn/Article/details/gwoswcaut.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.fehbvm.com/Article/details/ggxrzsiis.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.hesvh.cn/Article/details/gojqbdixm.sHtML

[G10] 访问控制
来源：http://baike.hesvh.cn/Article/details/gbgxndqai.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.zdbjq.cn/Article/details/gtxilfzno.sHtML

PHP:  public / protected / private
来源：http://blog.zdbjq.cn/Article/details/guuijrpuf.sHtML

JS:   #private 字段；其余公开
来源：http://wap.zdbjq.cn/Article/details/gpkodqyoc.sHtML

TS:   public / protected / private
来源：http://read.share.zdbjq.cn/Article/details/grvsqvnyw.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.zdbjq.cn/Article/details/gnyushzqt.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.hesvh.cn/Article/details/gnaiaffgm.sHtML

Ruby: public / protected / private
来源：http://mobile.fehbvm.com/Article/details/gwgxetabm.sHtML

C#:   public / protected / private / internal
来源：http://blog.fehbvm.com/Article/details/gscoiejjs.sHtML

[G11] getter / setter
来源：http://baike.zdbjq.cn/Article/details/ghhbzbnoi.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.zdbjq.cn/Article/details/gguindmna.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gvophozwl.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.zdbjq.cn/Article/details/gpltsrode.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.fehbvm.com/Article/details/gzifvacoz.sHtML

Java: public String getName() { return name; }
来源：http://baike.zdbjq.cn/Article/details/gpygbxoyl.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.fehbvm.com/Article/details/gxshsqdwg.sHtML

Ruby: attr_accessor :name
来源：http://baike.zdbjq.cn/Article/details/glfsxkaoi.sHtML

C#:   public string Name { get; set; }
来源：http://3g.hesvh.cn/Article/details/gvdvtbvws.sHtML

[G12] 对象转字符串
来源：http://www.blog.zdbjq.cn/Article/details/gzpsnzxdl.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.hesvh.cn/Article/details/gsjryiirg.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gqgaszmuq.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gugrollzo.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/grjuyrefu.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.zdbjq.cn/Article/details/gvefyghnf.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.zdbjq.cn/Article/details/gbeirxpsv.sHtML

Ruby: def to_s; @name; end
来源：http://blog.hesvh.cn/Article/details/grzmktggs.sHtML

C#:   public override string ToString() => Name;
来源：http://www.share.zdbjq.cn/Article/details/gbzrjysdl.sHtML

[G13] 判断对象类型
来源：http://www.share.hesvh.cn/Article/details/gwplkrhbl.sHtML

Py:   isinstance(u, User)
来源：http://wap.hesvh.cn/Article/details/gsgjtyyou.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.fehbvm.com/Article/details/gkzrsdfzp.sHtML

JS:   u instanceof User
来源：http://mobile.fehbvm.com/Article/details/gidlkceop.sHtML

TS:   u instanceof User
来源：http://3g.hesvh.cn/Article/details/guyzikwex.sHtML

Java: u instanceof User
来源：http://m.share.zdbjq.cn/Article/details/gxsewjybl.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.zdbjq.cn/Article/details/gabuvlzax.sHtML

Ruby: u.is_a?(User)
来源：http://wap.fehbvm.com/Article/details/gydyzgixt.sHtML

C#:   u is User
来源：http://blog.hesvh.cn/Article/details/grwscuasx.sHtML

[G14] 数据类 / record
来源：http://read.share.fehbvm.com/Article/details/gxgwohdje.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.zdbjq.cn/Article/details/gymakgell.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.zdbjq.cn/Article/details/gcqfexrcm.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.hesvh.cn/Article/details/ggrprxtaj.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.fehbvm.com/Article/details/gwffevjbl.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.hesvh.cn/Article/details/gshaxwfmx.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.hesvh.cn/Article/details/gtyindlig.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.hesvh.cn/Article/details/gjjkqbxrh.sHtML

C#:   record User(string Name, int Age);
来源：http://wap.fehbvm.com/Article/details/gzwrmakoo.sHtML

[G15] 枚举
来源：http://mobile.hesvh.cn/Article/details/gmbtamghj.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.fehbvm.com/Article/details/gdeqjekcb.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.m.share.hesvh.cn/Article/details/ghthsmbce.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.hesvh.cn/Article/details/gypvulqtd.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.fehbvm.com/Article/details/ghfdtvadd.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.hesvh.cn/Article/details/graswmvdg.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.hesvh.cn/Article/details/gvfqacwzx.sHtML

Ruby: Color = %i[red green].freeze
来源：http://read.share.fehbvm.com/Article/details/grqrlfwfm.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.hesvh.cn/Article/details/gcnzjwzri.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.hesvh.cn/Article/details/gzxfsfbcq.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.blog.fehbvm.com/Article/details/gykypnpfw.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.zdbjq.cn/Article/details/ggsmlzxpr.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gmhilskth.sHtML

TS:   Object.entries(obj)
来源：http://www.share.fehbvm.com/Article/details/gwpxpcuvx.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.fehbvm.com/Article/details/ghlsqoxjg.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.fehbvm.com/Article/details/gpwpwwxnx.sHtML

Ruby: obj.instance_variables
来源：http://read.share.hesvh.cn/Article/details/gscnvemjy.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.fehbvm.com/Article/details/gynuoehde.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gnwdggwnt.sHtML

H. 异常与错误处理
来源：http://www.m.share.hesvh.cn/Article/details/gzywvpwvr.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gfpxljpmq.sHtML

[H01] try / catch 基础
来源：http://baike.fehbvm.com/Article/details/glvjjijwa.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.hesvh.cn/Article/details/guuedxoad.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.hesvh.cn/Article/details/gwvnkojql.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.hesvh.cn/Article/details/gawgrosjx.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://m.share.fehbvm.com/Article/details/gestqcbdh.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.zdbjq.cn/Article/details/gjxxlbjhw.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://read.share.fehbvm.com/Article/details/gqlshlqmk.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.hesvh.cn/Article/details/gbqshyban.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://3g.hesvh.cn/Article/details/gcwsqdvia.sHtML

[H02] finally / ensure 收尾
来源：http://www.m.share.hesvh.cn/Article/details/gwrkwjkkb.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.zdbjq.cn/Article/details/gkvzypkuw.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.zdbjq.cn/Article/details/goxbqrolb.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.hesvh.cn/Article/details/gbkhcatcf.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.hesvh.cn/Article/details/gqrskcmzw.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/gjywbewfc.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.hesvh.cn/Article/details/gxybpfczf.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.fehbvm.com/Article/details/gqsxdptvy.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://baike.fehbvm.com/Article/details/gxacvmryf.sHtML

[H03] 主动抛出异常
来源：http://www.m.share.fehbvm.com/Article/details/gjybauazz.sHtML

Py:   raise ValueError("错误信息")
来源：http://3g.zdbjq.cn/Article/details/gcdwzevsn.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blog.fehbvm.com/Article/details/gbamdxshs.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.hesvh.cn/Article/details/gehqonefy.sHtML

TS:   throw new Error("错误信息");
来源：http://www.share.fehbvm.com/Article/details/gifrpgxxh.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.fehbvm.com/Article/details/gkenvxoam.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://3g.fehbvm.com/Article/details/gyncyesxw.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://blog.fehbvm.com/Article/details/gainnscxy.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.m.share.fehbvm.com/Article/details/giipadjbv.sHtML

[H04] 自定义异常类型
来源：http://read.share.zdbjq.cn/Article/details/gpemxiqpx.sHtML

Py:   class MyError(Exception): pass
来源：http://wap.hesvh.cn/Article/details/gspihlanu.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.share.hesvh.cn/Article/details/gogyfafrb.sHtML

JS:   class MyError extends Error {}
来源：http://www.m.share.fehbvm.com/Article/details/gbitsntnx.sHtML

TS:   class MyError extends Error {}
来源：http://3g.hesvh.cn/Article/details/ghklwsjze.sHtML

Java: class MyException extends RuntimeException {}
来源：http://3g.zdbjq.cn/Article/details/glgfsfcjm.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wap.zdbjq.cn/Article/details/ggysqosgw.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.zdbjq.cn/Article/details/gwbfewlde.sHtML

C#:   class MyException : Exception {}
来源：http://blog.zdbjq.cn/Article/details/gzafbauhf.sHtML

[H05] 捕获特定类型
来源：http://m.share.fehbvm.com/Article/details/gtfazwnwe.sHtML

Py:   except ValueError as e:
来源：http://www.m.share.hesvh.cn/Article/details/gbenlhgir.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.fehbvm.com/Article/details/gfgaejvtl.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://blog.zdbjq.cn/Article/details/gxewrahmr.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.blog.zdbjq.cn/Article/details/gejjrurlb.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.blog.fehbvm.com/Article/details/guuysivrv.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.share.fehbvm.com/Article/details/giyelsusk.sHtML

Ruby: rescue ArgumentError => e
来源：http://wap.zdbjq.cn/Article/details/gnoybrqmm.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.share.zdbjq.cn/Article/details/gquucgymb.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.zdbjq.cn/Article/details/gcsrrafno.sHtML

Py:   value = d.get("k") or default
来源：http://blog.fehbvm.com/Article/details/gvopcuepb.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://baike.fehbvm.com/Article/details/gqrfblwbz.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://3g.zdbjq.cn/Article/details/gajqqlltd.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://mobile.hesvh.cn/Article/details/gakplfmio.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.blog.zdbjq.cn/Article/details/gnultpyfa.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.blog.fehbvm.com/Article/details/gusvoebob.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.blog.zdbjq.cn/Article/details/gvditsvga.sHtML

C#:   obj?.A?.B ?? default
来源：http://read.share.zdbjq.cn/Article/details/gztubzaji.sHtML

[H07] 断言
来源：http://wap.fehbvm.com/Article/details/ghovokvwr.sHtML

Py:   assert x > 0, "必须为正"
来源：http://baike.zdbjq.cn/Article/details/gzeqghqhv.sHtML

PHP:  assert($x > 0);
来源：http://3g.hesvh.cn/Article/details/gdiocptqt.sHtML

JS:   console.assert(x > 0);
来源：http://3g.hesvh.cn/Article/details/ghfxfwtay.sHtML

TS:   console.assert(x > 0);
来源：http://mobile.zdbjq.cn/Article/details/giknwmfqw.sHtML

Java: assert x > 0 : "必须为正";
来源：http://wap.zdbjq.cn/Article/details/gjdmhaegy.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://3g.hesvh.cn/Article/details/gbzqvrzgx.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.blog.hesvh.cn/Article/details/gbhndbevi.sHtML

C#:   Debug.Assert(x > 0);
来源：http://3g.hesvh.cn/Article/details/ggorfvzma.sHtML

[H08] 获取错误信息与堆栈
来源：http://read.share.zdbjq.cn/Article/details/gjvycwkxf.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://baike.hesvh.cn/Article/details/gqxyecutf.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://3g.zdbjq.cn/Article/details/gfbbwyxsz.sHtML

JS:   e.message;  e.stack
来源：http://m.share.hesvh.cn/Article/details/gymtpxcyg.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.m.share.hesvh.cn/Article/details/gvtjnbmah.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.share.zdbjq.cn/Article/details/gciconqbz.sHtML

Go:   err.Error()
来源：http://baike.zdbjq.cn/Article/details/gikrrojkx.sHtML

Ruby: e.message;  e.backtrace
来源：http://mobile.hesvh.cn/Article/details/ghvazdyit.sHtML

C#:   e.Message;  e.StackTrace
来源：http://3g.fehbvm.com/Article/details/goeugzmnn.sHtML

[H09] 带错误码的异常
来源：http://3g.hesvh.cn/Article/details/giyaesbkm.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://baike.hesvh.cn/Article/details/gwagzkofm.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.blog.zdbjq.cn/Article/details/gqlddthsn.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.share.hesvh.cn/Article/details/gkpdcetfc.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mobile.hesvh.cn/Article/details/gsawxftoa.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://read.share.zdbjq.cn/Article/details/gfqituyzs.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.blog.hesvh.cn/Article/details/gdcvwaknt.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.m.share.fehbvm.com/Article/details/gigvyhtzg.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://blog.hesvh.cn/Article/details/gmbdjjxbw.sHtML

[H10] 资源自动释放
来源：http://blog.hesvh.cn/Article/details/golahejip.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.blog.fehbvm.com/Article/details/gmugalzfm.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mobile.zdbjq.cn/Article/details/gabntbxta.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.zdbjq.cn/Article/details/gsjrsymrm.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.hesvh.cn/Article/details/gsfnnnxmc.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://baike.fehbvm.com/Article/details/gaophhdtj.sHtML

Go:   defer f.Close()
来源：http://www.m.share.fehbvm.com/Article/details/gfcykzjcy.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.share.fehbvm.com/Article/details/gsbrxoizh.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://3g.fehbvm.com/Article/details/gywvnqayf.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gbumuuvaw.sHtML

I. 正则表达式
来源：http://3g.hesvh.cn/Article/details/guhhquges.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gqkejafkx.sHtML

[I01] 判断是否匹配
来源：http://www.blog.hesvh.cn/Article/details/gzqffpmle.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wap.fehbvm.com/Article/details/gvmjpmmna.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://blog.zdbjq.cn/Article/details/gzxvocfqb.sHtML

JS:   /\d+/.test(s)
来源：http://read.share.hesvh.cn/Article/details/giqrnrtyk.sHtML

TS:   /\d+/.test(s)
来源：http://wap.zdbjq.cn/Article/details/gfnsvlpru.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mobile.hesvh.cn/Article/details/gidtnpsyd.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gokrgwkxv.sHtML

Ruby: s.match?(/\d+/)
来源：http://read.share.zdbjq.cn/Article/details/gmkiyfhow.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://baike.hesvh.cn/Article/details/gombeywyy.sHtML

[I02] 提取所有匹配
来源：http://www.m.share.fehbvm.com/Article/details/ggagzrovh.sHtML

Py:   re.findall(r"\d+", s)
来源：http://m.share.zdbjq.cn/Article/details/gfsintbmn.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wap.zdbjq.cn/Article/details/gotnwldxp.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://read.share.fehbvm.com/Article/details/gfhndcorm.sHtML

TS:   s.match(/\d+/g)
来源：http://mobile.zdbjq.cn/Article/details/gyhnpnqek.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.m.share.zdbjq.cn/Article/details/grcgqzwnf.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://read.share.fehbvm.com/Article/details/gbtgopskq.sHtML

Ruby: s.scan(/\d+/)
来源：http://read.share.fehbvm.com/Article/details/ghiqtevqd.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/grxmulhhu.sHtML

[I03] 提取捕获分组
来源：http://read.share.hesvh.cn/Article/details/gwibvreke.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wap.zdbjq.cn/Article/details/gijazzdqn.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mobile.hesvh.cn/Article/details/gwbiiojaj.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.m.share.fehbvm.com/Article/details/gogwxboof.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.m.share.zdbjq.cn/Article/details/ghdefmztw.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wap.hesvh.cn/Article/details/gotzpznuj.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://m.share.fehbvm.com/Article/details/gucaftmnr.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.share.fehbvm.com/Article/details/gedlbnotm.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://baike.fehbvm.com/Article/details/gjbvhtqfh.sHtML

[I04] 正则替换
来源：http://read.share.zdbjq.cn/Article/details/gxftywwfa.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://baike.hesvh.cn/Article/details/gfhsiizjo.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://3g.fehbvm.com/Article/details/gwvdfvyxh.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://blog.zdbjq.cn/Article/details/gazibxkgh.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://wap.zdbjq.cn/Article/details/gjekzwzfk.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://read.share.hesvh.cn/Article/details/gglbyqctm.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://wap.hesvh.cn/Article/details/gqgeesioz.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.blog.zdbjq.cn/Article/details/grnprfpcj.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://baike.hesvh.cn/Article/details/ggcwfynho.sHtML

[I05] 按正则拆分
来源：http://read.share.fehbvm.com/Article/details/gsiaxwmuj.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://wap.zdbjq.cn/Article/details/gzxirpcxy.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://baike.fehbvm.com/Article/details/grydpqfrk.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.m.share.fehbvm.com/Article/details/gjepuuizz.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.m.share.hesvh.cn/Article/details/gkvcegbom.sHtML

Java: s.split("\\s*,\\s*")
来源：http://wap.hesvh.cn/Article/details/gqyfnjgtx.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://read.share.hesvh.cn/Article/details/gzwazdkpl.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://mobile.fehbvm.com/Article/details/gkrmckaxl.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://read.share.fehbvm.com/Article/details/gmtqwsaiv.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.m.share.fehbvm.com/Article/details/gvgyxjfxp.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://m.share.zdbjq.cn/Article/details/gediiogvn.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://mobile.zdbjq.cn/Article/details/gydjqurxe.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.zdbjq.cn/Article/details/ghuwrilty.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.fehbvm.com/Article/details/gnxiqcvwf.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.share.fehbvm.com/Article/details/gvkifdceo.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.blog.fehbvm.com/Article/details/ggjgfraxe.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://3g.fehbvm.com/Article/details/gxorvirrm.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.blog.hesvh.cn/Article/details/gnklpxemf.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.share.zdbjq.cn/Article/details/gfcrklvzw.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://3g.zdbjq.cn/Article/details/ggmedkmuh.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.blog.fehbvm.com/Article/details/gvvbpvpit.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://blog.fehbvm.com/Article/details/gldbyfccz.sHtML

TS:   /error/gim
来源：http://read.share.hesvh.cn/Article/details/gijzwfdbv.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://baike.hesvh.cn/Article/details/gmvnttmvl.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://baike.hesvh.cn/Article/details/grqldrmtl.sHtML

Ruby: s.scan(/error/i)
来源：http://mobile.hesvh.cn/Article/details/gxbzlfgme.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://read.share.zdbjq.cn/Article/details/guiqruteu.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.blog.hesvh.cn/Article/details/gyifgulfp.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://3g.hesvh.cn/Article/details/gifaxkekw.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://m.share.fehbvm.com/Article/details/gzawcxrzi.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.hesvh.cn/Article/details/goaqkghkl.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.hesvh.cn/Article/details/gxaggiyar.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://read.share.fehbvm.com/Article/details/gbjnofmkv.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.m.share.fehbvm.com/Article/details/guftfaioh.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://blog.zdbjq.cn/Article/details/gyccyskeh.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.share.zdbjq.cn/Article/details/gcbkyuaci.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gysbkvyii.sHtML

J. 日期与时间
来源：http://www.share.hesvh.cn/Article/details/gmdmfqitl.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gvbluypno.sHtML

[J01] 获取当前时间
来源：http://www.m.share.zdbjq.cn/Article/details/gjrifpewv.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://baike.fehbvm.com/Article/details/ghyoznjiq.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://blog.hesvh.cn/Article/details/girrojron.sHtML

JS:   new Date();  Date.now()
来源：http://blog.hesvh.cn/Article/details/giqqqjpiy.sHtML

TS:   new Date();  Date.now()
来源：http://www.share.zdbjq.cn/Article/details/gylcoined.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.m.share.zdbjq.cn/Article/details/gnpukczgg.sHtML

Go:   time.Now()
来源：http://wap.fehbvm.com/Article/details/gexcgsggr.sHtML

Ruby: Time.now
来源：http://www.share.fehbvm.com/Article/details/gvxliopts.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.share.fehbvm.com/Article/details/gigzennkk.sHtML

[J02] 格式化输出
来源：http://wap.zdbjq.cn/Article/details/gbgkixmte.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.zdbjq.cn/Article/details/gwxiebgai.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://3g.hesvh.cn/Article/details/gqzbrnwdk.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://m.share.fehbvm.com/Article/details/gxkduzvtg.sHtML

TS:   d.toISOString()
来源：http://www.blog.zdbjq.cn/Article/details/gppalaowt.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://blog.fehbvm.com/Article/details/gkzsstopb.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://mobile.zdbjq.cn/Article/details/gvuuxrbkk.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.fehbvm.com/Article/details/gkcolehxs.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.share.fehbvm.com/Article/details/gwshhonku.sHtML


<!-- 参考信息 -->