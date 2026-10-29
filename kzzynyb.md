代发 wailian999

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.zdbjq.cn/Article/details/gedeyfuun.sHtML

Ruby: def greet; @name; end
来源：http://baike.zdbjq.cn/Article/details/gaiqczwdi.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.zdbjq.cn/Article/details/gxhnfxsyo.sHtML

[G05] 继承
来源：http://read.share.zdbjq.cn/Article/details/ggwjiyjjq.sHtML

Py:   class Admin(User): pass
来源：http://mobile.hesvh.cn/Article/details/gyqwbnlhy.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/gtrbkvgzg.sHtML

JS:   class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/gfpkroevm.sHtML

TS:   class Admin extends User {}
来源：http://read.share.hesvh.cn/Article/details/gxajzahrf.sHtML

Java: class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/gvoukjjvx.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.hesvh.cn/Article/details/gqzacipwe.sHtML

Ruby: class Admin < User; end
来源：http://wap.fehbvm.com/Article/details/gjtzyxxgp.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.fehbvm.com/Article/details/gljdbdgbf.sHtML

[G06] 重写方法
来源：http://wap.zdbjq.cn/Article/details/gsgredbtd.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.hesvh.cn/Article/details/gdtltaict.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/gpzgvayta.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/gvkppvovw.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/glonsmsbm.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/gbdwacbmm.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.fehbvm.com/Article/details/gbegbkwym.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.fehbvm.com/Article/details/gsrcaocag.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.fehbvm.com/Article/details/gelchdujk.sHtML

[G07] 调用父类方法
来源：http://blog.fehbvm.com/Article/details/gjqguynei.sHtML

Py:   super().greet()
来源：http://blog.zdbjq.cn/Article/details/gdprjdtup.sHtML

PHP:  parent::greet();
来源：http://blog.hesvh.cn/Article/details/gobpvtsrt.sHtML

JS:   super.greet();
来源：http://read.share.hesvh.cn/Article/details/grcflnkap.sHtML

TS:   super.greet();
来源：http://www.blog.fehbvm.com/Article/details/gehjqcvfg.sHtML

Java: super.greet();
来源：http://m.share.fehbvm.com/Article/details/gprvnfgsn.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.zdbjq.cn/Article/details/gvjdnfsoy.sHtML

Ruby: super
来源：http://m.share.hesvh.cn/Article/details/ggnamjnaj.sHtML

C#:   base.Greet();
来源：http://blog.zdbjq.cn/Article/details/gquvrtofa.sHtML

[G08] 静态方法与属性
来源：http://m.share.fehbvm.com/Article/details/gygniidsi.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.hesvh.cn/Article/details/gwcrkriff.sHtML

PHP:  public static function f() {}
来源：http://www.blog.zdbjq.cn/Article/details/ggtjctkyy.sHtML

JS:   static f() {}
来源：http://www.share.zdbjq.cn/Article/details/gbvvmmkxn.sHtML

TS:   static f(): void {}
来源：http://wap.hesvh.cn/Article/details/glvtqrlzk.sHtML

Java: static void f() {}
来源：http://3g.fehbvm.com/Article/details/guajjotps.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.hesvh.cn/Article/details/gcqgmbwgo.sHtML

Ruby: def self.f; end
来源：http://www.m.share.hesvh.cn/Article/details/gdjldczms.sHtML

C#:   public static void F() {}
来源：http://m.share.fehbvm.com/Article/details/gpasjthgu.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.fehbvm.com/Article/details/gipeymfpk.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.zdbjq.cn/Article/details/gfvvoysiv.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.hesvh.cn/Article/details/gvgchewwm.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.hesvh.cn/Article/details/gwywiiods.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.hesvh.cn/Article/details/gnmqgxztp.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.fehbvm.com/Article/details/gtokqrgtw.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.hesvh.cn/Article/details/gvhbhpgmi.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.zdbjq.cn/Article/details/gcptdxneb.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.fehbvm.com/Article/details/gyyuxbzzp.sHtML

[G10] 访问控制
来源：http://www.share.fehbvm.com/Article/details/gfmfgelbq.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.zdbjq.cn/Article/details/gulbamoij.sHtML

PHP:  public / protected / private
来源：http://3g.zdbjq.cn/Article/details/glvqlvyvm.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.zdbjq.cn/Article/details/gqdsivjko.sHtML

TS:   public / protected / private
来源：http://baike.hesvh.cn/Article/details/guftnwpzk.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.hesvh.cn/Article/details/gwgycseyn.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.hesvh.cn/Article/details/gkjtucgzh.sHtML

Ruby: public / protected / private
来源：http://read.share.fehbvm.com/Article/details/gjkzsbint.sHtML

C#:   public / protected / private / internal
来源：http://read.share.hesvh.cn/Article/details/gyxqosclh.sHtML

[G11] getter / setter
来源：http://m.share.zdbjq.cn/Article/details/gmyebwjxq.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.zdbjq.cn/Article/details/gnlacidzy.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.fehbvm.com/Article/details/ghfaknllt.sHtML

JS:   get name() { return this._name; }
来源：http://baike.hesvh.cn/Article/details/gzmkxgayp.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.fehbvm.com/Article/details/goprtzfye.sHtML

Java: public String getName() { return name; }
来源：http://mobile.hesvh.cn/Article/details/gaudlrcbs.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.hesvh.cn/Article/details/guxkkvsmy.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.zdbjq.cn/Article/details/ggooitgll.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.hesvh.cn/Article/details/gidulfawy.sHtML

[G12] 对象转字符串
来源：http://blog.zdbjq.cn/Article/details/gpqsjxzwz.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.zdbjq.cn/Article/details/gmqtkexwg.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.fehbvm.com/Article/details/gdwvrwost.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/gjvpzjudz.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/gwliaqwmq.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.zdbjq.cn/Article/details/giwquaxws.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.hesvh.cn/Article/details/gzfsznevr.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.hesvh.cn/Article/details/gbbucmhfo.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.fehbvm.com/Article/details/giljfkdlk.sHtML

[G13] 判断对象类型
来源：http://www.blog.zdbjq.cn/Article/details/gasjwrqla.sHtML

Py:   isinstance(u, User)
来源：http://read.share.hesvh.cn/Article/details/gmyviwhhn.sHtML

PHP:  $u instanceof User
来源：http://m.share.zdbjq.cn/Article/details/gvfyockun.sHtML

JS:   u instanceof User
来源：http://read.share.zdbjq.cn/Article/details/gecacywvt.sHtML

TS:   u instanceof User
来源：http://www.blog.hesvh.cn/Article/details/grnzkrvtw.sHtML

Java: u instanceof User
来源：http://blog.fehbvm.com/Article/details/gmrujxkaq.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.fehbvm.com/Article/details/gdktxrnfi.sHtML

Ruby: u.is_a?(User)
来源：http://wap.zdbjq.cn/Article/details/gxlplufzg.sHtML

C#:   u is User
来源：http://wap.zdbjq.cn/Article/details/gjjjolswy.sHtML

[G14] 数据类 / record
来源：http://read.share.hesvh.cn/Article/details/ghskipxxo.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.hesvh.cn/Article/details/gznipkjjz.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://read.share.hesvh.cn/Article/details/gixyqqlwt.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.zdbjq.cn/Article/details/gdkwjdfxj.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.hesvh.cn/Article/details/gzuvygghs.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.fehbvm.com/Article/details/glmkozlzv.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.hesvh.cn/Article/details/gnhwcyojk.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.hesvh.cn/Article/details/gfbwgaukz.sHtML

C#:   record User(string Name, int Age);
来源：http://m.share.fehbvm.com/Article/details/gojyqwllp.sHtML

[G15] 枚举
来源：http://www.share.fehbvm.com/Article/details/ghbpykgrr.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.fehbvm.com/Article/details/gxoinumkl.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.zdbjq.cn/Article/details/gjdymlquu.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.zdbjq.cn/Article/details/gofysxslw.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.hesvh.cn/Article/details/gsvndsgsw.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.hesvh.cn/Article/details/gdlkyosvz.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.fehbvm.com/Article/details/gjtveubra.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.fehbvm.com/Article/details/gtcxuamii.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.fehbvm.com/Article/details/gzaotjzqz.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.zdbjq.cn/Article/details/gytsoknnd.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.blog.hesvh.cn/Article/details/gdkarfdmo.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.zdbjq.cn/Article/details/gszywzptr.sHtML

JS:   Object.entries(obj)
来源：http://3g.hesvh.cn/Article/details/gfyrrgkkp.sHtML

TS:   Object.entries(obj)
来源：http://m.share.fehbvm.com/Article/details/gzredfsnn.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://m.share.zdbjq.cn/Article/details/gvvoocfjd.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://wap.fehbvm.com/Article/details/ggvaioaue.sHtML

Ruby: obj.instance_variables
来源：http://mobile.fehbvm.com/Article/details/gbtpahqag.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.m.share.hesvh.cn/Article/details/geuqnzbir.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gqlbzqhal.sHtML

H. 异常与错误处理
来源：http://www.m.share.zdbjq.cn/Article/details/gfnrtozrs.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gjlfgkgeg.sHtML

[H01] try / catch 基础
来源：http://www.blog.fehbvm.com/Article/details/gzmnilcvn.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://baike.zdbjq.cn/Article/details/gipbcaudt.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.fehbvm.com/Article/details/gdellghjo.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.hesvh.cn/Article/details/gtxokhocm.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.fehbvm.com/Article/details/gwyojdqlb.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.m.share.fehbvm.com/Article/details/gnidmrjtf.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.blog.hesvh.cn/Article/details/gvluawkpo.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.hesvh.cn/Article/details/gssginggb.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.m.share.hesvh.cn/Article/details/gydnlejjd.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.hesvh.cn/Article/details/gcgdctgdw.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://3g.fehbvm.com/Article/details/gxjvubeic.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://blog.hesvh.cn/Article/details/gwqwguhhx.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://mobile.fehbvm.com/Article/details/gcawxxobt.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://blog.hesvh.cn/Article/details/gvnfnjuub.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.hesvh.cn/Article/details/govornxig.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://m.share.zdbjq.cn/Article/details/gbxtrewov.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.zdbjq.cn/Article/details/giixzhmco.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://baike.fehbvm.com/Article/details/gwujrtkgl.sHtML

[H03] 主动抛出异常
来源：http://wap.zdbjq.cn/Article/details/gblvqoypp.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.hesvh.cn/Article/details/geiqsnszk.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blog.hesvh.cn/Article/details/gsskanevc.sHtML

JS:   throw new Error("错误信息");
来源：http://baike.fehbvm.com/Article/details/gsvpnxztu.sHtML

TS:   throw new Error("错误信息");
来源：http://read.share.fehbvm.com/Article/details/gqslheumj.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.hesvh.cn/Article/details/gmlyhxmvz.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.blog.fehbvm.com/Article/details/ghhvwcxuq.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.m.share.hesvh.cn/Article/details/grsdflcti.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://baike.zdbjq.cn/Article/details/gdgehwyiu.sHtML

[H04] 自定义异常类型
来源：http://read.share.fehbvm.com/Article/details/gzntfzloo.sHtML

Py:   class MyError(Exception): pass
来源：http://www.share.zdbjq.cn/Article/details/gkibpucjr.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.m.share.zdbjq.cn/Article/details/gkghkxhpv.sHtML

JS:   class MyError extends Error {}
来源：http://3g.zdbjq.cn/Article/details/gafostgnp.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.zdbjq.cn/Article/details/gpsaplezr.sHtML

Java: class MyException extends RuntimeException {}
来源：http://wap.hesvh.cn/Article/details/gewrumuaa.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://baike.fehbvm.com/Article/details/gupgijlcc.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.fehbvm.com/Article/details/gsiylyaro.sHtML

C#:   class MyException : Exception {}
来源：http://wap.zdbjq.cn/Article/details/gtepavjtc.sHtML

[H05] 捕获特定类型
来源：http://blog.hesvh.cn/Article/details/gotlkvaaw.sHtML

Py:   except ValueError as e:
来源：http://www.blog.zdbjq.cn/Article/details/gtrywruyc.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.zdbjq.cn/Article/details/gkwssmpmb.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://baike.zdbjq.cn/Article/details/gkokeudrh.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://m.share.zdbjq.cn/Article/details/glottzfxi.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.m.share.hesvh.cn/Article/details/gknmpuldc.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mobile.hesvh.cn/Article/details/gejebluix.sHtML

Ruby: rescue ArgumentError => e
来源：http://3g.fehbvm.com/Article/details/gakbhobeg.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wap.hesvh.cn/Article/details/gmcicsxgo.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.m.share.hesvh.cn/Article/details/gijlwshwr.sHtML

Py:   value = d.get("k") or default
来源：http://www.m.share.hesvh.cn/Article/details/gpemgvlva.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://baike.hesvh.cn/Article/details/gcaymymra.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://read.share.zdbjq.cn/Article/details/gkckbutwh.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.share.fehbvm.com/Article/details/gprhsmfgg.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://m.share.fehbvm.com/Article/details/gntncyxcb.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://m.share.fehbvm.com/Article/details/gifygazrf.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.m.share.hesvh.cn/Article/details/ghvdnjyrz.sHtML

C#:   obj?.A?.B ?? default
来源：http://mobile.zdbjq.cn/Article/details/gksvzgugu.sHtML

[H07] 断言
来源：http://read.share.fehbvm.com/Article/details/gokwkizjt.sHtML

Py:   assert x > 0, "必须为正"
来源：http://3g.zdbjq.cn/Article/details/gcrmbhrys.sHtML

PHP:  assert($x > 0);
来源：http://www.blog.fehbvm.com/Article/details/gdyuuoewr.sHtML

JS:   console.assert(x > 0);
来源：http://baike.zdbjq.cn/Article/details/gazhieohe.sHtML

TS:   console.assert(x > 0);
来源：http://www.m.share.fehbvm.com/Article/details/gtcywovka.sHtML

Java: assert x > 0 : "必须为正";
来源：http://mobile.fehbvm.com/Article/details/gdqnahuew.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.share.fehbvm.com/Article/details/gdisbqwxi.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://m.share.zdbjq.cn/Article/details/gscczvjkg.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.share.hesvh.cn/Article/details/gpgcpbotq.sHtML

[H08] 获取错误信息与堆栈
来源：http://3g.zdbjq.cn/Article/details/gvemufsjr.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://mobile.zdbjq.cn/Article/details/gqkvpbbzt.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.m.share.hesvh.cn/Article/details/gsifzbnql.sHtML

JS:   e.message;  e.stack
来源：http://mobile.hesvh.cn/Article/details/gdmmzmfne.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.m.share.zdbjq.cn/Article/details/gwllefiqo.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://m.share.zdbjq.cn/Article/details/gjqnhvoih.sHtML

Go:   err.Error()
来源：http://baike.hesvh.cn/Article/details/glnqmekyk.sHtML

Ruby: e.message;  e.backtrace
来源：http://read.share.fehbvm.com/Article/details/gupatxmfi.sHtML

C#:   e.Message;  e.StackTrace
来源：http://read.share.hesvh.cn/Article/details/gkwmhquij.sHtML

[H09] 带错误码的异常
来源：http://wap.hesvh.cn/Article/details/giclfwrsz.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://baike.hesvh.cn/Article/details/gfjvkosvv.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://mobile.zdbjq.cn/Article/details/guuicenik.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://baike.fehbvm.com/Article/details/gzylyniyr.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://blog.fehbvm.com/Article/details/gsrhbkvsu.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://3g.zdbjq.cn/Article/details/gtlakgiji.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.m.share.hesvh.cn/Article/details/gllmyxgqf.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://baike.zdbjq.cn/Article/details/gjdoshpkj.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://3g.zdbjq.cn/Article/details/gfzwwywnr.sHtML

[H10] 资源自动释放
来源：http://mobile.hesvh.cn/Article/details/ghbupdiij.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://m.share.fehbvm.com/Article/details/gqnprgokk.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.blog.hesvh.cn/Article/details/gbfxamgix.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.fehbvm.com/Article/details/gtfkajihp.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.hesvh.cn/Article/details/ghkovxbvm.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.m.share.zdbjq.cn/Article/details/gxrupnakm.sHtML

Go:   defer f.Close()
来源：http://baike.hesvh.cn/Article/details/gfjwyawir.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.m.share.fehbvm.com/Article/details/gnyaoiesl.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gpockvxbb.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gxrbjqtfo.sHtML

I. 正则表达式
来源：http://blog.zdbjq.cn/Article/details/gibwqggak.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gntsaswwi.sHtML

[I01] 判断是否匹配
来源：http://blog.hesvh.cn/Article/details/goqjzvqfs.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.share.hesvh.cn/Article/details/gyfdtsxvb.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://m.share.hesvh.cn/Article/details/gmlizvwqm.sHtML

JS:   /\d+/.test(s)
来源：http://baike.hesvh.cn/Article/details/gkjjuifmq.sHtML

TS:   /\d+/.test(s)
来源：http://blog.hesvh.cn/Article/details/ggdblyimv.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://read.share.hesvh.cn/Article/details/geccotdbp.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wap.zdbjq.cn/Article/details/gjuswkwfv.sHtML

Ruby: s.match?(/\d+/)
来源：http://wap.hesvh.cn/Article/details/gqaawwcsh.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.blog.zdbjq.cn/Article/details/gxcaqhcnn.sHtML

[I02] 提取所有匹配
来源：http://read.share.hesvh.cn/Article/details/gvwgsoseh.sHtML

Py:   re.findall(r"\d+", s)
来源：http://mobile.hesvh.cn/Article/details/gayfdvzcp.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wap.fehbvm.com/Article/details/gsaxbataf.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wap.fehbvm.com/Article/details/gawgrcbbo.sHtML

TS:   s.match(/\d+/g)
来源：http://www.m.share.fehbvm.com/Article/details/ggwquffns.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.m.share.hesvh.cn/Article/details/gmicypjug.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mobile.hesvh.cn/Article/details/gkjmtzxoc.sHtML

Ruby: s.scan(/\d+/)
来源：http://3g.hesvh.cn/Article/details/gkjpopwmg.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.share.hesvh.cn/Article/details/gpxzzlylx.sHtML

[I03] 提取捕获分组
来源：http://www.blog.hesvh.cn/Article/details/gxvbtkqbs.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://read.share.zdbjq.cn/Article/details/gbfqdytft.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.share.hesvh.cn/Article/details/guykgbmev.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://read.share.fehbvm.com/Article/details/gwppuansn.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mobile.hesvh.cn/Article/details/gimwkzrhs.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.m.share.zdbjq.cn/Article/details/gvkjlzbfx.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.blog.hesvh.cn/Article/details/gmsdwabth.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://blog.hesvh.cn/Article/details/gtcphgjza.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://blog.fehbvm.com/Article/details/ghkewugki.sHtML

[I04] 正则替换
来源：http://www.m.share.zdbjq.cn/Article/details/gpdpeavgd.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://3g.fehbvm.com/Article/details/gmtefqkot.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://baike.fehbvm.com/Article/details/gqsxqazjb.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://blog.zdbjq.cn/Article/details/gsbmwcpsf.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://mobile.hesvh.cn/Article/details/ghvylxcda.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://m.share.hesvh.cn/Article/details/glpdbgpqy.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://baike.fehbvm.com/Article/details/gfmuhclsu.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.blog.hesvh.cn/Article/details/gvcjnqkrf.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.share.hesvh.cn/Article/details/glyunffcv.sHtML

[I05] 按正则拆分
来源：http://read.share.hesvh.cn/Article/details/gxslplriu.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://read.share.fehbvm.com/Article/details/gkvvskkrt.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://baike.fehbvm.com/Article/details/grcpmtpnt.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://read.share.fehbvm.com/Article/details/gkuqioktp.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.m.share.fehbvm.com/Article/details/gskkqxpxm.sHtML

Java: s.split("\\s*,\\s*")
来源：http://mobile.hesvh.cn/Article/details/geriarhfy.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.blog.hesvh.cn/Article/details/glvhfaqnt.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.m.share.hesvh.cn/Article/details/glkykxgbn.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://3g.hesvh.cn/Article/details/gwdtgpqsd.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.share.fehbvm.com/Article/details/gwsvjqohg.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://m.share.fehbvm.com/Article/details/gogrtqclb.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.m.share.hesvh.cn/Article/details/gtureoylh.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.hesvh.cn/Article/details/gilkhrayq.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.fehbvm.com/Article/details/gtsrtoghk.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://read.share.hesvh.cn/Article/details/gqhbihuia.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://m.share.hesvh.cn/Article/details/gyxnkionk.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://m.share.hesvh.cn/Article/details/gupcutfoy.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://read.share.hesvh.cn/Article/details/gqighwvvx.sHtML

[I07] 忽略大小写与多行模式
来源：http://m.share.hesvh.cn/Article/details/grnomoref.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mobile.zdbjq.cn/Article/details/gntkmoovf.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://read.share.hesvh.cn/Article/details/gccesuasx.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wap.hesvh.cn/Article/details/gohqqcuno.sHtML

TS:   /error/gim
来源：http://3g.zdbjq.cn/Article/details/gqmrodcnk.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://read.share.hesvh.cn/Article/details/glptbsfuf.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mobile.fehbvm.com/Article/details/gyoklkxld.sHtML

Ruby: s.scan(/error/i)
来源：http://read.share.hesvh.cn/Article/details/gmkjmmclm.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://read.share.hesvh.cn/Article/details/gnipshdvt.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://mobile.hesvh.cn/Article/details/gbnxwyxdc.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://blog.zdbjq.cn/Article/details/goiadbewq.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mobile.fehbvm.com/Article/details/gfzsbpeqj.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.hesvh.cn/Article/details/grzmmhwcz.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.hesvh.cn/Article/details/ghfgidjob.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://m.share.zdbjq.cn/Article/details/ganhxlbis.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://blog.zdbjq.cn/Article/details/ghgsqfjix.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.blog.hesvh.cn/Article/details/gglcozben.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.share.hesvh.cn/Article/details/gowvsiwxq.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/ghfwnopwo.sHtML

J. 日期与时间
来源：http://wap.fehbvm.com/Article/details/gxgpwsiwo.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gjziptttd.sHtML

[J01] 获取当前时间
来源：http://www.share.hesvh.cn/Article/details/gohhcvlzt.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.m.share.fehbvm.com/Article/details/gyfgngmeh.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.blog.zdbjq.cn/Article/details/gqqkinfyq.sHtML

JS:   new Date();  Date.now()
来源：http://read.share.zdbjq.cn/Article/details/gvmrdnyps.sHtML

TS:   new Date();  Date.now()
来源：http://blog.fehbvm.com/Article/details/gabfqmgdn.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://blog.hesvh.cn/Article/details/gjpxdjhmy.sHtML

Go:   time.Now()
来源：http://blog.fehbvm.com/Article/details/gdoeilyig.sHtML

Ruby: Time.now
来源：http://www.share.zdbjq.cn/Article/details/grxyztlkn.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://baike.hesvh.cn/Article/details/gydtwsgkv.sHtML

[J02] 格式化输出
来源：http://baike.zdbjq.cn/Article/details/gmrjvrspd.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.hesvh.cn/Article/details/goyxpxqcy.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mobile.zdbjq.cn/Article/details/gbipitixb.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.m.share.zdbjq.cn/Article/details/gxcfhmack.sHtML

TS:   d.toISOString()
来源：http://www.blog.fehbvm.com/Article/details/gslcuvfim.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://m.share.hesvh.cn/Article/details/gndrhntjm.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://baike.fehbvm.com/Article/details/gpekfliaj.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.fehbvm.com/Article/details/gomjnvqar.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://3g.zdbjq.cn/Article/details/gjslkhvge.sHtML


<!-- 参考信息 -->