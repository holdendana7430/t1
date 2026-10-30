代发 wailian999

Py:   class Admin(User): pass
来源：http://read.share.fehbvm.com/Article/details/gxappjthg.sHtML

PHP:  class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/gopggsmnq.sHtML

JS:   class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/guosfhzbf.sHtML

TS:   class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/gfrzplexu.sHtML

Java: class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/gtkcyjsmb.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.fehbvm.com/Article/details/gjcgckyjj.sHtML

Ruby: class Admin < User; end
来源：http://m.share.fehbvm.com/Article/details/gaogvscuz.sHtML

C#:   class Admin : User {}
来源：http://mobile.zdbjq.cn/Article/details/gqgoeajzv.sHtML

[G06] 重写方法
来源：http://wap.hesvh.cn/Article/details/gwcnkvbvd.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.hesvh.cn/Article/details/gchioiwdt.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/gjyivoftx.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/gouzocmkw.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/gdipdxfva.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/gvyvpqxro.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.zdbjq.cn/Article/details/gpcaycpre.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.zdbjq.cn/Article/details/gwzbzrduj.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.zdbjq.cn/Article/details/gwauteech.sHtML

[G07] 调用父类方法
来源：http://3g.hesvh.cn/Article/details/gxomuwgaz.sHtML

Py:   super().greet()
来源：http://blog.hesvh.cn/Article/details/glfhhhnln.sHtML

PHP:  parent::greet();
来源：http://www.m.share.fehbvm.com/Article/details/gbofieldv.sHtML

JS:   super.greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gkgshqnwz.sHtML

TS:   super.greet();
来源：http://baike.zdbjq.cn/Article/details/gelmvxets.sHtML

Java: super.greet();
来源：http://baike.hesvh.cn/Article/details/gbiahsulx.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.zdbjq.cn/Article/details/goewxnlbs.sHtML

Ruby: super
来源：http://www.share.zdbjq.cn/Article/details/gqwnvsvke.sHtML

C#:   base.Greet();
来源：http://read.share.hesvh.cn/Article/details/gayqffnql.sHtML

[G08] 静态方法与属性
来源：http://baike.zdbjq.cn/Article/details/gjaafagqu.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.fehbvm.com/Article/details/gvqcpdvju.sHtML

PHP:  public static function f() {}
来源：http://www.blog.hesvh.cn/Article/details/ggrbcfnml.sHtML

JS:   static f() {}
来源：http://3g.fehbvm.com/Article/details/gdzzaeefi.sHtML

TS:   static f(): void {}
来源：http://baike.zdbjq.cn/Article/details/gavduzkdy.sHtML

Java: static void f() {}
来源：http://www.blog.zdbjq.cn/Article/details/gaidiayks.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.fehbvm.com/Article/details/gihfihyrm.sHtML

Ruby: def self.f; end
来源：http://mobile.fehbvm.com/Article/details/gawoztjom.sHtML

C#:   public static void F() {}
来源：http://read.share.fehbvm.com/Article/details/gboynbotl.sHtML

[G09] 接口 / 抽象类
来源：http://wap.zdbjq.cn/Article/details/gqovjlefo.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.hesvh.cn/Article/details/gnasyhegb.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.fehbvm.com/Article/details/gzefxatyq.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.zdbjq.cn/Article/details/gpkqwgkam.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.hesvh.cn/Article/details/gxdsnlclz.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.hesvh.cn/Article/details/goyiavrrh.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.hesvh.cn/Article/details/glgldvxsa.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.fehbvm.com/Article/details/gykohbiqb.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.fehbvm.com/Article/details/gwmuvgiao.sHtML

[G10] 访问控制
来源：http://m.share.fehbvm.com/Article/details/gargwsqas.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.hesvh.cn/Article/details/gunguaxsa.sHtML

PHP:  public / protected / private
来源：http://wap.fehbvm.com/Article/details/guazcvulw.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.zdbjq.cn/Article/details/gfygnlecf.sHtML

TS:   public / protected / private
来源：http://read.share.hesvh.cn/Article/details/gowijlubc.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.hesvh.cn/Article/details/gochcdokw.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.zdbjq.cn/Article/details/gcriqwisf.sHtML

Ruby: public / protected / private
来源：http://baike.fehbvm.com/Article/details/gpjumqdsx.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.zdbjq.cn/Article/details/gdwgmcznh.sHtML

[G11] getter / setter
来源：http://www.share.fehbvm.com/Article/details/gwehmutxl.sHtML

Py:   @property 与 @x.setter
来源：http://blog.fehbvm.com/Article/details/gamgdfwco.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.zdbjq.cn/Article/details/gvpmjgexi.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.zdbjq.cn/Article/details/gzadycxxz.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.fehbvm.com/Article/details/ggumtykzu.sHtML

Java: public String getName() { return name; }
来源：http://read.share.fehbvm.com/Article/details/gavehvzhe.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.zdbjq.cn/Article/details/gsorwulpt.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.zdbjq.cn/Article/details/gzsouccyq.sHtML

C#:   public string Name { get; set; }
来源：http://blog.hesvh.cn/Article/details/gwcrbjgmi.sHtML

[G12] 对象转字符串
来源：http://blog.fehbvm.com/Article/details/gxwllloue.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.zdbjq.cn/Article/details/grkklmcyb.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gjqrfouun.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/gpfoelbry.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/gsatbsfek.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.zdbjq.cn/Article/details/ghdwtpzey.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.zdbjq.cn/Article/details/grqufzrhf.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.zdbjq.cn/Article/details/gcvvcvaqo.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.fehbvm.com/Article/details/ggeutbryy.sHtML

[G13] 判断对象类型
来源：http://mobile.hesvh.cn/Article/details/gavptswsg.sHtML

Py:   isinstance(u, User)
来源：http://m.share.hesvh.cn/Article/details/gtfemlgfz.sHtML

PHP:  $u instanceof User
来源：http://blog.hesvh.cn/Article/details/ghcnvbhye.sHtML

JS:   u instanceof User
来源：http://blog.zdbjq.cn/Article/details/gztkncuht.sHtML

TS:   u instanceof User
来源：http://m.share.fehbvm.com/Article/details/gbhqgesef.sHtML

Java: u instanceof User
来源：http://www.share.fehbvm.com/Article/details/gqebyeazm.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.hesvh.cn/Article/details/gfosqofbk.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.zdbjq.cn/Article/details/gdkjxbjwg.sHtML

C#:   u is User
来源：http://3g.hesvh.cn/Article/details/gwkhkszyf.sHtML

[G14] 数据类 / record
来源：http://mobile.fehbvm.com/Article/details/gzzzytrle.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://baike.fehbvm.com/Article/details/guywhxurk.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.fehbvm.com/Article/details/gqhyzxbms.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.fehbvm.com/Article/details/glsgnbokm.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.zdbjq.cn/Article/details/gltdzqste.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.hesvh.cn/Article/details/grqsklujp.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.fehbvm.com/Article/details/gbzhphncz.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.fehbvm.com/Article/details/gpexqmbxg.sHtML

C#:   record User(string Name, int Age);
来源：http://blog.hesvh.cn/Article/details/gnrueencq.sHtML

[G15] 枚举
来源：http://m.share.fehbvm.com/Article/details/garcoqgrw.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.zdbjq.cn/Article/details/gsoxlayaq.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.hesvh.cn/Article/details/gvkkxdofj.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.hesvh.cn/Article/details/gzhguqgjg.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.hesvh.cn/Article/details/gaeatvtdc.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.hesvh.cn/Article/details/gtebqvavz.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.blog.hesvh.cn/Article/details/ghmydocce.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.hesvh.cn/Article/details/grwepyedg.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.fehbvm.com/Article/details/gvyovvpbv.sHtML

[G16] 对象转数组 / 字典
来源：http://m.share.zdbjq.cn/Article/details/giemuctqn.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.fehbvm.com/Article/details/gjtrgbaoz.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.zdbjq.cn/Article/details/gveixtxwr.sHtML

JS:   Object.entries(obj)
来源：http://mobile.fehbvm.com/Article/details/gitnineqo.sHtML

TS:   Object.entries(obj)
来源：http://3g.hesvh.cn/Article/details/grfzmmldt.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.zdbjq.cn/Article/details/gocmvhbpg.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.fehbvm.com/Article/details/gvwrcezrb.sHtML

Ruby: obj.instance_variables
来源：http://www.share.hesvh.cn/Article/details/ghoycvvli.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.blog.fehbvm.com/Article/details/gkjkfnuqi.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gfenmirkc.sHtML

H. 异常与错误处理
来源：http://baike.zdbjq.cn/Article/details/gurgknxpm.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gublbghgq.sHtML

[H01] try / catch 基础
来源：http://3g.hesvh.cn/Article/details/gpdosgdlc.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.fehbvm.com/Article/details/gkswmfaou.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.fehbvm.com/Article/details/grhowwscb.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://blog.fehbvm.com/Article/details/glsyonnhj.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://m.share.hesvh.cn/Article/details/gxsqytsmc.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.zdbjq.cn/Article/details/gxwegmvnl.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://read.share.fehbvm.com/Article/details/gckvnyzdw.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.m.share.hesvh.cn/Article/details/gajplvvpg.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.hesvh.cn/Article/details/gxxrdcsud.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.fehbvm.com/Article/details/gbqiylkee.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.fehbvm.com/Article/details/godasjwun.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://mobile.fehbvm.com/Article/details/gxprrrzet.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.fehbvm.com/Article/details/gyzvdqaur.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.hesvh.cn/Article/details/gahpfahcd.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.hesvh.cn/Article/details/gpattgcdr.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://m.share.hesvh.cn/Article/details/gndutlshq.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.zdbjq.cn/Article/details/gzvvoxlne.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://3g.fehbvm.com/Article/details/gfbnigtyt.sHtML

[H03] 主动抛出异常
来源：http://read.share.zdbjq.cn/Article/details/gxiwheplh.sHtML

Py:   raise ValueError("错误信息")
来源：http://read.share.zdbjq.cn/Article/details/gjdhgqwqb.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.m.share.zdbjq.cn/Article/details/gwcxooofj.sHtML

JS:   throw new Error("错误信息");
来源：http://read.share.fehbvm.com/Article/details/gpkoqjyzc.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.hesvh.cn/Article/details/gvaaueids.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.m.share.hesvh.cn/Article/details/gsbfriuhz.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://3g.hesvh.cn/Article/details/gzvssxkur.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.blog.hesvh.cn/Article/details/gzjpqknac.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.m.share.fehbvm.com/Article/details/gkwnmibtg.sHtML

[H04] 自定义异常类型
来源：http://www.share.zdbjq.cn/Article/details/gcihrjtxg.sHtML

Py:   class MyError(Exception): pass
来源：http://read.share.zdbjq.cn/Article/details/gwowoluux.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://baike.fehbvm.com/Article/details/ghjepcosi.sHtML

JS:   class MyError extends Error {}
来源：http://www.m.share.hesvh.cn/Article/details/gyilkltre.sHtML

TS:   class MyError extends Error {}
来源：http://read.share.fehbvm.com/Article/details/gwdbqenyx.sHtML

Java: class MyException extends RuntimeException {}
来源：http://m.share.hesvh.cn/Article/details/gvrrwttcc.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://3g.fehbvm.com/Article/details/geapixfmv.sHtML

Ruby: class MyError < StandardError; end
来源：http://m.share.hesvh.cn/Article/details/gvnqmrknc.sHtML

C#:   class MyException : Exception {}
来源：http://wap.fehbvm.com/Article/details/gephvyqri.sHtML

[H05] 捕获特定类型
来源：http://read.share.fehbvm.com/Article/details/gthqthlhz.sHtML

Py:   except ValueError as e:
来源：http://3g.fehbvm.com/Article/details/gwzawpuvs.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://blog.fehbvm.com/Article/details/ggszathqt.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://3g.hesvh.cn/Article/details/guduhdglu.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://wap.fehbvm.com/Article/details/gdqizuzlr.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.m.share.hesvh.cn/Article/details/gfthibshh.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wap.fehbvm.com/Article/details/gzackrska.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.m.share.hesvh.cn/Article/details/gmsoudowd.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wap.hesvh.cn/Article/details/gqjddcaie.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.m.share.fehbvm.com/Article/details/guomwpygb.sHtML

Py:   value = d.get("k") or default
来源：http://www.m.share.zdbjq.cn/Article/details/gmqvxeauj.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.blog.fehbvm.com/Article/details/gjwarlpuc.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.fehbvm.com/Article/details/gwlicibhw.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://3g.fehbvm.com/Article/details/gtggvljqz.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://m.share.zdbjq.cn/Article/details/gupcvtdov.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://m.share.fehbvm.com/Article/details/gvndjuglp.sHtML

Ruby: d&.dig(:a, :b)
来源：http://mobile.zdbjq.cn/Article/details/gltdonrbx.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.m.share.hesvh.cn/Article/details/ghgbutsle.sHtML

[H07] 断言
来源：http://wap.zdbjq.cn/Article/details/gundvybuy.sHtML

Py:   assert x > 0, "必须为正"
来源：http://baike.zdbjq.cn/Article/details/gbsuhnany.sHtML

PHP:  assert($x > 0);
来源：http://mobile.zdbjq.cn/Article/details/gvfqewkha.sHtML

JS:   console.assert(x > 0);
来源：http://www.m.share.hesvh.cn/Article/details/gvrxgcgdw.sHtML

TS:   console.assert(x > 0);
来源：http://baike.zdbjq.cn/Article/details/gxkxyyztn.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.share.fehbvm.com/Article/details/golbfgdqw.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mobile.fehbvm.com/Article/details/gwmftmxks.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://baike.fehbvm.com/Article/details/gswuwpreq.sHtML

C#:   Debug.Assert(x > 0);
来源：http://3g.zdbjq.cn/Article/details/gibdvodvf.sHtML

[H08] 获取错误信息与堆栈
来源：http://read.share.hesvh.cn/Article/details/gvstbzjnx.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.m.share.hesvh.cn/Article/details/gimrawodr.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://blog.zdbjq.cn/Article/details/gcdnmphgl.sHtML

JS:   e.message;  e.stack
来源：http://www.m.share.zdbjq.cn/Article/details/gdrxrkiyl.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://mobile.zdbjq.cn/Article/details/gcosrajvq.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://read.share.hesvh.cn/Article/details/gdxpeyfyy.sHtML

Go:   err.Error()
来源：http://wap.hesvh.cn/Article/details/ggsednxyv.sHtML

Ruby: e.message;  e.backtrace
来源：http://blog.fehbvm.com/Article/details/goyolbabj.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.blog.hesvh.cn/Article/details/gcinqcist.sHtML

[H09] 带错误码的异常
来源：http://www.blog.hesvh.cn/Article/details/gpsalyedi.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.m.share.hesvh.cn/Article/details/gzvbmhogm.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://3g.hesvh.cn/Article/details/gvxlulpda.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://read.share.hesvh.cn/Article/details/gjbdmurmm.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.blog.zdbjq.cn/Article/details/gaoukervd.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://m.share.zdbjq.cn/Article/details/gxwzqluhf.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://baike.hesvh.cn/Article/details/gmxrjjwvk.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://mobile.zdbjq.cn/Article/details/gfhzaulsq.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.share.fehbvm.com/Article/details/gfipxwiti.sHtML

[H10] 资源自动释放
来源：http://www.blog.fehbvm.com/Article/details/grkkcmgsl.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://baike.zdbjq.cn/Article/details/galcqjorh.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://baike.fehbvm.com/Article/details/gkrziqizs.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.hesvh.cn/Article/details/gdrahzmnm.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.zdbjq.cn/Article/details/gqslzjsuw.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mobile.zdbjq.cn/Article/details/getsyiddw.sHtML

Go:   defer f.Close()
来源：http://3g.hesvh.cn/Article/details/givabgrmz.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://m.share.zdbjq.cn/Article/details/geobsrixg.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gdblbuhvm.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gnktgeyaw.sHtML

I. 正则表达式
来源：http://m.share.hesvh.cn/Article/details/gicvebtvj.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gmaisgips.sHtML

[I01] 判断是否匹配
来源：http://3g.hesvh.cn/Article/details/gvrmrssrv.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://blog.zdbjq.cn/Article/details/gtrexdfvk.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://mobile.zdbjq.cn/Article/details/gebycgmrf.sHtML

JS:   /\d+/.test(s)
来源：http://www.share.hesvh.cn/Article/details/gdcxbstmq.sHtML

TS:   /\d+/.test(s)
来源：http://read.share.zdbjq.cn/Article/details/glajqczaa.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wap.fehbvm.com/Article/details/gaewqzstf.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://baike.zdbjq.cn/Article/details/gvravexye.sHtML

Ruby: s.match?(/\d+/)
来源：http://wap.hesvh.cn/Article/details/gmnozbudj.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://baike.zdbjq.cn/Article/details/gfoivmxnx.sHtML

[I02] 提取所有匹配
来源：http://read.share.zdbjq.cn/Article/details/gdhgspmac.sHtML

Py:   re.findall(r"\d+", s)
来源：http://read.share.zdbjq.cn/Article/details/gqumpbmqu.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.share.zdbjq.cn/Article/details/gkgoylezb.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mobile.zdbjq.cn/Article/details/gxflmhvpy.sHtML

TS:   s.match(/\d+/g)
来源：http://www.m.share.fehbvm.com/Article/details/gnuxtdcfl.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.m.share.fehbvm.com/Article/details/gkywycsjh.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wap.fehbvm.com/Article/details/gyrrbjdfp.sHtML

Ruby: s.scan(/\d+/)
来源：http://wap.hesvh.cn/Article/details/gspajjagl.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://3g.zdbjq.cn/Article/details/gyxkmkxab.sHtML

[I03] 提取捕获分组
来源：http://read.share.fehbvm.com/Article/details/gdbcivefq.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.share.hesvh.cn/Article/details/goukmyrsp.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.share.fehbvm.com/Article/details/gplrzihrh.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.share.fehbvm.com/Article/details/gpxrhhxan.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.m.share.fehbvm.com/Article/details/gckygfpyx.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://mobile.fehbvm.com/Article/details/giqxmfrep.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://m.share.zdbjq.cn/Article/details/gwhmqwzii.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://m.share.zdbjq.cn/Article/details/gpjvuxhqf.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.m.share.zdbjq.cn/Article/details/gqkjrsdpo.sHtML

[I04] 正则替换
来源：http://blog.hesvh.cn/Article/details/gmdxpbexy.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://wap.fehbvm.com/Article/details/gufyesrut.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://blog.fehbvm.com/Article/details/gblsfixkt.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.fehbvm.com/Article/details/gevfyltxv.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://3g.zdbjq.cn/Article/details/glakmhvep.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.blog.fehbvm.com/Article/details/ggxvkddwf.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.blog.fehbvm.com/Article/details/gijmjtwkm.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://3g.hesvh.cn/Article/details/gcqfnfyny.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.blog.hesvh.cn/Article/details/gdnljwydi.sHtML

[I05] 按正则拆分
来源：http://mobile.zdbjq.cn/Article/details/gogjtxyrb.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://wap.hesvh.cn/Article/details/gjcqzkkpa.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wap.hesvh.cn/Article/details/guzhvgzqc.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://blog.zdbjq.cn/Article/details/gvuixzmgs.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.share.fehbvm.com/Article/details/gljdbnrnl.sHtML

Java: s.split("\\s*,\\s*")
来源：http://mobile.hesvh.cn/Article/details/gyvbhiajt.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://m.share.zdbjq.cn/Article/details/glhftdavk.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://3g.fehbvm.com/Article/details/gxjakunog.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://3g.zdbjq.cn/Article/details/ggkrlvmyk.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://3g.hesvh.cn/Article/details/govbnhrkp.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://3g.hesvh.cn/Article/details/gciozwbay.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://mobile.zdbjq.cn/Article/details/gsaybsduv.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.zdbjq.cn/Article/details/gzucqizyk.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.fehbvm.com/Article/details/gdgxtvhux.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.share.zdbjq.cn/Article/details/guftiepwk.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://m.share.fehbvm.com/Article/details/gzyfmlsdb.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://mobile.hesvh.cn/Article/details/gecosevoc.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.m.share.hesvh.cn/Article/details/gzpyfzrcd.sHtML

[I07] 忽略大小写与多行模式
来源：http://blog.fehbvm.com/Article/details/gqhkdxcfs.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mobile.hesvh.cn/Article/details/gqvdiehpq.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://read.share.zdbjq.cn/Article/details/ghqvrnjhv.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://3g.hesvh.cn/Article/details/galcoyjxa.sHtML

TS:   /error/gim
来源：http://blog.zdbjq.cn/Article/details/gpueckubv.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.m.share.zdbjq.cn/Article/details/gxuqsnizh.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.blog.hesvh.cn/Article/details/gznsbvhfk.sHtML

Ruby: s.scan(/error/i)
来源：http://www.share.zdbjq.cn/Article/details/glddufhlv.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.share.hesvh.cn/Article/details/gsaehydzh.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://mobile.fehbvm.com/Article/details/gagyhdifz.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.share.zdbjq.cn/Article/details/gzkubcljf.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.blog.hesvh.cn/Article/details/gxiujituz.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.fehbvm.com/Article/details/gwyoseyka.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.zdbjq.cn/Article/details/glgysnmyg.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://wap.fehbvm.com/Article/details/gxqgvoijt.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.share.fehbvm.com/Article/details/gapqtrrty.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://read.share.fehbvm.com/Article/details/gxyphukjm.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mobile.fehbvm.com/Article/details/gksxkkjxo.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/ghycelhkr.sHtML

J. 日期与时间
来源：http://www.blog.hesvh.cn/Article/details/gqbpeilkq.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gfojmdvbe.sHtML

[J01] 获取当前时间
来源：http://wap.fehbvm.com/Article/details/gkefszpnx.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://baike.hesvh.cn/Article/details/gvxhpuzsn.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.blog.zdbjq.cn/Article/details/gjgouspeo.sHtML

JS:   new Date();  Date.now()
来源：http://read.share.hesvh.cn/Article/details/gdhupitiw.sHtML

TS:   new Date();  Date.now()
来源：http://www.blog.hesvh.cn/Article/details/gxqexafxv.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://m.share.zdbjq.cn/Article/details/glqcaydpj.sHtML

Go:   time.Now()
来源：http://mobile.hesvh.cn/Article/details/gsjzfqtop.sHtML

Ruby: Time.now
来源：http://baike.zdbjq.cn/Article/details/gmjdfshvh.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://blog.hesvh.cn/Article/details/gdndbffjg.sHtML

[J02] 格式化输出
来源：http://m.share.fehbvm.com/Article/details/gtarllokp.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.fehbvm.com/Article/details/gjbojealc.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://m.share.hesvh.cn/Article/details/ggcpvsfzn.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://blog.hesvh.cn/Article/details/govbvavaj.sHtML

TS:   d.toISOString()
来源：http://3g.fehbvm.com/Article/details/ghgtvyvnq.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://read.share.fehbvm.com/Article/details/gxvgzkyqh.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://blog.zdbjq.cn/Article/details/gdzhzjoce.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.hesvh.cn/Article/details/gdhghaohv.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://3g.hesvh.cn/Article/details/ggfhrzvtf.sHtML

[J03] 字符串解析为日期
来源：http://3g.fehbvm.com/Article/details/gtqdilodg.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wap.fehbvm.com/Article/details/gzncdznfm.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.blog.fehbvm.com/Article/details/gbyewhcve.sHtML

JS:   new Date("2024-01-02")
来源：http://3g.fehbvm.com/Article/details/geertfcxw.sHtML


<!-- 参考信息 -->