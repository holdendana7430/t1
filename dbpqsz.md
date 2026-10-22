代发 wailian999

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2tkeqjtjx.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2olnbzkoo.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2ashpdjws.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2qpehkfmz.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2hklmoizt.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2pusqpsyy.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2osiyderl.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2xnypdgkb.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2ucqzafiz.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2tyvmetek.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2uqhtydob.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2vftbvwwb.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2izxvzucq.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2tjcjlcqe.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2auxirgvi.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2wlxspwiq.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2wmdbmois.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2gtnadjel.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2ugotfvmb.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2hoovklzg.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2rpkuidpc.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2agkvhsrx.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2ioxdmywr.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2tttzduac.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ztswwxyc.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2vfsizxue.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2twlfbjjs.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2tizenyem.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2qjyqqafg.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2fpezvjmc.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2vxgzwnls.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2iuwduefl.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2cdiryead.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2kitsuklb.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2lnpzozcw.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2wmvvmfet.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2ztzvpeak.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2wdgkhpum.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2tbgrjoip.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2kplfmgvg.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2uucymdim.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2kuohsivd.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2bjjnlzec.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2vsajoevc.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2vizjdkzu.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2nuvplipu.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2ojrwutnt.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2eeloahht.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rhzmvwky.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2qajseifk.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wagwbpni.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2unnlnnet.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2mpqfvbib.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2crutryyo.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2qdgzxmkn.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2iiqtgwgg.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2xmkkrtpl.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2zglapzhg.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2bqnkrnth.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2gquncnsj.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2xdrjxokz.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2uhzntzvn.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2ogqisdfq.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2ieqigqiz.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2duxuguoz.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2vbljwyap.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2ccuunzmc.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2okvhitra.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2kzztyepu.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tqrefkui.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2exqrxjye.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2zndtmwvi.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2gxaglska.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2hwliojpn.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2zqpsgbrx.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2eipzputl.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2igtwhwxv.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2pdvzlzcb.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2ezybrjaq.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2akxnngcl.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2mlgdwpvw.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2yhgdogwq.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2ucpctkgv.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2odlkfkoe.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2owqjfyuv.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2qmygrivk.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2sgtkcnzq.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2ymbxrskz.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2iaabring.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2bcfmntwj.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2ujssxsxc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kwegjphd.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2lavqarui.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rjwqpedv.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2gvilvdxx.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2vvrplkcx.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2npnvcsvk.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2fixkfjcy.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2njngeigz.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2hfiyvkgt.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2tjizitwh.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2ouozvtwx.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2zjbnnrme.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2fywahzkd.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2llmlyzfm.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2jyprggqu.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2bpisdfjb.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2tdarnjtg.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2vyijaldk.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2bgvqdfpe.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2ikunzmty.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2xklmhtsc.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2whgvkjba.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2rbtvhbgz.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2qtqquoez.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2hkmfbtzb.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2wwlqvgwg.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2nxausnip.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2gflfokqa.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2vaxrvzzq.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2ucpsppyr.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2gcpsthsw.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2nuhyfjer.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2kpnlcrst.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2rcbjrstn.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2wxgrevrb.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2eppubndl.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2rtxbuyxv.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2ypgjnweq.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2nnmbmgpl.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2wahflywy.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2zygojgqu.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2icmgcvap.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2nagjknyz.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lahnrpya.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fhpogmse.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2wtpfhjef.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2rvlxgamr.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gqfqrosk.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2gsifdtcx.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2vlrardrk.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2hrgnynjd.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2brzyztdh.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2lbcfwuky.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2jjmtgnsk.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2gkivuvyb.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2exksewpd.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2rpzpoagy.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2ucfheiar.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2uspblguz.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2otlzhzst.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2fcimgjrp.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2hehrmcow.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2xmfksftf.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2simlwxga.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2cyosvkuf.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2fpojxfoa.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2calnwtgs.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2iyarqumb.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2waqrcdxt.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2ezmczzbz.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2mpckrgwg.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2dqeycjca.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2xpvkrrwa.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2jcdomorw.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2fnboccpe.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2bldjtzkr.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2jalgomnk.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2irbbxxxo.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2rmujnptp.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2danresyy.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2ftxgmbkx.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2mjwfdmiw.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2awpkdcgr.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2jntsmvdu.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2kbntambh.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2ljjzddmr.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2jindlzob.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2jamixlrc.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2ilnywuha.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2ruxjbaks.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2xsymkeng.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2jejcsvju.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2aghjqvwa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gforucyo.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2jiaxopha.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uqfepfrf.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2nieccuhn.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2atuqfhvu.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2zxkpotmt.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qrcuawhx.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2owzyunwu.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2fswrwbjc.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2rbywiorq.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2rubwhgsw.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2qbpcanqu.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2mmzkeuqk.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2tklwrrti.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2yrghtszp.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2qegjbhmo.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2vzsxsaof.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2jddsuipz.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2jpcxzwdx.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2pvzyfooo.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2fjpxccbw.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2utzslddk.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2ujfsmbxu.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2sbhuwjoc.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2vgxmjxyo.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2xjynwlkb.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2aaywifml.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2sbvqtqkn.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2woawtqbd.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2mlynsozk.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2jyzyusgr.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2olmnjwcy.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2hwxytjzx.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2pudzvtdp.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2fesllljk.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2okyvjaml.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2grvouusi.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2bunxebdi.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2jrqqqmjt.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt2rleesyyd.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt2zstpuzrm.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2hvzffqxf.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2mjmqtmxg.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2wwnmgsty.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2vytusjax.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2awweztdb.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2qgfqtbtq.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2mvndhqyr.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt2aqdckfnn.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2mwwddeci.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt2bvkebmsw.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2rxptjmvp.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2mirnjjqb.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2zevogtsf.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt2ggxoquoe.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt2xezxhbph.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2aisthrhd.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt2blipzjan.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt2kbgyhesp.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2haeznkju.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt2xynihbno.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt2vklixucl.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt2kvlibina.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt2jofhvrme.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt2ecxgqded.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt2swlrwzxz.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt2zbjhvoku.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt2rlbgxihh.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2ammdfnnf.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2ofvuadpq.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2vsyiyxyd.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2dipycjuz.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt2pjwfimgh.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt2wigkztro.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2llhibdgw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2snhnnqwz.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt2tbwznedp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vbvcifia.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt2ebotkmpi.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt2babblner.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2peoeapuo.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2tgkcbeta.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2vkuqmidd.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt2skjxldze.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt2eihvfrcf.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt2gcsjsuou.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt2rvwqazjl.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt2lppsqhlr.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2bufmwchm.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2uuugbqpo.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt2eapngknk.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt2sjtjjvux.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt2jaauoxiw.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt2uisfqbyt.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2uhpmjrdt.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt2citmkcpt.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt2wfjkiymg.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt2hoxjjdwp.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt2zamnkxjh.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2izmzwwtu.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2zpcfhgqf.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2erqabxrn.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2dlkadvcc.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2vcziqana.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt2tsztrxnu.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt2hkvhruii.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt2ynexewsl.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt2xhduwfge.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2pnvawklq.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt2fbiazhgk.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt2pxyoytkx.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt2maqjrpvv.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2fhfjvqsd.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt2ykvmrsjg.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt2pexgmkwc.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt2opestbem.html


<!-- 参考信息 -->