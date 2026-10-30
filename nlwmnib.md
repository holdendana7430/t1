代发 wailian999

Ruby: @name = "x"
来源：http://3g.fehbvm.com/Article/details/gljxisgwl.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.fehbvm.com/Article/details/gtkobosla.sHtML

[G04] 定义方法
来源：http://read.share.fehbvm.com/Article/details/glzwuyxna.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.zdbjq.cn/Article/details/gprhcncoa.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.hesvh.cn/Article/details/gdqbneotc.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/gbmsquvzi.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/gdpeadulr.sHtML

Java: String greet() { return name; }
来源：http://mobile.zdbjq.cn/Article/details/gzehgatlc.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.hesvh.cn/Article/details/gxudomamn.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.zdbjq.cn/Article/details/gehchhlte.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.fehbvm.com/Article/details/gfubchhqa.sHtML

[G05] 继承
来源：http://www.blog.zdbjq.cn/Article/details/gqbtgdpxj.sHtML

Py:   class Admin(User): pass
来源：http://3g.fehbvm.com/Article/details/goswucxhu.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/gxiahtobm.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gnsyhzrqq.sHtML

TS:   class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/gxgvouzbk.sHtML

Java: class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/gvijppsbp.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.zdbjq.cn/Article/details/gfuunhlab.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.hesvh.cn/Article/details/gbkmpubyw.sHtML

C#:   class Admin : User {}
来源：http://3g.fehbvm.com/Article/details/gycxyzjmp.sHtML

[G06] 重写方法
来源：http://baike.zdbjq.cn/Article/details/ghinurjat.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.zdbjq.cn/Article/details/glyzhwdgu.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/gzibirlfr.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/gzikvspok.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/gkvkekozx.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/gzzcpukdc.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.fehbvm.com/Article/details/gmcibvmwk.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.hesvh.cn/Article/details/giqvqcgou.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.zdbjq.cn/Article/details/guohxxnyk.sHtML

[G07] 调用父类方法
来源：http://3g.zdbjq.cn/Article/details/gnyzdmoid.sHtML

Py:   super().greet()
来源：http://read.share.fehbvm.com/Article/details/ghwbwnyrk.sHtML

PHP:  parent::greet();
来源：http://www.m.share.hesvh.cn/Article/details/gsavizbhw.sHtML

JS:   super.greet();
来源：http://www.blog.hesvh.cn/Article/details/gkguwvyvj.sHtML

TS:   super.greet();
来源：http://read.share.zdbjq.cn/Article/details/gzzodleot.sHtML

Java: super.greet();
来源：http://baike.hesvh.cn/Article/details/ggfiagzeg.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.zdbjq.cn/Article/details/gxedvfhuc.sHtML

Ruby: super
来源：http://m.share.hesvh.cn/Article/details/grleonklr.sHtML

C#:   base.Greet();
来源：http://read.share.zdbjq.cn/Article/details/gbpzinodt.sHtML

[G08] 静态方法与属性
来源：http://mobile.zdbjq.cn/Article/details/gsmafyhgf.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.zdbjq.cn/Article/details/gpzomfotb.sHtML

PHP:  public static function f() {}
来源：http://mobile.hesvh.cn/Article/details/gxfeiexbk.sHtML

JS:   static f() {}
来源：http://m.share.fehbvm.com/Article/details/ghyqmtmvb.sHtML

TS:   static f(): void {}
来源：http://www.share.fehbvm.com/Article/details/goagurndp.sHtML

Java: static void f() {}
来源：http://m.share.hesvh.cn/Article/details/gpmkojijt.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.zdbjq.cn/Article/details/giozzoxtm.sHtML

Ruby: def self.f; end
来源：http://www.blog.hesvh.cn/Article/details/gdcjavrfk.sHtML

C#:   public static void F() {}
来源：http://blog.hesvh.cn/Article/details/gggjukrvh.sHtML

[G09] 接口 / 抽象类
来源：http://3g.hesvh.cn/Article/details/gowtbgopu.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.fehbvm.com/Article/details/gmbppvyql.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.zdbjq.cn/Article/details/gbmwjufxi.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.hesvh.cn/Article/details/guxlgbdzr.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.hesvh.cn/Article/details/ghywbupfi.sHtML

Java: interface Shape { double area(); }
来源：http://3g.hesvh.cn/Article/details/gfvuyezag.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.zdbjq.cn/Article/details/gorrhmzcc.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.hesvh.cn/Article/details/gbmfprrsu.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.zdbjq.cn/Article/details/guzkbdxqj.sHtML

[G10] 访问控制
来源：http://blog.hesvh.cn/Article/details/gmzyrwvki.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.zdbjq.cn/Article/details/gqqmbetkr.sHtML

PHP:  public / protected / private
来源：http://baike.hesvh.cn/Article/details/gwlbxpsif.sHtML

JS:   #private 字段；其余公开
来源：http://blog.fehbvm.com/Article/details/gtxwpnbhc.sHtML

TS:   public / protected / private
来源：http://read.share.hesvh.cn/Article/details/gtyldyksd.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.hesvh.cn/Article/details/gwhalflxp.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.zdbjq.cn/Article/details/gtgdisbsa.sHtML

Ruby: public / protected / private
来源：http://mobile.fehbvm.com/Article/details/gvqiyjery.sHtML

C#:   public / protected / private / internal
来源：http://read.share.zdbjq.cn/Article/details/ghkggihzg.sHtML

[G11] getter / setter
来源：http://wap.hesvh.cn/Article/details/gyutotzyz.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.zdbjq.cn/Article/details/ggtxmamin.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.fehbvm.com/Article/details/gsgtaftks.sHtML

JS:   get name() { return this._name; }
来源：http://baike.fehbvm.com/Article/details/gmubjihli.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.zdbjq.cn/Article/details/gbqxmdjrf.sHtML

Java: public String getName() { return name; }
来源：http://m.share.fehbvm.com/Article/details/gpqjwqhvy.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.fehbvm.com/Article/details/gpzpvlpsp.sHtML

Ruby: attr_accessor :name
来源：http://baike.fehbvm.com/Article/details/gtmmylejg.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.fehbvm.com/Article/details/gycxxglhy.sHtML

[G12] 对象转字符串
来源：http://m.share.hesvh.cn/Article/details/gmombigzz.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.zdbjq.cn/Article/details/ggaujahpy.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.hesvh.cn/Article/details/gvapwminv.sHtML

JS:   toString() { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/grrzsmdvb.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.zdbjq.cn/Article/details/gyhxdffyo.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.zdbjq.cn/Article/details/gptxmzzkf.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.fehbvm.com/Article/details/getilvodz.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.zdbjq.cn/Article/details/gvtkrpirb.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.fehbvm.com/Article/details/gqlbnzdgd.sHtML

[G13] 判断对象类型
来源：http://www.share.hesvh.cn/Article/details/grtdboqsd.sHtML

Py:   isinstance(u, User)
来源：http://3g.zdbjq.cn/Article/details/ghpaeeijc.sHtML

PHP:  $u instanceof User
来源：http://baike.hesvh.cn/Article/details/gauqehpca.sHtML

JS:   u instanceof User
来源：http://read.share.hesvh.cn/Article/details/gymsttyrb.sHtML

TS:   u instanceof User
来源：http://baike.hesvh.cn/Article/details/gvdnhkoth.sHtML

Java: u instanceof User
来源：http://3g.hesvh.cn/Article/details/gdffvsntb.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.zdbjq.cn/Article/details/ggsjroxzd.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.hesvh.cn/Article/details/gscbmpxbx.sHtML

C#:   u is User
来源：http://wap.hesvh.cn/Article/details/gxfowsnxf.sHtML

[G14] 数据类 / record
来源：http://wap.hesvh.cn/Article/details/gxayazrgc.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://baike.zdbjq.cn/Article/details/gjvfpdpuh.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.zdbjq.cn/Article/details/giwfvqqvy.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.zdbjq.cn/Article/details/gkwokcwof.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.share.hesvh.cn/Article/details/gwxnegdsl.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.fehbvm.com/Article/details/gsvchabxo.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.zdbjq.cn/Article/details/ggwnqcgbt.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.hesvh.cn/Article/details/ghfmqsnzp.sHtML

C#:   record User(string Name, int Age);
来源：http://wap.zdbjq.cn/Article/details/gmwumftcb.sHtML

[G15] 枚举
来源：http://3g.zdbjq.cn/Article/details/gpybyujvv.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://read.share.fehbvm.com/Article/details/gieitudag.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.hesvh.cn/Article/details/gyyftdtrf.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.fehbvm.com/Article/details/gjainwfpe.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://3g.zdbjq.cn/Article/details/gmdxousaj.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.hesvh.cn/Article/details/giaegqdsz.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.fehbvm.com/Article/details/gytyxltjs.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.m.share.hesvh.cn/Article/details/gegchvkww.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.fehbvm.com/Article/details/gktangdxg.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.hesvh.cn/Article/details/gacnwkuot.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.zdbjq.cn/Article/details/gvnbgorjz.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.fehbvm.com/Article/details/gwrbggays.sHtML

JS:   Object.entries(obj)
来源：http://baike.fehbvm.com/Article/details/gcqnfrnwo.sHtML

TS:   Object.entries(obj)
来源：http://read.share.zdbjq.cn/Article/details/gbcywhzwy.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://m.share.hesvh.cn/Article/details/gyeillxrx.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://3g.hesvh.cn/Article/details/gjdybipel.sHtML

Ruby: obj.instance_variables
来源：http://www.m.share.fehbvm.com/Article/details/geqzrpxqe.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.fehbvm.com/Article/details/gklhmlwps.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gengwvbsr.sHtML

H. 异常与错误处理
来源：http://www.blog.hesvh.cn/Article/details/gdhxcfylp.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gtyzzuufl.sHtML

[H01] try / catch 基础
来源：http://mobile.fehbvm.com/Article/details/gcsrbjbqm.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.zdbjq.cn/Article/details/ggqighnsg.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.fehbvm.com/Article/details/ggfxeeuhz.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.fehbvm.com/Article/details/gyxllduhi.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.zdbjq.cn/Article/details/gqfhxdorw.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.blog.zdbjq.cn/Article/details/gbzffdxsh.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.m.share.hesvh.cn/Article/details/gchzyqkfl.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wap.fehbvm.com/Article/details/gbtjovkit.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.zdbjq.cn/Article/details/grrydqtxl.sHtML

[H02] finally / ensure 收尾
来源：http://wap.fehbvm.com/Article/details/gboyjsohr.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.m.share.fehbvm.com/Article/details/gyndmfvkr.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.zdbjq.cn/Article/details/gviqyjhbx.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.fehbvm.com/Article/details/gpnzaorct.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/gfonafqoc.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.share.zdbjq.cn/Article/details/gyhfgqhnj.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://blog.hesvh.cn/Article/details/gzysfpldc.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://read.share.hesvh.cn/Article/details/gsewdtuct.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://wap.hesvh.cn/Article/details/gqwhgkmpb.sHtML

[H03] 主动抛出异常
来源：http://www.m.share.fehbvm.com/Article/details/gejnstpvo.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.share.hesvh.cn/Article/details/gtcxdbnet.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.m.share.hesvh.cn/Article/details/golklwbjv.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.hesvh.cn/Article/details/gngqfrkwt.sHtML

TS:   throw new Error("错误信息");
来源：http://www.m.share.zdbjq.cn/Article/details/gmhwalnsy.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://blog.hesvh.cn/Article/details/ggctbwnqv.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://baike.zdbjq.cn/Article/details/gjjjbmdgf.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.share.fehbvm.com/Article/details/gatbjdwkv.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://baike.fehbvm.com/Article/details/gqrxgudqq.sHtML

[H04] 自定义异常类型
来源：http://www.blog.hesvh.cn/Article/details/gmpqkkocf.sHtML

Py:   class MyError(Exception): pass
来源：http://m.share.hesvh.cn/Article/details/gqpnmgzlw.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.share.fehbvm.com/Article/details/giidatjyx.sHtML

JS:   class MyError extends Error {}
来源：http://www.blog.fehbvm.com/Article/details/gynrfhban.sHtML

TS:   class MyError extends Error {}
来源：http://www.share.zdbjq.cn/Article/details/gvmamyucx.sHtML

Java: class MyException extends RuntimeException {}
来源：http://baike.hesvh.cn/Article/details/gjvmjnrmf.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wap.hesvh.cn/Article/details/gsyvcoffn.sHtML

Ruby: class MyError < StandardError; end
来源：http://blog.fehbvm.com/Article/details/gidwefncx.sHtML

C#:   class MyException : Exception {}
来源：http://mobile.fehbvm.com/Article/details/gxmzngjru.sHtML

[H05] 捕获特定类型
来源：http://m.share.fehbvm.com/Article/details/gzsxjzojc.sHtML

Py:   except ValueError as e:
来源：http://baike.zdbjq.cn/Article/details/gxnbkqjui.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://read.share.fehbvm.com/Article/details/gqgxzrrgr.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.share.zdbjq.cn/Article/details/gjhqpqrna.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gykprouhg.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://m.share.zdbjq.cn/Article/details/gastkpyxq.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.blog.hesvh.cn/Article/details/gaakusynp.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.hesvh.cn/Article/details/gakqhhjpv.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://read.share.zdbjq.cn/Article/details/gqrsqiqzx.sHtML

[H06] 可选值 / 空值安全访问
来源：http://read.share.fehbvm.com/Article/details/gvyheopkx.sHtML

Py:   value = d.get("k") or default
来源：http://baike.zdbjq.cn/Article/details/gdoyeeohf.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://wap.hesvh.cn/Article/details/ggqxdqefq.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://baike.fehbvm.com/Article/details/gsltbdoui.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://m.share.fehbvm.com/Article/details/gdjqglkqd.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mobile.hesvh.cn/Article/details/gipfhpvwe.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://baike.fehbvm.com/Article/details/gugcusbqu.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.blog.hesvh.cn/Article/details/gxmjwgbgf.sHtML

C#:   obj?.A?.B ?? default
来源：http://wap.zdbjq.cn/Article/details/gojmtpuup.sHtML

[H07] 断言
来源：http://blog.hesvh.cn/Article/details/gfxdpvzxo.sHtML

Py:   assert x > 0, "必须为正"
来源：http://m.share.fehbvm.com/Article/details/geamaabko.sHtML

PHP:  assert($x > 0);
来源：http://baike.hesvh.cn/Article/details/gjvhnglxo.sHtML

JS:   console.assert(x > 0);
来源：http://baike.zdbjq.cn/Article/details/gjrgoschq.sHtML

TS:   console.assert(x > 0);
来源：http://wap.hesvh.cn/Article/details/gatxuratm.sHtML

Java: assert x > 0 : "必须为正";
来源：http://read.share.hesvh.cn/Article/details/gynmguafd.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://blog.hesvh.cn/Article/details/gzaqyxowa.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://m.share.zdbjq.cn/Article/details/gxirtdobr.sHtML

C#:   Debug.Assert(x > 0);
来源：http://3g.fehbvm.com/Article/details/gqrqikrzp.sHtML

[H08] 获取错误信息与堆栈
来源：http://wap.fehbvm.com/Article/details/gvzmjolvr.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://mobile.hesvh.cn/Article/details/grhjhmlvj.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://baike.fehbvm.com/Article/details/gqtzhyrpi.sHtML

JS:   e.message;  e.stack
来源：http://www.m.share.fehbvm.com/Article/details/gjaiwjbqk.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://blog.hesvh.cn/Article/details/gmjohfreb.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://read.share.fehbvm.com/Article/details/gykrxbytd.sHtML

Go:   err.Error()
来源：http://baike.hesvh.cn/Article/details/gpshxpswl.sHtML

Ruby: e.message;  e.backtrace
来源：http://3g.zdbjq.cn/Article/details/gomyxosge.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.share.hesvh.cn/Article/details/ggudhhikq.sHtML

[H09] 带错误码的异常
来源：http://mobile.hesvh.cn/Article/details/gjedeysue.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.m.share.fehbvm.com/Article/details/gngeecwxe.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://baike.zdbjq.cn/Article/details/gtmqyjbym.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mobile.fehbvm.com/Article/details/gsdmecbxr.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://blog.fehbvm.com/Article/details/gpcyxyzcd.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mobile.zdbjq.cn/Article/details/gmsxrzopk.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://read.share.fehbvm.com/Article/details/gqgsmxata.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.blog.zdbjq.cn/Article/details/gfqngayzt.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://m.share.zdbjq.cn/Article/details/gucbktsle.sHtML

[H10] 资源自动释放
来源：http://www.blog.hesvh.cn/Article/details/gzogholra.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://m.share.fehbvm.com/Article/details/gmhbljmze.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.share.fehbvm.com/Article/details/giowoormk.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.zdbjq.cn/Article/details/gfoqygohm.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.fehbvm.com/Article/details/gvpmvypoq.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://blog.hesvh.cn/Article/details/guloiuvqs.sHtML

Go:   defer f.Close()
来源：http://www.m.share.zdbjq.cn/Article/details/gwyibzmrr.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.m.share.fehbvm.com/Article/details/gcomxmahr.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://3g.hesvh.cn/Article/details/ggjhgynyw.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gsfqxrmeb.sHtML

I. 正则表达式
来源：http://www.m.share.fehbvm.com/Article/details/gkyhyiwar.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gcyfilkzj.sHtML

[I01] 判断是否匹配
来源：http://wap.hesvh.cn/Article/details/gdrzecpqa.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://read.share.hesvh.cn/Article/details/grbawpblx.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://mobile.hesvh.cn/Article/details/gtfkjrecs.sHtML

JS:   /\d+/.test(s)
来源：http://www.m.share.fehbvm.com/Article/details/giqanjlyj.sHtML

TS:   /\d+/.test(s)
来源：http://www.m.share.fehbvm.com/Article/details/gxbuukofo.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.share.fehbvm.com/Article/details/gqwxeadmx.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://m.share.fehbvm.com/Article/details/gtldcninr.sHtML

Ruby: s.match?(/\d+/)
来源：http://3g.hesvh.cn/Article/details/grtspaura.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://blog.hesvh.cn/Article/details/gtfcfkbvo.sHtML

[I02] 提取所有匹配
来源：http://read.share.fehbvm.com/Article/details/gxklrcvka.sHtML

Py:   re.findall(r"\d+", s)
来源：http://wap.hesvh.cn/Article/details/gzxhtxrli.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.share.zdbjq.cn/Article/details/gtvuqsmwd.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://m.share.zdbjq.cn/Article/details/gxbpjmext.sHtML

TS:   s.match(/\d+/g)
来源：http://wap.hesvh.cn/Article/details/gjgjywofb.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://3g.fehbvm.com/Article/details/gphucfvdg.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://baike.fehbvm.com/Article/details/gjyfvsguh.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.blog.fehbvm.com/Article/details/gsxfpcade.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://read.share.fehbvm.com/Article/details/gkrtcmmoe.sHtML

[I03] 提取捕获分组
来源：http://3g.zdbjq.cn/Article/details/gycsmtkzt.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://baike.hesvh.cn/Article/details/gntdkhydw.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wap.fehbvm.com/Article/details/gyhxmuhai.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mobile.fehbvm.com/Article/details/gycjusdgl.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://blog.hesvh.cn/Article/details/gyxhzllwg.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://blog.zdbjq.cn/Article/details/gbrnuaouk.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wap.fehbvm.com/Article/details/gaerwwdyy.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wap.hesvh.cn/Article/details/geextfzfk.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://blog.hesvh.cn/Article/details/gqechqupk.sHtML

[I04] 正则替换
来源：http://read.share.hesvh.cn/Article/details/ghxoxcbnt.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.blog.zdbjq.cn/Article/details/gngagdtyx.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/glodjjfqw.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://mobile.hesvh.cn/Article/details/gjnfodqof.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.blog.hesvh.cn/Article/details/gqatmcjvu.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://blog.hesvh.cn/Article/details/gufaovack.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://mobile.fehbvm.com/Article/details/gvgwzeaye.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://mobile.hesvh.cn/Article/details/ghnjxdcfc.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://3g.zdbjq.cn/Article/details/gdlqyzckd.sHtML

[I05] 按正则拆分
来源：http://www.blog.zdbjq.cn/Article/details/gahimoszt.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://3g.fehbvm.com/Article/details/gyjsagsdp.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://blog.fehbvm.com/Article/details/gxkjvtuaw.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.blog.fehbvm.com/Article/details/gaopzkttt.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.blog.hesvh.cn/Article/details/gwtkkotll.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.m.share.zdbjq.cn/Article/details/giaefbmdt.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://3g.hesvh.cn/Article/details/gfakqzfeu.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://m.share.hesvh.cn/Article/details/gpnoltgab.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.m.share.hesvh.cn/Article/details/gbvfzsqih.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wap.hesvh.cn/Article/details/gudfvbcpo.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.m.share.zdbjq.cn/Article/details/giavppweg.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://baike.zdbjq.cn/Article/details/gfjdbebss.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.zdbjq.cn/Article/details/gvkhlntqv.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.zdbjq.cn/Article/details/gbclvcdkt.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://m.share.fehbvm.com/Article/details/gwyogzzbo.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.m.share.fehbvm.com/Article/details/gdiaauvhp.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.share.hesvh.cn/Article/details/gfyfwyfvu.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.m.share.hesvh.cn/Article/details/gouyixeoj.sHtML

[I07] 忽略大小写与多行模式
来源：http://m.share.hesvh.cn/Article/details/gacxajmce.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.share.fehbvm.com/Article/details/ghjzbmcrk.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wap.zdbjq.cn/Article/details/gmsvgtvnq.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wap.hesvh.cn/Article/details/gshwzshtd.sHtML

TS:   /error/gim
来源：http://mobile.zdbjq.cn/Article/details/ghxbxvmfu.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://read.share.fehbvm.com/Article/details/gzgtwyiqe.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://blog.hesvh.cn/Article/details/gomibtmmo.sHtML

Ruby: s.scan(/error/i)
来源：http://www.blog.fehbvm.com/Article/details/gqylnywka.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://blog.zdbjq.cn/Article/details/gmnfobpte.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.blog.hesvh.cn/Article/details/gdyzddbak.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://baike.zdbjq.cn/Article/details/gvcsfslez.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mobile.zdbjq.cn/Article/details/gyxmqqvcp.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.fehbvm.com/Article/details/gacscnwup.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.hesvh.cn/Article/details/gucypxuum.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://read.share.fehbvm.com/Article/details/gdxkiwahe.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://3g.zdbjq.cn/Article/details/gojzgqypl.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mobile.fehbvm.com/Article/details/grupjrrtd.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://blog.hesvh.cn/Article/details/geolcphvr.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gqjtdvayq.sHtML

J. 日期与时间
来源：http://wap.hesvh.cn/Article/details/gdqtwovcw.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/ggunyprde.sHtML

[J01] 获取当前时间
来源：http://baike.fehbvm.com/Article/details/gjhugqjdw.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://mobile.hesvh.cn/Article/details/gtntixrob.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.m.share.zdbjq.cn/Article/details/ghkefkoci.sHtML

JS:   new Date();  Date.now()
来源：http://blog.hesvh.cn/Article/details/gnhvtgowl.sHtML

TS:   new Date();  Date.now()
来源：http://blog.hesvh.cn/Article/details/gdnfjokdt.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.share.fehbvm.com/Article/details/gcyqndbff.sHtML

Go:   time.Now()
来源：http://blog.fehbvm.com/Article/details/glxvanimh.sHtML

Ruby: Time.now
来源：http://www.share.zdbjq.cn/Article/details/gqkjmylcx.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://3g.fehbvm.com/Article/details/geeuhcodp.sHtML

[J02] 格式化输出
来源：http://m.share.fehbvm.com/Article/details/gjtjrdcog.sHtML


<!-- 参考信息 -->