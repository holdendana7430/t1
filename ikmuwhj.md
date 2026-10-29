代发 wailian999

[G06] 重写方法
来源：http://read.share.hesvh.cn/Article/details/gabrveunt.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.fehbvm.com/Article/details/gyohxrxmm.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/girnnskqx.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.zdbjq.cn/Article/details/gqoabcsqh.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/gihfnxnmh.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/gogaxwtfk.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.hesvh.cn/Article/details/guvgwpwof.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.zdbjq.cn/Article/details/gqatpapsf.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.hesvh.cn/Article/details/ggpwaxrzm.sHtML

[G07] 调用父类方法
来源：http://blog.hesvh.cn/Article/details/gcfrqlywm.sHtML

Py:   super().greet()
来源：http://3g.hesvh.cn/Article/details/genzjxfgu.sHtML

PHP:  parent::greet();
来源：http://wap.zdbjq.cn/Article/details/gkglneygx.sHtML

JS:   super.greet();
来源：http://wap.hesvh.cn/Article/details/gvbeimebi.sHtML

TS:   super.greet();
来源：http://www.m.share.zdbjq.cn/Article/details/goerjlhfq.sHtML

Java: super.greet();
来源：http://www.m.share.hesvh.cn/Article/details/gpulvjito.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.zdbjq.cn/Article/details/gwcqclhdp.sHtML

Ruby: super
来源：http://wap.fehbvm.com/Article/details/gavxmskwe.sHtML

C#:   base.Greet();
来源：http://wap.fehbvm.com/Article/details/gpjwjybad.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.hesvh.cn/Article/details/gpueyezvd.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.hesvh.cn/Article/details/grafexzmr.sHtML

PHP:  public static function f() {}
来源：http://blog.hesvh.cn/Article/details/gyfcesadu.sHtML

JS:   static f() {}
来源：http://wap.fehbvm.com/Article/details/gydaobffg.sHtML

TS:   static f(): void {}
来源：http://mobile.fehbvm.com/Article/details/gextuchac.sHtML

Java: static void f() {}
来源：http://www.blog.hesvh.cn/Article/details/gedxsdyms.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.fehbvm.com/Article/details/gbmtkfnil.sHtML

Ruby: def self.f; end
来源：http://baike.hesvh.cn/Article/details/grabaaong.sHtML

C#:   public static void F() {}
来源：http://mobile.zdbjq.cn/Article/details/gmfztbvxo.sHtML

[G09] 接口 / 抽象类
来源：http://baike.hesvh.cn/Article/details/gdxpcmzbq.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.hesvh.cn/Article/details/gupehuens.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.hesvh.cn/Article/details/gstvufkow.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.zdbjq.cn/Article/details/glbxktmoh.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.fehbvm.com/Article/details/gwzlkyrxn.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.zdbjq.cn/Article/details/gpouzxplj.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.hesvh.cn/Article/details/gdyqqjdus.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.hesvh.cn/Article/details/glbvieeqg.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.hesvh.cn/Article/details/guufzwmaa.sHtML

[G10] 访问控制
来源：http://3g.zdbjq.cn/Article/details/goqraaiup.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.zdbjq.cn/Article/details/gmiqyeltx.sHtML

PHP:  public / protected / private
来源：http://wap.hesvh.cn/Article/details/gfnyefnim.sHtML

JS:   #private 字段；其余公开
来源：http://baike.fehbvm.com/Article/details/giftunezt.sHtML

TS:   public / protected / private
来源：http://www.m.share.zdbjq.cn/Article/details/guoooerjf.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.hesvh.cn/Article/details/ggvrauagp.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.zdbjq.cn/Article/details/gyczojrun.sHtML

Ruby: public / protected / private
来源：http://3g.zdbjq.cn/Article/details/guyqtnpwa.sHtML

C#:   public / protected / private / internal
来源：http://baike.zdbjq.cn/Article/details/guknwvixs.sHtML

[G11] getter / setter
来源：http://mobile.zdbjq.cn/Article/details/gequxvzkr.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.zdbjq.cn/Article/details/gbsjzicvx.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.zdbjq.cn/Article/details/ghkqzmrpn.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.zdbjq.cn/Article/details/gogctbmte.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.hesvh.cn/Article/details/gxoxducfy.sHtML

Java: public String getName() { return name; }
来源：http://m.share.fehbvm.com/Article/details/glljrjgvb.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.fehbvm.com/Article/details/gvekhdkpj.sHtML

Ruby: attr_accessor :name
来源：http://wap.zdbjq.cn/Article/details/gydeidfzl.sHtML

C#:   public string Name { get; set; }
来源：http://wap.fehbvm.com/Article/details/gzxnbhpgv.sHtML

[G12] 对象转字符串
来源：http://3g.zdbjq.cn/Article/details/gciyddsxs.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.hesvh.cn/Article/details/ghprpscxg.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.fehbvm.com/Article/details/gplidcnxh.sHtML

JS:   toString() { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/gttufgdqa.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.hesvh.cn/Article/details/gtrrqzknz.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.fehbvm.com/Article/details/gfipohblu.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.fehbvm.com/Article/details/gpsnrwuja.sHtML

Ruby: def to_s; @name; end
来源：http://blog.zdbjq.cn/Article/details/gbbulmbrn.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.fehbvm.com/Article/details/gsshsjtmc.sHtML

[G13] 判断对象类型
来源：http://www.blog.fehbvm.com/Article/details/gnmhipgsm.sHtML

Py:   isinstance(u, User)
来源：http://wap.hesvh.cn/Article/details/gokcotxxg.sHtML

PHP:  $u instanceof User
来源：http://baike.hesvh.cn/Article/details/gplxskygx.sHtML

JS:   u instanceof User
来源：http://wap.fehbvm.com/Article/details/gveekhgem.sHtML

TS:   u instanceof User
来源：http://read.share.fehbvm.com/Article/details/gwqxxijbr.sHtML

Java: u instanceof User
来源：http://www.m.share.fehbvm.com/Article/details/gbnnxlklf.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.fehbvm.com/Article/details/gkmrpugdm.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.zdbjq.cn/Article/details/gtzdivefl.sHtML

C#:   u is User
来源：http://wap.zdbjq.cn/Article/details/gzimlxctc.sHtML

[G14] 数据类 / record
来源：http://m.share.zdbjq.cn/Article/details/gmaowqnoo.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.hesvh.cn/Article/details/gfupgqgyn.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.fehbvm.com/Article/details/gjvsfwvcr.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.hesvh.cn/Article/details/gwjhgzxjy.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.hesvh.cn/Article/details/gsvmbratd.sHtML

Java: record User(String name, int age) {}
来源：http://baike.zdbjq.cn/Article/details/gdbeqxemo.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.zdbjq.cn/Article/details/gtyakenzw.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://baike.fehbvm.com/Article/details/gpmnibbwk.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.zdbjq.cn/Article/details/gwaxpggew.sHtML

[G15] 枚举
来源：http://m.share.fehbvm.com/Article/details/gbwssnvcx.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://read.share.hesvh.cn/Article/details/grgwixaqy.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.hesvh.cn/Article/details/gfvrsfdnr.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.fehbvm.com/Article/details/gfgzahmjo.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.zdbjq.cn/Article/details/gseztjbdb.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.hesvh.cn/Article/details/gtisrlwao.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://blog.hesvh.cn/Article/details/gsegrrmxy.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.fehbvm.com/Article/details/gmyeemywn.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.fehbvm.com/Article/details/gtainevhr.sHtML

[G16] 对象转数组 / 字典
来源：http://www.m.share.zdbjq.cn/Article/details/gargzqsif.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.zdbjq.cn/Article/details/giajyoerr.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.hesvh.cn/Article/details/gzenznxwa.sHtML

JS:   Object.entries(obj)
来源：http://mobile.fehbvm.com/Article/details/ggprtklpg.sHtML

TS:   Object.entries(obj)
来源：http://blog.zdbjq.cn/Article/details/gnjmwmnfz.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.zdbjq.cn/Article/details/gffdapmsa.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://wap.zdbjq.cn/Article/details/gvuyofvsj.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.zdbjq.cn/Article/details/gnngokjhl.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.hesvh.cn/Article/details/gvoeqrnod.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gedkrrctj.sHtML

H. 异常与错误处理
来源：http://wap.fehbvm.com/Article/details/gppwnjfeh.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gwcsqmrml.sHtML

[H01] try / catch 基础
来源：http://read.share.zdbjq.cn/Article/details/ggosovfnp.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.hesvh.cn/Article/details/gsuxvgeju.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.zdbjq.cn/Article/details/gpzscphzu.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.blog.hesvh.cn/Article/details/gmywowxkq.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://m.share.zdbjq.cn/Article/details/gzmujzlya.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.fehbvm.com/Article/details/gzchcncey.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.blog.zdbjq.cn/Article/details/gqjfmigmr.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.zdbjq.cn/Article/details/giwtpmxkm.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://3g.hesvh.cn/Article/details/gwkoneewt.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.hesvh.cn/Article/details/gkkhfeqhq.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.fehbvm.com/Article/details/gcpxzxkqy.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://mobile.fehbvm.com/Article/details/ggquhxjzc.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://baike.hesvh.cn/Article/details/gbiwjieoa.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.zdbjq.cn/Article/details/galpmvwlj.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.fehbvm.com/Article/details/gjwgpmyle.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.zdbjq.cn/Article/details/gvwjgdqdg.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.hesvh.cn/Article/details/gtnakhtyr.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/gxgecczof.sHtML

[H03] 主动抛出异常
来源：http://blog.hesvh.cn/Article/details/gnpvpyarh.sHtML

Py:   raise ValueError("错误信息")
来源：http://wap.fehbvm.com/Article/details/ghheohqpn.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.hesvh.cn/Article/details/grswysshz.sHtML

JS:   throw new Error("错误信息");
来源：http://baike.zdbjq.cn/Article/details/gmnbctlgd.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.zdbjq.cn/Article/details/gfdnjejth.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://m.share.hesvh.cn/Article/details/gemjgiesn.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mobile.fehbvm.com/Article/details/gnokquljp.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.m.share.fehbvm.com/Article/details/gjtgnluvz.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://blog.fehbvm.com/Article/details/gxcuhfkhr.sHtML

[H04] 自定义异常类型
来源：http://m.share.zdbjq.cn/Article/details/gjrjlidfh.sHtML

Py:   class MyError(Exception): pass
来源：http://3g.zdbjq.cn/Article/details/gztapztzv.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://blog.fehbvm.com/Article/details/gvjhiqmcc.sHtML

JS:   class MyError extends Error {}
来源：http://www.m.share.zdbjq.cn/Article/details/gubuyghwb.sHtML

TS:   class MyError extends Error {}
来源：http://www.blog.zdbjq.cn/Article/details/gmnqedvkd.sHtML

Java: class MyException extends RuntimeException {}
来源：http://mobile.fehbvm.com/Article/details/gvqhmsxgp.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wap.zdbjq.cn/Article/details/gwoemjsaz.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.zdbjq.cn/Article/details/gjwjjrrcp.sHtML

C#:   class MyException : Exception {}
来源：http://mobile.hesvh.cn/Article/details/gmaovcykq.sHtML

[H05] 捕获特定类型
来源：http://wap.hesvh.cn/Article/details/gjklhjppt.sHtML

Py:   except ValueError as e:
来源：http://3g.fehbvm.com/Article/details/gwjxfnurc.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.blog.zdbjq.cn/Article/details/grcxjodwy.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://3g.hesvh.cn/Article/details/gzckzbcjq.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://mobile.hesvh.cn/Article/details/giptppgdk.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.zdbjq.cn/Article/details/gatuxpklz.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.share.zdbjq.cn/Article/details/gpkejupct.sHtML

Ruby: rescue ArgumentError => e
来源：http://mobile.fehbvm.com/Article/details/gopgrjuxn.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.blog.fehbvm.com/Article/details/gtadzgzca.sHtML

[H06] 可选值 / 空值安全访问
来源：http://wap.zdbjq.cn/Article/details/glpxviean.sHtML

Py:   value = d.get("k") or default
来源：http://m.share.fehbvm.com/Article/details/gnzcdspdt.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.hesvh.cn/Article/details/gycztueuv.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://3g.zdbjq.cn/Article/details/gedqcaduu.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://baike.fehbvm.com/Article/details/ggbrugqfr.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://3g.hesvh.cn/Article/details/gcnolrksz.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://wap.fehbvm.com/Article/details/gifwpzcfi.sHtML

Ruby: d&.dig(:a, :b)
来源：http://3g.fehbvm.com/Article/details/gvfoxtiiy.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.blog.fehbvm.com/Article/details/gvkxltxfy.sHtML

[H07] 断言
来源：http://m.share.fehbvm.com/Article/details/grrswuvih.sHtML

Py:   assert x > 0, "必须为正"
来源：http://blog.fehbvm.com/Article/details/gqfeduhvy.sHtML

PHP:  assert($x > 0);
来源：http://wap.zdbjq.cn/Article/details/gydjvfyus.sHtML

JS:   console.assert(x > 0);
来源：http://read.share.zdbjq.cn/Article/details/ghnmocgzh.sHtML

TS:   console.assert(x > 0);
来源：http://3g.fehbvm.com/Article/details/gvpidrsvi.sHtML

Java: assert x > 0 : "必须为正";
来源：http://wap.zdbjq.cn/Article/details/ghjwqziop.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://baike.fehbvm.com/Article/details/gehxgprwc.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://read.share.fehbvm.com/Article/details/gtxlxzapo.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.m.share.hesvh.cn/Article/details/gneimotkk.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.m.share.zdbjq.cn/Article/details/gpootaiey.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://read.share.zdbjq.cn/Article/details/gutmnwzec.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://read.share.zdbjq.cn/Article/details/gmueiekxg.sHtML

JS:   e.message;  e.stack
来源：http://blog.hesvh.cn/Article/details/gqzjxthfo.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.blog.fehbvm.com/Article/details/gsctarccs.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://3g.fehbvm.com/Article/details/gnsnubrmy.sHtML

Go:   err.Error()
来源：http://read.share.fehbvm.com/Article/details/gcdftnjhj.sHtML

Ruby: e.message;  e.backtrace
来源：http://3g.zdbjq.cn/Article/details/gtlfuyngn.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.share.zdbjq.cn/Article/details/grollqelr.sHtML

[H09] 带错误码的异常
来源：http://www.share.fehbvm.com/Article/details/gdlwegkqz.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.m.share.zdbjq.cn/Article/details/gdcmhvvyu.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://blog.fehbvm.com/Article/details/gfvkjilyx.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.blog.zdbjq.cn/Article/details/ggtdloupb.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wap.fehbvm.com/Article/details/gqejzvjyl.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://baike.fehbvm.com/Article/details/gzlgnatom.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://baike.hesvh.cn/Article/details/gomxitkba.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://3g.zdbjq.cn/Article/details/gpaagvwtd.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://read.share.fehbvm.com/Article/details/gcbuagrlx.sHtML

[H10] 资源自动释放
来源：http://3g.fehbvm.com/Article/details/gapgjgnwr.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.m.share.zdbjq.cn/Article/details/gdpgcfcao.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wap.zdbjq.cn/Article/details/gzzjdanbr.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.hesvh.cn/Article/details/gfqxcfxmh.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.hesvh.cn/Article/details/gwxbxqzdb.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.m.share.hesvh.cn/Article/details/gcgalhgtv.sHtML

Go:   defer f.Close()
来源：http://mobile.hesvh.cn/Article/details/gvinxnxxe.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.m.share.zdbjq.cn/Article/details/gxswjvkrk.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gggtlxfhb.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gfpiybpkw.sHtML

I. 正则表达式
来源：http://3g.hesvh.cn/Article/details/gkylazwrb.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gxxbguzkh.sHtML

[I01] 判断是否匹配
来源：http://www.share.hesvh.cn/Article/details/glghniued.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://3g.zdbjq.cn/Article/details/goiqvqjxs.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://read.share.fehbvm.com/Article/details/gmqtpnvdv.sHtML

JS:   /\d+/.test(s)
来源：http://wap.zdbjq.cn/Article/details/guwpgriem.sHtML

TS:   /\d+/.test(s)
来源：http://blog.fehbvm.com/Article/details/guuwyoyuz.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://baike.zdbjq.cn/Article/details/gkxsmmglc.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://3g.zdbjq.cn/Article/details/ghcokmtdb.sHtML

Ruby: s.match?(/\d+/)
来源：http://read.share.zdbjq.cn/Article/details/gacedqurp.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://baike.hesvh.cn/Article/details/galepzkgc.sHtML

[I02] 提取所有匹配
来源：http://wap.fehbvm.com/Article/details/gcsnyqsho.sHtML

Py:   re.findall(r"\d+", s)
来源：http://m.share.zdbjq.cn/Article/details/gdxcwdtsc.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://baike.hesvh.cn/Article/details/ghtgtdrfg.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wap.hesvh.cn/Article/details/gedjltzjk.sHtML

TS:   s.match(/\d+/g)
来源：http://wap.zdbjq.cn/Article/details/ggxgwcops.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://blog.fehbvm.com/Article/details/gdczohdjf.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.blog.fehbvm.com/Article/details/gnzyhmcur.sHtML

Ruby: s.scan(/\d+/)
来源：http://read.share.fehbvm.com/Article/details/gepoxwrrc.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.blog.hesvh.cn/Article/details/gaoivgvkm.sHtML

[I03] 提取捕获分组
来源：http://3g.fehbvm.com/Article/details/gictzotnt.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://blog.hesvh.cn/Article/details/gbnwnalbc.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://read.share.hesvh.cn/Article/details/gfkjyqcxy.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.blog.fehbvm.com/Article/details/gdzzrkwbq.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mobile.hesvh.cn/Article/details/gtttskcvv.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://baike.hesvh.cn/Article/details/gezxurdlq.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://read.share.fehbvm.com/Article/details/gcotcuvpv.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.m.share.fehbvm.com/Article/details/gccbccmir.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://blog.fehbvm.com/Article/details/gkgeihpkm.sHtML

[I04] 正则替换
来源：http://mobile.fehbvm.com/Article/details/gdnvsrixb.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://wap.fehbvm.com/Article/details/gmwwgozbl.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://read.share.hesvh.cn/Article/details/gtzhlgtou.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://baike.zdbjq.cn/Article/details/gxclgwokw.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.blog.fehbvm.com/Article/details/gkcjslnki.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.blog.zdbjq.cn/Article/details/grsmoxuwz.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://blog.zdbjq.cn/Article/details/gymrrfysv.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.blog.fehbvm.com/Article/details/gjvmecyhf.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://3g.fehbvm.com/Article/details/gzizhywke.sHtML

[I05] 按正则拆分
来源：http://www.blog.fehbvm.com/Article/details/gxnkajyrt.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://m.share.fehbvm.com/Article/details/gzuxycdrl.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.blog.zdbjq.cn/Article/details/ghbjxeied.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.m.share.zdbjq.cn/Article/details/gwdbtkyzp.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://m.share.zdbjq.cn/Article/details/gxzkgrjaz.sHtML

Java: s.split("\\s*,\\s*")
来源：http://blog.zdbjq.cn/Article/details/gkjjqwtdm.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.blog.hesvh.cn/Article/details/gocbmwcct.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://blog.fehbvm.com/Article/details/gabrbzjgv.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://3g.hesvh.cn/Article/details/ghlhjgpcj.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://blog.fehbvm.com/Article/details/glhtijwgj.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.share.fehbvm.com/Article/details/grfnfdmdm.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wap.hesvh.cn/Article/details/glfwoppio.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.fehbvm.com/Article/details/gpyrmzfea.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.hesvh.cn/Article/details/gzzkcvwmk.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://blog.hesvh.cn/Article/details/gqexdsfrs.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://read.share.zdbjq.cn/Article/details/gyqgvfqnd.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://m.share.hesvh.cn/Article/details/geyrbkgwk.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://3g.hesvh.cn/Article/details/gzgkaabbh.sHtML

[I07] 忽略大小写与多行模式
来源：http://m.share.zdbjq.cn/Article/details/gldtflvwm.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://m.share.fehbvm.com/Article/details/gugufldkl.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mobile.zdbjq.cn/Article/details/gvcqsstak.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.m.share.hesvh.cn/Article/details/gtvehxutz.sHtML

TS:   /error/gim
来源：http://mobile.fehbvm.com/Article/details/gigwahcnt.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://m.share.zdbjq.cn/Article/details/ghfpkcher.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://3g.fehbvm.com/Article/details/gvkqqipae.sHtML

Ruby: s.scan(/error/i)
来源：http://m.share.zdbjq.cn/Article/details/gtnkkdqru.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://blog.hesvh.cn/Article/details/gsziahyvu.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.share.zdbjq.cn/Article/details/ggrvxmnlg.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mobile.hesvh.cn/Article/details/gfypywdhz.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.m.share.hesvh.cn/Article/details/ghdihfgvl.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.hesvh.cn/Article/details/gmpdejzoe.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.zdbjq.cn/Article/details/gtxgwbgmg.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://m.share.fehbvm.com/Article/details/gynkbeccz.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://3g.fehbvm.com/Article/details/grpcbwowe.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://3g.fehbvm.com/Article/details/gfdcumbmr.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://blog.hesvh.cn/Article/details/gxvgajmww.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/guchbkodu.sHtML

J. 日期与时间
来源：http://read.share.zdbjq.cn/Article/details/ginajwjzc.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gewrchnbo.sHtML

[J01] 获取当前时间
来源：http://mobile.hesvh.cn/Article/details/gyzsuyttd.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.blog.fehbvm.com/Article/details/gvimylzeq.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://wap.fehbvm.com/Article/details/grsslyuso.sHtML

JS:   new Date();  Date.now()
来源：http://baike.fehbvm.com/Article/details/gubkprqjw.sHtML

TS:   new Date();  Date.now()
来源：http://blog.hesvh.cn/Article/details/goklnpzkb.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://baike.fehbvm.com/Article/details/grsptnhrs.sHtML

Go:   time.Now()
来源：http://blog.zdbjq.cn/Article/details/ghltpwred.sHtML

Ruby: Time.now
来源：http://www.share.fehbvm.com/Article/details/gagkxvtig.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.share.zdbjq.cn/Article/details/gvbixltqp.sHtML

[J02] 格式化输出
来源：http://baike.hesvh.cn/Article/details/gpoginfwr.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.zdbjq.cn/Article/details/gdzxhposa.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.m.share.zdbjq.cn/Article/details/gmoiyvfmb.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.share.fehbvm.com/Article/details/gobwhtazo.sHtML

TS:   d.toISOString()
来源：http://mobile.zdbjq.cn/Article/details/gmnuwlugj.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://baike.hesvh.cn/Article/details/gzrqgpolb.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://3g.hesvh.cn/Article/details/goppzwfbm.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.hesvh.cn/Article/details/ghbpjiwmn.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://m.share.fehbvm.com/Article/details/gnppgugyn.sHtML

[J03] 字符串解析为日期
来源：http://wap.hesvh.cn/Article/details/giqkngkpf.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.share.fehbvm.com/Article/details/gyndzedlu.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://blog.hesvh.cn/Article/details/gcpifdmkf.sHtML

JS:   new Date("2024-01-02")
来源：http://www.share.zdbjq.cn/Article/details/ghuggqwyj.sHtML

TS:   new Date("2024-01-02")
来源：http://m.share.hesvh.cn/Article/details/gzzmpwzcy.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://mobile.zdbjq.cn/Article/details/gdzweajkd.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wap.hesvh.cn/Article/details/gppuyqbhy.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://baike.hesvh.cn/Article/details/grsiklssx.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.blog.zdbjq.cn/Article/details/gnxmerviw.sHtML

[J04] 时间戳与日期互转
来源：http://www.share.zdbjq.cn/Article/details/gazsxfqgq.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://m.share.hesvh.cn/Article/details/gmaeltxoy.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://3g.hesvh.cn/Article/details/gyzynjofv.sHtML


<!-- 参考信息 -->