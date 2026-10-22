代发 wailian999

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2oatexizv.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2oaubvqce.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2jzzlzztl.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2vqwgriay.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2obmvnpgn.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2jwuguczv.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2pjlhaclm.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2gtqkqrhj.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2xvdtytzj.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2rcgzykrg.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2dtdngenf.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2kxayhvzu.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2xjhopwhq.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2dnqixier.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2krzhyggf.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2qwbulisp.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2apxuulls.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2vbqsqfzr.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2rembteul.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2tkcvwhzp.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2txvinbwf.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2blhqzeww.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2zwniieqz.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2ydbakskz.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2pnrqloys.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2mqctwsyo.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2pxipeoyv.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2oyroxhda.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2qdwlfjid.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2sxomywfk.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2mankzzoq.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2aiemefkc.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2rmcqqfix.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2iwuqtpqh.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2mmuihpin.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2smfthcmz.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2utrlhgyt.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2ezrxjyhn.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2kgruqhiu.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rzitywjk.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dfevaccx.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2kqwjkftm.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dmcmqepv.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2pdljpetb.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2kjzjsskp.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2rorysbju.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2yumcuyeg.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2yrirochg.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2cudjaqep.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2xkirzqlz.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2hgdrawxg.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bduhlnei.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2zubsxklt.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2shxhbxki.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2fbtegygy.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2urcmlspk.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2nifoywef.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2tpwyqexf.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2xmnjwidw.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2pbvvsjlb.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2huwxmefz.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2bxcpmgdg.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2jekzonsz.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2jfbjzson.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2pmhzvlas.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2pprvvuke.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2bnauunue.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2zknvshow.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2hvrghyxd.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hrleayni.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2iwqppjsd.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2ilyliwqr.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2vyvudhji.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2dmtlymjf.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2tveoynsh.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2njnrermv.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2pmntfxhe.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2tjyztsvz.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2zuydgmdp.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2oyanmpjj.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2yeirtdyu.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2chpqncqk.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2uucmeitd.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2ghugderr.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2cchjfptg.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2mqnnqgro.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2hlcgrwpi.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2zdkwqjvk.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2kzhwttwn.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2onkohuvm.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2ahlpniys.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zyxagktt.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2ddaevaez.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bblmzhaj.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2ynqwbwcq.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2rqecniop.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2suolcyad.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2luxbogww.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2tlfetsvx.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2oowbvwqy.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2fxiokbhq.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2mxhehrwk.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2rtmdtomg.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2xnagkmbx.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2unpnzmcu.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2vczvyfvv.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2ipltctan.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2utwjghbc.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2jtwccdod.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2uwntczjc.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2bbnvkyon.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2hnboudtt.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2umjlrucy.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2iwwtxeao.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2cdsjzrmm.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2yfbvqvrt.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2ffclvbsm.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2qgkcbioa.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2xzubhawa.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2osftgsjd.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2arkaclnz.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2giyaltes.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2corgoysr.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2zlwrmnkl.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2ostifjxv.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2zkxwqqso.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2iwxsihwh.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2zvfdudmj.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2msbvfrhr.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2fckxeqck.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2cpimdroy.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2xmrialaw.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2zjnotdak.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zhqkyhps.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2laqqinnp.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2lhjrtegl.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2yaoausit.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2imqspkoc.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pdheljxv.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2culrloty.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2rcuwkchx.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2naqpiayl.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2qtilbzzx.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2hruwvvaj.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2azmotxwn.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2jriqykrh.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2vjwyhpgc.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2fqqmlgxv.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2cfvnrdhi.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2pyivjsnk.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2smeplhon.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2lnqscmhq.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2xtrbrmue.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2hewdfkwf.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2jenivyvu.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2knpeedad.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2embzpnzv.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2sbbaosgw.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2zbqnhjiv.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2uuwqzlxl.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2azhkguds.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2fmpgdyzc.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2mzxervcc.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2nqtgawoi.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2rladwtqs.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2lumqbddx.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2uhetojzj.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2azklnvea.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2pciejems.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2gphfcitg.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2shtxvybk.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2drihjuwu.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2szerivdi.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2isytvwls.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2aavebvrt.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2rvbuvssj.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2yfetftjz.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2sprouqdj.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2oalboblh.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2gciztapg.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2glmpcuff.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2wgaleqrm.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2vlcjpuuy.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2bhwyxfzo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fliiohbn.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2jgjnzcvd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wpvyhgnf.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2aygrplco.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2bilihwmh.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2uuthwofo.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pypgqszf.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2lhpunvsm.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2njlcaozm.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2evrpgpoq.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2zhjhqcbh.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2wbzqnnge.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2bjiamxpq.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2gaziypvs.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2lzedzmxq.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2wfhjrpth.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2yeqlnrjd.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2canghidt.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2brustndi.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2ztceqyte.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2vuwfcgps.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2psaakwml.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2ikcboleb.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2lxmqyxoe.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2ydbrnzxb.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2xwucnark.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2xcjayxqj.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2hlhlwrnq.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2pcifuyhj.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2sflcisfn.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2ylizgumy.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2gcxnjarg.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ixhsplvp.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2zjfikqrn.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2mybykasi.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2nfavfsev.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2nwymwaxf.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2wttvqizg.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2lpkrinfl.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt2zkrwqagb.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt2qlkpggxv.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt2oxymlelx.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2dhobvnzc.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2lalvyywn.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2dumoount.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2qycyqnnc.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2jpueupfr.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2ocmhewgl.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt2dtpndcgk.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2mbiwssse.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt2wflhfssf.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2npgcjqce.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2tpqwppzr.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2hokjvbix.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt2yrvkmylh.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt2rqzvzlab.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2putzabmt.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt2omwsjahh.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt2qbfukckg.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2cdwtivgb.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt2hxanbiov.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt2miksddvj.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt2bqvbdgyd.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt2tsccunyd.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt2inweohwr.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt2thkntapc.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt2prsufscv.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt2kfblzafx.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2lpsucyux.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2zlsxxhno.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2bmkvakkg.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2ecixaaxx.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt2rifzavwe.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt2feuciwcv.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2ilemaung.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yufarslz.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt2zjsuzwyb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mxbibuze.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2ynxmkylh.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt2rrszuiyd.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2gqglngpn.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2owmxhuwc.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2djqxwbcg.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt2wdqhtoyc.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt2suhjxusx.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt2hyybagay.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt2jfhklnvk.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt2escpouyv.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2bcdwkezp.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2ukbsrfcw.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt2tathmxme.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt2bsuyirrm.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt2ugibqcxq.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt2xfhnjecb.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2exdimizs.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt2mgwatjql.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt2txgsuqnn.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt2jnuqvdka.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt2cpjwprye.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2cfpermfd.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2cjxwpoyh.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2ycabuvbg.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2oabntfpb.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2gjketflj.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt2lggowtid.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt2nsysnady.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt2jqexnkhy.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt2ccvuibjs.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt2kiuazrwi.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt2itrjoinm.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt2xzxvrfzm.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2jvhdmruh.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt2hhjwmiws.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2wnakpezj.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt2qivlwlzx.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt2osbttuwg.html


<!-- 参考信息 -->