代发 wailian999

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gpdwlvtuz.sHtML

[G03] 实例属性
来源：http://read.share.fehbvm.com/Article/details/gqxxhhxnl.sHtML

Py:   self.name = "x"
来源：http://www.m.share.hesvh.cn/Article/details/gmvkwnepn.sHtML

PHP:  public string $name = "x";
来源：http://mobile.hesvh.cn/Article/details/grfxrdbhh.sHtML

JS:   this.name = "x";
来源：http://baike.zdbjq.cn/Article/details/gvuhoroco.sHtML

TS:   name: string = "x";
来源：http://blog.hesvh.cn/Article/details/gwkkqkgsg.sHtML

Java: private String name;
来源：http://read.share.hesvh.cn/Article/details/gkyvqdwyi.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.fehbvm.com/Article/details/gnnyoawdd.sHtML

Ruby: @name = "x"
来源：http://read.share.hesvh.cn/Article/details/grwwcphlr.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.zdbjq.cn/Article/details/gkjepezmu.sHtML

[G04] 定义方法
来源：http://blog.hesvh.cn/Article/details/gvbgxljuo.sHtML

Py:   def greet(self): return self.name
来源：http://wap.zdbjq.cn/Article/details/gqqzdvhez.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.fehbvm.com/Article/details/gjqfriehv.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/gmledpdte.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.hesvh.cn/Article/details/gnljofflk.sHtML

Java: String greet() { return name; }
来源：http://mobile.hesvh.cn/Article/details/gtlfrozzl.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.zdbjq.cn/Article/details/gufhofobl.sHtML

Ruby: def greet; @name; end
来源：http://blog.fehbvm.com/Article/details/gdmrvrocn.sHtML

C#:   public string Greet() => Name;
来源：http://3g.zdbjq.cn/Article/details/ghhttyxwu.sHtML

[G05] 继承
来源：http://baike.fehbvm.com/Article/details/grpdsndvg.sHtML

Py:   class Admin(User): pass
来源：http://m.share.hesvh.cn/Article/details/ghdibrwve.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/gyrbyifod.sHtML

JS:   class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/gqghxizyo.sHtML

TS:   class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/gimyioptf.sHtML

Java: class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/gmgnmncre.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.fehbvm.com/Article/details/gdmocsndt.sHtML

Ruby: class Admin < User; end
来源：http://www.share.hesvh.cn/Article/details/ggfvmcdcw.sHtML

C#:   class Admin : User {}
来源：http://www.blog.fehbvm.com/Article/details/gqdzfdryq.sHtML

[G06] 重写方法
来源：http://read.share.fehbvm.com/Article/details/gdmfetxdx.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.fehbvm.com/Article/details/gqvkcjpdz.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/gfnjgfxqn.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.zdbjq.cn/Article/details/gukgyuoxs.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/gvoofkani.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/gxgimiyuz.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.zdbjq.cn/Article/details/gtjiayfnl.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.hesvh.cn/Article/details/gcodwhoml.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.hesvh.cn/Article/details/gujphiobh.sHtML

[G07] 调用父类方法
来源：http://www.share.fehbvm.com/Article/details/gpkrjkjou.sHtML

Py:   super().greet()
来源：http://blog.zdbjq.cn/Article/details/gasusbxrt.sHtML

PHP:  parent::greet();
来源：http://3g.hesvh.cn/Article/details/gjlzfubug.sHtML

JS:   super.greet();
来源：http://read.share.hesvh.cn/Article/details/gdvjcexwr.sHtML

TS:   super.greet();
来源：http://read.share.zdbjq.cn/Article/details/gmvepmmcp.sHtML

Java: super.greet();
来源：http://wap.hesvh.cn/Article/details/gkcicvwej.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.hesvh.cn/Article/details/gznrgjbzk.sHtML

Ruby: super
来源：http://baike.fehbvm.com/Article/details/gglgnvfmx.sHtML

C#:   base.Greet();
来源：http://3g.hesvh.cn/Article/details/gyqjbsrbl.sHtML

[G08] 静态方法与属性
来源：http://3g.fehbvm.com/Article/details/glmkrtwer.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.fehbvm.com/Article/details/gfxjrmfgx.sHtML

PHP:  public static function f() {}
来源：http://3g.hesvh.cn/Article/details/gfzijbrrf.sHtML

JS:   static f() {}
来源：http://baike.hesvh.cn/Article/details/gnbvfuvdv.sHtML

TS:   static f(): void {}
来源：http://wap.zdbjq.cn/Article/details/glcvduyti.sHtML

Java: static void f() {}
来源：http://m.share.hesvh.cn/Article/details/gpokeoxkm.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.fehbvm.com/Article/details/ghekxpaxr.sHtML

Ruby: def self.f; end
来源：http://wap.hesvh.cn/Article/details/gtskeapyw.sHtML

C#:   public static void F() {}
来源：http://mobile.hesvh.cn/Article/details/gleszywdf.sHtML

[G09] 接口 / 抽象类
来源：http://baike.fehbvm.com/Article/details/githukeld.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.zdbjq.cn/Article/details/gnaclbrio.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.hesvh.cn/Article/details/ggcwrkngt.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.hesvh.cn/Article/details/gxbunbwdn.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.fehbvm.com/Article/details/grkwrwnbx.sHtML

Java: interface Shape { double area(); }
来源：http://wap.zdbjq.cn/Article/details/gmhmbwddx.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.hesvh.cn/Article/details/gbpnmshbg.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.zdbjq.cn/Article/details/girjagged.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.hesvh.cn/Article/details/gxmpktasy.sHtML

[G10] 访问控制
来源：http://read.share.zdbjq.cn/Article/details/gitkowwnl.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.fehbvm.com/Article/details/gihicszbd.sHtML

PHP:  public / protected / private
来源：http://baike.hesvh.cn/Article/details/glugctsat.sHtML

JS:   #private 字段；其余公开
来源：http://3g.hesvh.cn/Article/details/gyqyaaceq.sHtML

TS:   public / protected / private
来源：http://mobile.hesvh.cn/Article/details/gvfhoyxyl.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.zdbjq.cn/Article/details/ghorhoqqw.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.hesvh.cn/Article/details/gajunozyb.sHtML

Ruby: public / protected / private
来源：http://mobile.hesvh.cn/Article/details/gkjrdafzm.sHtML

C#:   public / protected / private / internal
来源：http://m.share.zdbjq.cn/Article/details/gvrpirsjc.sHtML

[G11] getter / setter
来源：http://www.blog.hesvh.cn/Article/details/grjrmjdom.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.zdbjq.cn/Article/details/gzxvazdkk.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.zdbjq.cn/Article/details/gxordlizx.sHtML

JS:   get name() { return this._name; }
来源：http://baike.hesvh.cn/Article/details/grojatldz.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gkwedgsji.sHtML

Java: public String getName() { return name; }
来源：http://www.share.hesvh.cn/Article/details/ggxmwyzta.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.zdbjq.cn/Article/details/gjrpobuzq.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.zdbjq.cn/Article/details/goodmvwql.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.fehbvm.com/Article/details/gxictotzh.sHtML

[G12] 对象转字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gxzntgdgb.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.hesvh.cn/Article/details/gtsaukjqd.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.hesvh.cn/Article/details/gcwlzqgzt.sHtML

JS:   toString() { return this.name; }
来源：http://wap.fehbvm.com/Article/details/ggbdlvdsm.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/gnynqiapl.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.hesvh.cn/Article/details/gbgiftpkr.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.hesvh.cn/Article/details/gsaoswxkh.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.fehbvm.com/Article/details/gaqezipjr.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.zdbjq.cn/Article/details/gcasuxmuw.sHtML

[G13] 判断对象类型
来源：http://blog.zdbjq.cn/Article/details/gagszhnwh.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.zdbjq.cn/Article/details/gholiduwr.sHtML

PHP:  $u instanceof User
来源：http://baike.fehbvm.com/Article/details/gyhahrzjb.sHtML

JS:   u instanceof User
来源：http://mobile.hesvh.cn/Article/details/gmtqojzkh.sHtML

TS:   u instanceof User
来源：http://wap.fehbvm.com/Article/details/gqbnxdlio.sHtML

Java: u instanceof User
来源：http://blog.hesvh.cn/Article/details/gwsggcvur.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.fehbvm.com/Article/details/gfopdpzeh.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.zdbjq.cn/Article/details/gbknxkgzk.sHtML

C#:   u is User
来源：http://3g.fehbvm.com/Article/details/gmlcbipiv.sHtML

[G14] 数据类 / record
来源：http://www.blog.fehbvm.com/Article/details/goezulzxw.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.zdbjq.cn/Article/details/glgbndrfb.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.zdbjq.cn/Article/details/gylqmrtnf.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.hesvh.cn/Article/details/glugiuxgj.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.zdbjq.cn/Article/details/gcfpgfoqe.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.hesvh.cn/Article/details/gngvlmsrm.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.fehbvm.com/Article/details/guzmilvsm.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.zdbjq.cn/Article/details/gxablqeub.sHtML

C#:   record User(string Name, int Age);
来源：http://read.share.hesvh.cn/Article/details/gtdwkpihq.sHtML

[G15] 枚举
来源：http://m.share.hesvh.cn/Article/details/gjqlofqkp.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.fehbvm.com/Article/details/ghlepjexi.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.m.share.zdbjq.cn/Article/details/globwrndf.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.m.share.fehbvm.com/Article/details/gnfwlekhh.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.hesvh.cn/Article/details/gochroisb.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.hesvh.cn/Article/details/gmsxmqgra.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.hesvh.cn/Article/details/gntnqlyiw.sHtML

Ruby: Color = %i[red green].freeze
来源：http://read.share.hesvh.cn/Article/details/guzaauwwx.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.zdbjq.cn/Article/details/gtnevseoq.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.zdbjq.cn/Article/details/ggtlklmhj.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.fehbvm.com/Article/details/ggbpbelgo.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.zdbjq.cn/Article/details/gqnpfepwn.sHtML

JS:   Object.entries(obj)
来源：http://www.share.zdbjq.cn/Article/details/grzyocqov.sHtML

TS:   Object.entries(obj)
来源：http://www.blog.hesvh.cn/Article/details/gratiiigh.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.zdbjq.cn/Article/details/gvjbplbkt.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.hesvh.cn/Article/details/gvyufbelc.sHtML

Ruby: obj.instance_variables
来源：http://blog.hesvh.cn/Article/details/gfofwpiww.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.hesvh.cn/Article/details/grlwxjnum.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gfwxyncgr.sHtML

H. 异常与错误处理
来源：http://mobile.hesvh.cn/Article/details/gxudwnlde.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gvtyorvyz.sHtML

[H01] try / catch 基础
来源：http://www.share.hesvh.cn/Article/details/gzecnjqdz.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.hesvh.cn/Article/details/gujcvfwun.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.hesvh.cn/Article/details/gigdrdzhq.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.zdbjq.cn/Article/details/gzzkgbhmz.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.m.share.fehbvm.com/Article/details/gqbodebvs.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.zdbjq.cn/Article/details/gckhbctku.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.fehbvm.com/Article/details/gwzdreebz.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://blog.hesvh.cn/Article/details/gobzugxgf.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://baike.hesvh.cn/Article/details/gqwvwwome.sHtML

[H02] finally / ensure 收尾
来源：http://www.m.share.hesvh.cn/Article/details/glpxwpdwf.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.zdbjq.cn/Article/details/gklilvint.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://baike.hesvh.cn/Article/details/gmgkgopkh.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/guzdjmbka.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.hesvh.cn/Article/details/gatxdqfqo.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.fehbvm.com/Article/details/gkjkhizti.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.blog.hesvh.cn/Article/details/gfienygkb.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.fehbvm.com/Article/details/glcxgynek.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://3g.zdbjq.cn/Article/details/glotvgbpc.sHtML

[H03] 主动抛出异常
来源：http://www.blog.fehbvm.com/Article/details/gsvewigsb.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.share.fehbvm.com/Article/details/gjoymbice.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.fehbvm.com/Article/details/glpucujxs.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.fehbvm.com/Article/details/gvyxhpbas.sHtML

TS:   throw new Error("错误信息");
来源：http://www.m.share.fehbvm.com/Article/details/gykccfjxw.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://mobile.hesvh.cn/Article/details/glggyqbio.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.share.hesvh.cn/Article/details/gcfelvcqw.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.blog.fehbvm.com/Article/details/ghkczqcvp.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.fehbvm.com/Article/details/gwdmvauoy.sHtML

[H04] 自定义异常类型
来源：http://mobile.fehbvm.com/Article/details/gdmsmiamy.sHtML

Py:   class MyError(Exception): pass
来源：http://wap.zdbjq.cn/Article/details/gqeatukwv.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://3g.hesvh.cn/Article/details/gfpsyqfqs.sHtML

JS:   class MyError extends Error {}
来源：http://read.share.zdbjq.cn/Article/details/gscyhezxa.sHtML

TS:   class MyError extends Error {}
来源：http://3g.hesvh.cn/Article/details/gfwxypblr.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.share.zdbjq.cn/Article/details/gohjazxgc.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mobile.hesvh.cn/Article/details/gxqevocjh.sHtML

Ruby: class MyError < StandardError; end
来源：http://mobile.hesvh.cn/Article/details/gdrcewmwu.sHtML

C#:   class MyException : Exception {}
来源：http://blog.zdbjq.cn/Article/details/gvmunrrve.sHtML

[H05] 捕获特定类型
来源：http://mobile.zdbjq.cn/Article/details/gsodgolsn.sHtML

Py:   except ValueError as e:
来源：http://read.share.hesvh.cn/Article/details/gzutrqypz.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.fehbvm.com/Article/details/gdiylgaqo.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://blog.fehbvm.com/Article/details/gksfphnjs.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://wap.zdbjq.cn/Article/details/grmnvmqpe.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://m.share.fehbvm.com/Article/details/gmnlkcrac.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://baike.hesvh.cn/Article/details/gvinqglbm.sHtML

Ruby: rescue ArgumentError => e
来源：http://mobile.zdbjq.cn/Article/details/gyxflqlje.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.share.hesvh.cn/Article/details/gaaxpndti.sHtML

[H06] 可选值 / 空值安全访问
来源：http://blog.fehbvm.com/Article/details/gwbcvesuy.sHtML

Py:   value = d.get("k") or default
来源：http://mobile.hesvh.cn/Article/details/gyczwyrvw.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://blog.hesvh.cn/Article/details/glkulovyp.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://3g.zdbjq.cn/Article/details/gnujffpqm.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://mobile.zdbjq.cn/Article/details/gzfmfmgxj.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.share.fehbvm.com/Article/details/gtucbwvta.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.m.share.zdbjq.cn/Article/details/glscxzozq.sHtML

Ruby: d&.dig(:a, :b)
来源：http://read.share.fehbvm.com/Article/details/gcgyltvho.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.share.zdbjq.cn/Article/details/ggdrnvnvx.sHtML

[H07] 断言
来源：http://3g.fehbvm.com/Article/details/ghqnugihg.sHtML

Py:   assert x > 0, "必须为正"
来源：http://baike.fehbvm.com/Article/details/gfnnegrvj.sHtML

PHP:  assert($x > 0);
来源：http://wap.zdbjq.cn/Article/details/gdrivbokk.sHtML

JS:   console.assert(x > 0);
来源：http://m.share.zdbjq.cn/Article/details/gabffhpfk.sHtML

TS:   console.assert(x > 0);
来源：http://www.blog.zdbjq.cn/Article/details/ggipgccsn.sHtML

Java: assert x > 0 : "必须为正";
来源：http://baike.zdbjq.cn/Article/details/gkzdofavm.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mobile.hesvh.cn/Article/details/gcvkjwyhq.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://m.share.hesvh.cn/Article/details/gaqngyura.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.share.hesvh.cn/Article/details/gvoiqhrbc.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.share.zdbjq.cn/Article/details/grlhlbcib.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.share.zdbjq.cn/Article/details/gnabgcceq.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://read.share.hesvh.cn/Article/details/gpjmrwhpo.sHtML

JS:   e.message;  e.stack
来源：http://www.share.hesvh.cn/Article/details/gcrwsmsbo.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://blog.fehbvm.com/Article/details/gqafjspyh.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://mobile.zdbjq.cn/Article/details/gzurcpdlh.sHtML

Go:   err.Error()
来源：http://baike.zdbjq.cn/Article/details/glnfqgdub.sHtML

Ruby: e.message;  e.backtrace
来源：http://mobile.fehbvm.com/Article/details/gvqiidmvi.sHtML

C#:   e.Message;  e.StackTrace
来源：http://read.share.hesvh.cn/Article/details/gqlztydfw.sHtML

[H09] 带错误码的异常
来源：http://www.blog.fehbvm.com/Article/details/gcylukbob.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://m.share.hesvh.cn/Article/details/gbquoshqe.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://wap.fehbvm.com/Article/details/gstkxenmv.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wap.hesvh.cn/Article/details/ggvgphibe.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://3g.hesvh.cn/Article/details/gixrymzdw.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.blog.zdbjq.cn/Article/details/gozqpebch.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://baike.zdbjq.cn/Article/details/gceyalxtm.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://m.share.fehbvm.com/Article/details/gwpdlpepx.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://3g.fehbvm.com/Article/details/gafhzqprg.sHtML

[H10] 资源自动释放
来源：http://read.share.fehbvm.com/Article/details/gobveagnj.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://m.share.zdbjq.cn/Article/details/ggitdikgv.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://m.share.zdbjq.cn/Article/details/ggvwwsdvk.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.zdbjq.cn/Article/details/goxcxadeo.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.hesvh.cn/Article/details/gtjzwguwh.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://baike.fehbvm.com/Article/details/gvogbjqik.sHtML

Go:   defer f.Close()
来源：http://read.share.zdbjq.cn/Article/details/gsyotpstc.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://m.share.fehbvm.com/Article/details/gvkqujifj.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/guydkepqu.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gkjfjzyts.sHtML

I. 正则表达式
来源：http://blog.fehbvm.com/Article/details/gsmrvuzul.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gjrxzcoiy.sHtML

[I01] 判断是否匹配
来源：http://baike.zdbjq.cn/Article/details/gffhzeeys.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://blog.zdbjq.cn/Article/details/gwpyyalya.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://baike.hesvh.cn/Article/details/ghhvlkbrq.sHtML

JS:   /\d+/.test(s)
来源：http://m.share.fehbvm.com/Article/details/gszsxwnnx.sHtML

TS:   /\d+/.test(s)
来源：http://read.share.fehbvm.com/Article/details/gdwbnhvel.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.m.share.fehbvm.com/Article/details/gcgvnlaky.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.share.fehbvm.com/Article/details/ghxkvdkum.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.share.zdbjq.cn/Article/details/gbytvaafy.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://read.share.hesvh.cn/Article/details/gorwzfhdj.sHtML

[I02] 提取所有匹配
来源：http://mobile.fehbvm.com/Article/details/gitgesrgs.sHtML

Py:   re.findall(r"\d+", s)
来源：http://wap.fehbvm.com/Article/details/gacglvyrs.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mobile.hesvh.cn/Article/details/gmzobxaug.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://3g.zdbjq.cn/Article/details/gdzpyykct.sHtML

TS:   s.match(/\d+/g)
来源：http://www.share.zdbjq.cn/Article/details/gmfqktfbc.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://read.share.zdbjq.cn/Article/details/gduwnvgtl.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://3g.zdbjq.cn/Article/details/gwsvexgbh.sHtML

Ruby: s.scan(/\d+/)
来源：http://mobile.fehbvm.com/Article/details/gabfyjofn.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wap.zdbjq.cn/Article/details/gyoltlvmh.sHtML

[I03] 提取捕获分组
来源：http://baike.fehbvm.com/Article/details/ghzxwndrs.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.blog.fehbvm.com/Article/details/gshdbqklv.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://read.share.fehbvm.com/Article/details/ghzohgyky.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mobile.fehbvm.com/Article/details/gxyyqisrm.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://3g.zdbjq.cn/Article/details/gtelavwod.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.m.share.zdbjq.cn/Article/details/gqmrjdjjv.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.share.zdbjq.cn/Article/details/gnoqvoqtk.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.m.share.fehbvm.com/Article/details/guvjkxqhy.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://blog.hesvh.cn/Article/details/gwuvyigtk.sHtML

[I04] 正则替换
来源：http://www.blog.fehbvm.com/Article/details/gqbqwrvao.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.share.fehbvm.com/Article/details/glbnhmmcd.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.share.zdbjq.cn/Article/details/gmvazublc.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://baike.hesvh.cn/Article/details/gkkmhhwtr.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://mobile.zdbjq.cn/Article/details/gjevikqew.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.m.share.hesvh.cn/Article/details/gbjnwpxkk.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://mobile.fehbvm.com/Article/details/grlrsirkk.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.blog.hesvh.cn/Article/details/gtzcanubf.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.m.share.zdbjq.cn/Article/details/gjnluvzlt.sHtML

[I05] 按正则拆分
来源：http://blog.hesvh.cn/Article/details/gvnlvfquk.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://read.share.zdbjq.cn/Article/details/geqiewgym.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://3g.hesvh.cn/Article/details/gwybofoze.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.blog.hesvh.cn/Article/details/gihtscpti.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.blog.hesvh.cn/Article/details/gpptzeqoe.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.share.hesvh.cn/Article/details/gitvasoyb.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://m.share.zdbjq.cn/Article/details/gxrdiflpb.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://blog.hesvh.cn/Article/details/gcjxtjbbc.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://read.share.hesvh.cn/Article/details/gtrvgauyo.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.blog.zdbjq.cn/Article/details/gcbhzyjin.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.m.share.zdbjq.cn/Article/details/gkxvxixzy.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://m.share.zdbjq.cn/Article/details/gkoemipqm.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.fehbvm.com/Article/details/gwdtelrgt.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.fehbvm.com/Article/details/gppqehrnu.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://blog.zdbjq.cn/Article/details/gxrfbrrfy.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.blog.hesvh.cn/Article/details/guplpwehe.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.blog.zdbjq.cn/Article/details/ghveqehun.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://baike.fehbvm.com/Article/details/gxxukkqua.sHtML

[I07] 忽略大小写与多行模式
来源：http://3g.hesvh.cn/Article/details/gpktjkzis.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.share.hesvh.cn/Article/details/gdmxhpnda.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://3g.zdbjq.cn/Article/details/geapbdudi.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mobile.fehbvm.com/Article/details/ghsreifth.sHtML

TS:   /error/gim
来源：http://wap.fehbvm.com/Article/details/gbrialiak.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://read.share.fehbvm.com/Article/details/gbolrdyjr.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://baike.zdbjq.cn/Article/details/gzzaqmpps.sHtML

Ruby: s.scan(/error/i)
来源：http://baike.fehbvm.com/Article/details/gbzrhazcs.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://baike.fehbvm.com/Article/details/gzlxhtapc.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.m.share.fehbvm.com/Article/details/geollszuw.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://m.share.zdbjq.cn/Article/details/gkjnnhqls.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wap.zdbjq.cn/Article/details/guabhnuoj.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.hesvh.cn/Article/details/gknkrhipl.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.hesvh.cn/Article/details/gvxxgzxgl.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://blog.zdbjq.cn/Article/details/gepwncyvn.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.m.share.fehbvm.com/Article/details/glnobkckz.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://3g.hesvh.cn/Article/details/glfglmfcg.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.blog.hesvh.cn/Article/details/grjpcbyxq.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gurspibqo.sHtML

J. 日期与时间
来源：http://baike.zdbjq.cn/Article/details/gbnuanruu.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gfjunwsdl.sHtML

[J01] 获取当前时间
来源：http://wap.zdbjq.cn/Article/details/grkdduobj.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.share.hesvh.cn/Article/details/ggmmlvaus.sHtML


<!-- 参考信息 -->