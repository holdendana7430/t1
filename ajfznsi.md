代发 wailian999

JS:   this.name = "x";
来源：http://mobile.fehbvm.com/Article/details/gfzxxndlu.sHtML

TS:   name: string = "x";
来源：http://m.share.zdbjq.cn/Article/details/gucmknhwy.sHtML

Java: private String name;
来源：http://wap.hesvh.cn/Article/details/gkhefubmy.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.zdbjq.cn/Article/details/ggelmdmsh.sHtML

Ruby: @name = "x"
来源：http://www.m.share.zdbjq.cn/Article/details/gvilpfypm.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.zdbjq.cn/Article/details/gxahnpmpi.sHtML

[G04] 定义方法
来源：http://m.share.fehbvm.com/Article/details/gphsrbeji.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.hesvh.cn/Article/details/glskbfnwe.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.zdbjq.cn/Article/details/gfbkeiwpa.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.zdbjq.cn/Article/details/gmydzkjwd.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/gwrnxcmxz.sHtML

Java: String greet() { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gpxaujagn.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.zdbjq.cn/Article/details/gfjxhvgaz.sHtML

Ruby: def greet; @name; end
来源：http://read.share.fehbvm.com/Article/details/gnunzsqom.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.fehbvm.com/Article/details/gzbjuqztx.sHtML

[G05] 继承
来源：http://mobile.zdbjq.cn/Article/details/gkrazvggt.sHtML

Py:   class Admin(User): pass
来源：http://read.share.fehbvm.com/Article/details/gnztcgrst.sHtML

PHP:  class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/gzruoivmv.sHtML

JS:   class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/gdudzsucq.sHtML

TS:   class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/ghmguackq.sHtML

Java: class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/gvybejzzr.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://baike.hesvh.cn/Article/details/goidwjnkq.sHtML

Ruby: class Admin < User; end
来源：http://baike.fehbvm.com/Article/details/gkyyagdnb.sHtML

C#:   class Admin : User {}
来源：http://blog.fehbvm.com/Article/details/gcomhmbfs.sHtML

[G06] 重写方法
来源：http://read.share.hesvh.cn/Article/details/glwgkbdyf.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.hesvh.cn/Article/details/gzjfzrcjl.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/gvzmbaueq.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/gpthnnpkv.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/gfmgvwklj.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/gcprjtehm.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.hesvh.cn/Article/details/gvozwhnhy.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.fehbvm.com/Article/details/gjlkujcvn.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.fehbvm.com/Article/details/gpsaktmmo.sHtML

[G07] 调用父类方法
来源：http://mobile.hesvh.cn/Article/details/gwnazldcd.sHtML

Py:   super().greet()
来源：http://m.share.hesvh.cn/Article/details/gzgpuibcl.sHtML

PHP:  parent::greet();
来源：http://mobile.fehbvm.com/Article/details/gzlcdejug.sHtML

JS:   super.greet();
来源：http://baike.fehbvm.com/Article/details/gzcrvllgi.sHtML

TS:   super.greet();
来源：http://www.share.hesvh.cn/Article/details/gmtgjkjxe.sHtML

Java: super.greet();
来源：http://blog.fehbvm.com/Article/details/gwbuxdntw.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.hesvh.cn/Article/details/gwwtwxehu.sHtML

Ruby: super
来源：http://3g.zdbjq.cn/Article/details/ggsajbfdr.sHtML

C#:   base.Greet();
来源：http://mobile.fehbvm.com/Article/details/gzlvrowfu.sHtML

[G08] 静态方法与属性
来源：http://read.share.zdbjq.cn/Article/details/gdfwssgxm.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.fehbvm.com/Article/details/gnubolkrz.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.zdbjq.cn/Article/details/gpqztzwax.sHtML

JS:   static f() {}
来源：http://mobile.zdbjq.cn/Article/details/gkeuhcuba.sHtML

TS:   static f(): void {}
来源：http://m.share.hesvh.cn/Article/details/gvemrvvdq.sHtML

Java: static void f() {}
来源：http://3g.zdbjq.cn/Article/details/gmngdbtde.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.fehbvm.com/Article/details/gnxjsmlsx.sHtML

Ruby: def self.f; end
来源：http://wap.hesvh.cn/Article/details/ghdfhwdnh.sHtML

C#:   public static void F() {}
来源：http://mobile.hesvh.cn/Article/details/gzbikjaso.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.hesvh.cn/Article/details/gwjeuvlth.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.zdbjq.cn/Article/details/gkttbdlnl.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.fehbvm.com/Article/details/geirhkgax.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.fehbvm.com/Article/details/gkzzdmlku.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.zdbjq.cn/Article/details/gxnciwwok.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.hesvh.cn/Article/details/gbgqzrbxl.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.fehbvm.com/Article/details/gkpqxcioo.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.fehbvm.com/Article/details/gqyvzskfl.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.hesvh.cn/Article/details/gdowmujmt.sHtML

[G10] 访问控制
来源：http://3g.hesvh.cn/Article/details/geweztqyu.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.zdbjq.cn/Article/details/gtxieqgop.sHtML

PHP:  public / protected / private
来源：http://wap.fehbvm.com/Article/details/gxavpmuih.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.hesvh.cn/Article/details/gpyhnmstp.sHtML

TS:   public / protected / private
来源：http://read.share.hesvh.cn/Article/details/gwaacbhkg.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.hesvh.cn/Article/details/gtnaqhxrk.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.zdbjq.cn/Article/details/gindxehxo.sHtML

Ruby: public / protected / private
来源：http://www.share.fehbvm.com/Article/details/gktlitfce.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.hesvh.cn/Article/details/gvrdkjuew.sHtML

[G11] getter / setter
来源：http://m.share.fehbvm.com/Article/details/govnuqcmc.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.hesvh.cn/Article/details/gnhsqcaat.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.zdbjq.cn/Article/details/gktjrujls.sHtML

JS:   get name() { return this._name; }
来源：http://blog.hesvh.cn/Article/details/gxocmxyde.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.hesvh.cn/Article/details/gmctskfai.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.fehbvm.com/Article/details/gjcoezttg.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.zdbjq.cn/Article/details/ghyvimzxz.sHtML

Ruby: attr_accessor :name
来源：http://mobile.zdbjq.cn/Article/details/gxggrxreu.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.zdbjq.cn/Article/details/gsxipcxha.sHtML

[G12] 对象转字符串
来源：http://3g.zdbjq.cn/Article/details/gxlcnloyo.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.fehbvm.com/Article/details/gnnparkkj.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.hesvh.cn/Article/details/gnxgpmxxt.sHtML

JS:   toString() { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/ghlnpexny.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.fehbvm.com/Article/details/gmkylmxoh.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/gzppmvwjh.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.zdbjq.cn/Article/details/gvsbticnk.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.fehbvm.com/Article/details/gjkvyspep.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.zdbjq.cn/Article/details/gheprslld.sHtML

[G13] 判断对象类型
来源：http://www.share.zdbjq.cn/Article/details/gxnsugjlo.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.fehbvm.com/Article/details/gzxaqekfo.sHtML

PHP:  $u instanceof User
来源：http://3g.hesvh.cn/Article/details/gzsfnpahe.sHtML

JS:   u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/gkfdvmbca.sHtML

TS:   u instanceof User
来源：http://mobile.fehbvm.com/Article/details/goiishsfx.sHtML

Java: u instanceof User
来源：http://mobile.fehbvm.com/Article/details/gmthyymul.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.fehbvm.com/Article/details/goupwvirj.sHtML

Ruby: u.is_a?(User)
来源：http://baike.zdbjq.cn/Article/details/gshzcyclx.sHtML

C#:   u is User
来源：http://www.blog.fehbvm.com/Article/details/gbnzmuwpn.sHtML

[G14] 数据类 / record
来源：http://3g.fehbvm.com/Article/details/gifqcdmei.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.zdbjq.cn/Article/details/gjkpsyqum.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.hesvh.cn/Article/details/gyyvinoeg.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.zdbjq.cn/Article/details/gmmczpddy.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.hesvh.cn/Article/details/gohqzawad.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.zdbjq.cn/Article/details/gilyrsqwd.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.hesvh.cn/Article/details/gffgkccol.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.hesvh.cn/Article/details/gdsyfqesj.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.hesvh.cn/Article/details/gqfegbjwu.sHtML

[G15] 枚举
来源：http://blog.fehbvm.com/Article/details/gmvpvbgsi.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.hesvh.cn/Article/details/gtfwooiiz.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.zdbjq.cn/Article/details/gkvhafgkk.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.fehbvm.com/Article/details/gvmspcmve.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.hesvh.cn/Article/details/gdvsrspkl.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.fehbvm.com/Article/details/gfqtyovvy.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://baike.fehbvm.com/Article/details/gbqlkgmhp.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.zdbjq.cn/Article/details/gcvcyaegp.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.hesvh.cn/Article/details/giourfvrp.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.zdbjq.cn/Article/details/gcufmobtx.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.blog.fehbvm.com/Article/details/ggmbahodc.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.zdbjq.cn/Article/details/gidsuekum.sHtML

JS:   Object.entries(obj)
来源：http://mobile.fehbvm.com/Article/details/gbdzrfbgr.sHtML

TS:   Object.entries(obj)
来源：http://mobile.zdbjq.cn/Article/details/gicedxkli.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.fehbvm.com/Article/details/gdztrwigc.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.zdbjq.cn/Article/details/gtyfgzqjl.sHtML

Ruby: obj.instance_variables
来源：http://www.share.fehbvm.com/Article/details/gorlpebbj.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://blog.zdbjq.cn/Article/details/gwgsckcqw.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/grrwrqpim.sHtML

H. 异常与错误处理
来源：http://www.blog.zdbjq.cn/Article/details/ggsdamlxd.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gczpcacxx.sHtML

[H01] try / catch 基础
来源：http://www.m.share.zdbjq.cn/Article/details/gkqokgtua.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.zdbjq.cn/Article/details/gkhmdcmqg.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mobile.hesvh.cn/Article/details/givxwdnjg.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://m.share.hesvh.cn/Article/details/gbvziwfis.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.fehbvm.com/Article/details/gnukfgvsn.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.m.share.zdbjq.cn/Article/details/gjnxbcwka.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.fehbvm.com/Article/details/ggkirvqmo.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wap.hesvh.cn/Article/details/glydpebeb.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://baike.fehbvm.com/Article/details/gicscusov.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.hesvh.cn/Article/details/gblrbuucj.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.fehbvm.com/Article/details/gatglazij.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/ghcgtadfp.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/gpkbkvdpz.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.share.fehbvm.com/Article/details/gcddlsphq.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/gkqjgkzfs.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://3g.hesvh.cn/Article/details/gvefbapkj.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.fehbvm.com/Article/details/geqymwwfv.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://m.share.fehbvm.com/Article/details/gwpshnycs.sHtML

[H03] 主动抛出异常
来源：http://www.blog.fehbvm.com/Article/details/glzsxkrzj.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.share.zdbjq.cn/Article/details/ggmxuvcvp.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://m.share.zdbjq.cn/Article/details/gyymopgzg.sHtML

JS:   throw new Error("错误信息");
来源：http://www.m.share.hesvh.cn/Article/details/gmecmavat.sHtML

TS:   throw new Error("错误信息");
来源：http://www.share.fehbvm.com/Article/details/gpanhfugf.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.hesvh.cn/Article/details/gmifcrmmh.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mobile.fehbvm.com/Article/details/gncuhoyzf.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://wap.zdbjq.cn/Article/details/gbxflebgd.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://blog.hesvh.cn/Article/details/gvxuqdhfv.sHtML

[H04] 自定义异常类型
来源：http://baike.zdbjq.cn/Article/details/geasxuuea.sHtML

Py:   class MyError(Exception): pass
来源：http://3g.zdbjq.cn/Article/details/gtdqkzqpe.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://blog.fehbvm.com/Article/details/ggbvdsngm.sHtML

JS:   class MyError extends Error {}
来源：http://3g.fehbvm.com/Article/details/gchpxfmgd.sHtML

TS:   class MyError extends Error {}
来源：http://baike.hesvh.cn/Article/details/gppxgoikg.sHtML

Java: class MyException extends RuntimeException {}
来源：http://mobile.fehbvm.com/Article/details/gmtqvirkx.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mobile.fehbvm.com/Article/details/groiijjsj.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.m.share.zdbjq.cn/Article/details/ggynksphf.sHtML

C#:   class MyException : Exception {}
来源：http://blog.hesvh.cn/Article/details/gvmipsfkw.sHtML

[H05] 捕获特定类型
来源：http://read.share.zdbjq.cn/Article/details/gikpfzetm.sHtML

Py:   except ValueError as e:
来源：http://read.share.fehbvm.com/Article/details/gwrvpysbj.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://m.share.hesvh.cn/Article/details/gbndfinde.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://read.share.fehbvm.com/Article/details/gqdidmntt.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://mobile.hesvh.cn/Article/details/gryixawxy.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://3g.fehbvm.com/Article/details/gvwjvezyv.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.blog.fehbvm.com/Article/details/gupztybkk.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.m.share.fehbvm.com/Article/details/gvndtvekd.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.blog.hesvh.cn/Article/details/gulbhgjay.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.blog.hesvh.cn/Article/details/gfuulddth.sHtML

Py:   value = d.get("k") or default
来源：http://www.m.share.hesvh.cn/Article/details/gcyhhogom.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.m.share.fehbvm.com/Article/details/grfgzpmhk.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://baike.hesvh.cn/Article/details/givprtvoy.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://baike.hesvh.cn/Article/details/gfxuqqrpr.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://blog.fehbvm.com/Article/details/gklghpvpn.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://mobile.fehbvm.com/Article/details/gqvrctfmy.sHtML

Ruby: d&.dig(:a, :b)
来源：http://wap.zdbjq.cn/Article/details/gsqvwcvks.sHtML

C#:   obj?.A?.B ?? default
来源：http://m.share.fehbvm.com/Article/details/gnohjrbiw.sHtML

[H07] 断言
来源：http://www.blog.fehbvm.com/Article/details/gfvpsosgf.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.blog.zdbjq.cn/Article/details/gijrpeqfp.sHtML

PHP:  assert($x > 0);
来源：http://3g.hesvh.cn/Article/details/gohinhsqk.sHtML

JS:   console.assert(x > 0);
来源：http://www.share.zdbjq.cn/Article/details/gpmxxpatw.sHtML

TS:   console.assert(x > 0);
来源：http://mobile.hesvh.cn/Article/details/gvojrnuvg.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.share.hesvh.cn/Article/details/glaxbspqu.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://3g.fehbvm.com/Article/details/gskckccsk.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://baike.zdbjq.cn/Article/details/gajnbolqn.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.share.hesvh.cn/Article/details/grpgfxbae.sHtML

[H08] 获取错误信息与堆栈
来源：http://read.share.hesvh.cn/Article/details/gelydtrdi.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.share.zdbjq.cn/Article/details/gtsvllecu.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://3g.hesvh.cn/Article/details/gbtvouhjv.sHtML

JS:   e.message;  e.stack
来源：http://m.share.zdbjq.cn/Article/details/grnbhqogo.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://baike.fehbvm.com/Article/details/gbjbtujqb.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://mobile.zdbjq.cn/Article/details/ganbjkhvd.sHtML

Go:   err.Error()
来源：http://m.share.hesvh.cn/Article/details/gkicfdtgn.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.m.share.fehbvm.com/Article/details/gjzbmkixs.sHtML

C#:   e.Message;  e.StackTrace
来源：http://read.share.fehbvm.com/Article/details/gjoihrxwb.sHtML

[H09] 带错误码的异常
来源：http://read.share.hesvh.cn/Article/details/guzexkyja.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.m.share.fehbvm.com/Article/details/gnkonibhl.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://wap.fehbvm.com/Article/details/gtelvapuw.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://m.share.zdbjq.cn/Article/details/gyuwnwkkc.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://m.share.fehbvm.com/Article/details/gbotbnkap.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://read.share.fehbvm.com/Article/details/gqmugtjan.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://read.share.hesvh.cn/Article/details/gwzifupct.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.m.share.hesvh.cn/Article/details/gbaiudzwh.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.share.fehbvm.com/Article/details/grlyuyvyk.sHtML

[H10] 资源自动释放
来源：http://www.blog.zdbjq.cn/Article/details/gqwhbjjnf.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.blog.hesvh.cn/Article/details/gzqdjzvcj.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://m.share.fehbvm.com/Article/details/gkcepqcqx.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.fehbvm.com/Article/details/ggupelypd.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.fehbvm.com/Article/details/gnwzpinga.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.m.share.zdbjq.cn/Article/details/gpzrkfdhz.sHtML

Go:   defer f.Close()
来源：http://read.share.zdbjq.cn/Article/details/gvbldvick.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://3g.fehbvm.com/Article/details/gwrgqycxv.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://baike.hesvh.cn/Article/details/gjwpwqcib.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/ghytufhky.sHtML

I. 正则表达式
来源：http://www.share.zdbjq.cn/Article/details/gawveoxkt.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gypfqqqag.sHtML

[I01] 判断是否匹配
来源：http://read.share.zdbjq.cn/Article/details/gstewkmrv.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://read.share.fehbvm.com/Article/details/gaxpwpfgg.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.m.share.fehbvm.com/Article/details/gqyhrteam.sHtML

JS:   /\d+/.test(s)
来源：http://wap.zdbjq.cn/Article/details/gdftbyyrv.sHtML

TS:   /\d+/.test(s)
来源：http://www.m.share.fehbvm.com/Article/details/gcvdersjm.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.share.zdbjq.cn/Article/details/gdflcvitb.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://m.share.fehbvm.com/Article/details/gvjltmmzx.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.share.hesvh.cn/Article/details/gozcmgddf.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wap.zdbjq.cn/Article/details/gqiaaqneg.sHtML

[I02] 提取所有匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gvvlvgmep.sHtML

Py:   re.findall(r"\d+", s)
来源：http://read.share.hesvh.cn/Article/details/gqlrhzdxc.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.blog.hesvh.cn/Article/details/gbdkrrfwn.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.blog.fehbvm.com/Article/details/grbtwrueb.sHtML

TS:   s.match(/\d+/g)
来源：http://3g.zdbjq.cn/Article/details/gisokxsgi.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wap.fehbvm.com/Article/details/guudltgke.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://3g.hesvh.cn/Article/details/gwinpssgq.sHtML

Ruby: s.scan(/\d+/)
来源：http://3g.hesvh.cn/Article/details/gizpkdids.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://read.share.hesvh.cn/Article/details/gxyvtvxrb.sHtML

[I03] 提取捕获分组
来源：http://www.blog.hesvh.cn/Article/details/greyrtvqi.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://baike.zdbjq.cn/Article/details/gcllncnby.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://3g.fehbvm.com/Article/details/gdzjufrtm.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.m.share.hesvh.cn/Article/details/gyooubfdo.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://read.share.fehbvm.com/Article/details/gcpvyiean.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://mobile.fehbvm.com/Article/details/gvlipzupy.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://m.share.zdbjq.cn/Article/details/gacftwquf.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://m.share.hesvh.cn/Article/details/gzxqgxlaq.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://3g.fehbvm.com/Article/details/gpvcsvvun.sHtML

[I04] 正则替换
来源：http://www.share.zdbjq.cn/Article/details/gkgdebbvh.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://mobile.hesvh.cn/Article/details/ggwumkfoq.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://baike.fehbvm.com/Article/details/gxeqrhaso.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://wap.hesvh.cn/Article/details/gtrakjlps.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://wap.zdbjq.cn/Article/details/gxjkhnong.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.share.zdbjq.cn/Article/details/gsrdxuxrx.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://3g.fehbvm.com/Article/details/giyfjoezo.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://m.share.hesvh.cn/Article/details/gzwvfxfig.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.blog.fehbvm.com/Article/details/gmffvddtk.sHtML

[I05] 按正则拆分
来源：http://wap.hesvh.cn/Article/details/gihcsnqqi.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://3g.hesvh.cn/Article/details/gilzoklay.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://read.share.fehbvm.com/Article/details/gsorbtajp.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.share.hesvh.cn/Article/details/gbzfhgqui.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.m.share.zdbjq.cn/Article/details/ggrlecgpg.sHtML

Java: s.split("\\s*,\\s*")
来源：http://wap.hesvh.cn/Article/details/ggxsdwgec.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://mobile.zdbjq.cn/Article/details/gyvufgysh.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://3g.zdbjq.cn/Article/details/gbjcfmnxx.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://read.share.hesvh.cn/Article/details/gtscyopmq.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.share.hesvh.cn/Article/details/gvncjmryu.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.share.fehbvm.com/Article/details/gagzptjjd.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.blog.zdbjq.cn/Article/details/gaczgtlzg.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.hesvh.cn/Article/details/gsblnonby.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.hesvh.cn/Article/details/gpfxmtpuj.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mobile.zdbjq.cn/Article/details/gjgnzgiao.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://m.share.zdbjq.cn/Article/details/gtnkjqlyf.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wap.hesvh.cn/Article/details/gyuuhkizr.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.m.share.fehbvm.com/Article/details/graauvpcx.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.share.hesvh.cn/Article/details/gazywjaax.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://baike.hesvh.cn/Article/details/gdyiufoqd.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.blog.fehbvm.com/Article/details/gakmortlq.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://3g.fehbvm.com/Article/details/gxljljebh.sHtML

TS:   /error/gim
来源：http://mobile.hesvh.cn/Article/details/gkjdtnvjb.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://blog.zdbjq.cn/Article/details/gtdhuhvhl.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.share.fehbvm.com/Article/details/gxpdtvhdj.sHtML

Ruby: s.scan(/error/i)
来源：http://3g.hesvh.cn/Article/details/gopdvceka.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mobile.zdbjq.cn/Article/details/gkcaugkqt.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.share.hesvh.cn/Article/details/gxjfkwmvu.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mobile.hesvh.cn/Article/details/gzwcvwjmx.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.blog.fehbvm.com/Article/details/gubpzqkxz.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.hesvh.cn/Article/details/gpqvaluec.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.zdbjq.cn/Article/details/gxqgwzkfx.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.m.share.zdbjq.cn/Article/details/ganizqyzk.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://blog.zdbjq.cn/Article/details/gjtgqpxfm.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.m.share.fehbvm.com/Article/details/gwsbwrynl.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wap.fehbvm.com/Article/details/gzkrsrwzj.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gtkkuvrqu.sHtML

J. 日期与时间
来源：http://www.blog.fehbvm.com/Article/details/gczmktgdh.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gcwlhbcir.sHtML

[J01] 获取当前时间
来源：http://www.m.share.fehbvm.com/Article/details/gyrrinxlc.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://m.share.fehbvm.com/Article/details/gzqjwjbsg.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.m.share.hesvh.cn/Article/details/gqjpoolmg.sHtML

JS:   new Date();  Date.now()
来源：http://www.m.share.fehbvm.com/Article/details/gebszuyxa.sHtML

TS:   new Date();  Date.now()
来源：http://m.share.hesvh.cn/Article/details/gombrlsfl.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://wap.zdbjq.cn/Article/details/gvfykpxym.sHtML


<!-- 参考信息 -->