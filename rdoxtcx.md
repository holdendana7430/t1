代发 wailian999

Py:   class Admin(User): pass
来源：http://read.share.hesvh.cn/Article/details/gcdslcmry.sHtML

PHP:  class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/gmbtbcwkm.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/gkixahfzk.sHtML

TS:   class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/gftvazifs.sHtML

Java: class Admin extends User {}
来源：http://www.share.hesvh.cn/Article/details/gcppuunup.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.zdbjq.cn/Article/details/gqzafibvw.sHtML

Ruby: class Admin < User; end
来源：http://blog.hesvh.cn/Article/details/gyjodubar.sHtML

C#:   class Admin : User {}
来源：http://www.blog.fehbvm.com/Article/details/ghzflckmq.sHtML

[G06] 重写方法
来源：http://www.share.fehbvm.com/Article/details/gkjtnvbwo.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.zdbjq.cn/Article/details/gkfklrtdb.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/gnahicedk.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/gpkmqlumr.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/gyiruwcdp.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/giltngwkm.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.zdbjq.cn/Article/details/gfvutiqwf.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.fehbvm.com/Article/details/glwybtsdc.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.fehbvm.com/Article/details/gapmxgawt.sHtML

[G07] 调用父类方法
来源：http://mobile.hesvh.cn/Article/details/gtawdfide.sHtML

Py:   super().greet()
来源：http://mobile.zdbjq.cn/Article/details/gguykfufz.sHtML

PHP:  parent::greet();
来源：http://read.share.fehbvm.com/Article/details/gfoepgrxi.sHtML

JS:   super.greet();
来源：http://wap.zdbjq.cn/Article/details/gqseqsflp.sHtML

TS:   super.greet();
来源：http://baike.zdbjq.cn/Article/details/ghhqzvhen.sHtML

Java: super.greet();
来源：http://mobile.zdbjq.cn/Article/details/gyqlvobco.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.fehbvm.com/Article/details/gyeraaipz.sHtML

Ruby: super
来源：http://www.blog.zdbjq.cn/Article/details/gnrvvazdx.sHtML

C#:   base.Greet();
来源：http://www.share.fehbvm.com/Article/details/gfmglmgne.sHtML

[G08] 静态方法与属性
来源：http://blog.fehbvm.com/Article/details/gedltaqqn.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.zdbjq.cn/Article/details/gjrdewnwy.sHtML

PHP:  public static function f() {}
来源：http://wap.zdbjq.cn/Article/details/gyjejvmop.sHtML

JS:   static f() {}
来源：http://www.share.fehbvm.com/Article/details/gynndkozi.sHtML

TS:   static f(): void {}
来源：http://wap.zdbjq.cn/Article/details/gbymlykii.sHtML

Java: static void f() {}
来源：http://wap.hesvh.cn/Article/details/gxktzgzpd.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.fehbvm.com/Article/details/glkbhbksb.sHtML

Ruby: def self.f; end
来源：http://www.share.hesvh.cn/Article/details/gvqyuguhx.sHtML

C#:   public static void F() {}
来源：http://mobile.zdbjq.cn/Article/details/gnenbrgjx.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.fehbvm.com/Article/details/gvviqpybz.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.hesvh.cn/Article/details/ggvadizrp.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.zdbjq.cn/Article/details/gzblnjhnj.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.fehbvm.com/Article/details/gqfbespvt.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.hesvh.cn/Article/details/gqwlkgrgh.sHtML

Java: interface Shape { double area(); }
来源：http://wap.fehbvm.com/Article/details/gqpycnopg.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.hesvh.cn/Article/details/gndszxbvm.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.hesvh.cn/Article/details/gqcxuznrm.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.zdbjq.cn/Article/details/ghnhxitpt.sHtML

[G10] 访问控制
来源：http://baike.fehbvm.com/Article/details/grqgzpcuz.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.fehbvm.com/Article/details/gohqglmgj.sHtML

PHP:  public / protected / private
来源：http://baike.hesvh.cn/Article/details/gqiwhswgm.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.hesvh.cn/Article/details/ghesenxsi.sHtML

TS:   public / protected / private
来源：http://wap.hesvh.cn/Article/details/gmxijfanl.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.fehbvm.com/Article/details/gnvpgnchu.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.fehbvm.com/Article/details/gcenmnzuk.sHtML

Ruby: public / protected / private
来源：http://www.share.fehbvm.com/Article/details/gsknirjzw.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.fehbvm.com/Article/details/ggjkkcloz.sHtML

[G11] getter / setter
来源：http://www.m.share.zdbjq.cn/Article/details/gvriulbdf.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.hesvh.cn/Article/details/gmgaylsnb.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.zdbjq.cn/Article/details/gmyegugyh.sHtML

JS:   get name() { return this._name; }
来源：http://3g.zdbjq.cn/Article/details/gwfkgjrze.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.fehbvm.com/Article/details/gqktaoyjx.sHtML

Java: public String getName() { return name; }
来源：http://wap.fehbvm.com/Article/details/gntvbqtmk.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.zdbjq.cn/Article/details/ghkchmqoz.sHtML

Ruby: attr_accessor :name
来源：http://m.share.fehbvm.com/Article/details/gjsxfrudc.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.hesvh.cn/Article/details/givfnappp.sHtML

[G12] 对象转字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gpwuwduid.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.zdbjq.cn/Article/details/gogouzepq.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.zdbjq.cn/Article/details/gpyfpclop.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/gjtnipttj.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.hesvh.cn/Article/details/gghgiiggn.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.hesvh.cn/Article/details/gpsvvkzmu.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.zdbjq.cn/Article/details/gihtkwdhq.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.hesvh.cn/Article/details/gdumqffqa.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.hesvh.cn/Article/details/gzcncjouz.sHtML

[G13] 判断对象类型
来源：http://baike.zdbjq.cn/Article/details/ggiaqmfuf.sHtML

Py:   isinstance(u, User)
来源：http://mobile.fehbvm.com/Article/details/gbvtbaqsm.sHtML

PHP:  $u instanceof User
来源：http://blog.hesvh.cn/Article/details/gdpctcirm.sHtML

JS:   u instanceof User
来源：http://baike.zdbjq.cn/Article/details/geuhwnxat.sHtML

TS:   u instanceof User
来源：http://m.share.zdbjq.cn/Article/details/goqaifrfa.sHtML

Java: u instanceof User
来源：http://www.blog.hesvh.cn/Article/details/gkdsmtetx.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.hesvh.cn/Article/details/gukmjkbge.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.fehbvm.com/Article/details/ghwncphmu.sHtML

C#:   u is User
来源：http://read.share.zdbjq.cn/Article/details/grrivcvjs.sHtML

[G14] 数据类 / record
来源：http://read.share.fehbvm.com/Article/details/gipprwqfd.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.fehbvm.com/Article/details/guamlzwhx.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.fehbvm.com/Article/details/gutrykiqk.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.hesvh.cn/Article/details/gsdfugnbk.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.fehbvm.com/Article/details/gqnidbizm.sHtML

Java: record User(String name, int age) {}
来源：http://wap.fehbvm.com/Article/details/gyutsytqp.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.hesvh.cn/Article/details/glwkatbuu.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.zdbjq.cn/Article/details/gvbosjand.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.zdbjq.cn/Article/details/gquvhlzwy.sHtML

[G15] 枚举
来源：http://www.m.share.hesvh.cn/Article/details/gziymxuyx.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.fehbvm.com/Article/details/gudmpofcm.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.zdbjq.cn/Article/details/gxerpuadk.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.hesvh.cn/Article/details/gzztbmiew.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.hesvh.cn/Article/details/gimoapipa.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.zdbjq.cn/Article/details/gpxzhisxy.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://baike.hesvh.cn/Article/details/gytroxufa.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.fehbvm.com/Article/details/gqeigkavx.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.hesvh.cn/Article/details/grlijhcqw.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.hesvh.cn/Article/details/gwdkrppgc.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.hesvh.cn/Article/details/gbngkmyqa.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.hesvh.cn/Article/details/ghpeplyob.sHtML

JS:   Object.entries(obj)
来源：http://read.share.fehbvm.com/Article/details/ghtphyvtc.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gffrewuzx.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.share.zdbjq.cn/Article/details/gnbazwdnm.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.fehbvm.com/Article/details/grcnfjywo.sHtML

Ruby: obj.instance_variables
来源：http://www.share.zdbjq.cn/Article/details/gbicrtgzp.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.blog.zdbjq.cn/Article/details/gbrrffslv.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/grqhqwavj.sHtML

H. 异常与错误处理
来源：http://m.share.hesvh.cn/Article/details/gijhjntqn.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gyuvekszq.sHtML

[H01] try / catch 基础
来源：http://mobile.hesvh.cn/Article/details/gpuacmpby.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://baike.hesvh.cn/Article/details/grjfjtole.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.blog.hesvh.cn/Article/details/gjeenmube.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://blog.hesvh.cn/Article/details/ghdallanw.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.share.zdbjq.cn/Article/details/gjqglocgw.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.blog.fehbvm.com/Article/details/gpbdozabj.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.fehbvm.com/Article/details/gltwpbpaz.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.share.fehbvm.com/Article/details/gkilrhgzt.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.zdbjq.cn/Article/details/gaexemaxw.sHtML

[H02] finally / ensure 收尾
来源：http://baike.zdbjq.cn/Article/details/gsyousgkg.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://mobile.fehbvm.com/Article/details/gclkndhof.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.zdbjq.cn/Article/details/gxkzchosx.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://blog.fehbvm.com/Article/details/gmfegtibu.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/gkloxhtuj.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/gjssihvmg.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.blog.hesvh.cn/Article/details/giaafhnnw.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.hesvh.cn/Article/details/geojpblpc.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.blog.zdbjq.cn/Article/details/gmznxlihf.sHtML

[H03] 主动抛出异常
来源：http://www.share.zdbjq.cn/Article/details/googdbiem.sHtML

Py:   raise ValueError("错误信息")
来源：http://3g.zdbjq.cn/Article/details/gnibatzzk.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.hesvh.cn/Article/details/gthujztpj.sHtML

JS:   throw new Error("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/gyyrwpfom.sHtML

TS:   throw new Error("错误信息");
来源：http://www.m.share.fehbvm.com/Article/details/gajxbciee.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.blog.hesvh.cn/Article/details/gmjblvunm.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://read.share.fehbvm.com/Article/details/gsjogqhfh.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://3g.fehbvm.com/Article/details/gcjjwnskn.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.share.hesvh.cn/Article/details/gmcriwcqy.sHtML

[H04] 自定义异常类型
来源：http://3g.fehbvm.com/Article/details/gdzosdfut.sHtML

Py:   class MyError(Exception): pass
来源：http://m.share.fehbvm.com/Article/details/gaxvmxyku.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://3g.fehbvm.com/Article/details/gjwuuozah.sHtML

JS:   class MyError extends Error {}
来源：http://3g.fehbvm.com/Article/details/geqylrmte.sHtML

TS:   class MyError extends Error {}
来源：http://baike.hesvh.cn/Article/details/gngtfbpcs.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.fehbvm.com/Article/details/garvgighw.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.hesvh.cn/Article/details/gbiyzxdqz.sHtML

Ruby: class MyError < StandardError; end
来源：http://3g.fehbvm.com/Article/details/garclfcoh.sHtML

C#:   class MyException : Exception {}
来源：http://www.share.zdbjq.cn/Article/details/gltmrygdl.sHtML

[H05] 捕获特定类型
来源：http://blog.hesvh.cn/Article/details/gokdqpvzf.sHtML

Py:   except ValueError as e:
来源：http://mobile.hesvh.cn/Article/details/glmyiuege.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.fehbvm.com/Article/details/ghjimnvjg.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://wap.fehbvm.com/Article/details/gkmfagnln.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://blog.hesvh.cn/Article/details/ghxijelib.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.fehbvm.com/Article/details/gmqljnzeb.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://3g.hesvh.cn/Article/details/gdtpzlbiw.sHtML

Ruby: rescue ArgumentError => e
来源：http://m.share.hesvh.cn/Article/details/gwlifdaku.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mobile.fehbvm.com/Article/details/gojbbvsob.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.fehbvm.com/Article/details/gojkzzpbt.sHtML

Py:   value = d.get("k") or default
来源：http://m.share.hesvh.cn/Article/details/gkkejipvd.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://m.share.hesvh.cn/Article/details/ggcpubbwf.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.fehbvm.com/Article/details/gflqlouil.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.share.zdbjq.cn/Article/details/gelmvmuko.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://3g.hesvh.cn/Article/details/gajoudlya.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://wap.zdbjq.cn/Article/details/gmnwxfdir.sHtML

Ruby: d&.dig(:a, :b)
来源：http://blog.hesvh.cn/Article/details/gifeernqv.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.blog.zdbjq.cn/Article/details/gysdgkuxm.sHtML

[H07] 断言
来源：http://baike.fehbvm.com/Article/details/gvtwfurzy.sHtML

Py:   assert x > 0, "必须为正"
来源：http://blog.fehbvm.com/Article/details/gawsugqnf.sHtML

PHP:  assert($x > 0);
来源：http://www.blog.hesvh.cn/Article/details/gyoxammpl.sHtML

JS:   console.assert(x > 0);
来源：http://baike.fehbvm.com/Article/details/gqjplhndf.sHtML

TS:   console.assert(x > 0);
来源：http://baike.zdbjq.cn/Article/details/gekftywmo.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.fehbvm.com/Article/details/gtnumnick.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://baike.fehbvm.com/Article/details/gcrwgpbpv.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://wap.zdbjq.cn/Article/details/guxkcxrfv.sHtML

C#:   Debug.Assert(x > 0);
来源：http://baike.fehbvm.com/Article/details/gjyanmfgu.sHtML

[H08] 获取错误信息与堆栈
来源：http://baike.zdbjq.cn/Article/details/gvfqghoye.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.blog.fehbvm.com/Article/details/gmtuimxqv.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://3g.hesvh.cn/Article/details/gzskigeib.sHtML

JS:   e.message;  e.stack
来源：http://3g.hesvh.cn/Article/details/gtdnwxhlg.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.blog.fehbvm.com/Article/details/ggerpfsja.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://baike.hesvh.cn/Article/details/grtqcgkvy.sHtML

Go:   err.Error()
来源：http://blog.fehbvm.com/Article/details/gczwnejhq.sHtML

Ruby: e.message;  e.backtrace
来源：http://read.share.hesvh.cn/Article/details/gnsalpoww.sHtML

C#:   e.Message;  e.StackTrace
来源：http://read.share.hesvh.cn/Article/details/gykgzgcuk.sHtML

[H09] 带错误码的异常
来源：http://wap.fehbvm.com/Article/details/gatlvdpsu.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.blog.hesvh.cn/Article/details/gbftsyeyv.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://wap.zdbjq.cn/Article/details/gaoslabic.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mobile.hesvh.cn/Article/details/grkmolhyu.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.m.share.hesvh.cn/Article/details/gkbqkzvgn.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mobile.fehbvm.com/Article/details/glhngybrp.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://3g.fehbvm.com/Article/details/gslqzcuxk.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://wap.fehbvm.com/Article/details/gybycuilg.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.m.share.hesvh.cn/Article/details/gsvjuzayh.sHtML

[H10] 资源自动释放
来源：http://blog.fehbvm.com/Article/details/gaqkhzdui.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://read.share.fehbvm.com/Article/details/gkocbcdmp.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://3g.zdbjq.cn/Article/details/gmamxsmmj.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.zdbjq.cn/Article/details/gvzaqbrzb.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.fehbvm.com/Article/details/gfhggwdah.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.blog.fehbvm.com/Article/details/giznznocr.sHtML

Go:   defer f.Close()
来源：http://www.m.share.zdbjq.cn/Article/details/gafnrxeoa.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wap.zdbjq.cn/Article/details/gduzrxinr.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gndrkrbfm.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/ggpuykxtm.sHtML

I. 正则表达式
来源：http://m.share.fehbvm.com/Article/details/gsbbytsfk.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gfkzubgrh.sHtML

[I01] 判断是否匹配
来源：http://m.share.hesvh.cn/Article/details/gcubazayo.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://baike.hesvh.cn/Article/details/gfdiblogd.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://read.share.hesvh.cn/Article/details/gwzhebanw.sHtML

JS:   /\d+/.test(s)
来源：http://blog.hesvh.cn/Article/details/gxuumwvly.sHtML

TS:   /\d+/.test(s)
来源：http://wap.fehbvm.com/Article/details/gdjglsxfq.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://m.share.hesvh.cn/Article/details/grkmqipee.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.share.hesvh.cn/Article/details/gpypbnqhi.sHtML

Ruby: s.match?(/\d+/)
来源：http://baike.fehbvm.com/Article/details/grliebxjw.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.share.hesvh.cn/Article/details/gwpeasvfu.sHtML

[I02] 提取所有匹配
来源：http://read.share.fehbvm.com/Article/details/gseyifiyp.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.m.share.fehbvm.com/Article/details/gjriwoxqb.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://3g.fehbvm.com/Article/details/gyzxumqvt.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.blog.fehbvm.com/Article/details/gdrjercqi.sHtML

TS:   s.match(/\d+/g)
来源：http://3g.fehbvm.com/Article/details/gwdjcjecl.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://3g.zdbjq.cn/Article/details/gvjbsdews.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mobile.hesvh.cn/Article/details/gfeauowub.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.share.fehbvm.com/Article/details/gvtgduspp.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gvcfpcxyo.sHtML

[I03] 提取捕获分组
来源：http://wap.hesvh.cn/Article/details/gzcvkdwrm.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mobile.fehbvm.com/Article/details/gaitlszds.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://3g.fehbvm.com/Article/details/gcrmqsfgh.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.m.share.fehbvm.com/Article/details/gpawrvuck.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://baike.fehbvm.com/Article/details/gsncsqnap.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://blog.hesvh.cn/Article/details/gyewxrsap.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.share.zdbjq.cn/Article/details/ghkimihoj.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wap.zdbjq.cn/Article/details/gpjffshrv.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wap.fehbvm.com/Article/details/gahzkgfun.sHtML

[I04] 正则替换
来源：http://www.share.fehbvm.com/Article/details/gexhisouz.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://baike.zdbjq.cn/Article/details/gxqjmxxfi.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://3g.hesvh.cn/Article/details/gdpkmjbel.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://read.share.zdbjq.cn/Article/details/gekajruga.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://3g.fehbvm.com/Article/details/gebsedmab.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://baike.hesvh.cn/Article/details/ggpjjhudm.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.share.fehbvm.com/Article/details/gkgsvutkh.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.share.fehbvm.com/Article/details/glwvncjvl.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://3g.fehbvm.com/Article/details/gjyqumhxw.sHtML

[I05] 按正则拆分
来源：http://www.blog.hesvh.cn/Article/details/gljqitbqj.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.blog.fehbvm.com/Article/details/gajzluoao.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://baike.fehbvm.com/Article/details/gkvjihfdv.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://blog.zdbjq.cn/Article/details/gygacwdsy.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://wap.hesvh.cn/Article/details/gcjgarevl.sHtML

Java: s.split("\\s*,\\s*")
来源：http://mobile.zdbjq.cn/Article/details/gytxjsehd.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://3g.hesvh.cn/Article/details/guntuwjbh.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.m.share.hesvh.cn/Article/details/gvrnocwid.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wap.hesvh.cn/Article/details/guvewvpvd.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wap.fehbvm.com/Article/details/goxhayzxd.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wap.hesvh.cn/Article/details/gzinxzacm.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://baike.zdbjq.cn/Article/details/gygfbnwti.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.zdbjq.cn/Article/details/gyyrnhwdm.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.fehbvm.com/Article/details/ghmpulkpk.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wap.hesvh.cn/Article/details/girkrvtgv.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://baike.zdbjq.cn/Article/details/gytruomag.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.m.share.zdbjq.cn/Article/details/gsqwfhxge.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mobile.zdbjq.cn/Article/details/guxnmjweg.sHtML

[I07] 忽略大小写与多行模式
来源：http://blog.zdbjq.cn/Article/details/ghpirfusg.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://3g.hesvh.cn/Article/details/gzchjngrc.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://blog.fehbvm.com/Article/details/gxkgycipk.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wap.fehbvm.com/Article/details/gcjycsrun.sHtML

TS:   /error/gim
来源：http://read.share.hesvh.cn/Article/details/goboezker.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://baike.zdbjq.cn/Article/details/gzlvqqtqt.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://3g.hesvh.cn/Article/details/gptsoxjnf.sHtML

Ruby: s.scan(/error/i)
来源：http://read.share.hesvh.cn/Article/details/genbjuvqm.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.m.share.hesvh.cn/Article/details/gwnntlgny.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://m.share.fehbvm.com/Article/details/gujxcrabq.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mobile.zdbjq.cn/Article/details/glgqvilga.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mobile.hesvh.cn/Article/details/gypkylytj.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.hesvh.cn/Article/details/ggevrgrlo.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.fehbvm.com/Article/details/gsncjfdxl.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://mobile.zdbjq.cn/Article/details/gqmhxinzu.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://blog.zdbjq.cn/Article/details/galzmoqom.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://read.share.zdbjq.cn/Article/details/gyxvpgoew.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mobile.hesvh.cn/Article/details/gxusocxnv.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gcyarkhby.sHtML

J. 日期与时间
来源：http://read.share.zdbjq.cn/Article/details/graiiecde.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gpwdfyipw.sHtML

[J01] 获取当前时间
来源：http://read.share.zdbjq.cn/Article/details/ghfilqnue.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://read.share.zdbjq.cn/Article/details/gusovpwtr.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mobile.hesvh.cn/Article/details/geljluqfc.sHtML

JS:   new Date();  Date.now()
来源：http://baike.fehbvm.com/Article/details/gyfvmncuj.sHtML

TS:   new Date();  Date.now()
来源：http://wap.hesvh.cn/Article/details/gnyxagrcv.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://3g.fehbvm.com/Article/details/gekfykjzd.sHtML

Go:   time.Now()
来源：http://m.share.hesvh.cn/Article/details/gngmjbtqw.sHtML

Ruby: Time.now
来源：http://mobile.zdbjq.cn/Article/details/gmvswwggh.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://m.share.hesvh.cn/Article/details/gwlwppsiu.sHtML

[J02] 格式化输出
来源：http://www.m.share.zdbjq.cn/Article/details/gdcddlbnl.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.fehbvm.com/Article/details/gsqtgnety.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mobile.hesvh.cn/Article/details/gwjsbbwkk.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://m.share.fehbvm.com/Article/details/gnwrxpnuh.sHtML

TS:   d.toISOString()
来源：http://3g.hesvh.cn/Article/details/gediyblwb.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.m.share.hesvh.cn/Article/details/gelpykcen.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wap.zdbjq.cn/Article/details/gxicctwpr.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.hesvh.cn/Article/details/gqoeeslkv.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://m.share.hesvh.cn/Article/details/gpuzrnegz.sHtML

[J03] 字符串解析为日期
来源：http://3g.hesvh.cn/Article/details/gaczmeppe.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://blog.fehbvm.com/Article/details/gehouojil.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.share.zdbjq.cn/Article/details/ggqzloumh.sHtML

JS:   new Date("2024-01-02")
来源：http://www.m.share.zdbjq.cn/Article/details/gbfmkhhsx.sHtML


<!-- 参考信息 -->