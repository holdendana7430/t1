代发 wailian999

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2wmjhazqf.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2cbempqnq.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2tynalgfo.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2eommgfrj.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2dyqpgbwe.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bdaxefyx.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2jbiogqya.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2ldxwdzse.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2nttrppeh.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2vkpozmnp.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2lriuucyw.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2ysqjjhfh.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2uunxkzso.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2umdccyzl.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2tvtpobrt.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2mlplijoy.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2txzeoowl.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2uifwvsac.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2sihwhafe.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2ruljspqb.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2vbwwrhuq.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2fkebmxfi.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2xqbxomqe.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2jbkmmjsz.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2nzrgygyw.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2cnrsshwk.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2ttrkgmwu.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2kihjnlhs.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2rmnhnbiz.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2prdmwvue.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2ughyvqpg.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2uddrjwxd.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2fnnjehdx.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2qxvelzzo.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2nmqqfzev.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2erfitili.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2oprewdml.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2hcntbixc.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2thutmdrv.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2wuvalqjz.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2xbgxysei.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2bgqbkifc.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2lgbvjorj.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2iqfollwf.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2uhvrcqli.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2yvsvoqwc.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2xangeaph.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dpiysmls.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qiccbeha.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2khdzpgbk.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tvayvlxc.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2qcpwsfnb.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2hmoxacrp.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2vklzrxwz.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ibjmiewk.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2ficihfkq.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2nqcszpeu.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2gdpqmnoc.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ddrvopoi.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2mkapgiwg.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2tmqfrusi.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2jbtaockj.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2ufdwiuce.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2atzqablr.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2fwzvzppv.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2iwbmhxuk.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2gojjilxv.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2vtoxldog.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2cznonjgy.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2hkoxcrtq.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2nwbdqyvj.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2webpfebc.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2fwbdkjvg.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2unhojrfo.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2atzbejdu.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2faelhqxo.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2qqomxnbd.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bgyqyqru.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2wjjddmgr.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2nycsowgq.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2kmqwcioj.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2erevrlml.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2rtnhyjjd.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jflpelqc.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2jstkiryw.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2mfjqqodp.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2gkpohamd.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2yrrsbphu.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2imtzjuuy.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2miegzdol.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2gxpquyhq.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2ltmmfxfm.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2clpiocbs.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2iupsarsf.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2fmnklqdz.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2odifqhvh.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2xpibpixg.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2dowfwzqq.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2vxrpftgv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rrwpyfja.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2dfvdlalv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2oxquesyj.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2meoienuf.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2cesigima.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ssahexjw.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2obsvbxbn.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2mdakumyt.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2zoqvouki.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2irmxpopq.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2vqqyqbks.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2oedvzfgv.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2wafjcnco.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2firahjlp.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2uxxmwosp.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2qkmwmfhz.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2zmrjprjl.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2jufdinvn.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2cxkmswdv.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2zzsojsof.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2iqfwvxkn.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2ssccjmbo.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2lflonxek.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2lwzxsnuh.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2nmgwjyos.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2vyiguvqy.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2tdabkijn.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2osthmxmv.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2hzeodcui.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2hguorgez.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2hxgdsjsb.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2qwsmyfqt.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2nohieaer.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2leunbbdx.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2valqkbnf.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2upbsxnqk.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2kayfbhwc.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2stbssccm.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2dprnhjbr.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2acmkzfkd.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2pprlrbjg.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2epcnxelm.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2irocjuys.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2snequpzo.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vfzexokb.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2lnlhxbxz.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2wbhcbgds.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2komapbht.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2jcieghop.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2ebzqoxwj.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2uuqepeay.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2nbnsabhs.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2szxoueyn.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2efwzvmrl.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2gqsvpyhi.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2osnsvftl.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2gatkecuf.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2dgetjglf.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2ufbzpqth.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2egjryzeo.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2qfsdganr.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2smuwjovt.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2ayygqnzo.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2devmtyqh.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2cnkelmrj.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ruhpkxyn.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2jvhbzdtg.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2gssjnlhc.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2bhnldmey.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2gvomtdoz.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2jwdwrwol.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2ktzmuggj.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2xuhoapwd.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2rfilptjb.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2enyoktux.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2pgnsfdwx.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2twebkpbt.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2rkdomouj.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2yrlscpul.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2dklnjxft.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2bgaumikb.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2zulgewga.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2myakawcd.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2vhkmzgob.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2fcyumkmf.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2shpyqfla.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2vxkghjca.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2zzkktfjv.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2mmrmlezn.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2dabcxxiw.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2aduutvzc.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2zfxxgagm.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2xbgqazgy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rhvocpfp.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2jhvteiqi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vnxzvnrv.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2pgelkwir.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2qcgmwuzl.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2lloxshxl.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ygxtoehm.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2bbipuuzj.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2sjbhcote.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2uwtjccus.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2hqnmivea.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2zbdguixu.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2xsiikakq.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2vypbscai.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2zltsqhel.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2qtgsmfms.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2orntuaid.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2kyugkvew.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2oteokosa.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2nypqhbkz.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2jqmwhnxs.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2ojiwytkf.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2mblmrlsc.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2zdueiwbk.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2jrgtubiq.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2antjhtac.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2gfergisb.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2kpafrtwr.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2dvmhsgnf.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2tlesiyxl.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2cbptwckk.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2eknczzqi.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2gntijsfw.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2ygnulqwz.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2vfuerzva.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2sjgnstgj.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2zifpfaat.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2xarglrxb.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2aueltcbr.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt2coymksjb.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt2ikahutlp.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2qjrnjcib.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2emmrskcf.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2ldmrptbu.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2zuuzjshd.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2dtxowlto.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2prfuxsch.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2joziowum.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt2lmjftlrk.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2pspnwewk.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt2kbwvhjri.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2ptszdenh.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2vryatqrn.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2mxjdltld.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt2vmmphcat.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt2scapxzhb.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2kdoccfgc.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt2txfalmpr.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt2icineivd.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2zyxoinmg.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt2cpoilpjz.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt2qqetrtpp.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt2zwcpsfjt.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt2ydunjayv.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt2psjxhzlt.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt2ghpbgodn.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt2qymqsiuc.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt2ikvyjjbz.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2aomsibzh.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2yvcxxcxe.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2iqzswryo.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2xkwukybm.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt2apzvxzbh.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt2ggeprqov.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2bvardjes.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wbrjisat.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt2lkrvsgpl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2quccvslc.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2yonwadgy.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt2qceatwaw.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2pzzjxubz.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2louhufxt.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2jghvktxr.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt2vbwfqhqz.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt2lwjznqmf.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt2cxzillpr.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt2bgoxemvo.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2drbxwomz.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2rnvjwwch.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2lipndeew.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt2kfxvlvpe.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt2xxxvklqn.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt2wivsogry.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2qhfefwzq.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2xkmuekyj.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt2kmylcgfv.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt2dqpafaqh.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt2nbtytigk.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt2vqsclaft.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2vjjkrvdu.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2rymuzfcd.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2kqcrgmml.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2tmgskoqj.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2cqdvylvj.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt2fmzjqtgp.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt2rgfosayk.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt2vmnzeuip.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt2mipgytyw.html


<!-- 参考信息 -->