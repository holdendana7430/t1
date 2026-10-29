代发 wailian999

Ruby: @name = "x"
来源：http://3g.fehbvm.com/Article/details/gfddhofml.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.fehbvm.com/Article/details/gwcmkdove.sHtML

[G04] 定义方法
来源：http://mobile.zdbjq.cn/Article/details/gyhskwtra.sHtML

Py:   def greet(self): return self.name
来源：http://blog.zdbjq.cn/Article/details/gbpwuhixh.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.zdbjq.cn/Article/details/glnxiglut.sHtML

JS:   greet() { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/gatbtbdiy.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.hesvh.cn/Article/details/gzjilvsiz.sHtML

Java: String greet() { return name; }
来源：http://mobile.hesvh.cn/Article/details/gdprrlmqu.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.hesvh.cn/Article/details/gludztpdi.sHtML

Ruby: def greet; @name; end
来源：http://3g.hesvh.cn/Article/details/gdmgmzahi.sHtML

C#:   public string Greet() => Name;
来源：http://wap.fehbvm.com/Article/details/gitkvhxoo.sHtML

[G05] 继承
来源：http://www.m.share.zdbjq.cn/Article/details/gwspytkks.sHtML

Py:   class Admin(User): pass
来源：http://mobile.hesvh.cn/Article/details/gxadowluo.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/gnznwxloq.sHtML

JS:   class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/gjhowwxdr.sHtML

TS:   class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/gdfjtjpkr.sHtML

Java: class Admin extends User {}
来源：http://www.share.hesvh.cn/Article/details/gtzvtpglq.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.hesvh.cn/Article/details/gnxhvsjpy.sHtML

Ruby: class Admin < User; end
来源：http://baike.zdbjq.cn/Article/details/giktolvvl.sHtML

C#:   class Admin : User {}
来源：http://www.share.fehbvm.com/Article/details/gwsblurvt.sHtML

[G06] 重写方法
来源：http://wap.hesvh.cn/Article/details/gvzknxdjc.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.fehbvm.com/Article/details/gyxpcuafb.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/gibbhwdbb.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/ghiduzefv.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/gudngvueu.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/guypyumkq.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.hesvh.cn/Article/details/goxmgtgim.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.zdbjq.cn/Article/details/gaskcgnam.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.hesvh.cn/Article/details/gurlyikno.sHtML

[G07] 调用父类方法
来源：http://www.m.share.fehbvm.com/Article/details/gwzzlhcen.sHtML

Py:   super().greet()
来源：http://www.blog.fehbvm.com/Article/details/gvxrjzwcr.sHtML

PHP:  parent::greet();
来源：http://blog.zdbjq.cn/Article/details/gikphbtwd.sHtML

JS:   super.greet();
来源：http://read.share.zdbjq.cn/Article/details/gtwmlrcxw.sHtML

TS:   super.greet();
来源：http://baike.hesvh.cn/Article/details/gisajbbxm.sHtML

Java: super.greet();
来源：http://www.share.zdbjq.cn/Article/details/gtytezpzo.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.zdbjq.cn/Article/details/gaguwgljj.sHtML

Ruby: super
来源：http://wap.fehbvm.com/Article/details/glytfwwak.sHtML

C#:   base.Greet();
来源：http://mobile.zdbjq.cn/Article/details/gxyzdkfud.sHtML

[G08] 静态方法与属性
来源：http://3g.fehbvm.com/Article/details/gvfthdnvu.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.zdbjq.cn/Article/details/gqblfwgvx.sHtML

PHP:  public static function f() {}
来源：http://www.share.hesvh.cn/Article/details/gxvqjhxcy.sHtML

JS:   static f() {}
来源：http://blog.hesvh.cn/Article/details/gvvyvclmj.sHtML

TS:   static f(): void {}
来源：http://3g.fehbvm.com/Article/details/grupuhpas.sHtML

Java: static void f() {}
来源：http://www.blog.zdbjq.cn/Article/details/ggbdhaceq.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.hesvh.cn/Article/details/gxzpzxkla.sHtML

Ruby: def self.f; end
来源：http://read.share.zdbjq.cn/Article/details/gisxvohue.sHtML

C#:   public static void F() {}
来源：http://3g.fehbvm.com/Article/details/gynnlawsb.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.zdbjq.cn/Article/details/gxdggkwmh.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.hesvh.cn/Article/details/gnamuolzd.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.zdbjq.cn/Article/details/ggxawhmkm.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.fehbvm.com/Article/details/gunqkxbdb.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.hesvh.cn/Article/details/gvzjiocqm.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.zdbjq.cn/Article/details/gortbsscq.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.hesvh.cn/Article/details/gohatrvnb.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.hesvh.cn/Article/details/gprohijar.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gryhmdnal.sHtML

[G10] 访问控制
来源：http://www.blog.zdbjq.cn/Article/details/giltwfdmu.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.hesvh.cn/Article/details/gmivzbibd.sHtML

PHP:  public / protected / private
来源：http://mobile.zdbjq.cn/Article/details/gczqetggj.sHtML

JS:   #private 字段；其余公开
来源：http://baike.fehbvm.com/Article/details/gjvyeltse.sHtML

TS:   public / protected / private
来源：http://www.m.share.zdbjq.cn/Article/details/gbwhghkzh.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.hesvh.cn/Article/details/gfkjoijhx.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.zdbjq.cn/Article/details/gkpifbpie.sHtML

Ruby: public / protected / private
来源：http://www.share.hesvh.cn/Article/details/gfqsubsig.sHtML

C#:   public / protected / private / internal
来源：http://baike.hesvh.cn/Article/details/gcekafspx.sHtML

[G11] getter / setter
来源：http://read.share.fehbvm.com/Article/details/gsttjoprc.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.fehbvm.com/Article/details/ggsqtglcm.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.zdbjq.cn/Article/details/gepdmbruz.sHtML

JS:   get name() { return this._name; }
来源：http://baike.zdbjq.cn/Article/details/gjlsgxbuz.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.hesvh.cn/Article/details/gzdhmedwd.sHtML

Java: public String getName() { return name; }
来源：http://baike.hesvh.cn/Article/details/glllpmtpv.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.hesvh.cn/Article/details/gjlfimzch.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.zdbjq.cn/Article/details/graigjkln.sHtML

C#:   public string Name { get; set; }
来源：http://blog.hesvh.cn/Article/details/gkdnikyxm.sHtML

[G12] 对象转字符串
来源：http://www.m.share.hesvh.cn/Article/details/gxlqagalp.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.fehbvm.com/Article/details/gsuvzxnwc.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.hesvh.cn/Article/details/grxzlwgdl.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/gqeqvsjnt.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/gfshjkgtk.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.hesvh.cn/Article/details/gfilyaqnh.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.fehbvm.com/Article/details/gwhrdfcjs.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.hesvh.cn/Article/details/gnkvoplrs.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.hesvh.cn/Article/details/gcfovcrti.sHtML

[G13] 判断对象类型
来源：http://m.share.zdbjq.cn/Article/details/gqyzuviuj.sHtML

Py:   isinstance(u, User)
来源：http://mobile.hesvh.cn/Article/details/gmkxpehbo.sHtML

PHP:  $u instanceof User
来源：http://read.share.fehbvm.com/Article/details/glsjbleqv.sHtML

JS:   u instanceof User
来源：http://wap.fehbvm.com/Article/details/goovbqdps.sHtML

TS:   u instanceof User
来源：http://blog.hesvh.cn/Article/details/gkuteyjuq.sHtML

Java: u instanceof User
来源：http://read.share.hesvh.cn/Article/details/gtyturkgq.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.zdbjq.cn/Article/details/gwfyayvma.sHtML

Ruby: u.is_a?(User)
来源：http://baike.zdbjq.cn/Article/details/gopzheeze.sHtML

C#:   u is User
来源：http://m.share.hesvh.cn/Article/details/geaexinne.sHtML

[G14] 数据类 / record
来源：http://mobile.fehbvm.com/Article/details/gwhnctkxd.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.fehbvm.com/Article/details/gpofpwinu.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.zdbjq.cn/Article/details/gnupucjyu.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.zdbjq.cn/Article/details/gjtwrqsks.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.fehbvm.com/Article/details/gfsjgzjcc.sHtML

Java: record User(String name, int age) {}
来源：http://wap.hesvh.cn/Article/details/gykalbcui.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.zdbjq.cn/Article/details/gbqxmryvm.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.zdbjq.cn/Article/details/gydouveqk.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.zdbjq.cn/Article/details/gmmkqdjvx.sHtML

[G15] 枚举
来源：http://m.share.fehbvm.com/Article/details/gdynphupq.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.fehbvm.com/Article/details/gxrxatlvg.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.m.share.fehbvm.com/Article/details/gionhwcfx.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://read.share.zdbjq.cn/Article/details/gclppuclf.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.fehbvm.com/Article/details/ggrdgajsa.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.zdbjq.cn/Article/details/goiuyibkw.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.hesvh.cn/Article/details/gxcqluptg.sHtML

Ruby: Color = %i[red green].freeze
来源：http://m.share.fehbvm.com/Article/details/gzkqdxnqr.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.hesvh.cn/Article/details/grcycujvh.sHtML

[G16] 对象转数组 / 字典
来源：http://wap.hesvh.cn/Article/details/gfdwfrvjk.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://3g.zdbjq.cn/Article/details/gnbaznmkt.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.hesvh.cn/Article/details/gvoycqcjd.sHtML

JS:   Object.entries(obj)
来源：http://m.share.fehbvm.com/Article/details/gtldjmgut.sHtML

TS:   Object.entries(obj)
来源：http://read.share.zdbjq.cn/Article/details/gmuubllvu.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.fehbvm.com/Article/details/gvqfgsiys.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://wap.hesvh.cn/Article/details/gnthwospm.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.hesvh.cn/Article/details/gqnmxlocy.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.fehbvm.com/Article/details/geagwvazd.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gnhwyilfr.sHtML

H. 异常与错误处理
来源：http://mobile.zdbjq.cn/Article/details/gpofnhcix.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gmqmcimqq.sHtML

[H01] try / catch 基础
来源：http://read.share.hesvh.cn/Article/details/ghxcvupkv.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.fehbvm.com/Article/details/gesdwkgue.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.hesvh.cn/Article/details/gkmrukqrz.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.zdbjq.cn/Article/details/glvwjvrmr.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.share.fehbvm.com/Article/details/gyacrftyy.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.fehbvm.com/Article/details/gfjvswfae.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://baike.fehbvm.com/Article/details/gxovfegyw.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.hesvh.cn/Article/details/glboklmqf.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://3g.hesvh.cn/Article/details/gxfkxugkl.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.zdbjq.cn/Article/details/gpcxfcfvu.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://mobile.hesvh.cn/Article/details/gjrjuzogy.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.zdbjq.cn/Article/details/gpruxvnwp.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://m.share.fehbvm.com/Article/details/gukppgiwc.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gvwrwgfkj.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://mobile.fehbvm.com/Article/details/goscdjpll.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://read.share.hesvh.cn/Article/details/gkdiuktsy.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.m.share.fehbvm.com/Article/details/gigabrvka.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://3g.fehbvm.com/Article/details/gjrxnwute.sHtML

[H03] 主动抛出异常
来源：http://baike.hesvh.cn/Article/details/gypbunpen.sHtML

Py:   raise ValueError("错误信息")
来源：http://read.share.hesvh.cn/Article/details/gnblgfoax.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.fehbvm.com/Article/details/gdlxomwfv.sHtML

JS:   throw new Error("错误信息");
来源：http://www.share.fehbvm.com/Article/details/gvhgdpxbo.sHtML

TS:   throw new Error("错误信息");
来源：http://baike.fehbvm.com/Article/details/gcjlsiins.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.fehbvm.com/Article/details/gnityzjir.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.blog.zdbjq.cn/Article/details/gyuajbszm.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.blog.fehbvm.com/Article/details/gvrdzdtuf.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.blog.hesvh.cn/Article/details/grrseyetd.sHtML

[H04] 自定义异常类型
来源：http://www.m.share.fehbvm.com/Article/details/gdvrkxovy.sHtML

Py:   class MyError(Exception): pass
来源：http://m.share.fehbvm.com/Article/details/gfzgipuqk.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://read.share.hesvh.cn/Article/details/gulspbsqt.sHtML

JS:   class MyError extends Error {}
来源：http://baike.hesvh.cn/Article/details/gkpsnndfx.sHtML

TS:   class MyError extends Error {}
来源：http://www.share.hesvh.cn/Article/details/gxxikumxw.sHtML

Java: class MyException extends RuntimeException {}
来源：http://wap.hesvh.cn/Article/details/gvtqdlcec.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.blog.fehbvm.com/Article/details/gmkimfqty.sHtML

Ruby: class MyError < StandardError; end
来源：http://mobile.hesvh.cn/Article/details/gazzdvqvb.sHtML

C#:   class MyException : Exception {}
来源：http://mobile.fehbvm.com/Article/details/gldrzvgwe.sHtML

[H05] 捕获特定类型
来源：http://baike.hesvh.cn/Article/details/gmzbicvie.sHtML

Py:   except ValueError as e:
来源：http://wap.fehbvm.com/Article/details/gjrebnmbe.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://3g.fehbvm.com/Article/details/gxxdxnbew.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://read.share.hesvh.cn/Article/details/gnsutklgd.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://wap.zdbjq.cn/Article/details/gidcnzqaf.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://3g.fehbvm.com/Article/details/grzlptuyh.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mobile.hesvh.cn/Article/details/goqopraww.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.m.share.zdbjq.cn/Article/details/gnrpjyyuy.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://3g.fehbvm.com/Article/details/ganrrmyej.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.zdbjq.cn/Article/details/grqdmvqdz.sHtML

Py:   value = d.get("k") or default
来源：http://wap.fehbvm.com/Article/details/gjlacrjpp.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://blog.fehbvm.com/Article/details/gafoewnzi.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://read.share.zdbjq.cn/Article/details/gmdeehyjg.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://baike.hesvh.cn/Article/details/goefbqjsf.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wap.zdbjq.cn/Article/details/gsyfvlqhq.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://3g.fehbvm.com/Article/details/gpnuzfmma.sHtML

Ruby: d&.dig(:a, :b)
来源：http://baike.zdbjq.cn/Article/details/ghweuwtqz.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.share.fehbvm.com/Article/details/gcczbmrpj.sHtML

[H07] 断言
来源：http://m.share.hesvh.cn/Article/details/gftmvagmx.sHtML

Py:   assert x > 0, "必须为正"
来源：http://3g.hesvh.cn/Article/details/gaymzotvw.sHtML

PHP:  assert($x > 0);
来源：http://www.share.zdbjq.cn/Article/details/gstjgjfxc.sHtML

JS:   console.assert(x > 0);
来源：http://m.share.zdbjq.cn/Article/details/gqzsrpkxc.sHtML

TS:   console.assert(x > 0);
来源：http://www.share.fehbvm.com/Article/details/gnlmttpbu.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.blog.zdbjq.cn/Article/details/gvykjnmid.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.m.share.zdbjq.cn/Article/details/gjoajuqfq.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.m.share.hesvh.cn/Article/details/gpwtiiqyc.sHtML

C#:   Debug.Assert(x > 0);
来源：http://mobile.zdbjq.cn/Article/details/grlrnjpps.sHtML

[H08] 获取错误信息与堆栈
来源：http://3g.fehbvm.com/Article/details/guaandunz.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://wap.hesvh.cn/Article/details/ghmxrrxiz.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wap.zdbjq.cn/Article/details/gbkvmbkhx.sHtML

JS:   e.message;  e.stack
来源：http://wap.zdbjq.cn/Article/details/gdrnofqvh.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://m.share.zdbjq.cn/Article/details/gxcoulcmn.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://baike.hesvh.cn/Article/details/gwfsgvvpy.sHtML

Go:   err.Error()
来源：http://www.m.share.zdbjq.cn/Article/details/goapatvdr.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.m.share.hesvh.cn/Article/details/gfagipcog.sHtML

C#:   e.Message;  e.StackTrace
来源：http://read.share.hesvh.cn/Article/details/gxfllaqyd.sHtML

[H09] 带错误码的异常
来源：http://read.share.zdbjq.cn/Article/details/goomlnacv.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.share.hesvh.cn/Article/details/ggcqobnro.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.blog.fehbvm.com/Article/details/gigkrahdc.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.share.fehbvm.com/Article/details/gementffm.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://baike.zdbjq.cn/Article/details/gaskddbwq.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://blog.hesvh.cn/Article/details/gqogeodub.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mobile.fehbvm.com/Article/details/gxxmelxbi.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://mobile.hesvh.cn/Article/details/gertybstm.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://read.share.hesvh.cn/Article/details/gkkktjdrk.sHtML

[H10] 资源自动释放
来源：http://m.share.fehbvm.com/Article/details/gglubuwdd.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://m.share.hesvh.cn/Article/details/gidevckcz.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://read.share.hesvh.cn/Article/details/ggtnnwaqo.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.zdbjq.cn/Article/details/gvvjotpii.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.fehbvm.com/Article/details/gvwopmgoe.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://m.share.hesvh.cn/Article/details/gqfukrudw.sHtML

Go:   defer f.Close()
来源：http://mobile.zdbjq.cn/Article/details/gjjpqvvir.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://m.share.fehbvm.com/Article/details/guujxfouj.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gmubvphwf.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gvtnpaozf.sHtML

I. 正则表达式
来源：http://wap.zdbjq.cn/Article/details/gvogkouos.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gbggdknyw.sHtML

[I01] 判断是否匹配
来源：http://baike.fehbvm.com/Article/details/gojzmnfgo.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://m.share.zdbjq.cn/Article/details/ggxjitxkw.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://mobile.zdbjq.cn/Article/details/gxkvijvjm.sHtML

JS:   /\d+/.test(s)
来源：http://www.blog.hesvh.cn/Article/details/gmvbhaklx.sHtML

TS:   /\d+/.test(s)
来源：http://3g.fehbvm.com/Article/details/glciacohp.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.m.share.fehbvm.com/Article/details/ginxnbkkd.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://3g.hesvh.cn/Article/details/gttralwqp.sHtML

Ruby: s.match?(/\d+/)
来源：http://baike.hesvh.cn/Article/details/gcwlmjilg.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wap.zdbjq.cn/Article/details/gftbwmtie.sHtML

[I02] 提取所有匹配
来源：http://mobile.hesvh.cn/Article/details/gryhkizmr.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.share.fehbvm.com/Article/details/gqngdgwkr.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.share.fehbvm.com/Article/details/gfgznhheq.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.m.share.zdbjq.cn/Article/details/gekkxqqon.sHtML

TS:   s.match(/\d+/g)
来源：http://baike.fehbvm.com/Article/details/gjopjjctp.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.blog.zdbjq.cn/Article/details/gebzcchnd.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mobile.hesvh.cn/Article/details/gxxvauekj.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.blog.hesvh.cn/Article/details/gfwzzifjz.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wap.fehbvm.com/Article/details/gvloxfwbq.sHtML

[I03] 提取捕获分组
来源：http://read.share.hesvh.cn/Article/details/gfnuxdsrv.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mobile.zdbjq.cn/Article/details/ghgjnrxqf.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.m.share.hesvh.cn/Article/details/glralrgdw.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://read.share.zdbjq.cn/Article/details/gfnugqgxs.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.blog.hesvh.cn/Article/details/gemxcpege.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://baike.fehbvm.com/Article/details/ghhowbnue.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://blog.fehbvm.com/Article/details/gwohgqjcx.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://m.share.hesvh.cn/Article/details/gnzrcmvks.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.share.hesvh.cn/Article/details/gbbrqwrqn.sHtML

[I04] 正则替换
来源：http://www.m.share.fehbvm.com/Article/details/gyatimoou.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://blog.zdbjq.cn/Article/details/grwuqfobs.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.hesvh.cn/Article/details/gvwppxmmv.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://read.share.zdbjq.cn/Article/details/gnrciapaw.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.share.hesvh.cn/Article/details/gzhlentlp.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.m.share.hesvh.cn/Article/details/ghulgazka.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://read.share.zdbjq.cn/Article/details/gnrfozatd.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://3g.hesvh.cn/Article/details/ghpkbafty.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.m.share.fehbvm.com/Article/details/garhugpyw.sHtML

[I05] 按正则拆分
来源：http://read.share.fehbvm.com/Article/details/gvpshmkdo.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.m.share.zdbjq.cn/Article/details/gquqgihvp.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.m.share.hesvh.cn/Article/details/gdfeujqvi.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://m.share.hesvh.cn/Article/details/gpkbalszk.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://read.share.fehbvm.com/Article/details/gwinqptlz.sHtML

Java: s.split("\\s*,\\s*")
来源：http://read.share.fehbvm.com/Article/details/ghjbpgmzx.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://blog.fehbvm.com/Article/details/ggwpvvtdt.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.share.zdbjq.cn/Article/details/gckctaktn.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://3g.hesvh.cn/Article/details/gxoflopbf.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://blog.zdbjq.cn/Article/details/gwsqllwqh.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://blog.hesvh.cn/Article/details/gfljagmci.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.blog.zdbjq.cn/Article/details/gdduphcsl.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.zdbjq.cn/Article/details/gsblsanoc.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.hesvh.cn/Article/details/gqfqquxtz.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.blog.hesvh.cn/Article/details/gdgnhwpmr.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://3g.fehbvm.com/Article/details/gchqavpgq.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.share.fehbvm.com/Article/details/gorvjvddd.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://read.share.hesvh.cn/Article/details/gcyamfbgz.sHtML

[I07] 忽略大小写与多行模式
来源：http://mobile.fehbvm.com/Article/details/gcqejhmnk.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://m.share.fehbvm.com/Article/details/gflqlmzhv.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.share.fehbvm.com/Article/details/ghiilnfpm.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.share.zdbjq.cn/Article/details/goqnebxqz.sHtML

TS:   /error/gim
来源：http://m.share.hesvh.cn/Article/details/gctyfbjbs.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.blog.fehbvm.com/Article/details/gncnuhruy.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.m.share.zdbjq.cn/Article/details/gperilmey.sHtML

Ruby: s.scan(/error/i)
来源：http://blog.zdbjq.cn/Article/details/gndgqvftd.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://baike.fehbvm.com/Article/details/geewyiuqi.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.blog.zdbjq.cn/Article/details/gkyoptrli.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wap.fehbvm.com/Article/details/griajodfp.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://blog.fehbvm.com/Article/details/gztfxwofs.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.hesvh.cn/Article/details/grdwoqwbj.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.fehbvm.com/Article/details/gchlscxev.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.m.share.hesvh.cn/Article/details/gkmhbefqc.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.m.share.zdbjq.cn/Article/details/gwyxbhfgm.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://read.share.hesvh.cn/Article/details/gcqgjigzi.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://m.share.fehbvm.com/Article/details/guklmmwmj.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gsbjlndwx.sHtML

J. 日期与时间
来源：http://mobile.hesvh.cn/Article/details/gxqiedizc.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gxynbnnkk.sHtML

[J01] 获取当前时间
来源：http://m.share.fehbvm.com/Article/details/gpibxjore.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://baike.hesvh.cn/Article/details/gnabhxgmi.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://3g.fehbvm.com/Article/details/gbcsfgxqf.sHtML

JS:   new Date();  Date.now()
来源：http://3g.hesvh.cn/Article/details/gskqdbdih.sHtML

TS:   new Date();  Date.now()
来源：http://www.blog.zdbjq.cn/Article/details/gfwwwwyjm.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://mobile.hesvh.cn/Article/details/gcycwsrnt.sHtML

Go:   time.Now()
来源：http://blog.zdbjq.cn/Article/details/gtmtoslbd.sHtML

Ruby: Time.now
来源：http://baike.hesvh.cn/Article/details/gthucimux.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://read.share.hesvh.cn/Article/details/gtmrwsgei.sHtML

[J02] 格式化输出
来源：http://www.share.fehbvm.com/Article/details/gjrfxkqdq.sHtML


<!-- 参考信息 -->