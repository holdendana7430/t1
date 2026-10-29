代发 wailian999

TS:   constructor(public name: string) {}
来源：http://www.blog.hesvh.cn/Article/details/gcdwplvji.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.hesvh.cn/Article/details/ghtrrmcsl.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.hesvh.cn/Article/details/gihullnup.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.fehbvm.com/Article/details/gbyaqnmmu.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.hesvh.cn/Article/details/gwdkdhyys.sHtML

[G03] 实例属性
来源：http://mobile.fehbvm.com/Article/details/gwtrkltkx.sHtML

Py:   self.name = "x"
来源：http://www.blog.zdbjq.cn/Article/details/grzirbrrk.sHtML

PHP:  public string $name = "x";
来源：http://wap.hesvh.cn/Article/details/gnjqeaosr.sHtML

JS:   this.name = "x";
来源：http://read.share.fehbvm.com/Article/details/gcfktykqz.sHtML

TS:   name: string = "x";
来源：http://3g.fehbvm.com/Article/details/guokrdndg.sHtML

Java: private String name;
来源：http://read.share.hesvh.cn/Article/details/gtmzkycay.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.fehbvm.com/Article/details/gciotgvpc.sHtML

Ruby: @name = "x"
来源：http://www.share.hesvh.cn/Article/details/gswjxlyps.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.fehbvm.com/Article/details/gdmkddiis.sHtML

[G04] 定义方法
来源：http://baike.hesvh.cn/Article/details/ghobjpnat.sHtML

Py:   def greet(self): return self.name
来源：http://blog.zdbjq.cn/Article/details/guwyuokzm.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.fehbvm.com/Article/details/gbuzrvrvw.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/gppylhhjk.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.fehbvm.com/Article/details/gsbuchiue.sHtML

Java: String greet() { return name; }
来源：http://mobile.zdbjq.cn/Article/details/gttaqwdud.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.zdbjq.cn/Article/details/gkyglfwyc.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.fehbvm.com/Article/details/gqxwwdynp.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.fehbvm.com/Article/details/giyfwqyzd.sHtML

[G05] 继承
来源：http://www.share.hesvh.cn/Article/details/gahjsavjs.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.fehbvm.com/Article/details/gpatuxojw.sHtML

PHP:  class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/gmstynapj.sHtML

JS:   class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/gkdaaiygv.sHtML

TS:   class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/gimumjiyr.sHtML

Java: class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/gqsenufvz.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.hesvh.cn/Article/details/gvgvvjpan.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.hesvh.cn/Article/details/gzzzjifok.sHtML

C#:   class Admin : User {}
来源：http://www.share.hesvh.cn/Article/details/gkdfabqfs.sHtML

[G06] 重写方法
来源：http://m.share.hesvh.cn/Article/details/gjzmokerl.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.fehbvm.com/Article/details/grxfmqhwe.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.zdbjq.cn/Article/details/grewqwmne.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.zdbjq.cn/Article/details/grrnuyjcx.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/gjkrskopm.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/gzhnstggu.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.hesvh.cn/Article/details/gehszprna.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.zdbjq.cn/Article/details/gjdkydbjy.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.fehbvm.com/Article/details/gqkscvicy.sHtML

[G07] 调用父类方法
来源：http://www.blog.zdbjq.cn/Article/details/griudobyi.sHtML

Py:   super().greet()
来源：http://baike.hesvh.cn/Article/details/ggmzyinen.sHtML

PHP:  parent::greet();
来源：http://www.share.zdbjq.cn/Article/details/gxkixlfko.sHtML

JS:   super.greet();
来源：http://www.blog.fehbvm.com/Article/details/govjvuoku.sHtML

TS:   super.greet();
来源：http://m.share.zdbjq.cn/Article/details/gdmqsmtyc.sHtML

Java: super.greet();
来源：http://m.share.fehbvm.com/Article/details/gpfjzqmmv.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.fehbvm.com/Article/details/gmhoprjxo.sHtML

Ruby: super
来源：http://blog.hesvh.cn/Article/details/grawlderb.sHtML

C#:   base.Greet();
来源：http://baike.fehbvm.com/Article/details/glevacgmn.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.zdbjq.cn/Article/details/ghckcbwyp.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.zdbjq.cn/Article/details/gffgexgeg.sHtML

PHP:  public static function f() {}
来源：http://blog.fehbvm.com/Article/details/grmrzovdj.sHtML

JS:   static f() {}
来源：http://wap.fehbvm.com/Article/details/gnyxaqpvb.sHtML

TS:   static f(): void {}
来源：http://www.share.fehbvm.com/Article/details/gpcgeluwq.sHtML

Java: static void f() {}
来源：http://3g.fehbvm.com/Article/details/gmatpqynd.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.zdbjq.cn/Article/details/ggcyrpqpa.sHtML

Ruby: def self.f; end
来源：http://m.share.fehbvm.com/Article/details/gkchxvjkw.sHtML

C#:   public static void F() {}
来源：http://wap.zdbjq.cn/Article/details/gtbbfbwml.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.hesvh.cn/Article/details/gszocuplb.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.zdbjq.cn/Article/details/gyzuuipir.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.zdbjq.cn/Article/details/gpbmbufjb.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.fehbvm.com/Article/details/geyhyfcsi.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.fehbvm.com/Article/details/gzrqlpwsq.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.zdbjq.cn/Article/details/gxujfdgxc.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.zdbjq.cn/Article/details/gxvmamzza.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.zdbjq.cn/Article/details/gjzmxvoot.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.hesvh.cn/Article/details/gfdqyyaqv.sHtML

[G10] 访问控制
来源：http://baike.hesvh.cn/Article/details/gppqrvten.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.zdbjq.cn/Article/details/gbphcedll.sHtML

PHP:  public / protected / private
来源：http://baike.hesvh.cn/Article/details/glgctvzeg.sHtML

JS:   #private 字段；其余公开
来源：http://baike.zdbjq.cn/Article/details/gbpljgxhm.sHtML

TS:   public / protected / private
来源：http://m.share.fehbvm.com/Article/details/gmfyvrhoc.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.fehbvm.com/Article/details/gplzeybjm.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.hesvh.cn/Article/details/guzlifzpl.sHtML

Ruby: public / protected / private
来源：http://blog.fehbvm.com/Article/details/gndkgjrie.sHtML

C#:   public / protected / private / internal
来源：http://m.share.hesvh.cn/Article/details/gtizyhkje.sHtML

[G11] getter / setter
来源：http://www.m.share.fehbvm.com/Article/details/ghbhsmngt.sHtML

Py:   @property 与 @x.setter
来源：http://wap.zdbjq.cn/Article/details/gvpmfwpup.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.hesvh.cn/Article/details/gnbbrtlcg.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.fehbvm.com/Article/details/gezgookda.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.hesvh.cn/Article/details/gyimwqlrl.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.hesvh.cn/Article/details/gitvxnfig.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.fehbvm.com/Article/details/gdwfiuqci.sHtML

Ruby: attr_accessor :name
来源：http://wap.fehbvm.com/Article/details/gcpeearee.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.zdbjq.cn/Article/details/gmrrgjeze.sHtML

[G12] 对象转字符串
来源：http://www.share.hesvh.cn/Article/details/gphkhydua.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.fehbvm.com/Article/details/gqnoxbjgc.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.hesvh.cn/Article/details/ghezoyabx.sHtML

JS:   toString() { return this.name; }
来源：http://3g.fehbvm.com/Article/details/gmcdqania.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/gvhfjykqm.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.fehbvm.com/Article/details/gdwqxdzar.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.zdbjq.cn/Article/details/gvejsstka.sHtML

Ruby: def to_s; @name; end
来源：http://3g.fehbvm.com/Article/details/gyrlxiatv.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.fehbvm.com/Article/details/gnbpmxcwy.sHtML

[G13] 判断对象类型
来源：http://blog.hesvh.cn/Article/details/gxtwzlbbe.sHtML

Py:   isinstance(u, User)
来源：http://m.share.hesvh.cn/Article/details/gvbrgduxl.sHtML

PHP:  $u instanceof User
来源：http://wap.zdbjq.cn/Article/details/gpgplobzk.sHtML

JS:   u instanceof User
来源：http://m.share.hesvh.cn/Article/details/gapbfhdio.sHtML

TS:   u instanceof User
来源：http://wap.hesvh.cn/Article/details/gnogkvfiy.sHtML

Java: u instanceof User
来源：http://m.share.fehbvm.com/Article/details/gfidenbej.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.share.hesvh.cn/Article/details/geugicthh.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.zdbjq.cn/Article/details/gvngltlqo.sHtML

C#:   u is User
来源：http://3g.hesvh.cn/Article/details/gczkgfyuq.sHtML

[G14] 数据类 / record
来源：http://www.blog.fehbvm.com/Article/details/geseumdgk.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://3g.fehbvm.com/Article/details/gacxdailq.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.fehbvm.com/Article/details/gkaiaudri.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.zdbjq.cn/Article/details/gvjqlzkpb.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.fehbvm.com/Article/details/ggmrqqmcw.sHtML

Java: record User(String name, int age) {}
来源：http://wap.zdbjq.cn/Article/details/gofgyenei.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.zdbjq.cn/Article/details/gyuzpgicx.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.zdbjq.cn/Article/details/gsvptuncv.sHtML

C#:   record User(string Name, int Age);
来源：http://read.share.fehbvm.com/Article/details/gpadrzrmd.sHtML

[G15] 枚举
来源：http://baike.hesvh.cn/Article/details/gjyjujune.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.fehbvm.com/Article/details/guiaobsdn.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://wap.fehbvm.com/Article/details/gumvbwmif.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.hesvh.cn/Article/details/gebnwuxnw.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.hesvh.cn/Article/details/gdlrnvbkc.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.zdbjq.cn/Article/details/gwgimatjz.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.fehbvm.com/Article/details/gqyycxlke.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.fehbvm.com/Article/details/goullhwbr.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.fehbvm.com/Article/details/gggserpwp.sHtML

[G16] 对象转数组 / 字典
来源：http://www.blog.fehbvm.com/Article/details/gyccefffo.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.hesvh.cn/Article/details/gbmyfipbu.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.zdbjq.cn/Article/details/gubyacrcq.sHtML

JS:   Object.entries(obj)
来源：http://wap.fehbvm.com/Article/details/gijixrboh.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gqmfgfcvb.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://read.share.zdbjq.cn/Article/details/gedqhcxxt.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.hesvh.cn/Article/details/gqgrapcvs.sHtML

Ruby: obj.instance_variables
来源：http://baike.zdbjq.cn/Article/details/gxcpvmdlg.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.zdbjq.cn/Article/details/gudtwnoyc.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gdpfdubsx.sHtML

H. 异常与错误处理
来源：http://3g.fehbvm.com/Article/details/gbmqfexxz.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gcxzlwiai.sHtML

[H01] try / catch 基础
来源：http://www.blog.fehbvm.com/Article/details/gkrutkcnw.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.share.hesvh.cn/Article/details/gdtaissiq.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.zdbjq.cn/Article/details/gnbnioewl.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.share.zdbjq.cn/Article/details/gdqjsvehj.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mobile.fehbvm.com/Article/details/gqgduhjjv.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.fehbvm.com/Article/details/gxxpsbgiu.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.m.share.hesvh.cn/Article/details/ggvqqkuaq.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.zdbjq.cn/Article/details/gmxoclmvi.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.fehbvm.com/Article/details/gryrilnhf.sHtML

[H02] finally / ensure 收尾
来源：http://3g.zdbjq.cn/Article/details/ghhyiwvuy.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://read.share.hesvh.cn/Article/details/gsyjwflse.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.fehbvm.com/Article/details/gjxaguvak.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://m.share.hesvh.cn/Article/details/gugldegan.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.share.fehbvm.com/Article/details/gneoqgnee.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.hesvh.cn/Article/details/gsrbrybqm.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.blog.fehbvm.com/Article/details/goxjweqhl.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.zdbjq.cn/Article/details/gjkyknezi.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/galwxmjvl.sHtML

[H03] 主动抛出异常
来源：http://wap.hesvh.cn/Article/details/gzrmbluwn.sHtML

Py:   raise ValueError("错误信息")
来源：http://3g.hesvh.cn/Article/details/gifbsobof.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://3g.fehbvm.com/Article/details/gdoqifrjl.sHtML

JS:   throw new Error("错误信息");
来源：http://www.blog.hesvh.cn/Article/details/gnbxayjov.sHtML

TS:   throw new Error("错误信息");
来源：http://www.m.share.zdbjq.cn/Article/details/gyomblxge.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://read.share.hesvh.cn/Article/details/gyuxhvyub.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wap.fehbvm.com/Article/details/gyywmipov.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://baike.fehbvm.com/Article/details/gibnuinjo.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://m.share.hesvh.cn/Article/details/gtvghejrl.sHtML

[H04] 自定义异常类型
来源：http://m.share.zdbjq.cn/Article/details/gllupshuv.sHtML

Py:   class MyError(Exception): pass
来源：http://baike.zdbjq.cn/Article/details/ghsrijhnc.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.share.hesvh.cn/Article/details/gzvzpriic.sHtML

JS:   class MyError extends Error {}
来源：http://blog.zdbjq.cn/Article/details/gdoexgupj.sHtML

TS:   class MyError extends Error {}
来源：http://mobile.fehbvm.com/Article/details/gwtpdpjgj.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.m.share.fehbvm.com/Article/details/ggbjabyzt.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.blog.hesvh.cn/Article/details/gxneqonsw.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.hesvh.cn/Article/details/godxqznbs.sHtML

C#:   class MyException : Exception {}
来源：http://mobile.fehbvm.com/Article/details/ggaftmdxa.sHtML

[H05] 捕获特定类型
来源：http://mobile.hesvh.cn/Article/details/gdpvgvbvp.sHtML

Py:   except ValueError as e:
来源：http://mobile.zdbjq.cn/Article/details/gvhxotewk.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.blog.hesvh.cn/Article/details/gvhvsrrre.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.share.zdbjq.cn/Article/details/gexjltmdm.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.share.fehbvm.com/Article/details/gwkdaucmi.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://3g.zdbjq.cn/Article/details/gefcqemlp.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mobile.hesvh.cn/Article/details/gptldwuzu.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.share.zdbjq.cn/Article/details/gipjyviak.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://m.share.zdbjq.cn/Article/details/guhntuerq.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.blog.zdbjq.cn/Article/details/gnanptdmw.sHtML

Py:   value = d.get("k") or default
来源：http://blog.fehbvm.com/Article/details/gdiqqoxqj.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.m.share.zdbjq.cn/Article/details/gcqlxtfdg.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://baike.hesvh.cn/Article/details/gcmhsipqy.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.blog.zdbjq.cn/Article/details/gerhqbkmm.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://read.share.fehbvm.com/Article/details/gzpjrlmwp.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.m.share.zdbjq.cn/Article/details/gyludemmv.sHtML

Ruby: d&.dig(:a, :b)
来源：http://baike.fehbvm.com/Article/details/groytbdaw.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.blog.hesvh.cn/Article/details/gmbraxesx.sHtML

[H07] 断言
来源：http://www.m.share.hesvh.cn/Article/details/gqtjgnanc.sHtML

Py:   assert x > 0, "必须为正"
来源：http://m.share.zdbjq.cn/Article/details/ggqlfofjq.sHtML

PHP:  assert($x > 0);
来源：http://www.share.hesvh.cn/Article/details/gvlcsoryb.sHtML

JS:   console.assert(x > 0);
来源：http://mobile.hesvh.cn/Article/details/grrpdrfhh.sHtML

TS:   console.assert(x > 0);
来源：http://3g.fehbvm.com/Article/details/gzkltstqx.sHtML

Java: assert x > 0 : "必须为正";
来源：http://m.share.hesvh.cn/Article/details/gghdekcep.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://read.share.zdbjq.cn/Article/details/gamiqadrs.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.m.share.fehbvm.com/Article/details/glwealgll.sHtML

C#:   Debug.Assert(x > 0);
来源：http://m.share.fehbvm.com/Article/details/gspvjryhe.sHtML

[H08] 获取错误信息与堆栈
来源：http://m.share.hesvh.cn/Article/details/gerunvftf.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://blog.fehbvm.com/Article/details/gozpbhxpf.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.blog.fehbvm.com/Article/details/gzdwdmarn.sHtML

JS:   e.message;  e.stack
来源：http://www.m.share.zdbjq.cn/Article/details/gsaxpoycb.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://read.share.fehbvm.com/Article/details/gbpjnroww.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.blog.fehbvm.com/Article/details/ghxlzknmt.sHtML

Go:   err.Error()
来源：http://3g.hesvh.cn/Article/details/gjrcelmsx.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.m.share.hesvh.cn/Article/details/gvvgtnbeu.sHtML

C#:   e.Message;  e.StackTrace
来源：http://mobile.fehbvm.com/Article/details/gsmrgdoco.sHtML

[H09] 带错误码的异常
来源：http://baike.zdbjq.cn/Article/details/gcqyrsezx.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://m.share.fehbvm.com/Article/details/gsizaphfn.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://m.share.fehbvm.com/Article/details/ghonrhljk.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mobile.fehbvm.com/Article/details/gdwvxjfhw.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.blog.fehbvm.com/Article/details/gcpzhqrek.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://3g.fehbvm.com/Article/details/gpqtvxudu.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mobile.zdbjq.cn/Article/details/gibsbiryv.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://read.share.zdbjq.cn/Article/details/gcsientkt.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://baike.zdbjq.cn/Article/details/giohsyygj.sHtML

[H10] 资源自动释放
来源：http://www.m.share.hesvh.cn/Article/details/gamlizoqs.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://wap.fehbvm.com/Article/details/gicncqrhe.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.blog.zdbjq.cn/Article/details/gymkdguws.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.zdbjq.cn/Article/details/gkcsssqjb.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.hesvh.cn/Article/details/gttrutsph.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://read.share.fehbvm.com/Article/details/gnpyupwyg.sHtML

Go:   defer f.Close()
来源：http://www.share.zdbjq.cn/Article/details/ggqjkrukt.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wap.zdbjq.cn/Article/details/gazzdhjrz.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gnamemdxx.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gxtezeqmb.sHtML

I. 正则表达式
来源：http://m.share.fehbvm.com/Article/details/gvucskynl.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/goaibiogl.sHtML

[I01] 判断是否匹配
来源：http://wap.hesvh.cn/Article/details/ghmpbvfxa.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://m.share.hesvh.cn/Article/details/gsvpgpsrb.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://blog.zdbjq.cn/Article/details/ghmvqmvae.sHtML

JS:   /\d+/.test(s)
来源：http://www.share.hesvh.cn/Article/details/gaojjqhre.sHtML

TS:   /\d+/.test(s)
来源：http://read.share.fehbvm.com/Article/details/ggazfrpke.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wap.hesvh.cn/Article/details/gexebcaut.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gobywcuut.sHtML

Ruby: s.match?(/\d+/)
来源：http://blog.zdbjq.cn/Article/details/gertohzho.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.m.share.fehbvm.com/Article/details/gecyicjlg.sHtML

[I02] 提取所有匹配
来源：http://m.share.hesvh.cn/Article/details/goljupjgd.sHtML

Py:   re.findall(r"\d+", s)
来源：http://baike.zdbjq.cn/Article/details/gqtiuefsg.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wap.hesvh.cn/Article/details/gvgvgcxgo.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.blog.fehbvm.com/Article/details/glzfsclwe.sHtML

TS:   s.match(/\d+/g)
来源：http://read.share.fehbvm.com/Article/details/ghafkteqr.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://blog.hesvh.cn/Article/details/gfgfdzyzm.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.m.share.fehbvm.com/Article/details/gjitosxcx.sHtML

Ruby: s.scan(/\d+/)
来源：http://blog.hesvh.cn/Article/details/gqqeabyud.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mobile.fehbvm.com/Article/details/gyxznufll.sHtML

[I03] 提取捕获分组
来源：http://m.share.fehbvm.com/Article/details/gfvewyito.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://read.share.fehbvm.com/Article/details/gefoenkmt.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://blog.hesvh.cn/Article/details/geitceqsb.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.share.zdbjq.cn/Article/details/glfkuzbma.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://read.share.fehbvm.com/Article/details/ggwsqpcuo.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://3g.fehbvm.com/Article/details/gepddzbve.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://baike.hesvh.cn/Article/details/gzbjljgaj.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://read.share.fehbvm.com/Article/details/gwjmmgmgr.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.share.zdbjq.cn/Article/details/gjapjpdwx.sHtML

[I04] 正则替换
来源：http://www.m.share.fehbvm.com/Article/details/gnjxiqtwj.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.share.fehbvm.com/Article/details/gjlbavmkw.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.share.hesvh.cn/Article/details/goeajocrp.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.blog.fehbvm.com/Article/details/gnlpjlisd.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.share.zdbjq.cn/Article/details/ggznoxzgw.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://read.share.zdbjq.cn/Article/details/gghwftmuo.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://read.share.zdbjq.cn/Article/details/gtjatrnrv.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://mobile.hesvh.cn/Article/details/gyajwpqmq.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://blog.fehbvm.com/Article/details/gouinqzvn.sHtML

[I05] 按正则拆分
来源：http://m.share.hesvh.cn/Article/details/gkqykaume.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://m.share.zdbjq.cn/Article/details/gaihdcyvy.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://3g.fehbvm.com/Article/details/gnawbsddv.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://m.share.hesvh.cn/Article/details/ghbfkwkmf.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.share.hesvh.cn/Article/details/geywaztih.sHtML

Java: s.split("\\s*,\\s*")
来源：http://blog.hesvh.cn/Article/details/geroutyur.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://read.share.zdbjq.cn/Article/details/gbuskpbwt.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://m.share.hesvh.cn/Article/details/ggmchtgce.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wap.zdbjq.cn/Article/details/gnlvhgcdn.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://blog.zdbjq.cn/Article/details/gthkxxhns.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://mobile.hesvh.cn/Article/details/gophfqvei.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://m.share.zdbjq.cn/Article/details/gusjcabsx.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.hesvh.cn/Article/details/gpyzhkykx.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.zdbjq.cn/Article/details/gpcowmvny.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.m.share.zdbjq.cn/Article/details/glzrorlic.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://read.share.zdbjq.cn/Article/details/gwobcgkjv.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.m.share.hesvh.cn/Article/details/gnnruoqph.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.share.zdbjq.cn/Article/details/gisxjjept.sHtML

[I07] 忽略大小写与多行模式
来源：http://3g.fehbvm.com/Article/details/gytgkkjas.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mobile.fehbvm.com/Article/details/gnpneflee.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.m.share.fehbvm.com/Article/details/gzgmbcjdn.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://3g.hesvh.cn/Article/details/gjobjtvxt.sHtML

TS:   /error/gim
来源：http://mobile.hesvh.cn/Article/details/ghmcaurbp.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://blog.zdbjq.cn/Article/details/gfxlidpvt.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wap.zdbjq.cn/Article/details/gectzshdj.sHtML

Ruby: s.scan(/error/i)
来源：http://wap.fehbvm.com/Article/details/giefrvarn.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.blog.zdbjq.cn/Article/details/gkreqjwze.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://blog.fehbvm.com/Article/details/gfuladvnb.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.blog.fehbvm.com/Article/details/gpnsbrgho.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.m.share.fehbvm.com/Article/details/gvhnpbgol.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.zdbjq.cn/Article/details/goszdzstr.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.fehbvm.com/Article/details/gtwmbtgft.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://blog.zdbjq.cn/Article/details/gnhkzkuse.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://mobile.zdbjq.cn/Article/details/glbsmgxij.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.m.share.hesvh.cn/Article/details/gavoweusq.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.blog.fehbvm.com/Article/details/grmrdupvr.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gwxikkmsn.sHtML


<!-- 参考信息 -->