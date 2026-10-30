代发 wailian999

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.hesvh.cn/Article/details/ggatpfzki.sHtML

JS:   greet() { return this.name; }
来源：http://baike.hesvh.cn/Article/details/gpmplfqap.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gvsrcdbhk.sHtML

Java: String greet() { return name; }
来源：http://mobile.hesvh.cn/Article/details/gaemtwtgd.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.zdbjq.cn/Article/details/gegxfvaio.sHtML

Ruby: def greet; @name; end
来源：http://read.share.fehbvm.com/Article/details/gjfsxgcvz.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.hesvh.cn/Article/details/gczzjtxtg.sHtML

[G05] 继承
来源：http://www.blog.zdbjq.cn/Article/details/gkluyafgl.sHtML

Py:   class Admin(User): pass
来源：http://blog.zdbjq.cn/Article/details/gvjtmhqep.sHtML

PHP:  class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/gdrjvpaki.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/gpwmpqbwq.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/gmhguhatj.sHtML

Java: class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/gujqtgccy.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.fehbvm.com/Article/details/gnjlqttkb.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.zdbjq.cn/Article/details/gezxilgtj.sHtML

C#:   class Admin : User {}
来源：http://baike.fehbvm.com/Article/details/grkorhnlw.sHtML

[G06] 重写方法
来源：http://baike.hesvh.cn/Article/details/gggpxaqhh.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.fehbvm.com/Article/details/gjveyplgq.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/gaapuzkui.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/gpybzqzlu.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gystgfbms.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/gzxmaviht.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.zdbjq.cn/Article/details/ggypldnbo.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.fehbvm.com/Article/details/gorhuokuq.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.hesvh.cn/Article/details/gxapgnyup.sHtML

[G07] 调用父类方法
来源：http://www.blog.hesvh.cn/Article/details/gjsnftvvw.sHtML

Py:   super().greet()
来源：http://www.share.fehbvm.com/Article/details/ghvgjlznx.sHtML

PHP:  parent::greet();
来源：http://baike.hesvh.cn/Article/details/gebmnbryx.sHtML

JS:   super.greet();
来源：http://wap.hesvh.cn/Article/details/gyystnhuk.sHtML

TS:   super.greet();
来源：http://www.blog.zdbjq.cn/Article/details/gvjbzbavy.sHtML

Java: super.greet();
来源：http://www.m.share.hesvh.cn/Article/details/gzdrcconz.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.hesvh.cn/Article/details/gkobyjqlc.sHtML

Ruby: super
来源：http://3g.fehbvm.com/Article/details/ghtlzuveg.sHtML

C#:   base.Greet();
来源：http://www.blog.zdbjq.cn/Article/details/ghqonkguu.sHtML

[G08] 静态方法与属性
来源：http://read.share.fehbvm.com/Article/details/gwwaggyvf.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.zdbjq.cn/Article/details/gdcelvypa.sHtML

PHP:  public static function f() {}
来源：http://blog.hesvh.cn/Article/details/grgxxvrwx.sHtML

JS:   static f() {}
来源：http://3g.hesvh.cn/Article/details/gwztqiyjs.sHtML

TS:   static f(): void {}
来源：http://www.blog.hesvh.cn/Article/details/gwpkqtlrl.sHtML

Java: static void f() {}
来源：http://blog.fehbvm.com/Article/details/gcepjibeo.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.zdbjq.cn/Article/details/gdjxmzrsl.sHtML

Ruby: def self.f; end
来源：http://www.m.share.fehbvm.com/Article/details/gtxdajspk.sHtML

C#:   public static void F() {}
来源：http://www.m.share.fehbvm.com/Article/details/gshefknwz.sHtML

[G09] 接口 / 抽象类
来源：http://wap.zdbjq.cn/Article/details/gldjcetkf.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.fehbvm.com/Article/details/grqhhswoj.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.zdbjq.cn/Article/details/gsyadejog.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.zdbjq.cn/Article/details/gzvjafaif.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.fehbvm.com/Article/details/gzxbginpg.sHtML

Java: interface Shape { double area(); }
来源：http://blog.zdbjq.cn/Article/details/gdmafteeq.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.fehbvm.com/Article/details/gwiqrrbjo.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.fehbvm.com/Article/details/gwdrkaqee.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.fehbvm.com/Article/details/gytpuvoje.sHtML

[G10] 访问控制
来源：http://3g.zdbjq.cn/Article/details/gxgccswdg.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.zdbjq.cn/Article/details/gubrbisch.sHtML

PHP:  public / protected / private
来源：http://baike.zdbjq.cn/Article/details/gfoyxvsbm.sHtML

JS:   #private 字段；其余公开
来源：http://baike.hesvh.cn/Article/details/gkowglvcc.sHtML

TS:   public / protected / private
来源：http://3g.fehbvm.com/Article/details/gnemkdbtk.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.zdbjq.cn/Article/details/gpepdczlg.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.hesvh.cn/Article/details/gbzebwxbm.sHtML

Ruby: public / protected / private
来源：http://mobile.fehbvm.com/Article/details/gshykbern.sHtML

C#:   public / protected / private / internal
来源：http://read.share.hesvh.cn/Article/details/gwsmohlzo.sHtML

[G11] getter / setter
来源：http://read.share.fehbvm.com/Article/details/ghuzngtvw.sHtML

Py:   @property 与 @x.setter
来源：http://blog.zdbjq.cn/Article/details/gtthoiivt.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.zdbjq.cn/Article/details/gaqauqnco.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gmglrisyl.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.zdbjq.cn/Article/details/grdockzmn.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.hesvh.cn/Article/details/gfdolvirt.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.zdbjq.cn/Article/details/gvmvbdyew.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.fehbvm.com/Article/details/gaiseepai.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.zdbjq.cn/Article/details/grgnleoxt.sHtML

[G12] 对象转字符串
来源：http://m.share.hesvh.cn/Article/details/gmkteqvnn.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.zdbjq.cn/Article/details/gjkeztrqu.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.hesvh.cn/Article/details/ggwmegcdc.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gqxxzubnf.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gumrcoxfw.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.zdbjq.cn/Article/details/grdofehmr.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.hesvh.cn/Article/details/gumxspvng.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.hesvh.cn/Article/details/gqasstvcz.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.hesvh.cn/Article/details/gtbjkrdei.sHtML

[G13] 判断对象类型
来源：http://www.m.share.hesvh.cn/Article/details/gkqtbwyos.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.hesvh.cn/Article/details/gvyshkjch.sHtML

PHP:  $u instanceof User
来源：http://mobile.fehbvm.com/Article/details/gnsghpohe.sHtML

JS:   u instanceof User
来源：http://wap.hesvh.cn/Article/details/gfkmphjuh.sHtML

TS:   u instanceof User
来源：http://3g.fehbvm.com/Article/details/gejatpehm.sHtML

Java: u instanceof User
来源：http://wap.zdbjq.cn/Article/details/gmdsxzwcj.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.fehbvm.com/Article/details/gizxbrmsh.sHtML

Ruby: u.is_a?(User)
来源：http://blog.fehbvm.com/Article/details/ggvprxxbw.sHtML

C#:   u is User
来源：http://baike.fehbvm.com/Article/details/gjtxktokv.sHtML

[G14] 数据类 / record
来源：http://www.blog.hesvh.cn/Article/details/goycqbyge.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.hesvh.cn/Article/details/gtigvgdyp.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.zdbjq.cn/Article/details/gqjyfwtql.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.fehbvm.com/Article/details/gbmnbxhed.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.zdbjq.cn/Article/details/ggalxsugy.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.fehbvm.com/Article/details/gxbopkbjt.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.hesvh.cn/Article/details/gadvpxkcb.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.zdbjq.cn/Article/details/ghskvmcof.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.hesvh.cn/Article/details/geosxogtp.sHtML

[G15] 枚举
来源：http://3g.fehbvm.com/Article/details/gdmuwjydd.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.zdbjq.cn/Article/details/ggdzeoawo.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.zdbjq.cn/Article/details/gsshnbnys.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.m.share.hesvh.cn/Article/details/geogfirtu.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.hesvh.cn/Article/details/glnzbumcv.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.fehbvm.com/Article/details/gpfdehggh.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.fehbvm.com/Article/details/gvqmnwuex.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.hesvh.cn/Article/details/gdursqdcl.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.hesvh.cn/Article/details/gscuoyite.sHtML

[G16] 对象转数组 / 字典
来源：http://wap.hesvh.cn/Article/details/gryshonba.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.fehbvm.com/Article/details/gkayyrwju.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.fehbvm.com/Article/details/gezomucxy.sHtML

JS:   Object.entries(obj)
来源：http://www.share.hesvh.cn/Article/details/gpogtssax.sHtML

TS:   Object.entries(obj)
来源：http://3g.hesvh.cn/Article/details/gqyeqhire.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://read.share.fehbvm.com/Article/details/gjagwtuxi.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.hesvh.cn/Article/details/gxvqykcoi.sHtML

Ruby: obj.instance_variables
来源：http://www.m.share.fehbvm.com/Article/details/gkenxdauc.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.m.share.fehbvm.com/Article/details/gmovshrtb.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gddnosvgu.sHtML

H. 异常与错误处理
来源：http://www.blog.hesvh.cn/Article/details/gzvsumobb.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gwgtjgujk.sHtML

[H01] try / catch 基础
来源：http://www.blog.zdbjq.cn/Article/details/grxdtjumi.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.fehbvm.com/Article/details/grvjlokou.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.hesvh.cn/Article/details/gbbwdxxtp.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.fehbvm.com/Article/details/gbvhnspha.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.m.share.fehbvm.com/Article/details/gpdsipisq.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.blog.zdbjq.cn/Article/details/glnoyutga.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://blog.fehbvm.com/Article/details/gwfpmwepx.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.zdbjq.cn/Article/details/gledrdklo.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.hesvh.cn/Article/details/gsrqjadxj.sHtML

[H02] finally / ensure 收尾
来源：http://www.m.share.zdbjq.cn/Article/details/gqciuotif.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.fehbvm.com/Article/details/gujneyurx.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/ggtncuovd.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://3g.fehbvm.com/Article/details/gvhjqiyze.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://blog.fehbvm.com/Article/details/gegivxigr.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.hesvh.cn/Article/details/gyfidczyi.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://read.share.zdbjq.cn/Article/details/gunzywcuw.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.hesvh.cn/Article/details/gexmxjhpz.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/grevbdtlh.sHtML

[H03] 主动抛出异常
来源：http://m.share.hesvh.cn/Article/details/gewvnjimc.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.m.share.zdbjq.cn/Article/details/gqskmwfux.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.zdbjq.cn/Article/details/gqnewqilp.sHtML

JS:   throw new Error("错误信息");
来源：http://wap.fehbvm.com/Article/details/gygjjsxho.sHtML

TS:   throw new Error("错误信息");
来源：http://www.m.share.zdbjq.cn/Article/details/gjkoavxjq.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://m.share.hesvh.cn/Article/details/gmwfxglpo.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://baike.hesvh.cn/Article/details/gevgxkdzu.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://mobile.zdbjq.cn/Article/details/gacjqifwm.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://wap.hesvh.cn/Article/details/gjeoavuhj.sHtML

[H04] 自定义异常类型
来源：http://3g.zdbjq.cn/Article/details/gompltwqf.sHtML

Py:   class MyError(Exception): pass
来源：http://blog.zdbjq.cn/Article/details/gelalwfyf.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://wap.fehbvm.com/Article/details/gqjyyrqao.sHtML

JS:   class MyError extends Error {}
来源：http://3g.hesvh.cn/Article/details/gfedbxsuz.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.fehbvm.com/Article/details/ghpoqpxtr.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.hesvh.cn/Article/details/gwlzikdvy.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.blog.hesvh.cn/Article/details/gdmsrsuup.sHtML

Ruby: class MyError < StandardError; end
来源：http://m.share.fehbvm.com/Article/details/guvstuimn.sHtML

C#:   class MyException : Exception {}
来源：http://mobile.zdbjq.cn/Article/details/gqeaqoxsq.sHtML

[H05] 捕获特定类型
来源：http://m.share.zdbjq.cn/Article/details/gplajybpv.sHtML

Py:   except ValueError as e:
来源：http://baike.zdbjq.cn/Article/details/ggkdhkwvf.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.hesvh.cn/Article/details/gcwchlgmu.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.m.share.fehbvm.com/Article/details/gzcjchxgj.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://mobile.hesvh.cn/Article/details/gjowtrdzz.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://m.share.hesvh.cn/Article/details/glsjquqoc.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://3g.fehbvm.com/Article/details/gscwfjedr.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.share.hesvh.cn/Article/details/gghjvtzzb.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://read.share.fehbvm.com/Article/details/gxdkqytls.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.zdbjq.cn/Article/details/gdxoaqoye.sHtML

Py:   value = d.get("k") or default
来源：http://www.blog.hesvh.cn/Article/details/gatyhizfg.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://3g.fehbvm.com/Article/details/gaqzzaeak.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://mobile.fehbvm.com/Article/details/gzyneggkk.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.hesvh.cn/Article/details/gntirnfjc.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://read.share.hesvh.cn/Article/details/gkceqwpxx.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.m.share.zdbjq.cn/Article/details/gvqjearbd.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.share.hesvh.cn/Article/details/gdebrormd.sHtML

C#:   obj?.A?.B ?? default
来源：http://read.share.fehbvm.com/Article/details/ghlqsgxcb.sHtML

[H07] 断言
来源：http://www.m.share.fehbvm.com/Article/details/gdcfqzreb.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.blog.hesvh.cn/Article/details/gnvubqgda.sHtML

PHP:  assert($x > 0);
来源：http://www.share.hesvh.cn/Article/details/gnwgmonja.sHtML

JS:   console.assert(x > 0);
来源：http://wap.zdbjq.cn/Article/details/gsnmwgqvh.sHtML

TS:   console.assert(x > 0);
来源：http://blog.zdbjq.cn/Article/details/gsqfbsufs.sHtML

Java: assert x > 0 : "必须为正";
来源：http://mobile.hesvh.cn/Article/details/gcbvtzxfk.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://baike.zdbjq.cn/Article/details/gdrbaxsfx.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.blog.fehbvm.com/Article/details/gicartgfn.sHtML

C#:   Debug.Assert(x > 0);
来源：http://wap.zdbjq.cn/Article/details/gblytdkko.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.share.zdbjq.cn/Article/details/gcmwkkplx.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://wap.zdbjq.cn/Article/details/gyuneitfl.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://baike.fehbvm.com/Article/details/ggxlfuoby.sHtML

JS:   e.message;  e.stack
来源：http://m.share.hesvh.cn/Article/details/gdxkznoqg.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://wap.hesvh.cn/Article/details/gjfimpgzl.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://baike.fehbvm.com/Article/details/gzkirsujf.sHtML

Go:   err.Error()
来源：http://blog.fehbvm.com/Article/details/gmagdsljf.sHtML

Ruby: e.message;  e.backtrace
来源：http://baike.zdbjq.cn/Article/details/gqpjxeuds.sHtML

C#:   e.Message;  e.StackTrace
来源：http://3g.zdbjq.cn/Article/details/gkxchygmr.sHtML

[H09] 带错误码的异常
来源：http://wap.hesvh.cn/Article/details/ghmlfvefl.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://read.share.zdbjq.cn/Article/details/gfbtaexpw.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://mobile.fehbvm.com/Article/details/glbkmrwvx.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.blog.fehbvm.com/Article/details/gfgtkkjuj.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://read.share.zdbjq.cn/Article/details/gznvzlich.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.m.share.fehbvm.com/Article/details/geveuygnw.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.m.share.fehbvm.com/Article/details/gfcvjfbxk.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://mobile.zdbjq.cn/Article/details/gbigifhmz.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://mobile.zdbjq.cn/Article/details/gqsalkjsl.sHtML

[H10] 资源自动释放
来源：http://mobile.hesvh.cn/Article/details/gsulctmsh.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://mobile.fehbvm.com/Article/details/gopfxfxts.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://baike.fehbvm.com/Article/details/gdurxgejt.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.zdbjq.cn/Article/details/gdtwvvfnk.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.hesvh.cn/Article/details/gvvvarduz.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wap.zdbjq.cn/Article/details/gtahnimkx.sHtML

Go:   defer f.Close()
来源：http://mobile.hesvh.cn/Article/details/gxwyrgqpr.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mobile.fehbvm.com/Article/details/gkhjvaegd.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gnloeqhvz.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gikoimgpz.sHtML

I. 正则表达式
来源：http://blog.fehbvm.com/Article/details/ghkrihtri.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gcbkdjdul.sHtML

[I01] 判断是否匹配
来源：http://www.m.share.fehbvm.com/Article/details/gygaibyvz.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://m.share.hesvh.cn/Article/details/gzyrwdupg.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.blog.zdbjq.cn/Article/details/gboromiuy.sHtML

JS:   /\d+/.test(s)
来源：http://m.share.hesvh.cn/Article/details/ghrntrflb.sHtML

TS:   /\d+/.test(s)
来源：http://www.share.zdbjq.cn/Article/details/gpunaanrk.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.blog.hesvh.cn/Article/details/ghtseozre.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://read.share.zdbjq.cn/Article/details/gmnszqkru.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.m.share.hesvh.cn/Article/details/gvbticymx.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://3g.zdbjq.cn/Article/details/gpnesheup.sHtML

[I02] 提取所有匹配
来源：http://read.share.hesvh.cn/Article/details/gmcxvbfqa.sHtML

Py:   re.findall(r"\d+", s)
来源：http://blog.hesvh.cn/Article/details/ghwdzcdbj.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.blog.zdbjq.cn/Article/details/gywktjjrn.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.share.hesvh.cn/Article/details/gwwclyoyh.sHtML

TS:   s.match(/\d+/g)
来源：http://blog.zdbjq.cn/Article/details/geubccung.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mobile.hesvh.cn/Article/details/gdbbcmdtv.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wap.zdbjq.cn/Article/details/gdhibuxkk.sHtML

Ruby: s.scan(/\d+/)
来源：http://read.share.fehbvm.com/Article/details/gxmmayzvq.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://m.share.zdbjq.cn/Article/details/geyfamnlz.sHtML

[I03] 提取捕获分组
来源：http://read.share.zdbjq.cn/Article/details/gdcfbiqhr.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gwiqhatou.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.m.share.fehbvm.com/Article/details/gcuhiitjl.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://read.share.fehbvm.com/Article/details/gytnjkxfp.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.blog.hesvh.cn/Article/details/gbecssvwd.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://read.share.hesvh.cn/Article/details/gxosquknn.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://m.share.zdbjq.cn/Article/details/gtzxdemlz.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.share.hesvh.cn/Article/details/gjuoqvvpg.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://blog.zdbjq.cn/Article/details/glrjacjrt.sHtML

[I04] 正则替换
来源：http://read.share.zdbjq.cn/Article/details/glnheffys.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://mobile.hesvh.cn/Article/details/gbjovdnxg.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wap.zdbjq.cn/Article/details/gwjxbwksv.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://m.share.hesvh.cn/Article/details/gixlnvums.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.blog.fehbvm.com/Article/details/gggawwtcw.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://mobile.zdbjq.cn/Article/details/gnfneqcyh.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.m.share.hesvh.cn/Article/details/gqrfdohvk.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.blog.hesvh.cn/Article/details/gvucprnje.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.m.share.zdbjq.cn/Article/details/glxccdqnm.sHtML

[I05] 按正则拆分
来源：http://wap.fehbvm.com/Article/details/gkbqyqyhy.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.share.fehbvm.com/Article/details/gphfpprzx.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.blog.fehbvm.com/Article/details/gawdfiyzh.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://read.share.fehbvm.com/Article/details/gqtxjsoct.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://baike.hesvh.cn/Article/details/gicqwjeuf.sHtML

Java: s.split("\\s*,\\s*")
来源：http://baike.fehbvm.com/Article/details/ghfhdudfr.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://mobile.hesvh.cn/Article/details/genyvarnx.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://blog.zdbjq.cn/Article/details/gxcdsegbx.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://baike.fehbvm.com/Article/details/gjgsqlouq.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://3g.zdbjq.cn/Article/details/ghxgjakep.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://baike.zdbjq.cn/Article/details/gjfmaluma.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.m.share.fehbvm.com/Article/details/gtamtfdky.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.fehbvm.com/Article/details/gmauqrtdq.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.zdbjq.cn/Article/details/grhtlpclt.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://m.share.hesvh.cn/Article/details/gguyyfbqt.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://baike.hesvh.cn/Article/details/gbeeantjb.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.m.share.fehbvm.com/Article/details/gvlyalswn.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.share.hesvh.cn/Article/details/gwwaherlg.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.m.share.hesvh.cn/Article/details/gtkfjvxvg.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://read.share.fehbvm.com/Article/details/gtcbryycw.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wap.zdbjq.cn/Article/details/griyfdizu.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wap.zdbjq.cn/Article/details/gmbkttboq.sHtML

TS:   /error/gim
来源：http://blog.zdbjq.cn/Article/details/gbghwesus.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://baike.hesvh.cn/Article/details/gxkgcvtjh.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.m.share.zdbjq.cn/Article/details/glgdamhvw.sHtML

Ruby: s.scan(/error/i)
来源：http://mobile.fehbvm.com/Article/details/gkemiyejm.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.share.hesvh.cn/Article/details/gidlwudrs.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://blog.zdbjq.cn/Article/details/glpfhszmk.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://blog.fehbvm.com/Article/details/ghycuxqhw.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.blog.fehbvm.com/Article/details/gftlsgboc.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.fehbvm.com/Article/details/gotidrvpy.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.fehbvm.com/Article/details/govhlneqb.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://baike.zdbjq.cn/Article/details/gqzxseocz.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wap.hesvh.cn/Article/details/gxjiawgrg.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.m.share.fehbvm.com/Article/details/gilvrnbxy.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wap.fehbvm.com/Article/details/giqivlmst.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/ggstwgcao.sHtML

J. 日期与时间
来源：http://m.share.hesvh.cn/Article/details/gdwrabvgq.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gfkexvbih.sHtML

[J01] 获取当前时间
来源：http://www.blog.fehbvm.com/Article/details/gmyukyohx.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://read.share.zdbjq.cn/Article/details/gzqvjyoky.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://3g.zdbjq.cn/Article/details/gqiuprkdq.sHtML

JS:   new Date();  Date.now()
来源：http://www.m.share.zdbjq.cn/Article/details/gjvgrzqlo.sHtML

TS:   new Date();  Date.now()
来源：http://www.blog.zdbjq.cn/Article/details/gdsepshjp.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://mobile.fehbvm.com/Article/details/gvwtlqvmk.sHtML

Go:   time.Now()
来源：http://www.share.zdbjq.cn/Article/details/guizcupzn.sHtML

Ruby: Time.now
来源：http://www.share.fehbvm.com/Article/details/gccgssvqz.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.blog.zdbjq.cn/Article/details/goutaonsq.sHtML

[J02] 格式化输出
来源：http://m.share.hesvh.cn/Article/details/gornslbvd.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.hesvh.cn/Article/details/gvzewwwpg.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.m.share.hesvh.cn/Article/details/gqayykvka.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mobile.fehbvm.com/Article/details/gpwfkbgbl.sHtML

TS:   d.toISOString()
来源：http://read.share.fehbvm.com/Article/details/gghoxrbta.sHtML


<!-- 参考信息 -->