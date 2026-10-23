代发 wailian999

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ocfnznim.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3rvswqrmv.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3klkgbnzl.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3esejtkvn.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3quswexya.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3greaxgrd.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3xtjpuqli.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3cihjdzpq.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3mrzcqobb.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3wuwfobsb.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3hrvptctf.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3disfrrzz.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3ooxfbziv.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3iuiymewp.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3vwauwbcn.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3xyrdbmiu.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3xnyznlqb.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3exgupbaf.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3rswnrynx.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3aznasgil.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3wiokfaec.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3bckebrpp.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3dkulfkqd.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3jjkbemhs.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3zkijiweu.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3qnhjrgth.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3irpgymtf.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3beccpuqm.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3iflpkhik.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3vzlvvriu.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3wykyzlhy.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3sxherzai.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3hcbphxai.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3pwhxbykv.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3dizsgkaq.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3gbytxfbm.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3bgcrnada.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3lztivdda.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3ropzrhfy.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3stjtokyg.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3vjmgzaqe.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3ekkqphol.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3ytwpkxrj.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3xhhlenue.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3rcrqvbik.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3dvkskjjp.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3styhwexx.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3pncmdqrq.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3cccmoeig.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3snezugro.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3mhfrhizc.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3ijhdqyun.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3trrwtuxz.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rsptjnwk.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kuxvlqvf.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3wbhprsbm.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3arfenlir.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3rkeezyhk.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3nrutssqd.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3clealcru.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3cmjuiuvm.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ewspswzq.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zcpkjnsb.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wnrbcejl.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3ishxaxyn.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3exiqwsyw.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3dxqnucbq.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3fasquhfw.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3gtxrsxsf.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3ghjlpxgg.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3jovaqgnj.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3ltzeyzxi.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3vtegqtfb.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3ggstveui.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3elucmoji.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3qvixmjvy.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3eiclubnz.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3zxqhhzlr.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3dujefgwp.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3nrbauexz.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3jsrrjpon.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vyecizqt.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3bsfveijh.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3gpifmwrp.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3ibeedywy.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3lshtohcf.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3rkbiqomi.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xdcpskom.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3apxoblgt.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3mvwssyzv.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3nicdrjrp.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3vnrolwrf.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3szlnargw.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3yqwzikph.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3icdkuxuy.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3runilksl.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3vyvempwn.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3udevfevo.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3rtksuitm.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3manxabow.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3xxfzfzra.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3xexxdevn.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3dmcnyiol.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3htkuixvo.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3agyuxwel.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rucoclgk.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3nchymkyx.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3jpzqiqlp.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3izfqsjbu.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3obgiqymx.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3vnxhxbiv.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3wigsfalg.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3eukmrfbl.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3lognahbf.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3oqdjluoq.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3aprprpef.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3nfyqszab.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ladnrboh.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3yzwmpequ.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3zyizhdnj.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3eacdlyfl.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3ygioodvw.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3qdymioxv.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3absyyiwp.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3shsmgpsu.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3rmgmchox.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3dmakkbqv.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3nqbarayy.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3kgqfjsce.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3kgghmsin.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3fkbacugk.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3kuktshmi.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3dcxjpfch.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3oprozmou.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3gcvzxxoi.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3wmnllmse.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3gapfxiun.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3iznvceqg.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3ucjqmcos.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3nvbivian.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3nkcbnhhk.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3mnrwwmcr.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3rbyqjavg.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3ymevyfih.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3mohosqzi.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3phezjnnt.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ynabtfvo.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3syjipzbv.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3ijdjwjza.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3updwywrr.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3biifjbgm.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3jyeekymr.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3riwsmclr.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3pgltxtmx.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3fmzfferc.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3deyvsiit.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3axwnnzvf.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3cigxvgag.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3lrtyznnr.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3btcyarak.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3gnmwczsd.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3corneiam.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3wmklygui.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3jfakcvzk.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3bewrktjd.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3mbaypvsm.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3ivrfxmjt.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3kcinckgv.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3vacdqrff.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3bkxtltbm.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3xwtfeocw.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3iqrmkpvt.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3opszvnld.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3gnitxhyo.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3lalvelsc.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3tkoyvfgx.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3iogaelhv.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3srchgbkn.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3gztnlncf.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3wlkktlbz.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3vndihkwr.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3nwjpoqya.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3rfthgzti.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3rzqzcilg.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3thobpeiv.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3bjihhxqa.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3gbcihrcf.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3fwttrnxc.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3rajrqasp.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3qnzpiawm.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3ygwxzuey.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3bghceleu.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3fblpebvh.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3jxxenuyl.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3zqxunzdv.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3yjnzqmkm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fabldylr.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3amlawifa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bqinnsir.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3riqwdayy.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3xensynph.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3dpwhxphc.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3gyiulfow.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3svitkzaq.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3ingfmzhg.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3imdvrloc.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3zqvhbthz.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3idqpgwar.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3gyvvrmou.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3majjcrrg.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3obwpxpxj.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt3prkhkbrp.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3pcjvoemo.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt3fadsmuov.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3wbwngvhg.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3rhgoxbtz.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3yeaospsh.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt3mdvngnjk.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt3zguqwsxd.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3rcexyrom.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt3yxcleouh.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt3dhgrgwkk.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt3ituvjcfh.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt3uuugdtio.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt3nidqleqa.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt3jqndxrgv.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt3ezlvqdia.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3cwbhgmed.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3izwwaxdn.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3odkzjclj.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3gdaymvrl.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3fygpwgkv.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3wwzjtqqn.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3xgliqjef.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3zzqxmuhl.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt3hyxwtmxs.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt3vovqtekk.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3dimecaut.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3qysguwua.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3eruyokhp.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt3btjcwtkg.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3tmnakcpl.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3hkgwenxs.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt3qcjbcrvq.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt3sxmgyztf.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3tshzjwbq.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt3yixoaeez.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3khwgwmfq.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3aifycjhu.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3gqpyvwia.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt3wutwdski.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt3vlvzmvsi.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3jaztekne.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt3wnasdqmr.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt3xvogpgyq.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3cezqceln.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt3flwfrhwg.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt3ooxxgwmm.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt3dxoyjoku.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt3rgocqyjf.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt3cvpbtuki.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt3waoqbini.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ouaffaph.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt3nikgpxfx.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3iohpijgw.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3zfmvjclh.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3esbsdxmb.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3pihjhery.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt3smcnfvrv.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt3cshcadki.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3ypcxqaos.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3esmobkdv.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt3qkbldzpy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uwiwpyke.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt3tiqjrjla.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt3tkukbsdj.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3rpzcvvyn.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3recalrrh.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3zvstxdxn.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt3owgocgmr.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt3tadihtor.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt3wdmgyjma.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt3mrfgwhbm.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt3illnwbvl.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3jgimmmwl.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3hftowdoh.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt3uarmgvzi.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt3ymwzfmop.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt3fooxrpdv.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt3vxftndsr.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3jhnijbvi.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt3ookietnj.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt3assyljli.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt3huwmkmfl.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt3uovkbang.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3opohcjdc.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3ielqrrqe.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3piulbpzb.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3hpxxrebx.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3xamgmmaw.html


<!-- 参考信息 -->