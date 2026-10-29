代发 wailian999

C#:   public User(string name) { Name = name; }
来源：http://wap.fehbvm.com/Article/details/gwovfoftj.sHtML

[G03] 实例属性
来源：http://wap.hesvh.cn/Article/details/gwiwilojq.sHtML

Py:   self.name = "x"
来源：http://m.share.hesvh.cn/Article/details/gafitvmzi.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.fehbvm.com/Article/details/greopeeer.sHtML

JS:   this.name = "x";
来源：http://wap.hesvh.cn/Article/details/gameaqopy.sHtML

TS:   name: string = "x";
来源：http://www.share.zdbjq.cn/Article/details/gseynwpgh.sHtML

Java: private String name;
来源：http://wap.zdbjq.cn/Article/details/gcrqkrlxb.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.zdbjq.cn/Article/details/gkvqhavsu.sHtML

Ruby: @name = "x"
来源：http://www.blog.hesvh.cn/Article/details/glgjtmkam.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.fehbvm.com/Article/details/gzonntjzj.sHtML

[G04] 定义方法
来源：http://read.share.fehbvm.com/Article/details/gmvvxlmhx.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.hesvh.cn/Article/details/gejwvwzdi.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.hesvh.cn/Article/details/gairqlgyx.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/gekeylmky.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.hesvh.cn/Article/details/gphulnrbk.sHtML

Java: String greet() { return name; }
来源：http://baike.fehbvm.com/Article/details/ghtzgmxix.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.hesvh.cn/Article/details/gibrwnjbe.sHtML

Ruby: def greet; @name; end
来源：http://wap.hesvh.cn/Article/details/gctkxokhh.sHtML

C#:   public string Greet() => Name;
来源：http://3g.fehbvm.com/Article/details/gyxtuqljh.sHtML

[G05] 继承
来源：http://read.share.zdbjq.cn/Article/details/glnjtgbin.sHtML

Py:   class Admin(User): pass
来源：http://mobile.zdbjq.cn/Article/details/guhryalux.sHtML

PHP:  class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/gaqaconfv.sHtML

JS:   class Admin extends User {}
来源：http://mobile.fehbvm.com/Article/details/gghyainox.sHtML

TS:   class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/gvbaafwth.sHtML

Java: class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/gwpxagmge.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.hesvh.cn/Article/details/ggpajwbpm.sHtML

Ruby: class Admin < User; end
来源：http://read.share.hesvh.cn/Article/details/gnnisdyej.sHtML

C#:   class Admin : User {}
来源：http://www.share.fehbvm.com/Article/details/gvxuomtyi.sHtML

[G06] 重写方法
来源：http://read.share.hesvh.cn/Article/details/gdybzvbpo.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.zdbjq.cn/Article/details/grduxsnny.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/gvjnhvvyu.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.zdbjq.cn/Article/details/gycnrmawf.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/ghegwbusj.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/gvsfiosxy.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.zdbjq.cn/Article/details/gjadovjwu.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.hesvh.cn/Article/details/gcnvyuxob.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.zdbjq.cn/Article/details/gavcnfyit.sHtML

[G07] 调用父类方法
来源：http://read.share.zdbjq.cn/Article/details/gpgseptex.sHtML

Py:   super().greet()
来源：http://www.share.fehbvm.com/Article/details/grgxigjui.sHtML

PHP:  parent::greet();
来源：http://www.blog.fehbvm.com/Article/details/gsibwzdmo.sHtML

JS:   super.greet();
来源：http://mobile.fehbvm.com/Article/details/gayyhehra.sHtML

TS:   super.greet();
来源：http://baike.zdbjq.cn/Article/details/gcaiahcqw.sHtML

Java: super.greet();
来源：http://m.share.zdbjq.cn/Article/details/gsdoszlnc.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.zdbjq.cn/Article/details/gtmnphdoy.sHtML

Ruby: super
来源：http://m.share.hesvh.cn/Article/details/gloswsknk.sHtML

C#:   base.Greet();
来源：http://www.share.zdbjq.cn/Article/details/ggkhmjzbx.sHtML

[G08] 静态方法与属性
来源：http://3g.fehbvm.com/Article/details/ggydibymy.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.fehbvm.com/Article/details/gquofdosv.sHtML

PHP:  public static function f() {}
来源：http://wap.zdbjq.cn/Article/details/gichgulcr.sHtML

JS:   static f() {}
来源：http://wap.zdbjq.cn/Article/details/gpihuiiwx.sHtML

TS:   static f(): void {}
来源：http://www.share.zdbjq.cn/Article/details/gmpviyxov.sHtML

Java: static void f() {}
来源：http://3g.zdbjq.cn/Article/details/guznngjup.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.hesvh.cn/Article/details/gajuwisbc.sHtML

Ruby: def self.f; end
来源：http://blog.hesvh.cn/Article/details/gdjrqxucy.sHtML

C#:   public static void F() {}
来源：http://www.m.share.hesvh.cn/Article/details/gnydrjirs.sHtML

[G09] 接口 / 抽象类
来源：http://blog.hesvh.cn/Article/details/gsydnpyft.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.fehbvm.com/Article/details/gumyhbzzr.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.hesvh.cn/Article/details/gejbvelgt.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.hesvh.cn/Article/details/guxxpzjtj.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.hesvh.cn/Article/details/gssdjguoc.sHtML

Java: interface Shape { double area(); }
来源：http://3g.zdbjq.cn/Article/details/gcxobkvan.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.zdbjq.cn/Article/details/gmwexvnpy.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.zdbjq.cn/Article/details/gvxexdwov.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.zdbjq.cn/Article/details/gxujntfqz.sHtML

[G10] 访问控制
来源：http://read.share.fehbvm.com/Article/details/gqwhfkyrt.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.hesvh.cn/Article/details/gtsdykjfm.sHtML

PHP:  public / protected / private
来源：http://wap.hesvh.cn/Article/details/gilagakeh.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.fehbvm.com/Article/details/gfnyaxezk.sHtML

TS:   public / protected / private
来源：http://3g.zdbjq.cn/Article/details/gxxijtwbl.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.zdbjq.cn/Article/details/gchikiddm.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.fehbvm.com/Article/details/gbnduayqw.sHtML

Ruby: public / protected / private
来源：http://www.share.zdbjq.cn/Article/details/gkvbxrudc.sHtML

C#:   public / protected / private / internal
来源：http://www.share.fehbvm.com/Article/details/gtyrmydol.sHtML

[G11] getter / setter
来源：http://baike.zdbjq.cn/Article/details/goygudcuw.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.zdbjq.cn/Article/details/ghhoeuljv.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.hesvh.cn/Article/details/gvbhfcdjr.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.zdbjq.cn/Article/details/gmopckyaj.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.hesvh.cn/Article/details/gmwablbph.sHtML

Java: public String getName() { return name; }
来源：http://wap.fehbvm.com/Article/details/gwoaxrsos.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.zdbjq.cn/Article/details/ggplqoqyx.sHtML

Ruby: attr_accessor :name
来源：http://mobile.fehbvm.com/Article/details/gfcozulpl.sHtML

C#:   public string Name { get; set; }
来源：http://3g.zdbjq.cn/Article/details/gruvxhuzu.sHtML

[G12] 对象转字符串
来源：http://3g.hesvh.cn/Article/details/gqcbbpzld.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.zdbjq.cn/Article/details/gnsgrmacs.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.fehbvm.com/Article/details/gkeyguouo.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/gruvfgwvc.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/gvpviisru.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.zdbjq.cn/Article/details/gzmmecbxm.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.hesvh.cn/Article/details/gowlpvxvi.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.hesvh.cn/Article/details/gbhmepbvp.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.hesvh.cn/Article/details/gfpwxxcva.sHtML

[G13] 判断对象类型
来源：http://wap.zdbjq.cn/Article/details/gkubxgdpf.sHtML

Py:   isinstance(u, User)
来源：http://blog.fehbvm.com/Article/details/gkfxbuymz.sHtML

PHP:  $u instanceof User
来源：http://m.share.zdbjq.cn/Article/details/glruznlnv.sHtML

JS:   u instanceof User
来源：http://wap.hesvh.cn/Article/details/gzymvojkg.sHtML

TS:   u instanceof User
来源：http://www.share.fehbvm.com/Article/details/gypedpqnx.sHtML

Java: u instanceof User
来源：http://blog.hesvh.cn/Article/details/goprvdmpj.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.zdbjq.cn/Article/details/ghyabwctx.sHtML

Ruby: u.is_a?(User)
来源：http://3g.fehbvm.com/Article/details/gzthjpdzi.sHtML

C#:   u is User
来源：http://3g.hesvh.cn/Article/details/gxxjtehii.sHtML

[G14] 数据类 / record
来源：http://baike.zdbjq.cn/Article/details/gvuqoylrm.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.fehbvm.com/Article/details/gilzypvvs.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://read.share.hesvh.cn/Article/details/gjieblrgv.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.zdbjq.cn/Article/details/giusmrnkr.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.zdbjq.cn/Article/details/gwqfwqzsb.sHtML

Java: record User(String name, int age) {}
来源：http://wap.fehbvm.com/Article/details/gybhbjbtv.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.hesvh.cn/Article/details/gtcthqtbr.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.hesvh.cn/Article/details/gprxkynhw.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.zdbjq.cn/Article/details/gydgpjdyz.sHtML

[G15] 枚举
来源：http://baike.fehbvm.com/Article/details/gnvicfoib.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.fehbvm.com/Article/details/gfngnkltj.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.fehbvm.com/Article/details/gxujefpwh.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.zdbjq.cn/Article/details/gwsszmjdk.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.fehbvm.com/Article/details/gcdbqzzqn.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.zdbjq.cn/Article/details/giawansld.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.fehbvm.com/Article/details/gqjekytpj.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.fehbvm.com/Article/details/gtwcoogpt.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.zdbjq.cn/Article/details/gxilppscm.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.fehbvm.com/Article/details/gklccjumi.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://3g.hesvh.cn/Article/details/gbrbbnzxl.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.hesvh.cn/Article/details/gtqunsrsp.sHtML

JS:   Object.entries(obj)
来源：http://read.share.hesvh.cn/Article/details/gvomxdsob.sHtML

TS:   Object.entries(obj)
来源：http://wap.hesvh.cn/Article/details/gnanasudd.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.zdbjq.cn/Article/details/gjdbnvqso.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.fehbvm.com/Article/details/gfuxpkvco.sHtML

Ruby: obj.instance_variables
来源：http://www.m.share.zdbjq.cn/Article/details/gybifgswl.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.zdbjq.cn/Article/details/gntlkbsjy.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gihbagyva.sHtML

H. 异常与错误处理
来源：http://baike.fehbvm.com/Article/details/gcfbsqsjs.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gfdallgao.sHtML

[H01] try / catch 基础
来源：http://m.share.zdbjq.cn/Article/details/gwvcabcmm.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.fehbvm.com/Article/details/gjibdfqpv.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.fehbvm.com/Article/details/gcxmghhxb.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.blog.zdbjq.cn/Article/details/gxckegnax.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.hesvh.cn/Article/details/gnpeaypvq.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.zdbjq.cn/Article/details/ggagekmsb.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.m.share.hesvh.cn/Article/details/gjwgvjtyp.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.share.zdbjq.cn/Article/details/gahhojsgi.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://3g.hesvh.cn/Article/details/gxtashhbf.sHtML

[H02] finally / ensure 收尾
来源：http://baike.fehbvm.com/Article/details/gdmbjrncm.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://3g.fehbvm.com/Article/details/glmhdyhpn.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.share.fehbvm.com/Article/details/gkjwocmxf.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://wap.fehbvm.com/Article/details/gdqzrfjty.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://blog.zdbjq.cn/Article/details/grjgvdwtg.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://m.share.hesvh.cn/Article/details/gsclzkihn.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.share.zdbjq.cn/Article/details/gaqsdwwhb.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://blog.fehbvm.com/Article/details/gaaznnxeq.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://baike.hesvh.cn/Article/details/gyhgbrgzz.sHtML

[H03] 主动抛出异常
来源：http://wap.zdbjq.cn/Article/details/ggbbyrnib.sHtML

Py:   raise ValueError("错误信息")
来源：http://3g.zdbjq.cn/Article/details/gzmwnjrhb.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.zdbjq.cn/Article/details/gedzxffyl.sHtML

JS:   throw new Error("错误信息");
来源：http://www.share.fehbvm.com/Article/details/gybepzrfp.sHtML

TS:   throw new Error("错误信息");
来源：http://read.share.hesvh.cn/Article/details/glpqocwvh.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.fehbvm.com/Article/details/gxhfdunqw.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.hesvh.cn/Article/details/gwbgvlgoy.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://wap.hesvh.cn/Article/details/ghirbhysz.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.m.share.fehbvm.com/Article/details/gfrqfevnp.sHtML

[H04] 自定义异常类型
来源：http://baike.zdbjq.cn/Article/details/gzjhlnqeb.sHtML

Py:   class MyError(Exception): pass
来源：http://blog.zdbjq.cn/Article/details/gfvsvcuut.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.fehbvm.com/Article/details/gxueocjjm.sHtML

JS:   class MyError extends Error {}
来源：http://3g.zdbjq.cn/Article/details/ghpmuppmc.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.hesvh.cn/Article/details/gichakyxr.sHtML

Java: class MyException extends RuntimeException {}
来源：http://m.share.zdbjq.cn/Article/details/gzrgacpvj.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.zdbjq.cn/Article/details/ggkhnvpwv.sHtML

Ruby: class MyError < StandardError; end
来源：http://mobile.fehbvm.com/Article/details/gwzvqpkcq.sHtML

C#:   class MyException : Exception {}
来源：http://m.share.hesvh.cn/Article/details/gexctheum.sHtML

[H05] 捕获特定类型
来源：http://m.share.zdbjq.cn/Article/details/gljxtnhfs.sHtML

Py:   except ValueError as e:
来源：http://www.blog.hesvh.cn/Article/details/gelpslgzt.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://m.share.fehbvm.com/Article/details/gyvzmlxjf.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://wap.fehbvm.com/Article/details/gaftteunv.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://blog.fehbvm.com/Article/details/gjjbfsmqh.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://m.share.fehbvm.com/Article/details/gmpkfhwew.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://read.share.fehbvm.com/Article/details/ggyajkkft.sHtML

Ruby: rescue ArgumentError => e
来源：http://wap.hesvh.cn/Article/details/gzrszzwjy.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.m.share.fehbvm.com/Article/details/grzwqguti.sHtML

[H06] 可选值 / 空值安全访问
来源：http://baike.hesvh.cn/Article/details/gblifnrkf.sHtML

Py:   value = d.get("k") or default
来源：http://wap.hesvh.cn/Article/details/gjpcxbkzc.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.zdbjq.cn/Article/details/guorknhnn.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://wap.hesvh.cn/Article/details/gnbfbuygn.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://baike.fehbvm.com/Article/details/gaawezupu.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wap.hesvh.cn/Article/details/gdjreknkk.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://3g.zdbjq.cn/Article/details/ghykhsaxg.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.share.fehbvm.com/Article/details/guuqikjlr.sHtML

C#:   obj?.A?.B ?? default
来源：http://m.share.hesvh.cn/Article/details/gfgrypfcv.sHtML

[H07] 断言
来源：http://baike.hesvh.cn/Article/details/grtglccui.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.blog.zdbjq.cn/Article/details/gorvvskvl.sHtML

PHP:  assert($x > 0);
来源：http://blog.zdbjq.cn/Article/details/gumgfiudy.sHtML

JS:   console.assert(x > 0);
来源：http://www.share.hesvh.cn/Article/details/gezebfhva.sHtML

TS:   console.assert(x > 0);
来源：http://blog.hesvh.cn/Article/details/gjoiysdbv.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.hesvh.cn/Article/details/gxxkxlwch.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://3g.fehbvm.com/Article/details/gxrixhhqg.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://m.share.hesvh.cn/Article/details/gdcjcptjh.sHtML

C#:   Debug.Assert(x > 0);
来源：http://blog.zdbjq.cn/Article/details/gpcmejouj.sHtML

[H08] 获取错误信息与堆栈
来源：http://read.share.zdbjq.cn/Article/details/ghxbyjrci.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.m.share.fehbvm.com/Article/details/grmmiqjxj.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wap.hesvh.cn/Article/details/gtwmocotm.sHtML

JS:   e.message;  e.stack
来源：http://mobile.zdbjq.cn/Article/details/gzntyejgv.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://wap.fehbvm.com/Article/details/gnrgwgylu.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://wap.hesvh.cn/Article/details/gtleuukzj.sHtML

Go:   err.Error()
来源：http://baike.fehbvm.com/Article/details/gzqqhcqwc.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.share.hesvh.cn/Article/details/gpzwiogjf.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.blog.zdbjq.cn/Article/details/gqjozprlw.sHtML

[H09] 带错误码的异常
来源：http://wap.hesvh.cn/Article/details/gikyaztim.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mobile.hesvh.cn/Article/details/gbzykhmlp.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://m.share.fehbvm.com/Article/details/gppyoievh.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://m.share.fehbvm.com/Article/details/ggpvizsld.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wap.zdbjq.cn/Article/details/glmbhnkyi.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://m.share.hesvh.cn/Article/details/gtlzaizvh.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://blog.fehbvm.com/Article/details/gjyesqayq.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://m.share.zdbjq.cn/Article/details/gpgwdxcsq.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.share.zdbjq.cn/Article/details/gglexlarr.sHtML

[H10] 资源自动释放
来源：http://www.share.hesvh.cn/Article/details/gcbbmiaep.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://wap.zdbjq.cn/Article/details/gqnxshjpc.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://baike.zdbjq.cn/Article/details/gsnxcekiz.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.hesvh.cn/Article/details/gqzpquwln.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.fehbvm.com/Article/details/girnahmek.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://read.share.fehbvm.com/Article/details/gqfgrzogj.sHtML

Go:   defer f.Close()
来源：http://baike.hesvh.cn/Article/details/grvlmtvxl.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://read.share.hesvh.cn/Article/details/gtmgsmtkp.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gjdlhbjpa.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gnoxvquju.sHtML

I. 正则表达式
来源：http://www.m.share.hesvh.cn/Article/details/gtumbggfz.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gevvcipql.sHtML

[I01] 判断是否匹配
来源：http://www.blog.hesvh.cn/Article/details/gxfwgujyr.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://baike.zdbjq.cn/Article/details/glzlhfllm.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://mobile.fehbvm.com/Article/details/gfoginvac.sHtML

JS:   /\d+/.test(s)
来源：http://read.share.hesvh.cn/Article/details/ghygxnkpb.sHtML

TS:   /\d+/.test(s)
来源：http://www.share.hesvh.cn/Article/details/grrajybxe.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.share.fehbvm.com/Article/details/gtxmbewuw.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://m.share.zdbjq.cn/Article/details/gnhxhjtgy.sHtML

Ruby: s.match?(/\d+/)
来源：http://3g.fehbvm.com/Article/details/gzuxuhvzw.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wap.hesvh.cn/Article/details/gnrloaatx.sHtML

[I02] 提取所有匹配
来源：http://m.share.hesvh.cn/Article/details/gwysjyshm.sHtML

Py:   re.findall(r"\d+", s)
来源：http://read.share.zdbjq.cn/Article/details/gknhykqab.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://blog.zdbjq.cn/Article/details/gutlpibhl.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://read.share.zdbjq.cn/Article/details/gsxhmbnol.sHtML

TS:   s.match(/\d+/g)
来源：http://read.share.zdbjq.cn/Article/details/gbbieckuh.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://3g.hesvh.cn/Article/details/gwogoarui.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.blog.hesvh.cn/Article/details/gliwuurlq.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.blog.zdbjq.cn/Article/details/gufbdxnaz.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://3g.hesvh.cn/Article/details/glsiluibv.sHtML

[I03] 提取捕获分组
来源：http://www.blog.fehbvm.com/Article/details/gytiivnqz.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.m.share.hesvh.cn/Article/details/goodgipue.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wap.zdbjq.cn/Article/details/gydqvkufq.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.share.fehbvm.com/Article/details/guuczhaga.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://baike.hesvh.cn/Article/details/gtwnhxyod.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://mobile.zdbjq.cn/Article/details/gksaqtqkx.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://baike.hesvh.cn/Article/details/gldjyeetx.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.m.share.fehbvm.com/Article/details/gghpdpeuy.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://read.share.fehbvm.com/Article/details/gmaawhpiw.sHtML

[I04] 正则替换
来源：http://www.share.zdbjq.cn/Article/details/gjfspqnck.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.blog.zdbjq.cn/Article/details/galhjxwac.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://blog.fehbvm.com/Article/details/gbujijvxd.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://read.share.fehbvm.com/Article/details/gwvqncyeo.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://3g.fehbvm.com/Article/details/gejdvheaf.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.m.share.zdbjq.cn/Article/details/goqslncyv.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.m.share.hesvh.cn/Article/details/gpzhgvhrp.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://baike.zdbjq.cn/Article/details/gbfqssfqu.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.m.share.hesvh.cn/Article/details/gctkbqhtb.sHtML

[I05] 按正则拆分
来源：http://3g.fehbvm.com/Article/details/gtblaofcg.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.blog.fehbvm.com/Article/details/ggeoztilx.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://blog.zdbjq.cn/Article/details/gupgjfbsm.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://wap.hesvh.cn/Article/details/gjonyiqec.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://wap.fehbvm.com/Article/details/gvxhnjwxg.sHtML

Java: s.split("\\s*,\\s*")
来源：http://baike.hesvh.cn/Article/details/ghfwztlyg.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://blog.zdbjq.cn/Article/details/gtvdxjbib.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://baike.fehbvm.com/Article/details/gwslvlccp.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://3g.fehbvm.com/Article/details/gfxlggqze.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://m.share.zdbjq.cn/Article/details/gmapklttj.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.m.share.hesvh.cn/Article/details/gvimodtlg.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://3g.zdbjq.cn/Article/details/gslzeauwu.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.fehbvm.com/Article/details/gdwxyncph.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.zdbjq.cn/Article/details/gwjrswedz.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://read.share.hesvh.cn/Article/details/gsxbycwgt.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://baike.zdbjq.cn/Article/details/gyxexocex.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wap.hesvh.cn/Article/details/gbmmlbdgj.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://read.share.fehbvm.com/Article/details/gjwltikwx.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.blog.hesvh.cn/Article/details/ggdgkmgvp.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.m.share.hesvh.cn/Article/details/gnpeqgejg.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.blog.hesvh.cn/Article/details/gtuzgxzbt.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://3g.fehbvm.com/Article/details/giusgdlxa.sHtML

TS:   /error/gim
来源：http://read.share.zdbjq.cn/Article/details/gccskfcsf.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://baike.zdbjq.cn/Article/details/geovvkwgx.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://m.share.zdbjq.cn/Article/details/ghkpgfdkg.sHtML

Ruby: s.scan(/error/i)
来源：http://blog.fehbvm.com/Article/details/gzybnplsh.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.m.share.hesvh.cn/Article/details/gcefqbhke.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://3g.fehbvm.com/Article/details/gfpyhblqn.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://baike.hesvh.cn/Article/details/gnvczzigt.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wap.hesvh.cn/Article/details/gplamazei.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.hesvh.cn/Article/details/gmbdawmti.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.hesvh.cn/Article/details/gfzwaftig.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://read.share.zdbjq.cn/Article/details/gcinttvcg.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://read.share.zdbjq.cn/Article/details/gzfnlapcf.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wap.hesvh.cn/Article/details/gccjhmqdt.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wap.hesvh.cn/Article/details/gidjaoqns.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gsuawykxc.sHtML

J. 日期与时间
来源：http://www.blog.zdbjq.cn/Article/details/goevcxgiv.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gdpidilfl.sHtML

[J01] 获取当前时间
来源：http://3g.zdbjq.cn/Article/details/gfuxagnky.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://baike.fehbvm.com/Article/details/gyiwntkby.sHtML


<!-- 参考信息 -->