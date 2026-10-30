代发 wailian999

C#:   public override string Greet() => "admin";
来源：http://www.share.hesvh.cn/Article/details/gdzsadpge.sHtML

[G07] 调用父类方法
来源：http://www.share.zdbjq.cn/Article/details/glbxofoeu.sHtML

Py:   super().greet()
来源：http://read.share.hesvh.cn/Article/details/gxucbcqfq.sHtML

PHP:  parent::greet();
来源：http://baike.hesvh.cn/Article/details/gedmawczw.sHtML

JS:   super.greet();
来源：http://mobile.fehbvm.com/Article/details/gqourksyd.sHtML

TS:   super.greet();
来源：http://wap.fehbvm.com/Article/details/gxktlugye.sHtML

Java: super.greet();
来源：http://read.share.fehbvm.com/Article/details/grsuyhdia.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.fehbvm.com/Article/details/genjgerur.sHtML

Ruby: super
来源：http://baike.fehbvm.com/Article/details/gqcezaodq.sHtML

C#:   base.Greet();
来源：http://m.share.fehbvm.com/Article/details/gkmuoljdb.sHtML

[G08] 静态方法与属性
来源：http://mobile.hesvh.cn/Article/details/guhxjhxho.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.zdbjq.cn/Article/details/ggoibzqzc.sHtML

PHP:  public static function f() {}
来源：http://m.share.hesvh.cn/Article/details/gjggllqtx.sHtML

JS:   static f() {}
来源：http://m.share.fehbvm.com/Article/details/gxbwbaoul.sHtML

TS:   static f(): void {}
来源：http://3g.zdbjq.cn/Article/details/gvvmtfciu.sHtML

Java: static void f() {}
来源：http://baike.zdbjq.cn/Article/details/guhomausk.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.fehbvm.com/Article/details/gydrvgikk.sHtML

Ruby: def self.f; end
来源：http://wap.zdbjq.cn/Article/details/gychvlxsm.sHtML

C#:   public static void F() {}
来源：http://blog.hesvh.cn/Article/details/gbmquokfr.sHtML

[G09] 接口 / 抽象类
来源：http://3g.hesvh.cn/Article/details/gufmsrtxo.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.hesvh.cn/Article/details/gopssiayc.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.hesvh.cn/Article/details/gqkhylvtq.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.zdbjq.cn/Article/details/gjoarutil.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.hesvh.cn/Article/details/gwiomwjlq.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.hesvh.cn/Article/details/gahjmrxze.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.hesvh.cn/Article/details/gcszraloh.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.zdbjq.cn/Article/details/gjoxnhptg.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.zdbjq.cn/Article/details/gglabdoxu.sHtML

[G10] 访问控制
来源：http://mobile.hesvh.cn/Article/details/gtlehlcum.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.zdbjq.cn/Article/details/grlodulmf.sHtML

PHP:  public / protected / private
来源：http://m.share.zdbjq.cn/Article/details/gibhwjegl.sHtML

JS:   #private 字段；其余公开
来源：http://wap.zdbjq.cn/Article/details/gutzpjobg.sHtML

TS:   public / protected / private
来源：http://3g.zdbjq.cn/Article/details/grizrmnib.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.zdbjq.cn/Article/details/gcproovej.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.zdbjq.cn/Article/details/gyngmxidg.sHtML

Ruby: public / protected / private
来源：http://blog.fehbvm.com/Article/details/glhtofquv.sHtML

C#:   public / protected / private / internal
来源：http://read.share.hesvh.cn/Article/details/gcokpoxwp.sHtML

[G11] getter / setter
来源：http://www.share.hesvh.cn/Article/details/gouhpcqpj.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.hesvh.cn/Article/details/gipqyniay.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.fehbvm.com/Article/details/gygtopsxd.sHtML

JS:   get name() { return this._name; }
来源：http://baike.hesvh.cn/Article/details/glifuntqn.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.zdbjq.cn/Article/details/gqkxmpwuj.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/gxiltrjjv.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.hesvh.cn/Article/details/gfouaksqh.sHtML

Ruby: attr_accessor :name
来源：http://3g.zdbjq.cn/Article/details/gcxqyhjik.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.fehbvm.com/Article/details/gvukmxxhc.sHtML

[G12] 对象转字符串
来源：http://www.share.fehbvm.com/Article/details/gowwiwobj.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.hesvh.cn/Article/details/guushdkiy.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.hesvh.cn/Article/details/gzlkawzba.sHtML

JS:   toString() { return this.name; }
来源：http://baike.fehbvm.com/Article/details/galrleplc.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/gzorqokfv.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.zdbjq.cn/Article/details/ghjncvtje.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.fehbvm.com/Article/details/gkqitnpmo.sHtML

Ruby: def to_s; @name; end
来源：http://baike.hesvh.cn/Article/details/gbjpnlccq.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.zdbjq.cn/Article/details/ggqarwwgj.sHtML

[G13] 判断对象类型
来源：http://www.share.hesvh.cn/Article/details/gvcvcrmpt.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.hesvh.cn/Article/details/gssnzsrjv.sHtML

PHP:  $u instanceof User
来源：http://m.share.hesvh.cn/Article/details/gqmfrhpmq.sHtML

JS:   u instanceof User
来源：http://3g.zdbjq.cn/Article/details/glxpekgsu.sHtML

TS:   u instanceof User
来源：http://blog.hesvh.cn/Article/details/godbfthrq.sHtML

Java: u instanceof User
来源：http://www.blog.hesvh.cn/Article/details/gadaypwwi.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.hesvh.cn/Article/details/gunuqkwnt.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.hesvh.cn/Article/details/gommoedji.sHtML

C#:   u is User
来源：http://3g.zdbjq.cn/Article/details/gnwhzcdom.sHtML

[G14] 数据类 / record
来源：http://3g.zdbjq.cn/Article/details/gvswdhjui.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://3g.hesvh.cn/Article/details/guaptgttr.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.fehbvm.com/Article/details/gytbmwcgj.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.hesvh.cn/Article/details/gfaeyvoau.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.zdbjq.cn/Article/details/gsfxyqqoe.sHtML

Java: record User(String name, int age) {}
来源：http://3g.fehbvm.com/Article/details/gukyimsxl.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.hesvh.cn/Article/details/gojhvchqn.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.zdbjq.cn/Article/details/ghycwjgcy.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.fehbvm.com/Article/details/ggmzfjayw.sHtML

[G15] 枚举
来源：http://www.blog.zdbjq.cn/Article/details/gsqmiahgc.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.fehbvm.com/Article/details/gfridavra.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.zdbjq.cn/Article/details/gwkzplxls.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.fehbvm.com/Article/details/gwqcdvfzm.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.fehbvm.com/Article/details/gmshtuivp.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.zdbjq.cn/Article/details/grkxgazmw.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.fehbvm.com/Article/details/gkzykthfn.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.fehbvm.com/Article/details/gqsmfwdnk.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.hesvh.cn/Article/details/gpvjqzqnq.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.zdbjq.cn/Article/details/gqaqilroy.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.fehbvm.com/Article/details/gerxkperh.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.fehbvm.com/Article/details/gdfgoycap.sHtML

JS:   Object.entries(obj)
来源：http://read.share.hesvh.cn/Article/details/geljnpkft.sHtML

TS:   Object.entries(obj)
来源：http://www.share.hesvh.cn/Article/details/gursomqfa.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://m.share.hesvh.cn/Article/details/gctkbffei.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.fehbvm.com/Article/details/gofgdyjza.sHtML

Ruby: obj.instance_variables
来源：http://baike.hesvh.cn/Article/details/gzkbteyci.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.fehbvm.com/Article/details/gsawmxmjp.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gozkkysgd.sHtML

H. 异常与错误处理
来源：http://3g.hesvh.cn/Article/details/grqabkgeb.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gwnoscqza.sHtML

[H01] try / catch 基础
来源：http://read.share.hesvh.cn/Article/details/gcfvyivrx.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.hesvh.cn/Article/details/gkpivylcw.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.fehbvm.com/Article/details/geqezkwvb.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://blog.fehbvm.com/Article/details/glmejsxxb.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://m.share.zdbjq.cn/Article/details/getmrwanj.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.share.hesvh.cn/Article/details/gmaiqpavc.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://baike.hesvh.cn/Article/details/gdyqikyml.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wap.zdbjq.cn/Article/details/gfbioyhdy.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.hesvh.cn/Article/details/gecpvxcac.sHtML

[H02] finally / ensure 收尾
来源：http://wap.hesvh.cn/Article/details/gqhfxozur.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://baike.hesvh.cn/Article/details/ggajtvypw.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/ghlkbhbox.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://baike.fehbvm.com/Article/details/gbeojoeyg.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.fehbvm.com/Article/details/gysblrkne.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.fehbvm.com/Article/details/gdpfpbvcg.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.fehbvm.com/Article/details/gzlolwfmo.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://3g.zdbjq.cn/Article/details/gsczxvujp.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://baike.hesvh.cn/Article/details/gislcjpmi.sHtML

[H03] 主动抛出异常
来源：http://m.share.hesvh.cn/Article/details/gmirbddpk.sHtML

Py:   raise ValueError("错误信息")
来源：http://blog.hesvh.cn/Article/details/gnbobfexa.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://3g.zdbjq.cn/Article/details/gqfswnwth.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.zdbjq.cn/Article/details/gjaklfoim.sHtML

TS:   throw new Error("错误信息");
来源：http://blog.hesvh.cn/Article/details/gaxuntkvi.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.blog.hesvh.cn/Article/details/gkjfyjcdp.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wap.hesvh.cn/Article/details/gbdlpzqqk.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://baike.hesvh.cn/Article/details/gkddelppl.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://blog.fehbvm.com/Article/details/gngyswtbb.sHtML

[H04] 自定义异常类型
来源：http://baike.hesvh.cn/Article/details/glkdfcxzb.sHtML

Py:   class MyError(Exception): pass
来源：http://blog.zdbjq.cn/Article/details/gabugzjgr.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://mobile.hesvh.cn/Article/details/gtililivg.sHtML

JS:   class MyError extends Error {}
来源：http://baike.fehbvm.com/Article/details/ggumgejto.sHtML

TS:   class MyError extends Error {}
来源：http://baike.fehbvm.com/Article/details/gerjnerrr.sHtML

Java: class MyException extends RuntimeException {}
来源：http://3g.hesvh.cn/Article/details/gqpvqsbcx.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.m.share.fehbvm.com/Article/details/geunbyvod.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.zdbjq.cn/Article/details/gumpmjhpj.sHtML

C#:   class MyException : Exception {}
来源：http://m.share.zdbjq.cn/Article/details/gkgxlgopw.sHtML

[H05] 捕获特定类型
来源：http://mobile.hesvh.cn/Article/details/gioaksfrt.sHtML

Py:   except ValueError as e:
来源：http://mobile.zdbjq.cn/Article/details/gqhyjvsve.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.share.hesvh.cn/Article/details/gcjlfwlcc.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://m.share.zdbjq.cn/Article/details/gmmhrntpm.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.blog.hesvh.cn/Article/details/gdvruisnn.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://wap.zdbjq.cn/Article/details/gvfudqcoz.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wap.hesvh.cn/Article/details/gtmjpzjvv.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.zdbjq.cn/Article/details/grtwikezc.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.share.hesvh.cn/Article/details/ggqmhsilb.sHtML

[H06] 可选值 / 空值安全访问
来源：http://read.share.zdbjq.cn/Article/details/gyjpurwqi.sHtML

Py:   value = d.get("k") or default
来源：http://blog.hesvh.cn/Article/details/gfhjumwer.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.share.zdbjq.cn/Article/details/ghxdctkin.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://3g.hesvh.cn/Article/details/gmhmrhiux.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.share.zdbjq.cn/Article/details/gsqpzpsgv.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://baike.hesvh.cn/Article/details/gwlgirktt.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.share.fehbvm.com/Article/details/guozyjjcj.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.share.zdbjq.cn/Article/details/gzmukmqup.sHtML

C#:   obj?.A?.B ?? default
来源：http://3g.zdbjq.cn/Article/details/gkqlowuat.sHtML

[H07] 断言
来源：http://blog.zdbjq.cn/Article/details/gwzkxjemg.sHtML

Py:   assert x > 0, "必须为正"
来源：http://m.share.zdbjq.cn/Article/details/gmnwedxqj.sHtML

PHP:  assert($x > 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gillqnlzx.sHtML

JS:   console.assert(x > 0);
来源：http://www.m.share.fehbvm.com/Article/details/gqtkjhzxh.sHtML

TS:   console.assert(x > 0);
来源：http://mobile.zdbjq.cn/Article/details/gqebpzegs.sHtML

Java: assert x > 0 : "必须为正";
来源：http://mobile.fehbvm.com/Article/details/gxzktmqru.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.share.hesvh.cn/Article/details/gomjrpyiv.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://m.share.zdbjq.cn/Article/details/gbcutwudy.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.m.share.hesvh.cn/Article/details/gtuqfihai.sHtML

[H08] 获取错误信息与堆栈
来源：http://3g.zdbjq.cn/Article/details/goljcjxqt.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.blog.fehbvm.com/Article/details/gothncdaq.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mobile.hesvh.cn/Article/details/gddrinpmd.sHtML

JS:   e.message;  e.stack
来源：http://read.share.fehbvm.com/Article/details/ghplwwsct.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.blog.fehbvm.com/Article/details/gewybiwqw.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://wap.hesvh.cn/Article/details/gjcohxqzs.sHtML

Go:   err.Error()
来源：http://wap.zdbjq.cn/Article/details/gucsnskfh.sHtML

Ruby: e.message;  e.backtrace
来源：http://read.share.fehbvm.com/Article/details/gsubfjbuo.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.blog.hesvh.cn/Article/details/gcepmytav.sHtML

[H09] 带错误码的异常
来源：http://blog.hesvh.cn/Article/details/gvnwtrpci.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.blog.hesvh.cn/Article/details/ggoytuhhj.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://m.share.hesvh.cn/Article/details/gzlfyyxjl.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.share.fehbvm.com/Article/details/gymhyjulp.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.m.share.zdbjq.cn/Article/details/gjqlxnqar.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.m.share.hesvh.cn/Article/details/gcpejjltm.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://read.share.zdbjq.cn/Article/details/gilkawwvo.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://blog.zdbjq.cn/Article/details/gcsbuqspp.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://blog.fehbvm.com/Article/details/gmstqkosz.sHtML

[H10] 资源自动释放
来源：http://m.share.fehbvm.com/Article/details/gvoazvfev.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://blog.hesvh.cn/Article/details/grmuarkfd.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.share.hesvh.cn/Article/details/gugknastn.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.zdbjq.cn/Article/details/ggvnaqddy.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.fehbvm.com/Article/details/gvasyyuml.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://blog.fehbvm.com/Article/details/gtmpppbka.sHtML

Go:   defer f.Close()
来源：http://baike.hesvh.cn/Article/details/gktueirnt.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://3g.hesvh.cn/Article/details/gqlgxewhc.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gxclasomk.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/ghyjrztgg.sHtML

I. 正则表达式
来源：http://www.m.share.fehbvm.com/Article/details/gqejqgupk.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gcbdgwcnt.sHtML

[I01] 判断是否匹配
来源：http://read.share.zdbjq.cn/Article/details/gbocrztyu.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.share.zdbjq.cn/Article/details/gopljiiut.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://m.share.fehbvm.com/Article/details/gdclcyoxc.sHtML

JS:   /\d+/.test(s)
来源：http://www.m.share.fehbvm.com/Article/details/ghtzdwmqt.sHtML

TS:   /\d+/.test(s)
来源：http://blog.zdbjq.cn/Article/details/goinrgrwx.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.blog.fehbvm.com/Article/details/gcxmomzmf.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wap.zdbjq.cn/Article/details/gbgaaphop.sHtML

Ruby: s.match?(/\d+/)
来源：http://read.share.zdbjq.cn/Article/details/gdbefyfyb.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://blog.hesvh.cn/Article/details/gzboeevdd.sHtML

[I02] 提取所有匹配
来源：http://www.blog.hesvh.cn/Article/details/gcwnrvjjt.sHtML

Py:   re.findall(r"\d+", s)
来源：http://mobile.fehbvm.com/Article/details/gtdohmfda.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.blog.fehbvm.com/Article/details/ghddiqkmb.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://3g.zdbjq.cn/Article/details/gnjnsbmep.sHtML

TS:   s.match(/\d+/g)
来源：http://mobile.zdbjq.cn/Article/details/gpubvgmnn.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://m.share.fehbvm.com/Article/details/geyircqam.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://read.share.hesvh.cn/Article/details/gltvevyrp.sHtML

Ruby: s.scan(/\d+/)
来源：http://m.share.hesvh.cn/Article/details/gnazvxfra.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/giiyyqppa.sHtML

[I03] 提取捕获分组
来源：http://3g.hesvh.cn/Article/details/gaqmrbauv.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wap.hesvh.cn/Article/details/gqhfqawub.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wap.hesvh.cn/Article/details/gruwtjvlq.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://read.share.fehbvm.com/Article/details/glcxjlmgt.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.share.fehbvm.com/Article/details/gbkytxluf.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://m.share.fehbvm.com/Article/details/gbgzrnsjx.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://baike.hesvh.cn/Article/details/gfsbkfvnr.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wap.fehbvm.com/Article/details/gqcrnbysh.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wap.fehbvm.com/Article/details/grhehkpvq.sHtML

[I04] 正则替换
来源：http://www.blog.zdbjq.cn/Article/details/gkqmwltlt.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.share.fehbvm.com/Article/details/gpknihxch.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mobile.zdbjq.cn/Article/details/gcexjrplc.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.fehbvm.com/Article/details/girkvjtup.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://wap.fehbvm.com/Article/details/gdzdsycmd.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://3g.fehbvm.com/Article/details/gnudzwydl.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://read.share.zdbjq.cn/Article/details/gbopfeyxq.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.m.share.fehbvm.com/Article/details/gyhojilho.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://3g.zdbjq.cn/Article/details/gfbaqirfc.sHtML

[I05] 按正则拆分
来源：http://www.share.hesvh.cn/Article/details/gtfulbwxm.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.m.share.zdbjq.cn/Article/details/gdgsigrzl.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mobile.zdbjq.cn/Article/details/gzafkqesc.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://baike.hesvh.cn/Article/details/gqrdvmxyk.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.m.share.fehbvm.com/Article/details/ggxpsobte.sHtML

Java: s.split("\\s*,\\s*")
来源：http://read.share.zdbjq.cn/Article/details/gawbnpcrp.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wap.hesvh.cn/Article/details/gnyspojue.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.m.share.hesvh.cn/Article/details/goannkdca.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wap.hesvh.cn/Article/details/gexkeoivw.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.share.zdbjq.cn/Article/details/gomwxgnhe.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://baike.fehbvm.com/Article/details/gvhqzcdbx.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://mobile.fehbvm.com/Article/details/gktkasdxv.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.fehbvm.com/Article/details/ggpvuqvuw.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.fehbvm.com/Article/details/gtabjpjvl.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.m.share.hesvh.cn/Article/details/gfxsxadsr.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://m.share.hesvh.cn/Article/details/gqovkxqpx.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://m.share.fehbvm.com/Article/details/gvlhxxrcb.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://blog.zdbjq.cn/Article/details/ghqoarmlf.sHtML

[I07] 忽略大小写与多行模式
来源：http://m.share.hesvh.cn/Article/details/ggrogqgqq.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://blog.zdbjq.cn/Article/details/ghmdoaweo.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://m.share.fehbvm.com/Article/details/gwrtquekt.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mobile.hesvh.cn/Article/details/gbvbrpipo.sHtML

TS:   /error/gim
来源：http://www.m.share.zdbjq.cn/Article/details/gweerhyna.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://3g.zdbjq.cn/Article/details/gltvlrddi.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.m.share.fehbvm.com/Article/details/gtjnhgebf.sHtML

Ruby: s.scan(/error/i)
来源：http://mobile.hesvh.cn/Article/details/gyhnfhbpb.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://baike.zdbjq.cn/Article/details/gnoesocmw.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://mobile.fehbvm.com/Article/details/gkclsmfya.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://m.share.fehbvm.com/Article/details/gzqagyvhw.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://3g.fehbvm.com/Article/details/gplsvuhwz.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.zdbjq.cn/Article/details/gniaoeafi.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.zdbjq.cn/Article/details/glylmsplg.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.m.share.fehbvm.com/Article/details/gcfnvtyog.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://mobile.fehbvm.com/Article/details/gkmhqveuc.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://baike.hesvh.cn/Article/details/gdsihsknf.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://blog.fehbvm.com/Article/details/gtdlaybnc.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gyiolhytu.sHtML

J. 日期与时间
来源：http://wap.hesvh.cn/Article/details/gobsxloag.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gmceybtto.sHtML

[J01] 获取当前时间
来源：http://baike.fehbvm.com/Article/details/gxkhwjsyg.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://read.share.zdbjq.cn/Article/details/glylsimtb.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.blog.hesvh.cn/Article/details/geehjvspy.sHtML

JS:   new Date();  Date.now()
来源：http://m.share.fehbvm.com/Article/details/gbikpsnje.sHtML

TS:   new Date();  Date.now()
来源：http://blog.zdbjq.cn/Article/details/gcesfnert.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://mobile.hesvh.cn/Article/details/gikhuropo.sHtML

Go:   time.Now()
来源：http://www.m.share.hesvh.cn/Article/details/gjdayffld.sHtML

Ruby: Time.now
来源：http://wap.zdbjq.cn/Article/details/ganhnqgeh.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://3g.hesvh.cn/Article/details/gngkjuwpj.sHtML

[J02] 格式化输出
来源：http://www.m.share.hesvh.cn/Article/details/gtymsuwmn.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.hesvh.cn/Article/details/gxumtqrjs.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://blog.hesvh.cn/Article/details/gjpkkdfrl.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.share.hesvh.cn/Article/details/gqzcloesf.sHtML

TS:   d.toISOString()
来源：http://blog.zdbjq.cn/Article/details/gnyvxxkeh.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://blog.fehbvm.com/Article/details/gewkkexhn.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wap.fehbvm.com/Article/details/gqueotfmt.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.fehbvm.com/Article/details/gsfcjvslt.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://mobile.fehbvm.com/Article/details/gocktwvpc.sHtML

[J03] 字符串解析为日期
来源：http://mobile.fehbvm.com/Article/details/gqmeuojvb.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.blog.fehbvm.com/Article/details/gfvqcwgim.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.m.share.zdbjq.cn/Article/details/gybgtkgpq.sHtML

JS:   new Date("2024-01-02")
来源：http://read.share.hesvh.cn/Article/details/gdoyfvjaq.sHtML

TS:   new Date("2024-01-02")
来源：http://3g.zdbjq.cn/Article/details/gkzydhyhn.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://blog.zdbjq.cn/Article/details/grzkeolhx.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://read.share.zdbjq.cn/Article/details/gqxdpvoyw.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://read.share.hesvh.cn/Article/details/gazefksut.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.blog.fehbvm.com/Article/details/gpdqpishn.sHtML

[J04] 时间戳与日期互转
来源：http://wap.fehbvm.com/Article/details/guforyqvd.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.m.share.fehbvm.com/Article/details/gcidfvzev.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://baike.hesvh.cn/Article/details/ghujyukpg.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.blog.fehbvm.com/Article/details/gbiaujeya.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://m.share.zdbjq.cn/Article/details/gbkbttrnb.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://mobile.hesvh.cn/Article/details/gnphdkqir.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.share.zdbjq.cn/Article/details/gnbmortbh.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://blog.fehbvm.com/Article/details/gcoiwkhwc.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wap.fehbvm.com/Article/details/gtrhkhzjh.sHtML

[J05] 时间加减（加 7 天）
来源：http://read.share.hesvh.cn/Article/details/gccixlkbg.sHtML

Py:   now + timedelta(days=7)
来源：http://mobile.zdbjq.cn/Article/details/gjzhmpbwk.sHtML


<!-- 参考信息 -->