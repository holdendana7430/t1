代发 wailian999

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.fehbvm.com/Article/details/gtuolakhh.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/gijpzlnxd.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.zdbjq.cn/Article/details/ghtvfaxko.sHtML

Java: String greet() { return name; }
来源：http://read.share.hesvh.cn/Article/details/ggeslcyke.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.fehbvm.com/Article/details/ghivvieku.sHtML

Ruby: def greet; @name; end
来源：http://m.share.hesvh.cn/Article/details/gcwgczccn.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.fehbvm.com/Article/details/gurwqards.sHtML

[G05] 继承
来源：http://www.m.share.hesvh.cn/Article/details/gewebgnxe.sHtML

Py:   class Admin(User): pass
来源：http://www.share.hesvh.cn/Article/details/gahrybdim.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gpzvbeggk.sHtML

JS:   class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/gftpxwbzv.sHtML

TS:   class Admin extends User {}
来源：http://mobile.fehbvm.com/Article/details/gduchulyy.sHtML

Java: class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/gmcsnxfnr.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.hesvh.cn/Article/details/ghpkcmcoj.sHtML

Ruby: class Admin < User; end
来源：http://wap.fehbvm.com/Article/details/gvlebhcla.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gbtsknkwp.sHtML

[G06] 重写方法
来源：http://baike.fehbvm.com/Article/details/gznuanjyw.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.fehbvm.com/Article/details/gfdkyejfp.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/gouxwylcl.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/genirssti.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/gtjxepemg.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/gvyifiyrl.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.hesvh.cn/Article/details/gvcckjswd.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.fehbvm.com/Article/details/gzgwnthrv.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.zdbjq.cn/Article/details/gfhgctanv.sHtML

[G07] 调用父类方法
来源：http://wap.hesvh.cn/Article/details/gezevtfrg.sHtML

Py:   super().greet()
来源：http://blog.zdbjq.cn/Article/details/gigvbvbpg.sHtML

PHP:  parent::greet();
来源：http://3g.zdbjq.cn/Article/details/ggutadhye.sHtML

JS:   super.greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gwxxvpaza.sHtML

TS:   super.greet();
来源：http://3g.fehbvm.com/Article/details/gqrufmbjw.sHtML

Java: super.greet();
来源：http://m.share.hesvh.cn/Article/details/gqzmjcfwq.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.zdbjq.cn/Article/details/gnyuyzsxg.sHtML

Ruby: super
来源：http://www.m.share.hesvh.cn/Article/details/gjfbpeieg.sHtML

C#:   base.Greet();
来源：http://www.share.fehbvm.com/Article/details/gheirhfuh.sHtML

[G08] 静态方法与属性
来源：http://www.blog.fehbvm.com/Article/details/geqsvmfaa.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.fehbvm.com/Article/details/gfbbcuwjq.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.fehbvm.com/Article/details/gouliwifp.sHtML

JS:   static f() {}
来源：http://3g.hesvh.cn/Article/details/gmfmsnypl.sHtML

TS:   static f(): void {}
来源：http://mobile.fehbvm.com/Article/details/gmwjqpouz.sHtML

Java: static void f() {}
来源：http://m.share.zdbjq.cn/Article/details/gafwbzbmx.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.hesvh.cn/Article/details/gqvfqlpmx.sHtML

Ruby: def self.f; end
来源：http://wap.zdbjq.cn/Article/details/gatiwmcbm.sHtML

C#:   public static void F() {}
来源：http://mobile.zdbjq.cn/Article/details/gmhgrbpsd.sHtML

[G09] 接口 / 抽象类
来源：http://3g.zdbjq.cn/Article/details/gsuiyoebc.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.hesvh.cn/Article/details/gliazmamw.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.hesvh.cn/Article/details/gjefmxitm.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.hesvh.cn/Article/details/gknylakdn.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.zdbjq.cn/Article/details/gxmuvxuhm.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.zdbjq.cn/Article/details/gthfrdktg.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.hesvh.cn/Article/details/gchjmmwmn.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.zdbjq.cn/Article/details/gzyxuncej.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.fehbvm.com/Article/details/gzzhgrvyw.sHtML

[G10] 访问控制
来源：http://mobile.fehbvm.com/Article/details/gsaopbmwu.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.fehbvm.com/Article/details/gmimwjuwg.sHtML

PHP:  public / protected / private
来源：http://www.m.share.hesvh.cn/Article/details/gvbbqpiev.sHtML

JS:   #private 字段；其余公开
来源：http://baike.zdbjq.cn/Article/details/gkohlkcpq.sHtML

TS:   public / protected / private
来源：http://blog.hesvh.cn/Article/details/ggccytfvp.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.zdbjq.cn/Article/details/gmlikaiym.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.fehbvm.com/Article/details/ghwmincqj.sHtML

Ruby: public / protected / private
来源：http://mobile.zdbjq.cn/Article/details/gjbrzqdyd.sHtML

C#:   public / protected / private / internal
来源：http://baike.hesvh.cn/Article/details/ghtrqdxhd.sHtML

[G11] getter / setter
来源：http://blog.hesvh.cn/Article/details/geufkpyns.sHtML

Py:   @property 与 @x.setter
来源：http://3g.zdbjq.cn/Article/details/gtibxvnqc.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.fehbvm.com/Article/details/gzlvibgxk.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.fehbvm.com/Article/details/gwztyhbtf.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.fehbvm.com/Article/details/gaotpbieg.sHtML

Java: public String getName() { return name; }
来源：http://baike.zdbjq.cn/Article/details/glzxamteq.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.hesvh.cn/Article/details/gxqsxizni.sHtML

Ruby: attr_accessor :name
来源：http://www.share.zdbjq.cn/Article/details/grlhdjxwc.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.hesvh.cn/Article/details/gvpnzqyte.sHtML

[G12] 对象转字符串
来源：http://www.blog.hesvh.cn/Article/details/ggwyzzhth.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.fehbvm.com/Article/details/gaqwtxtsv.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.fehbvm.com/Article/details/gfkoddpvj.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/gewtstlrg.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.fehbvm.com/Article/details/gbljonpkg.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.zdbjq.cn/Article/details/ggklpqhfq.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.fehbvm.com/Article/details/gunyyhvdf.sHtML

Ruby: def to_s; @name; end
来源：http://blog.fehbvm.com/Article/details/gorncqdra.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.zdbjq.cn/Article/details/gcyezjvmv.sHtML

[G13] 判断对象类型
来源：http://mobile.hesvh.cn/Article/details/gwctyrcqm.sHtML

Py:   isinstance(u, User)
来源：http://wap.fehbvm.com/Article/details/gqdzabxhd.sHtML

PHP:  $u instanceof User
来源：http://www.blog.fehbvm.com/Article/details/gcmkizvpo.sHtML

JS:   u instanceof User
来源：http://m.share.fehbvm.com/Article/details/gqwcltqka.sHtML

TS:   u instanceof User
来源：http://blog.zdbjq.cn/Article/details/guhrifwyx.sHtML

Java: u instanceof User
来源：http://wap.zdbjq.cn/Article/details/gfzrvtcax.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.hesvh.cn/Article/details/gbysiedjd.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.zdbjq.cn/Article/details/gwwcqwyaw.sHtML

C#:   u is User
来源：http://www.blog.fehbvm.com/Article/details/gngfexzvg.sHtML

[G14] 数据类 / record
来源：http://m.share.fehbvm.com/Article/details/girpflgmh.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.zdbjq.cn/Article/details/gfvqproyw.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.hesvh.cn/Article/details/gojhskdkl.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.zdbjq.cn/Article/details/gxsgfsukp.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.fehbvm.com/Article/details/gvexpythx.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.zdbjq.cn/Article/details/gbnlwgllx.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.hesvh.cn/Article/details/gnfojpmmc.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.hesvh.cn/Article/details/gdphjudcx.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.fehbvm.com/Article/details/giknzzrsl.sHtML

[G15] 枚举
来源：http://www.share.fehbvm.com/Article/details/gdwowcjja.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.zdbjq.cn/Article/details/geadapxdj.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://baike.fehbvm.com/Article/details/gatuzmebw.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.hesvh.cn/Article/details/gothiwtux.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.fehbvm.com/Article/details/gxurlvuxn.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.hesvh.cn/Article/details/gcpruoncy.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.fehbvm.com/Article/details/gftkrnneu.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.hesvh.cn/Article/details/ggwlyldvr.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.zdbjq.cn/Article/details/guvvxgzyk.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.zdbjq.cn/Article/details/gbjudrmbk.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.hesvh.cn/Article/details/gkqaxintf.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.fehbvm.com/Article/details/gyssmgnds.sHtML

JS:   Object.entries(obj)
来源：http://mobile.zdbjq.cn/Article/details/gwjgnjmef.sHtML

TS:   Object.entries(obj)
来源：http://3g.zdbjq.cn/Article/details/gmsvttxph.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://read.share.fehbvm.com/Article/details/gkwzuosuo.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.zdbjq.cn/Article/details/gkgeqedjq.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.hesvh.cn/Article/details/gniyybezo.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.zdbjq.cn/Article/details/gkghuclps.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gjpcxramy.sHtML

H. 异常与错误处理
来源：http://m.share.hesvh.cn/Article/details/glpfkbjvz.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/ghbstxgrm.sHtML

[H01] try / catch 基础
来源：http://baike.zdbjq.cn/Article/details/gendscxxq.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://baike.fehbvm.com/Article/details/ghvwtogum.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.fehbvm.com/Article/details/gqvxritjc.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.blog.fehbvm.com/Article/details/gcnkpmqvp.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.fehbvm.com/Article/details/gvmazmeav.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.fehbvm.com/Article/details/gjbspdvfp.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.m.share.hesvh.cn/Article/details/glizjcawh.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.hesvh.cn/Article/details/gsfmxublu.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.zdbjq.cn/Article/details/getuqxkgq.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.zdbjq.cn/Article/details/gntrcamte.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://3g.zdbjq.cn/Article/details/ggflfrkuw.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gjxnsahrq.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://mobile.fehbvm.com/Article/details/gibaegxlm.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://blog.zdbjq.cn/Article/details/ggwegpzwt.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.blog.hesvh.cn/Article/details/gamnjzfcr.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://blog.zdbjq.cn/Article/details/ghnyhsukc.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.fehbvm.com/Article/details/glutihexd.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://baike.fehbvm.com/Article/details/gtwpetzfc.sHtML

[H03] 主动抛出异常
来源：http://m.share.zdbjq.cn/Article/details/gqomlomaq.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.share.hesvh.cn/Article/details/gybrryygh.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mobile.fehbvm.com/Article/details/gapgvvqet.sHtML

JS:   throw new Error("错误信息");
来源：http://www.share.fehbvm.com/Article/details/gydkndybo.sHtML

TS:   throw new Error("错误信息");
来源：http://baike.zdbjq.cn/Article/details/gbrmzoqjo.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.blog.hesvh.cn/Article/details/gsynvwugt.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mobile.zdbjq.cn/Article/details/gqxzbijon.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.blog.hesvh.cn/Article/details/gdrfdvzcb.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.blog.fehbvm.com/Article/details/gfxjxrwzl.sHtML

[H04] 自定义异常类型
来源：http://m.share.hesvh.cn/Article/details/gnicujvxm.sHtML

Py:   class MyError(Exception): pass
来源：http://wap.zdbjq.cn/Article/details/gavxcmfxi.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://read.share.fehbvm.com/Article/details/ggbdtvzwe.sHtML

JS:   class MyError extends Error {}
来源：http://wap.zdbjq.cn/Article/details/gelxnawxl.sHtML

TS:   class MyError extends Error {}
来源：http://mobile.hesvh.cn/Article/details/gcvwruguj.sHtML

Java: class MyException extends RuntimeException {}
来源：http://m.share.fehbvm.com/Article/details/gielaumrt.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.m.share.hesvh.cn/Article/details/gootnaous.sHtML

Ruby: class MyError < StandardError; end
来源：http://mobile.fehbvm.com/Article/details/gwhrqsusg.sHtML

C#:   class MyException : Exception {}
来源：http://blog.hesvh.cn/Article/details/gqdehkjuk.sHtML

[H05] 捕获特定类型
来源：http://mobile.zdbjq.cn/Article/details/gnvqdnpuf.sHtML

Py:   except ValueError as e:
来源：http://read.share.fehbvm.com/Article/details/gigptdnlk.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://baike.zdbjq.cn/Article/details/guqkdqggy.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://blog.zdbjq.cn/Article/details/gllwarjse.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.share.fehbvm.com/Article/details/ggxnfmivl.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.m.share.hesvh.cn/Article/details/gihuamrzg.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.m.share.zdbjq.cn/Article/details/guaqtitre.sHtML

Ruby: rescue ArgumentError => e
来源：http://mobile.hesvh.cn/Article/details/gtqgmpejp.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wap.fehbvm.com/Article/details/glhovjpcd.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.blog.hesvh.cn/Article/details/grbpbprsk.sHtML

Py:   value = d.get("k") or default
来源：http://mobile.zdbjq.cn/Article/details/gmbvujakb.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://mobile.zdbjq.cn/Article/details/gamytbedu.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://3g.zdbjq.cn/Article/details/gphjtkuvp.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.share.fehbvm.com/Article/details/gyltehkao.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mobile.zdbjq.cn/Article/details/gqerdhhba.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://mobile.zdbjq.cn/Article/details/gmfyqgiwg.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.blog.fehbvm.com/Article/details/gwgqslybr.sHtML

C#:   obj?.A?.B ?? default
来源：http://mobile.hesvh.cn/Article/details/gymgipzoz.sHtML

[H07] 断言
来源：http://m.share.zdbjq.cn/Article/details/gfuavwlta.sHtML

Py:   assert x > 0, "必须为正"
来源：http://baike.zdbjq.cn/Article/details/gkxeuiaan.sHtML

PHP:  assert($x > 0);
来源：http://mobile.fehbvm.com/Article/details/gywvqcurf.sHtML

JS:   console.assert(x > 0);
来源：http://m.share.fehbvm.com/Article/details/gxetzsoan.sHtML

TS:   console.assert(x > 0);
来源：http://www.m.share.fehbvm.com/Article/details/gcwruovqg.sHtML

Java: assert x > 0 : "必须为正";
来源：http://m.share.zdbjq.cn/Article/details/gmkwplqnz.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://baike.zdbjq.cn/Article/details/grfqowwzm.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://m.share.fehbvm.com/Article/details/gyxdaayvk.sHtML

C#:   Debug.Assert(x > 0);
来源：http://wap.zdbjq.cn/Article/details/gaitjhnsw.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.m.share.fehbvm.com/Article/details/graphwpkq.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://read.share.zdbjq.cn/Article/details/gojmalmrj.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://3g.hesvh.cn/Article/details/gpzmxclzv.sHtML

JS:   e.message;  e.stack
来源：http://mobile.zdbjq.cn/Article/details/gkkcupzod.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://blog.fehbvm.com/Article/details/gkahzbjnf.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.share.zdbjq.cn/Article/details/gnpuodkyi.sHtML

Go:   err.Error()
来源：http://m.share.zdbjq.cn/Article/details/gkemvihye.sHtML

Ruby: e.message;  e.backtrace
来源：http://wap.zdbjq.cn/Article/details/gwlkhowdg.sHtML

C#:   e.Message;  e.StackTrace
来源：http://read.share.zdbjq.cn/Article/details/guxamjflm.sHtML

[H09] 带错误码的异常
来源：http://3g.zdbjq.cn/Article/details/gfxjopzrm.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.m.share.hesvh.cn/Article/details/gltpijszg.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.m.share.hesvh.cn/Article/details/gwlpzudcg.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://m.share.hesvh.cn/Article/details/gcamwvfje.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.m.share.fehbvm.com/Article/details/gmxdwebqh.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.share.hesvh.cn/Article/details/gpqhsxwww.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.m.share.hesvh.cn/Article/details/gfijtdnfl.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.m.share.zdbjq.cn/Article/details/gkbmpnuap.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.blog.fehbvm.com/Article/details/gbjwqufgv.sHtML

[H10] 资源自动释放
来源：http://3g.fehbvm.com/Article/details/gqorilwga.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://mobile.fehbvm.com/Article/details/geyaiienc.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mobile.zdbjq.cn/Article/details/gzllkdapk.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.zdbjq.cn/Article/details/gnzypftvd.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.zdbjq.cn/Article/details/ggguftukj.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://blog.zdbjq.cn/Article/details/gpmfpqnqq.sHtML

Go:   defer f.Close()
来源：http://www.m.share.hesvh.cn/Article/details/gawkkcgyt.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.m.share.fehbvm.com/Article/details/gswilqmfn.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/garfvywzt.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gkvtfwsss.sHtML

I. 正则表达式
来源：http://mobile.fehbvm.com/Article/details/gymrsixwu.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gafdraawy.sHtML

[I01] 判断是否匹配
来源：http://3g.zdbjq.cn/Article/details/ghhqxfzxs.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://blog.zdbjq.cn/Article/details/gqhhxeqfe.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://mobile.zdbjq.cn/Article/details/gkniwgrds.sHtML

JS:   /\d+/.test(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gsvwfkgat.sHtML

TS:   /\d+/.test(s)
来源：http://www.blog.zdbjq.cn/Article/details/gmbgsduil.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://blog.hesvh.cn/Article/details/gsrrplzyl.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.blog.hesvh.cn/Article/details/gxaeziiox.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.m.share.fehbvm.com/Article/details/gousbusqy.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mobile.fehbvm.com/Article/details/gyuefjecu.sHtML

[I02] 提取所有匹配
来源：http://www.share.fehbvm.com/Article/details/gpajmyvsl.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.share.fehbvm.com/Article/details/gztdgjspy.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://baike.fehbvm.com/Article/details/gdxxzuaix.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://baike.hesvh.cn/Article/details/gppkkemgl.sHtML

TS:   s.match(/\d+/g)
来源：http://m.share.fehbvm.com/Article/details/gipejxeqh.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wap.hesvh.cn/Article/details/gymvaqlud.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wap.fehbvm.com/Article/details/gkrcpvxda.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.share.fehbvm.com/Article/details/grqditizb.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wap.hesvh.cn/Article/details/guapabqzj.sHtML

[I03] 提取捕获分组
来源：http://read.share.hesvh.cn/Article/details/gadrqohhh.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.blog.zdbjq.cn/Article/details/gibyakcwa.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://blog.zdbjq.cn/Article/details/gntsdbvnj.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mobile.hesvh.cn/Article/details/geiodofsx.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://blog.hesvh.cn/Article/details/gmhsalpik.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.share.zdbjq.cn/Article/details/glfbwntja.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://blog.hesvh.cn/Article/details/gbcxnjjqw.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://blog.hesvh.cn/Article/details/gwcbmvuil.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://blog.fehbvm.com/Article/details/gwqmosefw.sHtML

[I04] 正则替换
来源：http://mobile.zdbjq.cn/Article/details/grvfbnooq.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://3g.fehbvm.com/Article/details/gnihhymar.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://blog.zdbjq.cn/Article/details/gmpgppoci.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://mobile.hesvh.cn/Article/details/gymadxgsr.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.share.zdbjq.cn/Article/details/gfcnsruut.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://baike.hesvh.cn/Article/details/geqsjoytq.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://read.share.zdbjq.cn/Article/details/gjudogjqn.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://m.share.zdbjq.cn/Article/details/gpiaosiyy.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.share.hesvh.cn/Article/details/gsjtqqmeh.sHtML

[I05] 按正则拆分
来源：http://www.share.hesvh.cn/Article/details/gztmoijaz.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://wap.fehbvm.com/Article/details/gygietcop.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.share.fehbvm.com/Article/details/gggeogpbe.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.share.fehbvm.com/Article/details/gveuozxfp.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://3g.zdbjq.cn/Article/details/gaqvqdqhx.sHtML

Java: s.split("\\s*,\\s*")
来源：http://3g.hesvh.cn/Article/details/giuemzbzb.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://mobile.fehbvm.com/Article/details/gilabmiuw.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://wap.fehbvm.com/Article/details/gwgrjsqjv.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://baike.hesvh.cn/Article/details/gzkxhpits.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://m.share.hesvh.cn/Article/details/gobvskcho.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://m.share.hesvh.cn/Article/details/gdxftqibz.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.m.share.hesvh.cn/Article/details/ghlvtzlez.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.zdbjq.cn/Article/details/gnydlqwav.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.hesvh.cn/Article/details/grttnetgy.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://3g.hesvh.cn/Article/details/gvhglcoaa.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wap.fehbvm.com/Article/details/gjtzrzadp.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://mobile.hesvh.cn/Article/details/glvjldixo.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.m.share.fehbvm.com/Article/details/gezzjavno.sHtML

[I07] 忽略大小写与多行模式
来源：http://blog.fehbvm.com/Article/details/grapvuuzh.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mobile.zdbjq.cn/Article/details/gwoxvdvwk.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://blog.zdbjq.cn/Article/details/gpzqfmlvh.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wap.zdbjq.cn/Article/details/gxepiggdm.sHtML

TS:   /error/gim
来源：http://www.share.hesvh.cn/Article/details/gzscjuixh.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.blog.hesvh.cn/Article/details/gthwyjwge.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://baike.hesvh.cn/Article/details/gjxathvzt.sHtML

Ruby: s.scan(/error/i)
来源：http://3g.fehbvm.com/Article/details/gtgcevsve.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://3g.zdbjq.cn/Article/details/gkgpduqji.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.blog.fehbvm.com/Article/details/geepextfv.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.share.zdbjq.cn/Article/details/gdmzlltyt.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://read.share.hesvh.cn/Article/details/gtbytgmyw.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.fehbvm.com/Article/details/grhfowdpt.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.zdbjq.cn/Article/details/ghrhgamem.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.blog.fehbvm.com/Article/details/gzqhtsexq.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.blog.hesvh.cn/Article/details/gqlkszmnc.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mobile.fehbvm.com/Article/details/guwstkjhw.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://blog.zdbjq.cn/Article/details/gdnozjrks.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gygliwnph.sHtML

J. 日期与时间
来源：http://read.share.hesvh.cn/Article/details/gquugvqvg.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gvesibsnt.sHtML

[J01] 获取当前时间
来源：http://www.m.share.hesvh.cn/Article/details/gcuypnics.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://3g.zdbjq.cn/Article/details/gtwujxdsc.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://m.share.fehbvm.com/Article/details/gkbhamjvs.sHtML

JS:   new Date();  Date.now()
来源：http://www.share.fehbvm.com/Article/details/gvkzozimb.sHtML

TS:   new Date();  Date.now()
来源：http://read.share.zdbjq.cn/Article/details/gemyfyvsr.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.share.zdbjq.cn/Article/details/gtedzskhz.sHtML

Go:   time.Now()
来源：http://baike.fehbvm.com/Article/details/gbtthfwcr.sHtML

Ruby: Time.now
来源：http://baike.hesvh.cn/Article/details/giblgzhuo.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://baike.hesvh.cn/Article/details/gjbsrbuhv.sHtML

[J02] 格式化输出
来源：http://mobile.hesvh.cn/Article/details/guoayehjv.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.hesvh.cn/Article/details/gudrqucvu.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wap.fehbvm.com/Article/details/gxqprmtmr.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.blog.hesvh.cn/Article/details/ggravoudn.sHtML

TS:   d.toISOString()
来源：http://mobile.hesvh.cn/Article/details/gkgrjgfbc.sHtML


<!-- 参考信息 -->