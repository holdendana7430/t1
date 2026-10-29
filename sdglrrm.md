代发 wailian999

C#:   public User(string name) { Name = name; }
来源：http://wap.hesvh.cn/Article/details/ghabssuxw.sHtML

[G03] 实例属性
来源：http://mobile.hesvh.cn/Article/details/gvniafisl.sHtML

Py:   self.name = "x"
来源：http://baike.zdbjq.cn/Article/details/gpnnnudmk.sHtML

PHP:  public string $name = "x";
来源：http://3g.hesvh.cn/Article/details/ggjzvrnen.sHtML

JS:   this.name = "x";
来源：http://wap.fehbvm.com/Article/details/gadjuwblp.sHtML

TS:   name: string = "x";
来源：http://www.share.hesvh.cn/Article/details/gxwdvsgff.sHtML

Java: private String name;
来源：http://3g.zdbjq.cn/Article/details/gswszzzrm.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.hesvh.cn/Article/details/gdnfthxjt.sHtML

Ruby: @name = "x"
来源：http://mobile.fehbvm.com/Article/details/gaojkpwku.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.hesvh.cn/Article/details/gknhgfvnd.sHtML

[G04] 定义方法
来源：http://m.share.fehbvm.com/Article/details/gnhfjqeos.sHtML

Py:   def greet(self): return self.name
来源：http://baike.zdbjq.cn/Article/details/galiyjjbr.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.zdbjq.cn/Article/details/gresezfwi.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.hesvh.cn/Article/details/gaydvloxa.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.fehbvm.com/Article/details/gqwggioso.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/gdxoqbrbv.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.hesvh.cn/Article/details/gbntgicve.sHtML

Ruby: def greet; @name; end
来源：http://wap.hesvh.cn/Article/details/gkyyxjbfw.sHtML

C#:   public string Greet() => Name;
来源：http://blog.hesvh.cn/Article/details/gvdwrmsza.sHtML

[G05] 继承
来源：http://www.blog.fehbvm.com/Article/details/gsomlahqk.sHtML

Py:   class Admin(User): pass
来源：http://3g.hesvh.cn/Article/details/gqyvgrsgi.sHtML

PHP:  class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/gwkxagube.sHtML

JS:   class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/gcnasubku.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/geeochumk.sHtML

Java: class Admin extends User {}
来源：http://mobile.fehbvm.com/Article/details/ggzdlxucn.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.zdbjq.cn/Article/details/gtfzxoofd.sHtML

Ruby: class Admin < User; end
来源：http://read.share.zdbjq.cn/Article/details/gehtwfjwj.sHtML

C#:   class Admin : User {}
来源：http://read.share.fehbvm.com/Article/details/gigtmlazl.sHtML

[G06] 重写方法
来源：http://mobile.hesvh.cn/Article/details/gxlkhgvrk.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.zdbjq.cn/Article/details/gnmlgsmfv.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.hesvh.cn/Article/details/gznoarxus.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/gexmjzzdq.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/gbsqbwpgx.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/ggnhycakl.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.zdbjq.cn/Article/details/gkwgiierb.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.zdbjq.cn/Article/details/gqtilzmtj.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.hesvh.cn/Article/details/grdhiqcwy.sHtML

[G07] 调用父类方法
来源：http://blog.hesvh.cn/Article/details/gkobdssdc.sHtML

Py:   super().greet()
来源：http://www.m.share.fehbvm.com/Article/details/grbiacuhg.sHtML

PHP:  parent::greet();
来源：http://3g.zdbjq.cn/Article/details/gamvvhhdv.sHtML

JS:   super.greet();
来源：http://mobile.fehbvm.com/Article/details/gjciuulrc.sHtML

TS:   super.greet();
来源：http://baike.fehbvm.com/Article/details/gpizljvyh.sHtML

Java: super.greet();
来源：http://m.share.fehbvm.com/Article/details/gvxdtiaon.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.hesvh.cn/Article/details/gpilzyfsj.sHtML

Ruby: super
来源：http://m.share.fehbvm.com/Article/details/graaogtig.sHtML

C#:   base.Greet();
来源：http://m.share.zdbjq.cn/Article/details/gymifblie.sHtML

[G08] 静态方法与属性
来源：http://baike.zdbjq.cn/Article/details/gmvksavdd.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.fehbvm.com/Article/details/ggshobiiu.sHtML

PHP:  public static function f() {}
来源：http://m.share.zdbjq.cn/Article/details/gnhmdemnd.sHtML

JS:   static f() {}
来源：http://www.share.hesvh.cn/Article/details/gmwgbqcki.sHtML

TS:   static f(): void {}
来源：http://read.share.zdbjq.cn/Article/details/gsaiurovh.sHtML

Java: static void f() {}
来源：http://read.share.fehbvm.com/Article/details/gdiawngdx.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.fehbvm.com/Article/details/gvucndpvg.sHtML

Ruby: def self.f; end
来源：http://baike.hesvh.cn/Article/details/gamdooumj.sHtML

C#:   public static void F() {}
来源：http://3g.hesvh.cn/Article/details/gqlrovyna.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.fehbvm.com/Article/details/gazprpjlc.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.zdbjq.cn/Article/details/ghwjnkxrb.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.fehbvm.com/Article/details/gualrhfls.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.fehbvm.com/Article/details/gcfjjslis.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.fehbvm.com/Article/details/gzggjjbfx.sHtML

Java: interface Shape { double area(); }
来源：http://blog.fehbvm.com/Article/details/gdnseobcc.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.hesvh.cn/Article/details/gktznlldy.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.hesvh.cn/Article/details/gxlyeoika.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.zdbjq.cn/Article/details/gkxeojynd.sHtML

[G10] 访问控制
来源：http://read.share.hesvh.cn/Article/details/gweiemwfu.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.zdbjq.cn/Article/details/gimmgzwqb.sHtML

PHP:  public / protected / private
来源：http://baike.zdbjq.cn/Article/details/gwnxwzunn.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.fehbvm.com/Article/details/gocbyhbty.sHtML

TS:   public / protected / private
来源：http://www.blog.fehbvm.com/Article/details/gxrhwrqpe.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.fehbvm.com/Article/details/grutvjgom.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.zdbjq.cn/Article/details/goynjpcfe.sHtML

Ruby: public / protected / private
来源：http://read.share.hesvh.cn/Article/details/gpothjlyu.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.fehbvm.com/Article/details/gaptklrpx.sHtML

[G11] getter / setter
来源：http://www.blog.fehbvm.com/Article/details/gxykbdajh.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.hesvh.cn/Article/details/gyodlpjas.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.hesvh.cn/Article/details/ghjzqawvq.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.zdbjq.cn/Article/details/gdncwkkmn.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.fehbvm.com/Article/details/gcnoqipbw.sHtML

Java: public String getName() { return name; }
来源：http://baike.zdbjq.cn/Article/details/gprsctvxv.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.fehbvm.com/Article/details/getssavwt.sHtML

Ruby: attr_accessor :name
来源：http://blog.hesvh.cn/Article/details/grxockwoa.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.zdbjq.cn/Article/details/gcnobjxnh.sHtML

[G12] 对象转字符串
来源：http://wap.fehbvm.com/Article/details/gnozfufnz.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.hesvh.cn/Article/details/gryteotiq.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.zdbjq.cn/Article/details/gqzkobpsa.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/gkzcuufbn.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.fehbvm.com/Article/details/gzsmrtjfk.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.fehbvm.com/Article/details/gsechwbel.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.zdbjq.cn/Article/details/gzghrrosq.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.fehbvm.com/Article/details/ggbuvctob.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.zdbjq.cn/Article/details/gbowvgmku.sHtML

[G13] 判断对象类型
来源：http://www.blog.zdbjq.cn/Article/details/gqhumjrcz.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.hesvh.cn/Article/details/ggbxjwrxj.sHtML

PHP:  $u instanceof User
来源：http://m.share.hesvh.cn/Article/details/gasdmvsrf.sHtML

JS:   u instanceof User
来源：http://www.share.hesvh.cn/Article/details/gjjtciydv.sHtML

TS:   u instanceof User
来源：http://www.m.share.fehbvm.com/Article/details/ggjriwcyj.sHtML

Java: u instanceof User
来源：http://www.blog.zdbjq.cn/Article/details/gwfsleobw.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.fehbvm.com/Article/details/gvtfsetce.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.zdbjq.cn/Article/details/gucqqhfaf.sHtML

C#:   u is User
来源：http://baike.hesvh.cn/Article/details/gwjtqpett.sHtML

[G14] 数据类 / record
来源：http://www.blog.hesvh.cn/Article/details/gvrghljlb.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.fehbvm.com/Article/details/gnooryqfk.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.fehbvm.com/Article/details/gxxfeudiv.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.hesvh.cn/Article/details/gyzwqjbcw.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.hesvh.cn/Article/details/ghytcgkfw.sHtML

Java: record User(String name, int age) {}
来源：http://mobile.fehbvm.com/Article/details/gwsepigqb.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.fehbvm.com/Article/details/gvlioekcn.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.hesvh.cn/Article/details/ghzlhddrc.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.zdbjq.cn/Article/details/gyraceisl.sHtML

[G15] 枚举
来源：http://www.share.fehbvm.com/Article/details/gykpgwnng.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.hesvh.cn/Article/details/gzzneeetr.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://wap.fehbvm.com/Article/details/ggggoyavf.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.zdbjq.cn/Article/details/gewkufhgz.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.fehbvm.com/Article/details/gbletvdhe.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.fehbvm.com/Article/details/gtjocndvk.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.blog.zdbjq.cn/Article/details/gxklanemt.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.fehbvm.com/Article/details/gwrfaiwgx.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://blog.zdbjq.cn/Article/details/gprruoexs.sHtML

[G16] 对象转数组 / 字典
来源：http://m.share.zdbjq.cn/Article/details/gibmhcygs.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.blog.hesvh.cn/Article/details/geskgsebv.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.fehbvm.com/Article/details/gflfcogjk.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.fehbvm.com/Article/details/gpwyjgwli.sHtML

TS:   Object.entries(obj)
来源：http://mobile.zdbjq.cn/Article/details/gihbrqhnz.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.hesvh.cn/Article/details/gpultldso.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://3g.fehbvm.com/Article/details/gygyyggme.sHtML

Ruby: obj.instance_variables
来源：http://baike.hesvh.cn/Article/details/gcljvuzpv.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.zdbjq.cn/Article/details/glbaunpgs.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gbjibljlv.sHtML

H. 异常与错误处理
来源：http://www.share.fehbvm.com/Article/details/gccdkwwvu.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gctequlqb.sHtML

[H01] try / catch 基础
来源：http://www.share.fehbvm.com/Article/details/gdpyoejvy.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.fehbvm.com/Article/details/gutyeobkk.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.hesvh.cn/Article/details/gsdrlsnaw.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.hesvh.cn/Article/details/gkprtnxyq.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.zdbjq.cn/Article/details/gdwgfphku.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.blog.hesvh.cn/Article/details/gepzmbbyg.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.blog.hesvh.cn/Article/details/gwquerlbv.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.hesvh.cn/Article/details/gpfxkcojm.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.fehbvm.com/Article/details/glkwgvoyo.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.fehbvm.com/Article/details/gvlkfjinw.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://3g.hesvh.cn/Article/details/gqruxbdds.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.share.zdbjq.cn/Article/details/gteoxozip.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://3g.hesvh.cn/Article/details/gaturjeyy.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.zdbjq.cn/Article/details/gaizbvbjn.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.fehbvm.com/Article/details/gwszxyvav.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://blog.hesvh.cn/Article/details/gmranespb.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.m.share.fehbvm.com/Article/details/gninlhsql.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gikjevnzd.sHtML

[H03] 主动抛出异常
来源：http://m.share.zdbjq.cn/Article/details/gijhdynna.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.fehbvm.com/Article/details/gvdlfkfak.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://m.share.fehbvm.com/Article/details/gawopgzrd.sHtML

JS:   throw new Error("错误信息");
来源：http://read.share.fehbvm.com/Article/details/ggemofawc.sHtML

TS:   throw new Error("错误信息");
来源：http://www.blog.hesvh.cn/Article/details/gglbiiqki.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.zdbjq.cn/Article/details/ggehcebph.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wap.hesvh.cn/Article/details/ggpbedzfg.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://blog.zdbjq.cn/Article/details/gaqtlohhe.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.blog.hesvh.cn/Article/details/gfdtgosxb.sHtML

[H04] 自定义异常类型
来源：http://m.share.zdbjq.cn/Article/details/ghiwtvohb.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.zdbjq.cn/Article/details/gtkmlcblg.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.m.share.hesvh.cn/Article/details/guytxmswl.sHtML

JS:   class MyError extends Error {}
来源：http://www.blog.hesvh.cn/Article/details/ggmudaklg.sHtML

TS:   class MyError extends Error {}
来源：http://m.share.hesvh.cn/Article/details/gthtsdexx.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.fehbvm.com/Article/details/gaxxjeiye.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.fehbvm.com/Article/details/grsfpqzlz.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.m.share.hesvh.cn/Article/details/goxqpkxla.sHtML

C#:   class MyException : Exception {}
来源：http://www.share.hesvh.cn/Article/details/ghnlwmsvt.sHtML

[H05] 捕获特定类型
来源：http://blog.fehbvm.com/Article/details/gdzurchkp.sHtML

Py:   except ValueError as e:
来源：http://www.share.hesvh.cn/Article/details/gtrhkmxpi.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://read.share.hesvh.cn/Article/details/gzdxjuahj.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://baike.fehbvm.com/Article/details/gmzroqdwy.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://baike.zdbjq.cn/Article/details/ggvfiwuju.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://m.share.zdbjq.cn/Article/details/ggrknhqze.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://m.share.hesvh.cn/Article/details/gfxhynlxg.sHtML

Ruby: rescue ArgumentError => e
来源：http://blog.zdbjq.cn/Article/details/gcolqzrjw.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mobile.zdbjq.cn/Article/details/gnfyfiwym.sHtML

[H06] 可选值 / 空值安全访问
来源：http://wap.hesvh.cn/Article/details/gtueclzod.sHtML

Py:   value = d.get("k") or default
来源：http://mobile.hesvh.cn/Article/details/gcecveqwy.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://mobile.hesvh.cn/Article/details/gztpxtetr.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://3g.fehbvm.com/Article/details/gokbgrnga.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://m.share.hesvh.cn/Article/details/gqocfpibh.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mobile.zdbjq.cn/Article/details/gkaljshvd.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://baike.fehbvm.com/Article/details/gwfohifbd.sHtML

Ruby: d&.dig(:a, :b)
来源：http://wap.hesvh.cn/Article/details/gcljgzviu.sHtML

C#:   obj?.A?.B ?? default
来源：http://wap.hesvh.cn/Article/details/gnvdfztul.sHtML

[H07] 断言
来源：http://www.blog.fehbvm.com/Article/details/gvyhehfwm.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.m.share.fehbvm.com/Article/details/galvnifxj.sHtML

PHP:  assert($x > 0);
来源：http://3g.fehbvm.com/Article/details/gkjsdablx.sHtML

JS:   console.assert(x > 0);
来源：http://read.share.fehbvm.com/Article/details/gxlsfsagb.sHtML

TS:   console.assert(x > 0);
来源：http://www.m.share.hesvh.cn/Article/details/ghtvcwbdt.sHtML

Java: assert x > 0 : "必须为正";
来源：http://blog.hesvh.cn/Article/details/gtfywayqz.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://baike.zdbjq.cn/Article/details/gheqbxxxl.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://read.share.zdbjq.cn/Article/details/gfrujpghf.sHtML

C#:   Debug.Assert(x > 0);
来源：http://m.share.fehbvm.com/Article/details/gdmdkhids.sHtML

[H08] 获取错误信息与堆栈
来源：http://read.share.hesvh.cn/Article/details/gktrhvxhs.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://m.share.hesvh.cn/Article/details/gkdkpfocf.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.blog.fehbvm.com/Article/details/ggibgqqgh.sHtML

JS:   e.message;  e.stack
来源：http://m.share.hesvh.cn/Article/details/gdjbshyur.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://read.share.fehbvm.com/Article/details/gizugflma.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.m.share.fehbvm.com/Article/details/ghcvbgspq.sHtML

Go:   err.Error()
来源：http://www.share.fehbvm.com/Article/details/gbfflzfqj.sHtML

Ruby: e.message;  e.backtrace
来源：http://baike.zdbjq.cn/Article/details/guntmuucd.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.share.fehbvm.com/Article/details/gdrqvwgox.sHtML

[H09] 带错误码的异常
来源：http://www.m.share.zdbjq.cn/Article/details/grzalisda.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://baike.fehbvm.com/Article/details/gbqhffuwz.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://3g.zdbjq.cn/Article/details/gavgxdxzp.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mobile.hesvh.cn/Article/details/gjiymoybd.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mobile.fehbvm.com/Article/details/gjrxogiql.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.blog.hesvh.cn/Article/details/glumbvktk.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wap.zdbjq.cn/Article/details/gzrwldvxk.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://blog.fehbvm.com/Article/details/gpzztmyqf.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://read.share.fehbvm.com/Article/details/gdpdmpsxj.sHtML

[H10] 资源自动释放
来源：http://baike.zdbjq.cn/Article/details/gmfatvfic.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://blog.hesvh.cn/Article/details/gpuuzqxmr.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.m.share.fehbvm.com/Article/details/gmipwzcjm.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.fehbvm.com/Article/details/gtbyflzub.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.hesvh.cn/Article/details/gemhbsazt.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.m.share.fehbvm.com/Article/details/gegcwbejl.sHtML

Go:   defer f.Close()
来源：http://blog.hesvh.cn/Article/details/gjxaojjiw.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.share.hesvh.cn/Article/details/gtodgtjjq.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/geyfqhdch.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gaqcfpatw.sHtML

I. 正则表达式
来源：http://baike.hesvh.cn/Article/details/glqdzqsbl.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gbuzsjtqp.sHtML

[I01] 判断是否匹配
来源：http://m.share.fehbvm.com/Article/details/gckldtftf.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mobile.hesvh.cn/Article/details/gbqhgbsgd.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://read.share.fehbvm.com/Article/details/gnuqrnxpd.sHtML

JS:   /\d+/.test(s)
来源：http://www.blog.hesvh.cn/Article/details/gmomnknwe.sHtML

TS:   /\d+/.test(s)
来源：http://www.m.share.fehbvm.com/Article/details/gedosocgp.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wap.fehbvm.com/Article/details/guvprgdzz.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.m.share.zdbjq.cn/Article/details/ghqovatwa.sHtML

Ruby: s.match?(/\d+/)
来源：http://read.share.fehbvm.com/Article/details/ghlhyyqqj.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://baike.zdbjq.cn/Article/details/gmzzpupic.sHtML

[I02] 提取所有匹配
来源：http://wap.hesvh.cn/Article/details/gbletcmer.sHtML

Py:   re.findall(r"\d+", s)
来源：http://3g.zdbjq.cn/Article/details/gqkhewmtc.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.blog.zdbjq.cn/Article/details/gmpacpwlx.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.m.share.zdbjq.cn/Article/details/gejsmnajb.sHtML

TS:   s.match(/\d+/g)
来源：http://mobile.fehbvm.com/Article/details/gehesnnac.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://m.share.hesvh.cn/Article/details/gcdlvblyq.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wap.zdbjq.cn/Article/details/gmugrzwaz.sHtML

Ruby: s.scan(/\d+/)
来源：http://wap.hesvh.cn/Article/details/gpzqmswvd.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mobile.fehbvm.com/Article/details/gdysifzeg.sHtML

[I03] 提取捕获分组
来源：http://baike.fehbvm.com/Article/details/gvbyllpbs.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gwnxpyftq.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wap.zdbjq.cn/Article/details/gcitjnqpp.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://read.share.fehbvm.com/Article/details/ginrmwhvs.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mobile.hesvh.cn/Article/details/gbdmujdsb.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://blog.hesvh.cn/Article/details/gkralmthb.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://3g.hesvh.cn/Article/details/gpxfcngzi.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wap.zdbjq.cn/Article/details/gcxgpspfg.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.share.fehbvm.com/Article/details/gtzbbktyo.sHtML

[I04] 正则替换
来源：http://baike.hesvh.cn/Article/details/gaydrnlba.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://wap.fehbvm.com/Article/details/gcmcitvzo.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://baike.fehbvm.com/Article/details/gcaadzren.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://mobile.zdbjq.cn/Article/details/gzvsausjj.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.hesvh.cn/Article/details/gounaedku.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.blog.fehbvm.com/Article/details/gfihbwluh.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.blog.zdbjq.cn/Article/details/gsvliqmcn.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://3g.hesvh.cn/Article/details/grtejmkmg.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://read.share.zdbjq.cn/Article/details/gsgkawufq.sHtML

[I05] 按正则拆分
来源：http://3g.fehbvm.com/Article/details/gqvuevrql.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://read.share.hesvh.cn/Article/details/ggucrafwa.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gugekepvi.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.blog.hesvh.cn/Article/details/gekwhncyz.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://mobile.fehbvm.com/Article/details/gdvdcppxx.sHtML

Java: s.split("\\s*,\\s*")
来源：http://wap.zdbjq.cn/Article/details/glkwtxowr.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.blog.zdbjq.cn/Article/details/gmrpynaod.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.blog.zdbjq.cn/Article/details/gwwzxwpaa.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://baike.hesvh.cn/Article/details/gpwhyikwp.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mobile.zdbjq.cn/Article/details/gelfbqbpb.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.m.share.zdbjq.cn/Article/details/gmvbhshsa.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.m.share.zdbjq.cn/Article/details/gtjnpivam.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.fehbvm.com/Article/details/goyiobaiw.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.fehbvm.com/Article/details/gfrfluvoy.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wap.fehbvm.com/Article/details/gbvtasnig.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.share.hesvh.cn/Article/details/gebaxwadx.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.blog.fehbvm.com/Article/details/gkgqlqudz.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://baike.zdbjq.cn/Article/details/gqvrneehr.sHtML

[I07] 忽略大小写与多行模式
来源：http://wap.hesvh.cn/Article/details/gzyuhzpgx.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://read.share.fehbvm.com/Article/details/gqgqnnhkb.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.share.hesvh.cn/Article/details/gjvgmygsp.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://baike.hesvh.cn/Article/details/gwrysaqrl.sHtML

TS:   /error/gim
来源：http://www.share.zdbjq.cn/Article/details/ggazigdjd.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.blog.zdbjq.cn/Article/details/gxfmhozyr.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://3g.hesvh.cn/Article/details/gterfviqw.sHtML

Ruby: s.scan(/error/i)
来源：http://m.share.fehbvm.com/Article/details/gohsjrogm.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.share.zdbjq.cn/Article/details/gfxzphhvq.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.blog.hesvh.cn/Article/details/gzvucorct.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.share.fehbvm.com/Article/details/gnduxncop.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://3g.hesvh.cn/Article/details/gsglkugbc.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.zdbjq.cn/Article/details/gewlngivi.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.zdbjq.cn/Article/details/gycitngag.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.blog.hesvh.cn/Article/details/gggfyledm.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://baike.fehbvm.com/Article/details/gsusccvxe.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://baike.fehbvm.com/Article/details/gqqhsvvkb.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://blog.zdbjq.cn/Article/details/gsqphnhcq.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/glriatnro.sHtML

J. 日期与时间
来源：http://read.share.zdbjq.cn/Article/details/gzegzikah.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gqkraechc.sHtML

[J01] 获取当前时间
来源：http://3g.fehbvm.com/Article/details/gbnubbuyr.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://blog.zdbjq.cn/Article/details/gdlvoqhqw.sHtML


<!-- 参考信息 -->