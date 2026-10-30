代发 wailian999

[G06] 重写方法
来源：http://mobile.zdbjq.cn/Article/details/gykabhizd.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.fehbvm.com/Article/details/gatolvwkl.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/gyyekevxr.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/ggygtnagx.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/gnaxciyaj.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/gppnramyt.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.zdbjq.cn/Article/details/gkblokunj.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.hesvh.cn/Article/details/gjxwgoatv.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.zdbjq.cn/Article/details/gpftdjtwn.sHtML

[G07] 调用父类方法
来源：http://m.share.fehbvm.com/Article/details/gwhklfhyi.sHtML

Py:   super().greet()
来源：http://wap.hesvh.cn/Article/details/gxfvoalcg.sHtML

PHP:  parent::greet();
来源：http://m.share.zdbjq.cn/Article/details/gudyuekqx.sHtML

JS:   super.greet();
来源：http://m.share.hesvh.cn/Article/details/gntpjnpql.sHtML

TS:   super.greet();
来源：http://baike.fehbvm.com/Article/details/gmbtkqgec.sHtML

Java: super.greet();
来源：http://m.share.zdbjq.cn/Article/details/ganwcnija.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.hesvh.cn/Article/details/gjynlwgjp.sHtML

Ruby: super
来源：http://blog.hesvh.cn/Article/details/gxsodrvht.sHtML

C#:   base.Greet();
来源：http://blog.fehbvm.com/Article/details/gqfwbqdrq.sHtML

[G08] 静态方法与属性
来源：http://wap.hesvh.cn/Article/details/gwrbnbdnb.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.hesvh.cn/Article/details/gwxwmzhbw.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.zdbjq.cn/Article/details/glsawulev.sHtML

JS:   static f() {}
来源：http://read.share.fehbvm.com/Article/details/gfrlyulhx.sHtML

TS:   static f(): void {}
来源：http://www.m.share.zdbjq.cn/Article/details/gcuwkptnp.sHtML

Java: static void f() {}
来源：http://www.blog.fehbvm.com/Article/details/gaqzdwvgk.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.fehbvm.com/Article/details/gnykhafzg.sHtML

Ruby: def self.f; end
来源：http://baike.zdbjq.cn/Article/details/gvrdtgqbm.sHtML

C#:   public static void F() {}
来源：http://blog.fehbvm.com/Article/details/gxziyugdx.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.fehbvm.com/Article/details/guqonaybe.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.fehbvm.com/Article/details/ghrheodhg.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.hesvh.cn/Article/details/gmxqzcdzo.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.zdbjq.cn/Article/details/gfjlbdkwk.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.fehbvm.com/Article/details/gublsmvmu.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.hesvh.cn/Article/details/gdnfwnnyb.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.fehbvm.com/Article/details/gyhueiumy.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.fehbvm.com/Article/details/gctgwgeuv.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.hesvh.cn/Article/details/gxdtqiqrn.sHtML

[G10] 访问控制
来源：http://mobile.hesvh.cn/Article/details/gvlxsbqbw.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.hesvh.cn/Article/details/gmijkjqtv.sHtML

PHP:  public / protected / private
来源：http://blog.hesvh.cn/Article/details/geovdgktu.sHtML

JS:   #private 字段；其余公开
来源：http://wap.fehbvm.com/Article/details/gzzphsxgw.sHtML

TS:   public / protected / private
来源：http://baike.hesvh.cn/Article/details/gvzoamkbg.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.fehbvm.com/Article/details/gwtvknlit.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.fehbvm.com/Article/details/gkemiouwj.sHtML

Ruby: public / protected / private
来源：http://wap.fehbvm.com/Article/details/gwuqhuqnn.sHtML

C#:   public / protected / private / internal
来源：http://blog.zdbjq.cn/Article/details/gskucdlam.sHtML

[G11] getter / setter
来源：http://m.share.fehbvm.com/Article/details/glewkauhq.sHtML

Py:   @property 与 @x.setter
来源：http://baike.hesvh.cn/Article/details/gljbtliej.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.zdbjq.cn/Article/details/gvzzlutul.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.fehbvm.com/Article/details/gzycczxnc.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.hesvh.cn/Article/details/gayuxmwls.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.hesvh.cn/Article/details/gtrrmecph.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.hesvh.cn/Article/details/gxdmqrrcl.sHtML

Ruby: attr_accessor :name
来源：http://baike.fehbvm.com/Article/details/gxktncxmh.sHtML

C#:   public string Name { get; set; }
来源：http://wap.zdbjq.cn/Article/details/glbhqppcz.sHtML

[G12] 对象转字符串
来源：http://3g.zdbjq.cn/Article/details/gkxwduhrr.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.zdbjq.cn/Article/details/gdhdddcou.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.zdbjq.cn/Article/details/grbphvaxk.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gfhwxazaf.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.hesvh.cn/Article/details/gorubrwgr.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.fehbvm.com/Article/details/gxjsexktl.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.zdbjq.cn/Article/details/ghsqetkrr.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.hesvh.cn/Article/details/gondvbxul.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.fehbvm.com/Article/details/gohuayfnk.sHtML

[G13] 判断对象类型
来源：http://www.m.share.zdbjq.cn/Article/details/gzyesxcwn.sHtML

Py:   isinstance(u, User)
来源：http://read.share.zdbjq.cn/Article/details/gktvslbgg.sHtML

PHP:  $u instanceof User
来源：http://wap.zdbjq.cn/Article/details/gopgdvxjq.sHtML

JS:   u instanceof User
来源：http://m.share.zdbjq.cn/Article/details/gaffjdftg.sHtML

TS:   u instanceof User
来源：http://www.m.share.hesvh.cn/Article/details/ghcyzlxyd.sHtML

Java: u instanceof User
来源：http://blog.hesvh.cn/Article/details/glpwwkebp.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.hesvh.cn/Article/details/gyioimbim.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.zdbjq.cn/Article/details/glnsezcok.sHtML

C#:   u is User
来源：http://m.share.zdbjq.cn/Article/details/gepqiqqmr.sHtML

[G14] 数据类 / record
来源：http://www.share.zdbjq.cn/Article/details/geareeung.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.fehbvm.com/Article/details/gfathqovb.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.zdbjq.cn/Article/details/givpdfabx.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.fehbvm.com/Article/details/gezcwrreo.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.zdbjq.cn/Article/details/gwcgrdfiu.sHtML

Java: record User(String name, int age) {}
来源：http://blog.zdbjq.cn/Article/details/gzkqmcsun.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.zdbjq.cn/Article/details/gcippwkuv.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.hesvh.cn/Article/details/gcdlayote.sHtML

C#:   record User(string Name, int Age);
来源：http://wap.hesvh.cn/Article/details/ghsynjcsh.sHtML

[G15] 枚举
来源：http://wap.hesvh.cn/Article/details/gqciaegtv.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.fehbvm.com/Article/details/gtxtoqahr.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.hesvh.cn/Article/details/gwkhfkjmi.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.hesvh.cn/Article/details/geucvdluy.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.zdbjq.cn/Article/details/gnnttwskr.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.fehbvm.com/Article/details/gngiwvrpp.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.fehbvm.com/Article/details/gsjtgqgrd.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.zdbjq.cn/Article/details/givgbaogx.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.fehbvm.com/Article/details/gevbmsnvl.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.hesvh.cn/Article/details/gvzbklgpt.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.fehbvm.com/Article/details/gsorppjqi.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.hesvh.cn/Article/details/gtrskuzqo.sHtML

JS:   Object.entries(obj)
来源：http://read.share.fehbvm.com/Article/details/gewlcycma.sHtML

TS:   Object.entries(obj)
来源：http://read.share.hesvh.cn/Article/details/gkmdndyrx.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.share.zdbjq.cn/Article/details/gojdjlkly.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.zdbjq.cn/Article/details/gogegfrgv.sHtML

Ruby: obj.instance_variables
来源：http://mobile.zdbjq.cn/Article/details/gvufxmisi.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.zdbjq.cn/Article/details/gmrjqvcde.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gkeywewjs.sHtML

H. 异常与错误处理
来源：http://www.m.share.zdbjq.cn/Article/details/geggikkoi.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gxjvmkpbp.sHtML

[H01] try / catch 基础
来源：http://blog.fehbvm.com/Article/details/grfonnbar.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.fehbvm.com/Article/details/giumblwzp.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.fehbvm.com/Article/details/grfjtzrfg.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.zdbjq.cn/Article/details/gqiddfkoh.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.zdbjq.cn/Article/details/gzftuqpym.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.zdbjq.cn/Article/details/giclzxqdn.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.fehbvm.com/Article/details/ggdvnihxd.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.m.share.hesvh.cn/Article/details/gwltezbpj.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://blog.hesvh.cn/Article/details/gtqwphnwz.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.zdbjq.cn/Article/details/gcdbnnzsy.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.m.share.zdbjq.cn/Article/details/ggsorobgz.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.fehbvm.com/Article/details/gymyvrlzj.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://m.share.zdbjq.cn/Article/details/gfdglqgcf.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/gncxfnlvt.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://m.share.hesvh.cn/Article/details/gyfwqtnuy.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.share.hesvh.cn/Article/details/gyiwjgsnl.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.fehbvm.com/Article/details/gajzuuefd.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/gbwmxquyj.sHtML

[H03] 主动抛出异常
来源：http://www.blog.hesvh.cn/Article/details/gdsfhspde.sHtML

Py:   raise ValueError("错误信息")
来源：http://read.share.hesvh.cn/Article/details/gjzxeanyl.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://baike.hesvh.cn/Article/details/gniakntnx.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.fehbvm.com/Article/details/gcqyqburo.sHtML

TS:   throw new Error("错误信息");
来源：http://read.share.fehbvm.com/Article/details/gpbtxuqal.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.zdbjq.cn/Article/details/guzzjrxee.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://m.share.fehbvm.com/Article/details/gtryaekqh.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.blog.hesvh.cn/Article/details/ggvzbxfkq.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.m.share.zdbjq.cn/Article/details/gixmwhdgz.sHtML

[H04] 自定义异常类型
来源：http://www.m.share.zdbjq.cn/Article/details/gqghvswvs.sHtML

Py:   class MyError(Exception): pass
来源：http://3g.hesvh.cn/Article/details/gxhwhpxzu.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://wap.zdbjq.cn/Article/details/gtkukzray.sHtML

JS:   class MyError extends Error {}
来源：http://m.share.hesvh.cn/Article/details/ghtfmaihz.sHtML

TS:   class MyError extends Error {}
来源：http://m.share.fehbvm.com/Article/details/guqmlourv.sHtML

Java: class MyException extends RuntimeException {}
来源：http://mobile.zdbjq.cn/Article/details/gsayrzfsz.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://read.share.zdbjq.cn/Article/details/gemgpqfsx.sHtML

Ruby: class MyError < StandardError; end
来源：http://read.share.zdbjq.cn/Article/details/gndfsxnrm.sHtML

C#:   class MyException : Exception {}
来源：http://www.m.share.zdbjq.cn/Article/details/gyspgvhaz.sHtML

[H05] 捕获特定类型
来源：http://www.share.fehbvm.com/Article/details/glfsgerpg.sHtML

Py:   except ValueError as e:
来源：http://baike.fehbvm.com/Article/details/gnftbstay.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://baike.zdbjq.cn/Article/details/gtqargivn.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://blog.hesvh.cn/Article/details/gnnxvfeqy.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://blog.zdbjq.cn/Article/details/ggdagctaq.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.m.share.hesvh.cn/Article/details/gaoemhant.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.share.fehbvm.com/Article/details/gsbsonqdx.sHtML

Ruby: rescue ArgumentError => e
来源：http://read.share.zdbjq.cn/Article/details/gxaotmduu.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://blog.hesvh.cn/Article/details/ghmwdamqb.sHtML

[H06] 可选值 / 空值安全访问
来源：http://mobile.hesvh.cn/Article/details/gxjkgpawd.sHtML

Py:   value = d.get("k") or default
来源：http://blog.zdbjq.cn/Article/details/gfaxaoihd.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.m.share.zdbjq.cn/Article/details/gbhaxngqm.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://baike.hesvh.cn/Article/details/gwtmcpswo.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://mobile.zdbjq.cn/Article/details/gmhiibhep.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://blog.fehbvm.com/Article/details/gglcvfreb.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://blog.hesvh.cn/Article/details/gbwohhjto.sHtML

Ruby: d&.dig(:a, :b)
来源：http://baike.hesvh.cn/Article/details/goaofutkp.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.blog.hesvh.cn/Article/details/gxrujjpxu.sHtML

[H07] 断言
来源：http://read.share.fehbvm.com/Article/details/grjycudoc.sHtML

Py:   assert x > 0, "必须为正"
来源：http://blog.fehbvm.com/Article/details/gvipicxxb.sHtML

PHP:  assert($x > 0);
来源：http://www.blog.hesvh.cn/Article/details/gaklzzsiz.sHtML

JS:   console.assert(x > 0);
来源：http://read.share.fehbvm.com/Article/details/gepujcokg.sHtML

TS:   console.assert(x > 0);
来源：http://www.blog.fehbvm.com/Article/details/gscgafsiy.sHtML

Java: assert x > 0 : "必须为正";
来源：http://blog.hesvh.cn/Article/details/gzgxgunog.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wap.zdbjq.cn/Article/details/gwohxfzjh.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.share.zdbjq.cn/Article/details/guezipkka.sHtML

C#:   Debug.Assert(x > 0);
来源：http://mobile.zdbjq.cn/Article/details/gzzsmzjaz.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.m.share.hesvh.cn/Article/details/gzfytzbui.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://baike.hesvh.cn/Article/details/gwktttmpi.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.blog.zdbjq.cn/Article/details/gptabfnrw.sHtML

JS:   e.message;  e.stack
来源：http://www.blog.fehbvm.com/Article/details/gkkfgmzhp.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://m.share.hesvh.cn/Article/details/gdxiumkuo.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.m.share.fehbvm.com/Article/details/gzqnaosfg.sHtML

Go:   err.Error()
来源：http://www.blog.hesvh.cn/Article/details/gvlpjmsbl.sHtML

Ruby: e.message;  e.backtrace
来源：http://wap.hesvh.cn/Article/details/gnysdshsp.sHtML

C#:   e.Message;  e.StackTrace
来源：http://3g.fehbvm.com/Article/details/ghgqakczq.sHtML

[H09] 带错误码的异常
来源：http://www.blog.hesvh.cn/Article/details/gncwtftar.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://blog.zdbjq.cn/Article/details/ghnugfdzt.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://3g.zdbjq.cn/Article/details/ghusghblf.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://blog.zdbjq.cn/Article/details/gdtyrnrxn.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.share.zdbjq.cn/Article/details/ghcktruac.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://read.share.fehbvm.com/Article/details/galhixygr.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.m.share.fehbvm.com/Article/details/gnduqssod.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://3g.fehbvm.com/Article/details/gkqjkaxbi.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.blog.hesvh.cn/Article/details/ghifbtpty.sHtML

[H10] 资源自动释放
来源：http://m.share.zdbjq.cn/Article/details/gvktotflu.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://mobile.hesvh.cn/Article/details/goyireptu.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mobile.hesvh.cn/Article/details/gjzkfmfya.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.fehbvm.com/Article/details/gagpalfok.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.zdbjq.cn/Article/details/gnvuozuuz.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://blog.zdbjq.cn/Article/details/gbtqdpixm.sHtML

Go:   defer f.Close()
来源：http://blog.hesvh.cn/Article/details/gvnrbuotg.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://baike.fehbvm.com/Article/details/glzgjtrfa.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gkquqajdh.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/goidkpxba.sHtML

I. 正则表达式
来源：http://www.m.share.fehbvm.com/Article/details/gwlfdlsfp.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gearbhrmr.sHtML

[I01] 判断是否匹配
来源：http://read.share.hesvh.cn/Article/details/gtxbpyqym.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mobile.hesvh.cn/Article/details/geymrubqn.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://m.share.fehbvm.com/Article/details/gokyzksjd.sHtML

JS:   /\d+/.test(s)
来源：http://read.share.zdbjq.cn/Article/details/gdgzixeic.sHtML

TS:   /\d+/.test(s)
来源：http://m.share.fehbvm.com/Article/details/gjsrkufwv.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mobile.hesvh.cn/Article/details/gvcimmpmt.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://m.share.fehbvm.com/Article/details/gxllnsdfu.sHtML

Ruby: s.match?(/\d+/)
来源：http://m.share.fehbvm.com/Article/details/ghcvaemze.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://m.share.zdbjq.cn/Article/details/gkqybikhc.sHtML

[I02] 提取所有匹配
来源：http://read.share.hesvh.cn/Article/details/gegheifui.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.blog.fehbvm.com/Article/details/gdmbaulxm.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wap.hesvh.cn/Article/details/glzfwxviz.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.m.share.hesvh.cn/Article/details/gpjmkllhj.sHtML

TS:   s.match(/\d+/g)
来源：http://www.m.share.hesvh.cn/Article/details/grpgiuzav.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://3g.hesvh.cn/Article/details/gdwtapuzb.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.blog.fehbvm.com/Article/details/gwceoqnba.sHtML

Ruby: s.scan(/\d+/)
来源：http://m.share.hesvh.cn/Article/details/gikqlklba.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mobile.zdbjq.cn/Article/details/gnferuxnj.sHtML

[I03] 提取捕获分组
来源：http://wap.zdbjq.cn/Article/details/gzckaofti.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://read.share.fehbvm.com/Article/details/gpxqbrvbl.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.m.share.hesvh.cn/Article/details/gxjsxvwrv.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.share.zdbjq.cn/Article/details/gnsqngllt.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.blog.fehbvm.com/Article/details/gyhsxoohi.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://3g.hesvh.cn/Article/details/gxpbdpzuv.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://blog.hesvh.cn/Article/details/ghgcdgqzd.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://baike.zdbjq.cn/Article/details/gdopvxpox.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wap.hesvh.cn/Article/details/gapagcyxf.sHtML

[I04] 正则替换
来源：http://mobile.fehbvm.com/Article/details/gwsgrniyc.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://mobile.hesvh.cn/Article/details/grhvchvqm.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.share.fehbvm.com/Article/details/gjruchtal.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.zdbjq.cn/Article/details/gobaaepry.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://wap.hesvh.cn/Article/details/gwccmwbpp.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://3g.hesvh.cn/Article/details/gbzxujdqd.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.blog.zdbjq.cn/Article/details/gjbgkmbfj.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://wap.fehbvm.com/Article/details/gpeggmucn.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.share.fehbvm.com/Article/details/gnsjfpuwt.sHtML

[I05] 按正则拆分
来源：http://3g.zdbjq.cn/Article/details/gtvaomjgw.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.share.fehbvm.com/Article/details/glclbpvtx.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://m.share.fehbvm.com/Article/details/goqzgvown.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://m.share.hesvh.cn/Article/details/ggthlvpxb.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.m.share.zdbjq.cn/Article/details/ghedcyuxw.sHtML

Java: s.split("\\s*,\\s*")
来源：http://wap.zdbjq.cn/Article/details/gswjewakm.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://read.share.zdbjq.cn/Article/details/grzlardwy.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.m.share.zdbjq.cn/Article/details/gqltyzjmu.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.m.share.zdbjq.cn/Article/details/gfnvbjuey.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.share.zdbjq.cn/Article/details/gebswuquz.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://m.share.fehbvm.com/Article/details/ganxuoeyz.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://m.share.zdbjq.cn/Article/details/gpbqonubu.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.fehbvm.com/Article/details/gwdtnovye.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.hesvh.cn/Article/details/gznoifpwp.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://read.share.zdbjq.cn/Article/details/gltdbwoqi.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://baike.fehbvm.com/Article/details/gdtxpkitx.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wap.fehbvm.com/Article/details/gvwzurpxn.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.blog.hesvh.cn/Article/details/gqebbqbxw.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.share.zdbjq.cn/Article/details/gyjfzsgmo.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.share.hesvh.cn/Article/details/gmzhodpmc.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.share.hesvh.cn/Article/details/gvzpatsbq.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.m.share.hesvh.cn/Article/details/gcdtwxncu.sHtML

TS:   /error/gim
来源：http://www.share.hesvh.cn/Article/details/gidfkjbin.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mobile.fehbvm.com/Article/details/gownceudg.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://baike.zdbjq.cn/Article/details/gzjhmvhkl.sHtML

Ruby: s.scan(/error/i)
来源：http://blog.zdbjq.cn/Article/details/gnksaysev.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://m.share.fehbvm.com/Article/details/guwjdljfe.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://baike.zdbjq.cn/Article/details/gumpebece.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mobile.zdbjq.cn/Article/details/gbcsykhnj.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://3g.hesvh.cn/Article/details/gkevcxzdr.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.fehbvm.com/Article/details/gwhyuntcn.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.hesvh.cn/Article/details/gougbuhxc.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://wap.hesvh.cn/Article/details/gieboihfe.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://3g.hesvh.cn/Article/details/gpmogbpvc.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://3g.zdbjq.cn/Article/details/gdzdvhggs.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wap.zdbjq.cn/Article/details/gyofxbedl.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/geqeyzlsy.sHtML

J. 日期与时间
来源：http://read.share.hesvh.cn/Article/details/gcxwjnwgy.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/giutbojob.sHtML

[J01] 获取当前时间
来源：http://read.share.hesvh.cn/Article/details/ghybkjzay.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://baike.hesvh.cn/Article/details/gulxxrvmp.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.blog.hesvh.cn/Article/details/gkqfmefuj.sHtML

JS:   new Date();  Date.now()
来源：http://wap.zdbjq.cn/Article/details/gmvdazkfk.sHtML

TS:   new Date();  Date.now()
来源：http://blog.zdbjq.cn/Article/details/gfrfdzhap.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://read.share.fehbvm.com/Article/details/grawvyick.sHtML

Go:   time.Now()
来源：http://mobile.fehbvm.com/Article/details/ghxbubkek.sHtML

Ruby: Time.now
来源：http://baike.zdbjq.cn/Article/details/gvxxnjsxv.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.blog.zdbjq.cn/Article/details/gxfamyflg.sHtML

[J02] 格式化输出
来源：http://m.share.zdbjq.cn/Article/details/gukgoedov.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.zdbjq.cn/Article/details/gdbptvofw.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://blog.fehbvm.com/Article/details/gdwmbqwlz.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://3g.zdbjq.cn/Article/details/graojhvlw.sHtML

TS:   d.toISOString()
来源：http://baike.zdbjq.cn/Article/details/gfliyqyof.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.share.fehbvm.com/Article/details/gpsqysuip.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.blog.zdbjq.cn/Article/details/gwhgcemph.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.fehbvm.com/Article/details/gyeymvanz.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://blog.fehbvm.com/Article/details/gxkzfvkpc.sHtML

[J03] 字符串解析为日期
来源：http://read.share.hesvh.cn/Article/details/gmwawrsxw.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://3g.zdbjq.cn/Article/details/gmbbsppwo.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://mobile.fehbvm.com/Article/details/gmzvjgrqv.sHtML

JS:   new Date("2024-01-02")
来源：http://3g.zdbjq.cn/Article/details/gmsufhspq.sHtML

TS:   new Date("2024-01-02")
来源：http://read.share.hesvh.cn/Article/details/gfajocjpq.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://blog.hesvh.cn/Article/details/gevevfped.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.share.fehbvm.com/Article/details/gzaalgqzn.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://mobile.zdbjq.cn/Article/details/gwnpfvsmi.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://blog.fehbvm.com/Article/details/gabxhhquw.sHtML

[J04] 时间戳与日期互转
来源：http://blog.fehbvm.com/Article/details/gjtmxmkgo.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://read.share.hesvh.cn/Article/details/gmwoyqqye.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://3g.zdbjq.cn/Article/details/gjrkzszlt.sHtML


<!-- 参考信息 -->