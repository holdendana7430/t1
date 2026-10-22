代发 wailian999

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2jxppaace.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2jlvfwnvz.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2gkkhircx.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2lakbfpng.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2ofdbadqg.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2sjgbcjwq.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2wcfypugw.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2lebxjngb.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2evqezcbv.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2czezceie.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2pvivlgpx.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2ezvgvocv.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2vodvxdcr.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2fehmbhfx.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2xyehzblf.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2ztekgbqz.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2eegrsrjk.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2mkkjruue.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2rehpjmnv.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2zlivxowv.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2tnxgycqt.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2hwvmeeyy.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2soibpidx.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2isuodczb.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2relgvxwy.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2ynoduhor.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2vrbthxjw.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2uqlsayyg.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2qxvvopcc.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2zgijwbpv.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2ddzrdtge.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2vftkxwkp.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2iysuxeyy.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2tlutaphk.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2jwbfjesl.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2cjsrnkmw.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2lffxpktz.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2uluyhpgk.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2sqjlmzeg.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2chepsaix.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2lkpxpqcn.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2rwitmpde.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2crvkveph.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2qxmvcwsz.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2pgtjgdoo.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2abiklczn.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2comvufpm.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2dppwzmjb.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2rcbgsmty.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2envttkrr.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2uckixjth.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2cfhbikeh.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zewhydtv.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fqfdmpnh.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2djjhxukb.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2tlfplimx.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2bffabrzg.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2fsfxfgxl.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2epqftcpi.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2mxrqvfsn.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mfrozjuh.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zlyqlhqd.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fkwqunts.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qqgsvlci.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2gjfkvjuw.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2mnhdeqtb.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2lcbxvscl.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2fjiegfrq.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2aecrdaul.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2uqvugkgl.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2phnyqkyl.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2eigbtufx.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2oaoqufey.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2jqzhhjfb.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2zrwzapoe.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2hjoctybh.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2axwtksxv.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2yuvzhdeq.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2odahgwmv.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2knlkcwga.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2vhstakai.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2wvyzbxll.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2xskcrmgh.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2shgkshua.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2loryzvem.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2xqxcopfr.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2ymmwcqia.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2ncxmtktz.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2yuzcevxj.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2bbvcgrmn.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2jfuqlioy.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2fuvfxngk.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2yyutxfnx.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2qeydldrh.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2hyrajtum.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2avywzyrd.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2hisqhtkk.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2dtfymezd.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2uunfopbx.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2cwheokls.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2euidprei.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2ywhqijih.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2juuneerx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jjoaydtq.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2jhbmpcqa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zksenqxf.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2gixmpjum.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2ycmxpqjd.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2vxmtscxu.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2jjexvpyd.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2jhmdxhbt.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2nxtfupru.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2nrugzrwj.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2fsfjtdyz.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2ndzbzosx.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2klcoiwww.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2uboytkcz.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2rviqwgvs.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2exftsmfi.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2txpiwnrc.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2yipwhlzg.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2pantpput.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2tupnwtxi.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2atofnoyp.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2qwipuiiz.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2ajtjjxzx.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2ygidjmgv.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2rozlsilq.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2jpjgiygb.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2sqhyffje.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2nzudvvzn.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2ugayajwr.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2tmpccvoj.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2utmohenl.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2frpccdyw.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2tkdturlm.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2msyjcbcq.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2mfbsgyzo.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2mxdselib.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2bucsgjnr.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2iaagwxig.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2odndcycb.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2mayrwoqq.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2gvotabnh.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2hdreioij.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2dolbrldb.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2satsfgij.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2itwqfeqd.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2bnwmlcgj.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2qcfgrfzx.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2djlocuec.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2goncqnwu.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2sxophlka.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2esenambv.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2rihtzeuc.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2azmhuqak.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2wjtuarai.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2wsisafxe.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2cfnjzzjs.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2mcobdpch.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2khgalwdb.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2jwvwnbel.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2hcotbgtj.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2kwzfliky.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2pjecbyef.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2vaxesuaw.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2jgpbyjpp.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2wrkxryqn.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2cuypahsa.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2ggwikfxd.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2igaxzckv.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2bbpvzgsc.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2ilmxuaab.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2psilshao.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2cnbkjhcw.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2opvmylyi.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2lffbjzja.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2uhgrdwxh.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2bxgmzbtk.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2lrxwhbbh.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2fswlkfmo.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2xgwjloms.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2zhirrhla.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2dwkpfcwe.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2pvzwbmkn.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2rowapfuu.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2nklitjot.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2mhgzhnkq.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2csxoqzpk.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2yfnbhwjg.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2dhjiluoy.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2lpnysvwj.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2woqhlikv.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2nrwrizoi.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2keyklwjw.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ovmvzsvb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ehelexuv.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2lljrjasw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ubvjaizw.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2qvvvuzuv.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2hckyewyw.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ezsmcsbo.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2zbtdrfdr.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2decqtgly.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2yrkbpaeu.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2cmhlxmmk.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2crcpufis.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2wvljsceq.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2yltrzyor.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2ecjnzxgr.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2qgsuwldm.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2xzsuteax.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2ofewgsjx.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2vaambcdi.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2wiybyxfz.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2sabrmceu.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2ljihnfwf.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2imeklscy.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2jyjstoxc.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2sxhgxwis.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2qgwwjejd.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2bvbngjpn.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2qmduqddl.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2qepdxlta.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2lyxdjjuj.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2wcopgbkz.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2xrckfncw.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2bzvihfwv.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2yunmdilf.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2pydhwnuh.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2icmffnxh.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2bhqwgmfv.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2azbhaygq.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2caomafnv.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2uhdwnyxy.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt2rbroqtem.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt2gjswtlwp.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2vqiefxnm.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2xnwgzyhf.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2bjigshye.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2vzypwgji.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2xvjvybal.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2xronavop.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2adnasgfr.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt2nkeegrvb.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2ihikuvin.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt2hxbmjueo.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2adyaayyr.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2nvekgdcz.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2mpqawjip.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt2hzbjjczd.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt2skytptin.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2yzzrsxss.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt2qplgqtze.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt2bztrfirt.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2nudmdryq.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt2zcrfzsfm.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt2jehqogsl.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt2gkekovjn.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt2gyvsigqa.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt2nkzshoqk.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt2tpecrora.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt2lqokwnrs.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt2brmfyfpf.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2jvuuopsa.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2lzphgakp.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2vwhqccen.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2esvpadvz.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt2yobhmqzr.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt2iyijtfcf.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2asjnaixx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uektyyng.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt2kavhmgix.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ejgxexqb.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2fpxillba.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt2jlmppzbz.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2wqsdxkyz.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2dqzaofbd.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2ltxqciqd.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt2artvfimf.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt2cjwoqozb.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt2efxwjzas.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt2ycvkimbl.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt2qnrskgio.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2kuicnoqn.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2fwqloydj.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt2ckrsjppv.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt2euxvneyx.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt2rdzeoslc.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt2xlwznuqy.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2pekiersx.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt2abslsfev.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt2numrgzez.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt2efvijqux.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt2fplatisp.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2vuicoctj.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2grpeqwki.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2snklauka.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2cshsznoq.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2fddmzmux.html


<!-- 参考信息 -->