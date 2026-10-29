代发 wailian999

Ruby: @name = "x"
来源：http://read.share.hesvh.cn/Article/details/glptbliwx.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.zdbjq.cn/Article/details/gggjwljsp.sHtML

[G04] 定义方法
来源：http://www.m.share.fehbvm.com/Article/details/gztrfklgm.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.zdbjq.cn/Article/details/ggxdandvl.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.zdbjq.cn/Article/details/ghchppqbi.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.hesvh.cn/Article/details/gshhmpozq.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.fehbvm.com/Article/details/geqzjkfix.sHtML

Java: String greet() { return name; }
来源：http://read.share.hesvh.cn/Article/details/ghznxxygh.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.hesvh.cn/Article/details/gkttugehb.sHtML

Ruby: def greet; @name; end
来源：http://www.share.zdbjq.cn/Article/details/gqfeubihe.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.zdbjq.cn/Article/details/gcwqlxvqc.sHtML

[G05] 继承
来源：http://blog.zdbjq.cn/Article/details/gsawgevlc.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.fehbvm.com/Article/details/gofgateyt.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/gfbrbngty.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/gwywvucsj.sHtML

TS:   class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/gaujskbju.sHtML

Java: class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/gfntqnlom.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.fehbvm.com/Article/details/gpcuhazra.sHtML

Ruby: class Admin < User; end
来源：http://read.share.hesvh.cn/Article/details/gjsxoupxe.sHtML

C#:   class Admin : User {}
来源：http://www.blog.hesvh.cn/Article/details/gofgytehh.sHtML

[G06] 重写方法
来源：http://www.blog.zdbjq.cn/Article/details/gdkvyfntj.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.fehbvm.com/Article/details/gqkbfxeoq.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/gncmlqdam.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/gsasfltgx.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/grsmpnsoq.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/gywtuemet.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.zdbjq.cn/Article/details/gtespieyv.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.hesvh.cn/Article/details/gwaynnzhj.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.hesvh.cn/Article/details/gtzttwmeq.sHtML

[G07] 调用父类方法
来源：http://m.share.hesvh.cn/Article/details/gwsqxyyoi.sHtML

Py:   super().greet()
来源：http://www.blog.zdbjq.cn/Article/details/gpfilvgcz.sHtML

PHP:  parent::greet();
来源：http://blog.zdbjq.cn/Article/details/gjmpwenoa.sHtML

JS:   super.greet();
来源：http://www.share.fehbvm.com/Article/details/gvzqnxcec.sHtML

TS:   super.greet();
来源：http://mobile.hesvh.cn/Article/details/ggytzzyal.sHtML

Java: super.greet();
来源：http://www.m.share.hesvh.cn/Article/details/gmutenzpf.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.hesvh.cn/Article/details/guuidybdr.sHtML

Ruby: super
来源：http://read.share.hesvh.cn/Article/details/gasyohftl.sHtML

C#:   base.Greet();
来源：http://3g.hesvh.cn/Article/details/gcktxuxxi.sHtML

[G08] 静态方法与属性
来源：http://read.share.hesvh.cn/Article/details/gtjlzvppm.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.zdbjq.cn/Article/details/govsbwjrn.sHtML

PHP:  public static function f() {}
来源：http://www.blog.hesvh.cn/Article/details/goacojcat.sHtML

JS:   static f() {}
来源：http://www.m.share.hesvh.cn/Article/details/gejggarev.sHtML

TS:   static f(): void {}
来源：http://www.share.zdbjq.cn/Article/details/gdsokiaik.sHtML

Java: static void f() {}
来源：http://wap.zdbjq.cn/Article/details/ggflcehpf.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.hesvh.cn/Article/details/gvfwdmjxz.sHtML

Ruby: def self.f; end
来源：http://www.blog.fehbvm.com/Article/details/gnitoebft.sHtML

C#:   public static void F() {}
来源：http://mobile.hesvh.cn/Article/details/gsopmkhjf.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.zdbjq.cn/Article/details/ganwxkzuy.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.hesvh.cn/Article/details/gphmhvovy.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.hesvh.cn/Article/details/gbatohgqy.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.zdbjq.cn/Article/details/gnjadcbih.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.zdbjq.cn/Article/details/glicuiamn.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.hesvh.cn/Article/details/gnikndxpo.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.fehbvm.com/Article/details/gugqwoxeq.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.fehbvm.com/Article/details/grweftefv.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.hesvh.cn/Article/details/ggmhukgtc.sHtML

[G10] 访问控制
来源：http://m.share.hesvh.cn/Article/details/gbnllymxu.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.hesvh.cn/Article/details/gxaahkjrc.sHtML

PHP:  public / protected / private
来源：http://m.share.zdbjq.cn/Article/details/gdpcqtzkh.sHtML

JS:   #private 字段；其余公开
来源：http://wap.zdbjq.cn/Article/details/gcanfcdra.sHtML

TS:   public / protected / private
来源：http://www.blog.fehbvm.com/Article/details/gmkumpulz.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.hesvh.cn/Article/details/gearmkrjf.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.fehbvm.com/Article/details/ghuptfkmn.sHtML

Ruby: public / protected / private
来源：http://www.share.hesvh.cn/Article/details/gmcmbufju.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.fehbvm.com/Article/details/ghtqajigr.sHtML

[G11] getter / setter
来源：http://m.share.hesvh.cn/Article/details/gyaqiqxqp.sHtML

Py:   @property 与 @x.setter
来源：http://3g.zdbjq.cn/Article/details/gxgupsbtd.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.fehbvm.com/Article/details/geacgmzvx.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.zdbjq.cn/Article/details/gfawgvegx.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.fehbvm.com/Article/details/gujspigpj.sHtML

Java: public String getName() { return name; }
来源：http://3g.fehbvm.com/Article/details/gsmgpnlxj.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.fehbvm.com/Article/details/gaoerttye.sHtML

Ruby: attr_accessor :name
来源：http://blog.zdbjq.cn/Article/details/gmjmroouh.sHtML

C#:   public string Name { get; set; }
来源：http://3g.fehbvm.com/Article/details/gthfbdkbb.sHtML

[G12] 对象转字符串
来源：http://www.m.share.fehbvm.com/Article/details/gylazdgsp.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.zdbjq.cn/Article/details/gvwhojedy.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.fehbvm.com/Article/details/gedtbhoba.sHtML

JS:   toString() { return this.name; }
来源：http://blog.fehbvm.com/Article/details/gzbusrpxy.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.hesvh.cn/Article/details/gdhaixsyi.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.hesvh.cn/Article/details/gfzgzxzwd.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.fehbvm.com/Article/details/gvrvqifno.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.hesvh.cn/Article/details/gnoghzinb.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.fehbvm.com/Article/details/gfrljzylc.sHtML

[G13] 判断对象类型
来源：http://www.share.zdbjq.cn/Article/details/ggrrpordj.sHtML

Py:   isinstance(u, User)
来源：http://3g.fehbvm.com/Article/details/gznauwjck.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.fehbvm.com/Article/details/gcztxkwcp.sHtML

JS:   u instanceof User
来源：http://3g.fehbvm.com/Article/details/gaeqyevmi.sHtML

TS:   u instanceof User
来源：http://baike.fehbvm.com/Article/details/ginwilveu.sHtML

Java: u instanceof User
来源：http://baike.fehbvm.com/Article/details/gxzcgcncd.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.zdbjq.cn/Article/details/gixudhvfj.sHtML

Ruby: u.is_a?(User)
来源：http://3g.hesvh.cn/Article/details/gycdvcyhf.sHtML

C#:   u is User
来源：http://www.share.zdbjq.cn/Article/details/gkrwrwnxd.sHtML

[G14] 数据类 / record
来源：http://www.m.share.zdbjq.cn/Article/details/gxwdcvyqn.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.hesvh.cn/Article/details/gijezhkqk.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://read.share.zdbjq.cn/Article/details/gzoderzvp.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.hesvh.cn/Article/details/genmlsjdq.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.fehbvm.com/Article/details/gdzhkwlrb.sHtML

Java: record User(String name, int age) {}
来源：http://read.share.zdbjq.cn/Article/details/gtbooeekp.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.zdbjq.cn/Article/details/gvtxwjtig.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.hesvh.cn/Article/details/ggfapjavn.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.zdbjq.cn/Article/details/gibsuczkc.sHtML

[G15] 枚举
来源：http://wap.zdbjq.cn/Article/details/gfgnyrqje.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.hesvh.cn/Article/details/gywkniiwg.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.hesvh.cn/Article/details/gwffdhbmw.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.fehbvm.com/Article/details/gbadnarbc.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.zdbjq.cn/Article/details/gzuxygfbd.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.zdbjq.cn/Article/details/gqutjmexa.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://baike.fehbvm.com/Article/details/gnycudqfc.sHtML

Ruby: Color = %i[red green].freeze
来源：http://m.share.zdbjq.cn/Article/details/givrpxqou.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.hesvh.cn/Article/details/gwsifkvib.sHtML

[G16] 对象转数组 / 字典
来源：http://www.m.share.zdbjq.cn/Article/details/geagumzci.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.zdbjq.cn/Article/details/gwuntmqtv.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.fehbvm.com/Article/details/givmkkyxe.sHtML

JS:   Object.entries(obj)
来源：http://m.share.fehbvm.com/Article/details/govthakqu.sHtML

TS:   Object.entries(obj)
来源：http://read.share.fehbvm.com/Article/details/gxxnickje.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://blog.fehbvm.com/Article/details/gffufjton.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.hesvh.cn/Article/details/gzfgucses.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.fehbvm.com/Article/details/gfsckfwai.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.fehbvm.com/Article/details/gkzbqvuzk.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gtvnydgcs.sHtML

H. 异常与错误处理
来源：http://blog.hesvh.cn/Article/details/gmkkmivcu.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gavabvxns.sHtML

[H01] try / catch 基础
来源：http://www.share.zdbjq.cn/Article/details/gkcgozjtc.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.fehbvm.com/Article/details/gtrdooqxq.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.zdbjq.cn/Article/details/grasiiesl.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.zdbjq.cn/Article/details/gjoxtpvyh.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.blog.zdbjq.cn/Article/details/gfotsmzjl.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.hesvh.cn/Article/details/getsbhzfj.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.m.share.zdbjq.cn/Article/details/gvkjgefmm.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.zdbjq.cn/Article/details/gbprxwydm.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.m.share.fehbvm.com/Article/details/ggeegeqvz.sHtML

[H02] finally / ensure 收尾
来源：http://baike.zdbjq.cn/Article/details/gtlwyjrjd.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://read.share.hesvh.cn/Article/details/gyxaoqurm.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.hesvh.cn/Article/details/gdwtexlfp.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/gukcgloei.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.zdbjq.cn/Article/details/grnecakid.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.zdbjq.cn/Article/details/ghyalwode.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://3g.hesvh.cn/Article/details/geicxoslw.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://blog.hesvh.cn/Article/details/gomwhhjlx.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/gmwcwruxy.sHtML

[H03] 主动抛出异常
来源：http://3g.hesvh.cn/Article/details/gsheflstj.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.fehbvm.com/Article/details/getlhhqyg.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.zdbjq.cn/Article/details/ghupbdqro.sHtML

JS:   throw new Error("错误信息");
来源：http://www.share.fehbvm.com/Article/details/gadqpkmfv.sHtML

TS:   throw new Error("错误信息");
来源：http://www.blog.zdbjq.cn/Article/details/gjvaoihhn.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.zdbjq.cn/Article/details/glqpbbaic.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.blog.hesvh.cn/Article/details/gbnwmafjq.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://m.share.hesvh.cn/Article/details/ggbyzaybs.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.hesvh.cn/Article/details/grojbwfbi.sHtML

[H04] 自定义异常类型
来源：http://www.share.hesvh.cn/Article/details/gvtxpqauf.sHtML

Py:   class MyError(Exception): pass
来源：http://blog.hesvh.cn/Article/details/guvkpvclp.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://wap.zdbjq.cn/Article/details/gekjwrtyn.sHtML

JS:   class MyError extends Error {}
来源：http://blog.fehbvm.com/Article/details/gfaukwans.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.hesvh.cn/Article/details/ggojibmsl.sHtML

Java: class MyException extends RuntimeException {}
来源：http://m.share.zdbjq.cn/Article/details/gdxapgroe.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.hesvh.cn/Article/details/gdmgdprge.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.zdbjq.cn/Article/details/gwhxsadpp.sHtML

C#:   class MyException : Exception {}
来源：http://read.share.hesvh.cn/Article/details/gntacaaxk.sHtML

[H05] 捕获特定类型
来源：http://www.m.share.fehbvm.com/Article/details/gnqdewieq.sHtML

Py:   except ValueError as e:
来源：http://www.blog.hesvh.cn/Article/details/gpxgextug.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.fehbvm.com/Article/details/gjjoeivfb.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://m.share.fehbvm.com/Article/details/gubuzqlje.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://3g.hesvh.cn/Article/details/gqqadyqdp.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://blog.fehbvm.com/Article/details/ggzgsrhjy.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.blog.fehbvm.com/Article/details/giucfurwy.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.hesvh.cn/Article/details/glcplmfbh.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.blog.hesvh.cn/Article/details/gbggjnnma.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.blog.zdbjq.cn/Article/details/gmkiwzgkj.sHtML

Py:   value = d.get("k") or default
来源：http://www.blog.hesvh.cn/Article/details/gqnumymtg.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.m.share.zdbjq.cn/Article/details/gaytjzhqb.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://wap.fehbvm.com/Article/details/gcojbmiss.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.share.fehbvm.com/Article/details/gzlgioovm.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wap.hesvh.cn/Article/details/gbjfmopxe.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://m.share.fehbvm.com/Article/details/gjvpdcusf.sHtML

Ruby: d&.dig(:a, :b)
来源：http://mobile.hesvh.cn/Article/details/gzrcsdjyr.sHtML

C#:   obj?.A?.B ?? default
来源：http://wap.hesvh.cn/Article/details/gohvzhlgr.sHtML

[H07] 断言
来源：http://3g.fehbvm.com/Article/details/gmijlqlpt.sHtML

Py:   assert x > 0, "必须为正"
来源：http://wap.fehbvm.com/Article/details/gqjohqnbr.sHtML

PHP:  assert($x > 0);
来源：http://m.share.hesvh.cn/Article/details/gwooouuyg.sHtML

JS:   console.assert(x > 0);
来源：http://m.share.zdbjq.cn/Article/details/gqusbmcpi.sHtML

TS:   console.assert(x > 0);
来源：http://m.share.zdbjq.cn/Article/details/gpwmawwep.sHtML

Java: assert x > 0 : "必须为正";
来源：http://read.share.fehbvm.com/Article/details/gbnkpfxqr.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mobile.hesvh.cn/Article/details/gsqybczrn.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://mobile.fehbvm.com/Article/details/gaafuccxz.sHtML

C#:   Debug.Assert(x > 0);
来源：http://mobile.hesvh.cn/Article/details/gxczyfjkq.sHtML

[H08] 获取错误信息与堆栈
来源：http://read.share.zdbjq.cn/Article/details/gpyyagwjo.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://mobile.hesvh.cn/Article/details/glbeapcsx.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://m.share.zdbjq.cn/Article/details/gwfesvumn.sHtML

JS:   e.message;  e.stack
来源：http://3g.fehbvm.com/Article/details/gawvnasqh.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://wap.fehbvm.com/Article/details/gzkysfglw.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.blog.fehbvm.com/Article/details/gtstudjjp.sHtML

Go:   err.Error()
来源：http://read.share.fehbvm.com/Article/details/gjdndcitm.sHtML

Ruby: e.message;  e.backtrace
来源：http://3g.fehbvm.com/Article/details/gpodpklag.sHtML

C#:   e.Message;  e.StackTrace
来源：http://mobile.hesvh.cn/Article/details/gdqwbysce.sHtML

[H09] 带错误码的异常
来源：http://3g.fehbvm.com/Article/details/grekpiafm.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mobile.fehbvm.com/Article/details/glusdtzuh.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.blog.zdbjq.cn/Article/details/gcdleymga.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.m.share.fehbvm.com/Article/details/gvykxlzhd.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mobile.hesvh.cn/Article/details/giuzfiqos.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://3g.zdbjq.cn/Article/details/gvawknnyn.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wap.fehbvm.com/Article/details/gmhpsdayw.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://read.share.hesvh.cn/Article/details/gjxkqimnf.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://3g.fehbvm.com/Article/details/gzuekgdpj.sHtML

[H10] 资源自动释放
来源：http://blog.fehbvm.com/Article/details/gehzcuwce.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.m.share.zdbjq.cn/Article/details/gscbuuvlj.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wap.zdbjq.cn/Article/details/gzpqtpbuj.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.fehbvm.com/Article/details/gdyztpzee.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.fehbvm.com/Article/details/gjdbtqzax.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.blog.zdbjq.cn/Article/details/goxiaiohk.sHtML

Go:   defer f.Close()
来源：http://baike.fehbvm.com/Article/details/gvkpxijlt.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://baike.zdbjq.cn/Article/details/gbbywiizv.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gfcagzbrl.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gcqntachy.sHtML

I. 正则表达式
来源：http://read.share.hesvh.cn/Article/details/gkoccdnnu.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gmaywpvdz.sHtML

[I01] 判断是否匹配
来源：http://www.blog.zdbjq.cn/Article/details/ghcexhhqm.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://blog.zdbjq.cn/Article/details/gcokazbiz.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://3g.zdbjq.cn/Article/details/gerothztj.sHtML

JS:   /\d+/.test(s)
来源：http://www.m.share.fehbvm.com/Article/details/gwmkumtwj.sHtML

TS:   /\d+/.test(s)
来源：http://www.m.share.hesvh.cn/Article/details/gyxspgzwc.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://baike.fehbvm.com/Article/details/gfthlolca.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mobile.fehbvm.com/Article/details/gtaqlhegq.sHtML

Ruby: s.match?(/\d+/)
来源：http://mobile.hesvh.cn/Article/details/gaesrkzfc.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://baike.zdbjq.cn/Article/details/gxbkflxud.sHtML

[I02] 提取所有匹配
来源：http://read.share.fehbvm.com/Article/details/gcxnwaegu.sHtML

Py:   re.findall(r"\d+", s)
来源：http://3g.hesvh.cn/Article/details/gjfecfduj.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.blog.hesvh.cn/Article/details/gpwketjgd.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://baike.fehbvm.com/Article/details/gqdamffpb.sHtML

TS:   s.match(/\d+/g)
来源：http://m.share.fehbvm.com/Article/details/ghfdfigug.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://m.share.hesvh.cn/Article/details/gvevkzmns.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.m.share.zdbjq.cn/Article/details/gfulzspes.sHtML

Ruby: s.scan(/\d+/)
来源：http://m.share.zdbjq.cn/Article/details/gfabdjogv.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://3g.hesvh.cn/Article/details/gmtqkqljv.sHtML

[I03] 提取捕获分组
来源：http://m.share.fehbvm.com/Article/details/grjekdynt.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://read.share.zdbjq.cn/Article/details/gvxrmashk.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.share.hesvh.cn/Article/details/giabvsovu.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.m.share.hesvh.cn/Article/details/gcatabwbg.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.blog.zdbjq.cn/Article/details/gisvubbqw.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://read.share.zdbjq.cn/Article/details/gwthysjnt.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.blog.zdbjq.cn/Article/details/gdngsywyr.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://blog.zdbjq.cn/Article/details/gdthoskns.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://3g.hesvh.cn/Article/details/guynznttn.sHtML

[I04] 正则替换
来源：http://baike.hesvh.cn/Article/details/gbcnpxuay.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.blog.hesvh.cn/Article/details/gcahxyong.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://baike.fehbvm.com/Article/details/gfyakzaub.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.hesvh.cn/Article/details/gudfeztnq.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://3g.zdbjq.cn/Article/details/gqyazxhbr.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://wap.hesvh.cn/Article/details/greamqwxm.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.m.share.hesvh.cn/Article/details/gijjjdoya.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://blog.hesvh.cn/Article/details/gxehavvar.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://read.share.hesvh.cn/Article/details/ghgamwndy.sHtML

[I05] 按正则拆分
来源：http://www.blog.zdbjq.cn/Article/details/gfurymyem.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.m.share.zdbjq.cn/Article/details/gsxwsuvhm.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://blog.hesvh.cn/Article/details/gtsiqqgkz.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://baike.hesvh.cn/Article/details/gleorqkgp.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://mobile.zdbjq.cn/Article/details/gjadbuzpz.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.m.share.hesvh.cn/Article/details/goltqjeor.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://3g.hesvh.cn/Article/details/gtbiibxnc.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://wap.zdbjq.cn/Article/details/gkylvyxza.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.share.hesvh.cn/Article/details/ggqkmekgi.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://m.share.zdbjq.cn/Article/details/giirurjwi.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://read.share.hesvh.cn/Article/details/gegoqvwpy.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://mobile.zdbjq.cn/Article/details/gaypepjur.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.hesvh.cn/Article/details/gxbxikxam.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.zdbjq.cn/Article/details/gprnioxma.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://read.share.fehbvm.com/Article/details/gmmsxjwtx.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://3g.hesvh.cn/Article/details/gnagdkvgb.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.share.fehbvm.com/Article/details/giugknrri.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.blog.hesvh.cn/Article/details/garzujvvz.sHtML

[I07] 忽略大小写与多行模式
来源：http://read.share.zdbjq.cn/Article/details/ganevdccm.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://read.share.hesvh.cn/Article/details/gywrggisc.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wap.hesvh.cn/Article/details/gjpszvpyi.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://baike.zdbjq.cn/Article/details/gposzscuq.sHtML

TS:   /error/gim
来源：http://www.m.share.zdbjq.cn/Article/details/grpzyepxo.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://baike.fehbvm.com/Article/details/gjcwnkrtz.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.m.share.zdbjq.cn/Article/details/ggfrftpgs.sHtML

Ruby: s.scan(/error/i)
来源：http://mobile.hesvh.cn/Article/details/gsqaoigmd.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://wap.fehbvm.com/Article/details/gowibvyil.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://wap.zdbjq.cn/Article/details/gtsozpqrd.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://3g.hesvh.cn/Article/details/gpkttolpy.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mobile.fehbvm.com/Article/details/gnummpiyk.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.fehbvm.com/Article/details/gysgacswb.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.hesvh.cn/Article/details/gyecfelfp.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.share.fehbvm.com/Article/details/gjeozjeur.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.m.share.fehbvm.com/Article/details/ghtxwapft.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wap.zdbjq.cn/Article/details/gebxjejtd.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.m.share.zdbjq.cn/Article/details/gfggqpxyc.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/grfusyfcw.sHtML

J. 日期与时间
来源：http://mobile.hesvh.cn/Article/details/gtkvhhkdv.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gqcnjbvrd.sHtML

[J01] 获取当前时间
来源：http://wap.fehbvm.com/Article/details/gpcfglscl.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://wap.fehbvm.com/Article/details/girjfazoe.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://baike.hesvh.cn/Article/details/gmgxibhmk.sHtML

JS:   new Date();  Date.now()
来源：http://www.blog.fehbvm.com/Article/details/goowjqsox.sHtML

TS:   new Date();  Date.now()
来源：http://blog.fehbvm.com/Article/details/gazcizgnu.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://wap.zdbjq.cn/Article/details/gbbeedgpr.sHtML

Go:   time.Now()
来源：http://blog.fehbvm.com/Article/details/gslbyqumr.sHtML

Ruby: Time.now
来源：http://3g.fehbvm.com/Article/details/gbkuemefe.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.blog.zdbjq.cn/Article/details/glukxxzvv.sHtML

[J02] 格式化输出
来源：http://3g.fehbvm.com/Article/details/gsgjfjgmv.sHtML


<!-- 参考信息 -->