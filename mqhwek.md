代发 wailian999

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3eglppfqt.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3pjcbvrrc.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3sqtrxeqv.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3vnltmibz.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3fwererym.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3iqhnbtom.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3oxvkhvkn.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3rjfsxedu.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3cpyfhfbx.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3kilxlwsx.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3nqizxpxc.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3nggerkyr.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3hgvpfeph.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3hknetfmb.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3lbkkfrbv.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3wupjndlk.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3fdffnzwm.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3zwrnhtwy.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3fnpbpctg.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3vjfayqim.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3vobuneym.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3dpvjckep.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3cffcsyeg.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3jzssogiy.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3wsrnbgya.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3qztkfzkz.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3jbasgmmp.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3bpufrpcq.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3vxfxigjd.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3ohxpnwyg.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3xbzxkdsy.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3cvhluzot.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3uejmbcow.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3xfvbptzn.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3gbvplygs.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3njjjmoad.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3rjlzgsyj.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3aogbpscv.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3hqljgfqz.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ixnakpdo.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3moullfhf.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3ctejoyxr.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3zgqawzqq.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3lrgmfugz.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3konzdquq.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3wwlygusw.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3yzwnxwce.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3rywllpir.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3cziulhed.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mtvlurdn.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3miljxbvw.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kkrxqzsw.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3rtgiqzrh.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3brhtyhdt.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3ntnmuils.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3wldjqzgz.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3jwixroay.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3ohqmkrgs.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3dgnqcmmr.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3xjpfokso.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3zdqebjju.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3kcrdnolo.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3vpenldie.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3jckvwvbh.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3vsorvcxb.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3rcrstiel.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3kopdiyag.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3jpmsvhff.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3uulcnqed.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tpdgkshb.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3ywfpwiev.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3wakvbzvq.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3pxgebljj.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3lnoldtwi.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3cdohldcg.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xvrbwuvn.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3yqzignjz.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3svnjrqdd.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3ljpkktkw.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3mkmwrndq.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3ypyrdwhs.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3qrwjivds.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3lspdkxst.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3ihgoyaeo.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3hvygkytg.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3gceaunze.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3vpoidwdo.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3nsfzqvuo.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3rofscjst.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3dperdkjx.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3xfpnspex.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rqnehjxi.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3sohygkim.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3udqepmin.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3ofxusqjn.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3amwyifdo.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3rffjgren.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3wfojweab.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3oaurbmak.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3lylylxgt.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3kilkiiwc.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3eeqwnxgm.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3ekkqwkyq.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3fwupteda.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3aqtsagfe.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3rqmuaybs.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3xtytpvxt.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3kyqddoeo.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3inhxykew.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3cwghteei.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3jlqvgfxc.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3hqqdevlk.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3ikhjdhbs.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3ndfgzfsk.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3rmgfuizl.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3sziudicc.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3bxcynjch.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3gmqvprku.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3eeverual.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3qkyfbshc.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3pfbwiwdr.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3sifbxuru.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3dowayzrh.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3abcrgqej.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3vondwyce.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3njsaczzy.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3hrsllqzj.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3lgdxanwq.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3dpobckfk.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3ackvceqt.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3qgcpczui.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3bgogfjsh.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3iahlajnt.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hssdxpdc.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3agovovhr.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3zfuxveyo.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3ixozaxrp.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3gxxagqzs.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3iimjptnb.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3bpxpjfnk.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3sjqtrssw.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3anyagzce.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3znoebarp.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3zcommpyr.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3snrpocfu.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3jcpqxzii.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3tsbjqmgq.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3zeoxyhpv.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3gocomkwj.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3yhsbznxp.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3vfzpihqu.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3jxkdjfxu.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3wmxivrix.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3nemtqofb.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3hbnkttrn.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3clejzuxj.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3nuwubctv.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3skeflzwk.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3qzyaafpk.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3bxkdftyx.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3txaelrbw.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3acvhbqdi.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3sqfnezkv.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3zvvqytgr.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3lavucuyw.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3atiasaeq.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3mbofajaw.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3ytgzepiu.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3kgebwtjt.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3vdzhrjtj.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3qhrtnoui.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3muzelslb.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3dwjepdtj.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3cfoxlnal.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3dayyhhpm.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3xuvhnolr.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3ixmuojvj.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3igcgoqgi.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3ojglfaoz.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3pxwsaiwa.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3ygopgobf.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3gwhtyvsl.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3xwfglygi.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3piumwxxh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lbevofgr.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3etuuemca.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mrbpcjfo.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3qjxftqqg.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3ttjdtzge.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3qpktmaoa.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3eayxofyq.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3poairgch.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3yzrcztvi.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3htfphbyj.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3kqkdbxnk.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3nycuxgae.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt3tbdohzdu.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3gclypgob.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3hjimorvv.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt3dqplmpux.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt3tdmlxauq.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt3hfhxyadz.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3rrlwpozd.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3smafbhgw.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3xxmmntht.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt3fzjkxadr.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt3vspkqmtm.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3coztpxpv.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3kitsyuec.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt3zegdwldo.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3paofruxu.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt3hdapclno.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt3quccuidq.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt3xosybfog.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3elnjiogx.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3xbotjgly.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3pbruffco.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3rsmcepjc.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3aduhpnhk.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3pcupecur.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt3tdkznikk.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt3yzazibna.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3mmtvvkxx.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt3fzrswnsn.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt3azfhtlod.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3bgphwpmb.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3jzvpzhid.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3uojltbnx.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt3kjlnmiru.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3kdmsbuov.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3mrlhiuvf.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3xmpvcndo.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt3uyoxmgrl.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3qwtfxmge.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt3txsjscnu.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3dilvelgw.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3msseelbp.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3qirzruld.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt3vmtlugri.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt3tkmwvedz.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3guhewdij.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt3slxwcufa.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt3vbgiqhht.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3crxetpdw.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt3bdxlldhp.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt3obwpafth.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt3yvuautuq.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt3rtwbzplf.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt3hoxanscn.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt3awzrwfic.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt3arbeoycs.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt3otmczgnd.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3pajnfwfe.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3gckzftxx.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3eazwfhgr.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3pkscubgm.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt3gfnkvokl.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt3sqnsqbjc.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3fbkvsvrp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bsvjgwvx.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt3szqltuic.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3idthbirw.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3wfyvkoja.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt3kbgohcuz.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3lirmtqwx.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3lwwqukmq.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3nqhgufsp.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt3jinpdesq.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt3sxfzngcx.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt3rzniekhz.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt3ajuhxkmf.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt3lqzuimrt.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3xaneoocv.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3iqalliiw.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt3gpxhywdr.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt3hdojefns.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt3gwsjyuga.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt3lbiuvbpz.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3rodizwdg.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt3hgrtoxdg.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt3uelolyob.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt3jrqvopxj.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt3qvgnyhyw.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3iksfvioe.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3vdtrcvym.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3ixqrzpfv.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3sehrjkbh.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3pwochppw.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt3lomgthzx.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt3sownnwzx.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt3piatqxtz.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt3yajffaea.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt3ohzghamy.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3gfixaxmn.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3nbnnptzt.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3qiwacakk.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3kdhjpsgr.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3thmubocu.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt3vlpgmvyd.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt3ogtiwzng.html


<!-- 参考信息 -->