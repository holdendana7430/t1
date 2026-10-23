代发 wailian999

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3tvjpoxro.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3itwfcwou.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3wyaahwwa.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3foytiiua.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3umziarly.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3mqnojiev.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3elksuvug.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3bcwodayh.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3fcyhztkc.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3vqfmcorw.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3vqybsatf.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3zxsrkkvw.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3utgogvlp.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3nwlvyibe.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3kygfklva.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3zrupukqv.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3funicgla.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3sqcnjcgc.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3edikbuwq.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3fqogxwop.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3lkquzswv.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3pnpcjnub.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3mvzycihh.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3ngocoyxi.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3vccsnrdm.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3evdqfuyt.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3dpgcffds.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3nbykjpbv.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3oknvdqqp.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3dnhzmxxd.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3xuppskaq.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3cessvmkp.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3flrdaojo.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3doigfbcz.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3xhxnjfjj.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3rywyiztv.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3xlmfqssd.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3eosuyhud.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3zribhrha.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3cxcdldht.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3feujhysa.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3ahavknnb.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3jytflkcl.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wwgjxcfe.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3jpqdintl.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fatmknac.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3gfohljld.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3mvlblyif.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3xabwoymj.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3nojttalh.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3wpyagpxc.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3atgavptp.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3kfztrvfy.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3anvpomxv.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3vsdonxzg.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ruvmztgi.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3kribazwr.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3rbiybziv.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3yzkgvmvq.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3rsxwacxd.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3vjinwazx.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3xrjteuld.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3hquvymfj.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3iedugysq.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3qdqbrwvk.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3ymkupaiw.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3mdsbtemh.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3evkbbxks.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3wubbnahr.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3xyjjugrt.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3bensvamk.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3rsgulbmh.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3tqjzmasw.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3bhqtwpza.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3yfgjuxog.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3pvoqvtrq.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3uherqdcp.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3jgcrzykp.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3qqexnhua.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wlyvhqrj.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3qylaygpk.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3rldgodfp.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3gyfcjxyg.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3nomjptou.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3fbjzhsxo.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3hgieytzu.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3wyhpvwju.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3jdmuyhpx.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3aoodsehn.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3wbzeggxa.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3jbnnbijm.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3dwbmeltu.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3kvktvkgx.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3gkzhzqka.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3nqwmqvie.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kzsdwcbc.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3htddshym.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3imzaiaeh.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3txrnscst.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3bcypzdpy.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3tdneeske.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3gaybamnd.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3utmeksge.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3wivxwghs.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3mhhmkamd.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3lardbvsg.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3arumfnhu.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3phksvmko.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3wozktfps.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3optqahvo.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3amjfnyux.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3bcckckgd.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3pvgokrvk.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3fckarwid.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3nzkwepba.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3vfnofaqz.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3gtzualod.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3qccoelsi.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3tbazhfpx.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3nnunuqll.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3rhnykusd.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3wrctrrsy.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3jwxaofll.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3pkofkqtl.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3hpigbwnu.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3oxxejhod.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3vlyucecc.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3rfnplnbs.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3zweebcft.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3jakoqwio.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3twadeheo.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3wckzblyw.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3pxspnmcj.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3oizdlftr.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3ooltujla.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3lbmifzmg.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3ppjnifdi.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3sjjrgbkz.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3uxbqjjtr.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wasntpgs.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3ebpqadjk.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3mtdppqny.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3xvhvzryu.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3slqujynk.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3oabemymn.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3lfeqeedz.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3bffjxalu.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3epdspqwu.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3hyyazpty.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3qqfpzywv.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3qojzsseq.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3jikecpwc.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3stwhhetd.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3xanmadhb.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3yntkeuqx.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3coyjtavl.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3qaelgyvv.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3zawtbrfj.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3wieccdeo.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3bsiesptu.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3mysyhxej.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3kqufhlsb.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3mwrflkig.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3ngyqrreb.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3xolbhhmt.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3rfpntaxe.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3dcmjaovf.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3ltorwdqa.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3nnhqzpxe.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3xrtjzcnr.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3vmwwunjj.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3gfaagsax.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3iptwhxgz.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3broumajj.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3fyhrfsnw.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3xgunfjln.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3udvoytvq.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3lkwtimqm.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3hhveccpa.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3okdfhpun.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3qvktyiyq.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3zbqrwgbv.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3rvsxhfmv.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3yitpudta.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3txcjoctc.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3xlsttabu.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3hhbvxsbu.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3lwzkbnjx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3awnbqtcb.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3xsmukwxn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ovytkmhg.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3sgtfzouz.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3btaqgehc.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ljlgrxfj.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3jcmzafmh.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3syisopjj.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3svnaohxw.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3firnucma.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3cleqrbcn.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3recwnlgu.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3qkvhyjsg.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3amcomgrf.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt3mgqouhuo.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3pyzhkwtj.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3sgqojgve.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt3fbgnjjrf.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3sakfzeeo.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3tuxmilkc.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3dptddwdc.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3sbhdmkyu.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3xabkckqi.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3jzwashdh.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3laklxtuy.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt3pzwfzbzu.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt3wxlslsxy.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt3etxoutha.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt3bqevfxym.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt3klocmflh.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt3wkjmdjia.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt3lfehuiwj.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3vjvpkuvj.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3awdnaikf.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3xdiqkucm.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3abembflt.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3jeztvyyj.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt3rlfssurl.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3dgmtbfyk.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt3yajdfyrr.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt3kvptehcm.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt3ovwbwmff.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3hxghzxpa.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3zyzelfor.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3wtsjvxnl.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3akgauyai.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3lyjmfwvj.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt3mslwusnw.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt3ucruonfs.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3durmroua.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt3nehvloyk.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3aidzowke.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3lffffxae.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3vcpuvasv.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt3sjoujebs.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt3vcqbrfdt.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3kxezhqnv.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt3fibrgkat.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt3oyvymrow.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3aczmpfdj.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt3xnidbcgj.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt3gifuzvmw.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt3wgqckjlg.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt3opvfsoiu.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt3umbvbzax.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt3vmwromfx.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt3doznghus.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt3oiulrqaj.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3vnniucbx.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3mfxkozfy.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3lyyjkwpm.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3okpndpcq.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt3vroicgdz.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt3ntvqnxey.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3edhsnbcf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ynkcaaot.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt3cxqyiogh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jtxrorff.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt3nhmooskh.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt3kmffjjnf.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3cjsmmsnd.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3hibpaibb.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3khpzjnwo.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt3jvvwgijh.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt3pvwgvucs.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt3vpnouqda.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt3bymsomlm.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3axglxlqk.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3jsitkwrw.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3tbpilasr.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt3vdpragkz.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt3xrlfctzb.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt3edvlxfut.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt3vokwowwr.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3pgbkfivy.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt3zetafumk.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt3pihfzjdw.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt3xratwusg.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt3vcayjxpp.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3qqasmczf.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3gsglgeyg.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3blgzpkdz.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3ebnhgmeo.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3lomqenqq.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt3wxotjmwp.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt3bkupxbxn.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3wuooxvsl.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt3nrwlmtxl.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt3lheqtnud.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt3dmxtdfaw.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3fbpbowzy.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3twefrnoe.html


<!-- 参考信息 -->