代发 wailian999

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.zdbjq.cn/Article/details/gocebimwm.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/giyxypwis.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/gurdfqfxu.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gwtryzkbn.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.fehbvm.com/Article/details/gaetigdut.sHtML

Ruby: def greet; @name; end
来源：http://m.share.zdbjq.cn/Article/details/gegbgsfoj.sHtML

C#:   public string Greet() => Name;
来源：http://blog.hesvh.cn/Article/details/gozqjkdqu.sHtML

[G05] 继承
来源：http://read.share.zdbjq.cn/Article/details/goriovofi.sHtML

Py:   class Admin(User): pass
来源：http://m.share.fehbvm.com/Article/details/gjxotladi.sHtML

PHP:  class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/goysuczcj.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/gyhfwwdba.sHtML

TS:   class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/gjmtnlxmu.sHtML

Java: class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/geobkqyiq.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.hesvh.cn/Article/details/gkaqviwug.sHtML

Ruby: class Admin < User; end
来源：http://mobile.fehbvm.com/Article/details/gcksnreyz.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gfnflpuzr.sHtML

[G06] 重写方法
来源：http://read.share.hesvh.cn/Article/details/gcbgvignf.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.fehbvm.com/Article/details/gcxfejfjt.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/gipivtbln.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/gxvpyktha.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/ggiepahzo.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/gonabmlfr.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.zdbjq.cn/Article/details/guxdkigyp.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.zdbjq.cn/Article/details/gwavlppal.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.zdbjq.cn/Article/details/gvoftxmzh.sHtML

[G07] 调用父类方法
来源：http://blog.fehbvm.com/Article/details/gquaqapfb.sHtML

Py:   super().greet()
来源：http://wap.hesvh.cn/Article/details/gmqsdczxz.sHtML

PHP:  parent::greet();
来源：http://baike.hesvh.cn/Article/details/glujgdztq.sHtML

JS:   super.greet();
来源：http://www.blog.zdbjq.cn/Article/details/gujkxoqqa.sHtML

TS:   super.greet();
来源：http://mobile.hesvh.cn/Article/details/gtdpoavbi.sHtML

Java: super.greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gfuocyqpz.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.fehbvm.com/Article/details/gsuwfhyim.sHtML

Ruby: super
来源：http://wap.hesvh.cn/Article/details/grhcpkhkk.sHtML

C#:   base.Greet();
来源：http://wap.fehbvm.com/Article/details/gvvnzuhyd.sHtML

[G08] 静态方法与属性
来源：http://m.share.hesvh.cn/Article/details/gfyfacpzq.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.fehbvm.com/Article/details/gfruntjxx.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.zdbjq.cn/Article/details/gwvbkosyi.sHtML

JS:   static f() {}
来源：http://baike.fehbvm.com/Article/details/gvqyhtnyv.sHtML

TS:   static f(): void {}
来源：http://mobile.hesvh.cn/Article/details/gmqtdyhqy.sHtML

Java: static void f() {}
来源：http://blog.fehbvm.com/Article/details/gazqnokfq.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.zdbjq.cn/Article/details/gvvyhehao.sHtML

Ruby: def self.f; end
来源：http://baike.fehbvm.com/Article/details/gncodkoti.sHtML

C#:   public static void F() {}
来源：http://mobile.fehbvm.com/Article/details/gupszjnjn.sHtML

[G09] 接口 / 抽象类
来源：http://wap.fehbvm.com/Article/details/gclbqztur.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.hesvh.cn/Article/details/gvsersmbd.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.fehbvm.com/Article/details/giimmjrlk.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.fehbvm.com/Article/details/gcxwxharz.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.fehbvm.com/Article/details/gpclmnjcy.sHtML

Java: interface Shape { double area(); }
来源：http://blog.fehbvm.com/Article/details/gwoeqlhmy.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.fehbvm.com/Article/details/gkhmbwgyc.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.hesvh.cn/Article/details/goxklmhph.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.zdbjq.cn/Article/details/gdybwozzm.sHtML

[G10] 访问控制
来源：http://baike.zdbjq.cn/Article/details/gjucploiz.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.zdbjq.cn/Article/details/ggldnqvyr.sHtML

PHP:  public / protected / private
来源：http://m.share.fehbvm.com/Article/details/gxyxqlugt.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.zdbjq.cn/Article/details/gjszqkmqp.sHtML

TS:   public / protected / private
来源：http://3g.hesvh.cn/Article/details/gmaeomfbo.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.hesvh.cn/Article/details/gcdpnlzlu.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.fehbvm.com/Article/details/gkskvzcft.sHtML

Ruby: public / protected / private
来源：http://www.share.zdbjq.cn/Article/details/gzfoyhurf.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.zdbjq.cn/Article/details/gdbsaxhfy.sHtML

[G11] getter / setter
来源：http://wap.fehbvm.com/Article/details/gtfjokafe.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.hesvh.cn/Article/details/gxuojcriu.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.fehbvm.com/Article/details/gpylapybh.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.hesvh.cn/Article/details/gfhxgwokh.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.zdbjq.cn/Article/details/gpfilpluu.sHtML

Java: public String getName() { return name; }
来源：http://blog.fehbvm.com/Article/details/gwqdperbl.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.hesvh.cn/Article/details/gwgnlgpfx.sHtML

Ruby: attr_accessor :name
来源：http://read.share.fehbvm.com/Article/details/gvyvbongp.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.fehbvm.com/Article/details/ggksoeina.sHtML

[G12] 对象转字符串
来源：http://m.share.fehbvm.com/Article/details/gxzxqxkvz.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.fehbvm.com/Article/details/gilnzewcs.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.zdbjq.cn/Article/details/ggbzmwbzo.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/gvluzddny.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.hesvh.cn/Article/details/gppkeudji.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.zdbjq.cn/Article/details/ghieoahpc.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.hesvh.cn/Article/details/gmoiilebk.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.hesvh.cn/Article/details/gjkdpputc.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.fehbvm.com/Article/details/gtvhzvnmt.sHtML

[G13] 判断对象类型
来源：http://baike.fehbvm.com/Article/details/ggarolfhg.sHtML

Py:   isinstance(u, User)
来源：http://read.share.zdbjq.cn/Article/details/ggravbdvj.sHtML

PHP:  $u instanceof User
来源：http://mobile.fehbvm.com/Article/details/gsiglskef.sHtML

JS:   u instanceof User
来源：http://m.share.zdbjq.cn/Article/details/gzswdvwkf.sHtML

TS:   u instanceof User
来源：http://mobile.hesvh.cn/Article/details/gvzgpfmsz.sHtML

Java: u instanceof User
来源：http://www.blog.hesvh.cn/Article/details/gdmdyycmr.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.fehbvm.com/Article/details/gjhhjzmti.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.fehbvm.com/Article/details/grzbdfjsh.sHtML

C#:   u is User
来源：http://www.blog.hesvh.cn/Article/details/gspsjcziu.sHtML

[G14] 数据类 / record
来源：http://m.share.zdbjq.cn/Article/details/gmnomgmxw.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.fehbvm.com/Article/details/guasismrv.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.zdbjq.cn/Article/details/gayhtthzk.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.zdbjq.cn/Article/details/ghwejlnvt.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.fehbvm.com/Article/details/grubmkpyj.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.zdbjq.cn/Article/details/gskxroaea.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.hesvh.cn/Article/details/gvzkamdir.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.zdbjq.cn/Article/details/gujlziunx.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.fehbvm.com/Article/details/grvkyefpc.sHtML

[G15] 枚举
来源：http://www.share.fehbvm.com/Article/details/glfpgkipy.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.hesvh.cn/Article/details/gekqxwwkx.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.hesvh.cn/Article/details/gyipauhpw.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.fehbvm.com/Article/details/ggvpykbhl.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.zdbjq.cn/Article/details/gqoftoanc.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.zdbjq.cn/Article/details/gscsypniz.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.fehbvm.com/Article/details/gmeqjcpww.sHtML

Ruby: Color = %i[red green].freeze
来源：http://read.share.fehbvm.com/Article/details/grfpfzsxb.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.hesvh.cn/Article/details/giqatlkts.sHtML

[G16] 对象转数组 / 字典
来源：http://m.share.zdbjq.cn/Article/details/gjpoqykln.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.fehbvm.com/Article/details/gvzizeseb.sHtML

PHP:  get_object_vars($obj);
来源：http://3g.hesvh.cn/Article/details/gxadhtrsr.sHtML

JS:   Object.entries(obj)
来源：http://read.share.hesvh.cn/Article/details/gaturbtsn.sHtML

TS:   Object.entries(obj)
来源：http://read.share.fehbvm.com/Article/details/gouqodvim.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.zdbjq.cn/Article/details/gucaikkdy.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.hesvh.cn/Article/details/ghefkqabh.sHtML

Ruby: obj.instance_variables
来源：http://3g.zdbjq.cn/Article/details/gvopaupus.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.blog.fehbvm.com/Article/details/gkvvfmckq.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gqnldkmle.sHtML

H. 异常与错误处理
来源：http://read.share.zdbjq.cn/Article/details/gtcjrfyad.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gfqevqpqi.sHtML

[H01] try / catch 基础
来源：http://www.blog.hesvh.cn/Article/details/ggljztxqc.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.fehbvm.com/Article/details/gpynonstg.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.hesvh.cn/Article/details/gqfcheyni.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.hesvh.cn/Article/details/gwtloykle.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.m.share.zdbjq.cn/Article/details/gzwlvhunb.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.hesvh.cn/Article/details/gvitonlmy.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://baike.hesvh.cn/Article/details/gjtcaqikv.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.share.hesvh.cn/Article/details/gmvtyguft.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.fehbvm.com/Article/details/gqalvfhky.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.fehbvm.com/Article/details/gazgdckxp.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://3g.fehbvm.com/Article/details/gnobwirpv.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://3g.hesvh.cn/Article/details/gzoykvzzg.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.zdbjq.cn/Article/details/ggffbjegc.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://blog.fehbvm.com/Article/details/gkeinwtol.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://wap.hesvh.cn/Article/details/ggomfdmjo.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.fehbvm.com/Article/details/gqtxshbem.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://read.share.hesvh.cn/Article/details/gptscumoz.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.share.hesvh.cn/Article/details/gmwzoqrjn.sHtML

[H03] 主动抛出异常
来源：http://www.share.fehbvm.com/Article/details/gzdjyssdr.sHtML

Py:   raise ValueError("错误信息")
来源：http://3g.zdbjq.cn/Article/details/ggvtukdms.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blog.zdbjq.cn/Article/details/gfbwjamvm.sHtML

JS:   throw new Error("错误信息");
来源：http://blog.zdbjq.cn/Article/details/gjoysqbmp.sHtML

TS:   throw new Error("错误信息");
来源：http://mobile.hesvh.cn/Article/details/gmfatjxdt.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.m.share.fehbvm.com/Article/details/gklrgtexn.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.m.share.hesvh.cn/Article/details/gugpnxzvz.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://3g.hesvh.cn/Article/details/gxwqzsqwn.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://baike.hesvh.cn/Article/details/gmlwqefqh.sHtML

[H04] 自定义异常类型
来源：http://mobile.fehbvm.com/Article/details/gbxxymhmt.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.zdbjq.cn/Article/details/gznsmiixp.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://3g.fehbvm.com/Article/details/gjyphofyc.sHtML

JS:   class MyError extends Error {}
来源：http://wap.zdbjq.cn/Article/details/ghadjagxk.sHtML

TS:   class MyError extends Error {}
来源：http://wap.hesvh.cn/Article/details/guxqucnby.sHtML

Java: class MyException extends RuntimeException {}
来源：http://m.share.hesvh.cn/Article/details/gfcxirbwd.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.m.share.fehbvm.com/Article/details/gxlztdfjp.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.zdbjq.cn/Article/details/gqevxlbrl.sHtML

C#:   class MyException : Exception {}
来源：http://baike.zdbjq.cn/Article/details/gjmcdfhve.sHtML

[H05] 捕获特定类型
来源：http://3g.hesvh.cn/Article/details/gtgmyluzi.sHtML

Py:   except ValueError as e:
来源：http://read.share.fehbvm.com/Article/details/gwkfyiasl.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://read.share.hesvh.cn/Article/details/gwewiyhkq.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.m.share.hesvh.cn/Article/details/gbudtbfhc.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://read.share.fehbvm.com/Article/details/geiqgrbji.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://blog.hesvh.cn/Article/details/gzmweubrj.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://baike.hesvh.cn/Article/details/gjqitsxgu.sHtML

Ruby: rescue ArgumentError => e
来源：http://mobile.zdbjq.cn/Article/details/grvhrjzls.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.share.hesvh.cn/Article/details/gnkzeggdb.sHtML

[H06] 可选值 / 空值安全访问
来源：http://wap.hesvh.cn/Article/details/gsvghsnhn.sHtML

Py:   value = d.get("k") or default
来源：http://www.share.hesvh.cn/Article/details/gbjnsohty.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.blog.zdbjq.cn/Article/details/gazixgfuc.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://wap.fehbvm.com/Article/details/ganbranfe.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://mobile.hesvh.cn/Article/details/gpesswjql.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://m.share.zdbjq.cn/Article/details/guuewzwnp.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://m.share.hesvh.cn/Article/details/gfrmotdow.sHtML

Ruby: d&.dig(:a, :b)
来源：http://wap.zdbjq.cn/Article/details/gzlzhzhty.sHtML

C#:   obj?.A?.B ?? default
来源：http://wap.fehbvm.com/Article/details/gdvxcincm.sHtML

[H07] 断言
来源：http://mobile.zdbjq.cn/Article/details/gluexcape.sHtML

Py:   assert x > 0, "必须为正"
来源：http://read.share.fehbvm.com/Article/details/gehmdddwq.sHtML

PHP:  assert($x > 0);
来源：http://m.share.fehbvm.com/Article/details/ggogmxiww.sHtML

JS:   console.assert(x > 0);
来源：http://wap.fehbvm.com/Article/details/gfphcyjnb.sHtML

TS:   console.assert(x > 0);
来源：http://m.share.zdbjq.cn/Article/details/gbidfbjzi.sHtML

Java: assert x > 0 : "必须为正";
来源：http://blog.hesvh.cn/Article/details/gkuavueho.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://blog.hesvh.cn/Article/details/gtoixfouk.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://read.share.zdbjq.cn/Article/details/gscglxswi.sHtML

C#:   Debug.Assert(x > 0);
来源：http://baike.hesvh.cn/Article/details/gagbxegvk.sHtML

[H08] 获取错误信息与堆栈
来源：http://mobile.fehbvm.com/Article/details/gvazmnkdo.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://3g.fehbvm.com/Article/details/gvamextus.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wap.hesvh.cn/Article/details/gvfnrtcdm.sHtML

JS:   e.message;  e.stack
来源：http://blog.fehbvm.com/Article/details/gixhtlphr.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.share.hesvh.cn/Article/details/geziltzyq.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.m.share.hesvh.cn/Article/details/gvclegsmx.sHtML

Go:   err.Error()
来源：http://read.share.fehbvm.com/Article/details/gqdrfnsip.sHtML

Ruby: e.message;  e.backtrace
来源：http://read.share.zdbjq.cn/Article/details/gntjmzyjp.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.m.share.hesvh.cn/Article/details/gzegnwsvm.sHtML

[H09] 带错误码的异常
来源：http://read.share.hesvh.cn/Article/details/gddmfsmwg.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.share.fehbvm.com/Article/details/gqfxeumin.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://wap.fehbvm.com/Article/details/govzmlilp.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mobile.zdbjq.cn/Article/details/ghmwioyts.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wap.hesvh.cn/Article/details/gyyajuxjx.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://read.share.zdbjq.cn/Article/details/gagcrlhhg.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://blog.zdbjq.cn/Article/details/gwvkkifvb.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://wap.zdbjq.cn/Article/details/gnfxytngp.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.share.hesvh.cn/Article/details/gwrydbqii.sHtML

[H10] 资源自动释放
来源：http://www.share.hesvh.cn/Article/details/guagtlnrb.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://read.share.zdbjq.cn/Article/details/gbzkitjue.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://m.share.zdbjq.cn/Article/details/goxjbfykv.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.zdbjq.cn/Article/details/gysvsnrav.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.hesvh.cn/Article/details/gshocqcxp.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://3g.fehbvm.com/Article/details/gpabrfwhu.sHtML

Go:   defer f.Close()
来源：http://m.share.fehbvm.com/Article/details/gtajyqnzd.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wap.zdbjq.cn/Article/details/gpbnnmtfg.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/ghifzlxvj.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gvtfkilcl.sHtML

I. 正则表达式
来源：http://baike.zdbjq.cn/Article/details/geojgbqii.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gfffinsew.sHtML

[I01] 判断是否匹配
来源：http://blog.hesvh.cn/Article/details/gvxbrqgzp.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://blog.fehbvm.com/Article/details/ggztusrtl.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.m.share.hesvh.cn/Article/details/gnogauubs.sHtML

JS:   /\d+/.test(s)
来源：http://wap.zdbjq.cn/Article/details/gaqbulqld.sHtML

TS:   /\d+/.test(s)
来源：http://wap.fehbvm.com/Article/details/gcszsmajw.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.blog.zdbjq.cn/Article/details/gjlzixvak.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://3g.fehbvm.com/Article/details/gktfwywae.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.share.zdbjq.cn/Article/details/gkkjptvyr.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wap.fehbvm.com/Article/details/gmizdfshw.sHtML

[I02] 提取所有匹配
来源：http://www.share.zdbjq.cn/Article/details/gbqopoifn.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.blog.fehbvm.com/Article/details/gjopvifdr.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://blog.zdbjq.cn/Article/details/gjjruecej.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://m.share.fehbvm.com/Article/details/gpzazflcf.sHtML

TS:   s.match(/\d+/g)
来源：http://blog.hesvh.cn/Article/details/gtziawulf.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://blog.hesvh.cn/Article/details/grptbheui.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.blog.zdbjq.cn/Article/details/gevullxsl.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.share.fehbvm.com/Article/details/gfupkzfxq.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gwlagbvoc.sHtML

[I03] 提取捕获分组
来源：http://blog.hesvh.cn/Article/details/gydtqpfvn.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://3g.fehbvm.com/Article/details/ggnsjtfzm.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.m.share.zdbjq.cn/Article/details/grngugpjn.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.blog.zdbjq.cn/Article/details/guxiiwqvf.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://m.share.zdbjq.cn/Article/details/gdzvmsibq.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://m.share.zdbjq.cn/Article/details/gvijxmabn.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://3g.zdbjq.cn/Article/details/gjlmgqndx.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wap.fehbvm.com/Article/details/gayyxalow.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://baike.zdbjq.cn/Article/details/gaamqnybg.sHtML

[I04] 正则替换
来源：http://www.share.zdbjq.cn/Article/details/gektcajgo.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://mobile.zdbjq.cn/Article/details/gvxnudcny.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.fehbvm.com/Article/details/gghduqncs.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.hesvh.cn/Article/details/gvshjkmpr.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://baike.zdbjq.cn/Article/details/gqnsjhymw.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://3g.hesvh.cn/Article/details/gyfckvatx.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://read.share.fehbvm.com/Article/details/gjcpqmptz.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://m.share.fehbvm.com/Article/details/gpaubiged.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.m.share.hesvh.cn/Article/details/gjggwhcfl.sHtML

[I05] 按正则拆分
来源：http://wap.hesvh.cn/Article/details/gdrczpqes.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://m.share.zdbjq.cn/Article/details/gokjftxfb.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.blog.zdbjq.cn/Article/details/gvwjztldo.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.blog.zdbjq.cn/Article/details/gmpufptkx.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://m.share.zdbjq.cn/Article/details/gfdnffqny.sHtML

Java: s.split("\\s*,\\s*")
来源：http://blog.hesvh.cn/Article/details/ghjtovxkk.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://m.share.fehbvm.com/Article/details/gfquvynzv.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://m.share.fehbvm.com/Article/details/gkjrgulmb.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://read.share.zdbjq.cn/Article/details/grjuxembl.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://blog.zdbjq.cn/Article/details/gxpgilwjx.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.blog.hesvh.cn/Article/details/gvsnvxeeg.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://read.share.hesvh.cn/Article/details/gckowiqqq.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.hesvh.cn/Article/details/giaxxjrvk.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.fehbvm.com/Article/details/gmhdmzqkt.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.share.fehbvm.com/Article/details/gjqyyxbwh.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://mobile.fehbvm.com/Article/details/geiflgvnn.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://3g.zdbjq.cn/Article/details/gkotxzupl.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.m.share.hesvh.cn/Article/details/gjnfnryai.sHtML

[I07] 忽略大小写与多行模式
来源：http://3g.fehbvm.com/Article/details/groapotws.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mobile.zdbjq.cn/Article/details/gtgnvtnpj.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.share.fehbvm.com/Article/details/grkevyeii.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mobile.zdbjq.cn/Article/details/gilsxjhst.sHtML

TS:   /error/gim
来源：http://3g.fehbvm.com/Article/details/goztzrptv.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mobile.hesvh.cn/Article/details/gyiqinqyi.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mobile.zdbjq.cn/Article/details/gqkbyjwwy.sHtML

Ruby: s.scan(/error/i)
来源：http://www.share.hesvh.cn/Article/details/guyzhiaka.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://3g.zdbjq.cn/Article/details/ggazrhcfy.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.m.share.hesvh.cn/Article/details/gocxhmyrh.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wap.zdbjq.cn/Article/details/gxyupxqou.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://baike.fehbvm.com/Article/details/gbobslaqw.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.hesvh.cn/Article/details/gdatqrcfk.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.fehbvm.com/Article/details/ggwoteuyv.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://m.share.hesvh.cn/Article/details/gmpqohpsc.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.blog.zdbjq.cn/Article/details/gbstighcy.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.m.share.fehbvm.com/Article/details/gsavsdizo.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://baike.zdbjq.cn/Article/details/gazkunmnb.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gmsyknabz.sHtML

J. 日期与时间
来源：http://www.share.fehbvm.com/Article/details/gjmuzwhcr.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gbcnmnsfi.sHtML

[J01] 获取当前时间
来源：http://www.blog.zdbjq.cn/Article/details/ggxgiizbf.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.m.share.zdbjq.cn/Article/details/giuwlttce.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://blog.hesvh.cn/Article/details/giqiukjcv.sHtML

JS:   new Date();  Date.now()
来源：http://mobile.hesvh.cn/Article/details/gkpxurcjh.sHtML

TS:   new Date();  Date.now()
来源：http://wap.zdbjq.cn/Article/details/gligqvrfj.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.blog.hesvh.cn/Article/details/gzilhunkd.sHtML

Go:   time.Now()
来源：http://www.m.share.hesvh.cn/Article/details/gvwnuavhj.sHtML

Ruby: Time.now
来源：http://www.m.share.zdbjq.cn/Article/details/grltbginf.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://3g.fehbvm.com/Article/details/garauycov.sHtML

[J02] 格式化输出
来源：http://www.share.fehbvm.com/Article/details/gutbwjrai.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.fehbvm.com/Article/details/gkxfvjgsu.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.blog.fehbvm.com/Article/details/gshommbeh.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://baike.hesvh.cn/Article/details/gikpmwzdn.sHtML

TS:   d.toISOString()
来源：http://www.m.share.fehbvm.com/Article/details/gqxwudvjr.sHtML


<!-- 参考信息 -->