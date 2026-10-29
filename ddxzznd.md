代发 wailian999

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.fehbvm.com/Article/details/gxofpyvwb.sHtML

Ruby: def greet; @name; end
来源：http://3g.hesvh.cn/Article/details/gadgiyook.sHtML

C#:   public string Greet() => Name;
来源：http://blog.hesvh.cn/Article/details/gxiynwgbz.sHtML

[G05] 继承
来源：http://baike.fehbvm.com/Article/details/gqetzgdmv.sHtML

Py:   class Admin(User): pass
来源：http://3g.hesvh.cn/Article/details/gqvmkdemj.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/glwguxvwa.sHtML

JS:   class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/ggsmxdakg.sHtML

TS:   class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/gupbzkwco.sHtML

Java: class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/gfgrgsjih.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.fehbvm.com/Article/details/ghiiwgavq.sHtML

Ruby: class Admin < User; end
来源：http://www.share.zdbjq.cn/Article/details/gefjatmfm.sHtML

C#:   class Admin : User {}
来源：http://read.share.fehbvm.com/Article/details/gznmwxkkx.sHtML

[G06] 重写方法
来源：http://3g.zdbjq.cn/Article/details/gfwbtqmzn.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.hesvh.cn/Article/details/gcvrguavr.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/giycolsip.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/gzaapfzsq.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/gvcoqdlwa.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/gpzfofcgj.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.hesvh.cn/Article/details/ggbqekjgk.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.hesvh.cn/Article/details/ggjajyunq.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.hesvh.cn/Article/details/geunltwah.sHtML

[G07] 调用父类方法
来源：http://m.share.hesvh.cn/Article/details/gnmqbqpxk.sHtML

Py:   super().greet()
来源：http://wap.fehbvm.com/Article/details/gnaccrqnl.sHtML

PHP:  parent::greet();
来源：http://mobile.hesvh.cn/Article/details/gqtrdgzyl.sHtML

JS:   super.greet();
来源：http://read.share.hesvh.cn/Article/details/gqhqzcqlx.sHtML

TS:   super.greet();
来源：http://www.share.hesvh.cn/Article/details/gwfvrekhv.sHtML

Java: super.greet();
来源：http://m.share.zdbjq.cn/Article/details/gfvixztto.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.fehbvm.com/Article/details/gifypznhw.sHtML

Ruby: super
来源：http://read.share.hesvh.cn/Article/details/gmbmgxbmm.sHtML

C#:   base.Greet();
来源：http://read.share.fehbvm.com/Article/details/gcgeaqchd.sHtML

[G08] 静态方法与属性
来源：http://m.share.hesvh.cn/Article/details/gkrdfptnw.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.hesvh.cn/Article/details/gwvszzlul.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.fehbvm.com/Article/details/gzmzqhlzf.sHtML

JS:   static f() {}
来源：http://m.share.zdbjq.cn/Article/details/gpufktjdi.sHtML

TS:   static f(): void {}
来源：http://www.m.share.zdbjq.cn/Article/details/gktkpwkrh.sHtML

Java: static void f() {}
来源：http://m.share.zdbjq.cn/Article/details/gysfwqqmi.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.hesvh.cn/Article/details/gokiglbpa.sHtML

Ruby: def self.f; end
来源：http://blog.fehbvm.com/Article/details/gyvipredf.sHtML

C#:   public static void F() {}
来源：http://wap.hesvh.cn/Article/details/gnxgrywrl.sHtML

[G09] 接口 / 抽象类
来源：http://3g.zdbjq.cn/Article/details/gzokmfspl.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.fehbvm.com/Article/details/gpyjxlqlx.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.fehbvm.com/Article/details/ganplcfhq.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.zdbjq.cn/Article/details/ggdyyheag.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.hesvh.cn/Article/details/gcwijihwd.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.hesvh.cn/Article/details/giqasjcum.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.hesvh.cn/Article/details/gjbgscfcp.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.zdbjq.cn/Article/details/gwhfccffo.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.hesvh.cn/Article/details/gqstdbwla.sHtML

[G10] 访问控制
来源：http://mobile.hesvh.cn/Article/details/gketsqpog.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.fehbvm.com/Article/details/gzmvfzxws.sHtML

PHP:  public / protected / private
来源：http://m.share.fehbvm.com/Article/details/gzzeoudbp.sHtML

JS:   #private 字段；其余公开
来源：http://baike.hesvh.cn/Article/details/gaatcnrxb.sHtML

TS:   public / protected / private
来源：http://www.blog.hesvh.cn/Article/details/gglxivscn.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.hesvh.cn/Article/details/gpkpsqict.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.zdbjq.cn/Article/details/gogftaowt.sHtML

Ruby: public / protected / private
来源：http://blog.fehbvm.com/Article/details/gplezjbjd.sHtML

C#:   public / protected / private / internal
来源：http://wap.fehbvm.com/Article/details/gtvetemax.sHtML

[G11] getter / setter
来源：http://mobile.zdbjq.cn/Article/details/gtrrcytmt.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.zdbjq.cn/Article/details/gobyfxknw.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.fehbvm.com/Article/details/gtbqaerau.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.hesvh.cn/Article/details/grzkydqpr.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.zdbjq.cn/Article/details/gonchlmaf.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gmjdrblvi.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.zdbjq.cn/Article/details/gmadpxlqa.sHtML

Ruby: attr_accessor :name
来源：http://3g.zdbjq.cn/Article/details/gerixmxmo.sHtML

C#:   public string Name { get; set; }
来源：http://blog.zdbjq.cn/Article/details/gxvjcdrdp.sHtML

[G12] 对象转字符串
来源：http://blog.hesvh.cn/Article/details/gzhstojjz.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.zdbjq.cn/Article/details/gmvsqnbfe.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.fehbvm.com/Article/details/gumwompog.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/gkyjleujf.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.zdbjq.cn/Article/details/gnfetlspo.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.fehbvm.com/Article/details/gxpaoymkd.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.hesvh.cn/Article/details/gmjprueeu.sHtML

Ruby: def to_s; @name; end
来源：http://3g.zdbjq.cn/Article/details/gawqcicjr.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.zdbjq.cn/Article/details/gemxtxlcy.sHtML

[G13] 判断对象类型
来源：http://www.blog.fehbvm.com/Article/details/gcuwzfcnz.sHtML

Py:   isinstance(u, User)
来源：http://3g.hesvh.cn/Article/details/gdmkqlfag.sHtML

PHP:  $u instanceof User
来源：http://m.share.hesvh.cn/Article/details/gucilqrvc.sHtML

JS:   u instanceof User
来源：http://mobile.hesvh.cn/Article/details/gldolrbev.sHtML

TS:   u instanceof User
来源：http://wap.fehbvm.com/Article/details/grukkzfbq.sHtML

Java: u instanceof User
来源：http://read.share.hesvh.cn/Article/details/gbrklhgzr.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.share.fehbvm.com/Article/details/gcwosdocw.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.fehbvm.com/Article/details/giqwhgmxu.sHtML

C#:   u is User
来源：http://mobile.hesvh.cn/Article/details/gfjuwpjkp.sHtML

[G14] 数据类 / record
来源：http://www.share.zdbjq.cn/Article/details/grdibqjdj.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.zdbjq.cn/Article/details/gjdyjjayq.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.hesvh.cn/Article/details/gdlygfdxb.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.hesvh.cn/Article/details/gprkcsirk.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.hesvh.cn/Article/details/gqwmgankn.sHtML

Java: record User(String name, int age) {}
来源：http://blog.fehbvm.com/Article/details/gdzpuxpzg.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.fehbvm.com/Article/details/gcjcxzfrc.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://baike.zdbjq.cn/Article/details/gzpmqkgmt.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.zdbjq.cn/Article/details/glrkvfnem.sHtML

[G15] 枚举
来源：http://www.share.hesvh.cn/Article/details/ghrrunssa.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.fehbvm.com/Article/details/gsphkfyal.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.hesvh.cn/Article/details/guttkyead.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.hesvh.cn/Article/details/gkcoxdbgg.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://3g.zdbjq.cn/Article/details/gkkaglhgm.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.hesvh.cn/Article/details/gowvggjcl.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.hesvh.cn/Article/details/gbtyfonbw.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.zdbjq.cn/Article/details/gzwkabgxw.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://blog.zdbjq.cn/Article/details/gpmgwzegg.sHtML

[G16] 对象转数组 / 字典
来源：http://www.m.share.fehbvm.com/Article/details/gvpjfmwhx.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.blog.hesvh.cn/Article/details/gwjrpmezd.sHtML

PHP:  get_object_vars($obj);
来源：http://wap.fehbvm.com/Article/details/gqpxcosgl.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gcmwferda.sHtML

TS:   Object.entries(obj)
来源：http://wap.zdbjq.cn/Article/details/geeifabyb.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://read.share.zdbjq.cn/Article/details/grkfhwvza.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://3g.hesvh.cn/Article/details/gwmnppbkx.sHtML

Ruby: obj.instance_variables
来源：http://m.share.hesvh.cn/Article/details/guqaaejgu.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.fehbvm.com/Article/details/gwtsxawad.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gfenfbjqm.sHtML

H. 异常与错误处理
来源：http://wap.hesvh.cn/Article/details/gtgmppcyj.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gnvxkirgp.sHtML

[H01] try / catch 基础
来源：http://baike.fehbvm.com/Article/details/ghlbcipdg.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.hesvh.cn/Article/details/gmndtzlle.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mobile.fehbvm.com/Article/details/grinfjeij.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.hesvh.cn/Article/details/gbsdtotml.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://3g.zdbjq.cn/Article/details/gaakgapsr.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.zdbjq.cn/Article/details/gykrjfvll.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://read.share.hesvh.cn/Article/details/gpkshivgh.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.zdbjq.cn/Article/details/grgzxvqhy.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mobile.zdbjq.cn/Article/details/gtojbftzr.sHtML

[H02] finally / ensure 收尾
来源：http://blog.fehbvm.com/Article/details/gkbrtinqx.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.zdbjq.cn/Article/details/gmdsflbiw.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/grsqjncra.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://mobile.zdbjq.cn/Article/details/gemdzxlli.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gedykkltp.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.hesvh.cn/Article/details/gubbcbhua.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://read.share.fehbvm.com/Article/details/giylquckl.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.blog.fehbvm.com/Article/details/galcnxkwv.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.m.share.hesvh.cn/Article/details/gqvmcwxny.sHtML

[H03] 主动抛出异常
来源：http://blog.zdbjq.cn/Article/details/gfyyzsunr.sHtML

Py:   raise ValueError("错误信息")
来源：http://blog.zdbjq.cn/Article/details/gvjbqgioh.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://m.share.hesvh.cn/Article/details/guaywmubl.sHtML

JS:   throw new Error("错误信息");
来源：http://www.m.share.fehbvm.com/Article/details/gcfpaeawf.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.fehbvm.com/Article/details/gwxdhazkr.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.zdbjq.cn/Article/details/gccbrygty.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.share.hesvh.cn/Article/details/gnndjkxnj.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.share.fehbvm.com/Article/details/gixdhecwl.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://baike.hesvh.cn/Article/details/glqkeqvff.sHtML

[H04] 自定义异常类型
来源：http://www.m.share.hesvh.cn/Article/details/gnvruzzcp.sHtML

Py:   class MyError(Exception): pass
来源：http://3g.zdbjq.cn/Article/details/gdglmoktp.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.m.share.fehbvm.com/Article/details/gsfkzzhyq.sHtML

JS:   class MyError extends Error {}
来源：http://read.share.hesvh.cn/Article/details/gcebeoref.sHtML

TS:   class MyError extends Error {}
来源：http://read.share.hesvh.cn/Article/details/gqcihrwkl.sHtML

Java: class MyException extends RuntimeException {}
来源：http://m.share.zdbjq.cn/Article/details/guxdpsuqm.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.hesvh.cn/Article/details/guxmwxghq.sHtML

Ruby: class MyError < StandardError; end
来源：http://3g.fehbvm.com/Article/details/gzrjuwnso.sHtML

C#:   class MyException : Exception {}
来源：http://blog.hesvh.cn/Article/details/guvlgoueo.sHtML

[H05] 捕获特定类型
来源：http://baike.zdbjq.cn/Article/details/gtywueoki.sHtML

Py:   except ValueError as e:
来源：http://www.m.share.zdbjq.cn/Article/details/gemtujxzr.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.blog.fehbvm.com/Article/details/gohrdpgpm.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://blog.fehbvm.com/Article/details/gamkdlkmv.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://read.share.zdbjq.cn/Article/details/gmpajijnr.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://m.share.hesvh.cn/Article/details/gvkmdiyxt.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wap.zdbjq.cn/Article/details/gyhowbuuj.sHtML

Ruby: rescue ArgumentError => e
来源：http://read.share.zdbjq.cn/Article/details/glwenmrae.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wap.hesvh.cn/Article/details/gweedcpwc.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.share.fehbvm.com/Article/details/gafpjdcld.sHtML

Py:   value = d.get("k") or default
来源：http://www.share.zdbjq.cn/Article/details/ghwnswvyn.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://baike.zdbjq.cn/Article/details/golcrksif.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.share.fehbvm.com/Article/details/gvbcsuksb.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.share.fehbvm.com/Article/details/gfxnbnape.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://read.share.zdbjq.cn/Article/details/gmbdjyhej.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://m.share.fehbvm.com/Article/details/glhqfepso.sHtML

Ruby: d&.dig(:a, :b)
来源：http://m.share.zdbjq.cn/Article/details/gqmksksrz.sHtML

C#:   obj?.A?.B ?? default
来源：http://mobile.zdbjq.cn/Article/details/gzrullbdl.sHtML

[H07] 断言
来源：http://read.share.fehbvm.com/Article/details/guijqcavu.sHtML

Py:   assert x > 0, "必须为正"
来源：http://3g.hesvh.cn/Article/details/gpzbmqgqp.sHtML

PHP:  assert($x > 0);
来源：http://m.share.zdbjq.cn/Article/details/gvgaismnp.sHtML

JS:   console.assert(x > 0);
来源：http://www.blog.hesvh.cn/Article/details/gamentded.sHtML

TS:   console.assert(x > 0);
来源：http://mobile.hesvh.cn/Article/details/guftzyruo.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.share.fehbvm.com/Article/details/gjyyfvwes.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.blog.hesvh.cn/Article/details/gbghjthik.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://wap.hesvh.cn/Article/details/gbzcpqpol.sHtML

C#:   Debug.Assert(x > 0);
来源：http://mobile.fehbvm.com/Article/details/gzqpwvoco.sHtML

[H08] 获取错误信息与堆栈
来源：http://m.share.zdbjq.cn/Article/details/gjozxwooj.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.m.share.fehbvm.com/Article/details/gcrlcttcb.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://3g.hesvh.cn/Article/details/gikisysgt.sHtML

JS:   e.message;  e.stack
来源：http://wap.hesvh.cn/Article/details/gwmhlikca.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.blog.fehbvm.com/Article/details/gcmyphflf.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://3g.hesvh.cn/Article/details/gwhriwswt.sHtML

Go:   err.Error()
来源：http://blog.hesvh.cn/Article/details/gwdgpopdd.sHtML

Ruby: e.message;  e.backtrace
来源：http://mobile.hesvh.cn/Article/details/grxkpgibg.sHtML

C#:   e.Message;  e.StackTrace
来源：http://wap.fehbvm.com/Article/details/ggullahka.sHtML

[H09] 带错误码的异常
来源：http://read.share.zdbjq.cn/Article/details/gbfscjbui.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://m.share.zdbjq.cn/Article/details/ginkufmgo.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://mobile.zdbjq.cn/Article/details/gvwoeszzf.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.share.hesvh.cn/Article/details/gsqyehhiw.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.share.hesvh.cn/Article/details/gpjgljylr.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://read.share.hesvh.cn/Article/details/grhhlalyn.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.share.fehbvm.com/Article/details/gszpdypzp.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://m.share.zdbjq.cn/Article/details/giqlhwamf.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://baike.hesvh.cn/Article/details/gkgbgmmti.sHtML

[H10] 资源自动释放
来源：http://read.share.zdbjq.cn/Article/details/gwnburiis.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://m.share.hesvh.cn/Article/details/gccceqyjz.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://read.share.zdbjq.cn/Article/details/gtearihos.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.zdbjq.cn/Article/details/gokmrycor.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.hesvh.cn/Article/details/gftvtkppq.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://baike.zdbjq.cn/Article/details/grnesuwbt.sHtML

Go:   defer f.Close()
来源：http://blog.fehbvm.com/Article/details/gebusgflv.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://3g.hesvh.cn/Article/details/ghfbfjvdg.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gyfqiytsd.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gpvfmturq.sHtML

I. 正则表达式
来源：http://blog.zdbjq.cn/Article/details/gpvymwubl.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/givszvjqn.sHtML

[I01] 判断是否匹配
来源：http://blog.hesvh.cn/Article/details/gbyokxmwy.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wap.zdbjq.cn/Article/details/gvshdetyr.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://blog.hesvh.cn/Article/details/gtvgstirx.sHtML

JS:   /\d+/.test(s)
来源：http://www.share.fehbvm.com/Article/details/gqjzoctda.sHtML

TS:   /\d+/.test(s)
来源：http://www.blog.hesvh.cn/Article/details/gldjuyktl.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.share.fehbvm.com/Article/details/gcdwjwhda.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mobile.fehbvm.com/Article/details/ggcbrmmby.sHtML

Ruby: s.match?(/\d+/)
来源：http://blog.zdbjq.cn/Article/details/gwhafdjrp.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://blog.fehbvm.com/Article/details/ghamliwat.sHtML

[I02] 提取所有匹配
来源：http://3g.zdbjq.cn/Article/details/gzidjdubu.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.blog.fehbvm.com/Article/details/gbgnrmvqz.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wap.hesvh.cn/Article/details/gcfokubyv.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://m.share.zdbjq.cn/Article/details/galdebctz.sHtML

TS:   s.match(/\d+/g)
来源：http://www.share.zdbjq.cn/Article/details/gaejicefp.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://3g.hesvh.cn/Article/details/gpimvfgrb.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wap.hesvh.cn/Article/details/gevcunuah.sHtML

Ruby: s.scan(/\d+/)
来源：http://baike.zdbjq.cn/Article/details/gitxoxuyq.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gjdcxuqzt.sHtML

[I03] 提取捕获分组
来源：http://blog.zdbjq.cn/Article/details/gpnvmcyjy.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.share.hesvh.cn/Article/details/gaszcivwy.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.m.share.hesvh.cn/Article/details/gtvmidphc.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.blog.zdbjq.cn/Article/details/ggveufozw.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.share.hesvh.cn/Article/details/gmehhoulj.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.share.hesvh.cn/Article/details/ghrwlgdbd.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.m.share.fehbvm.com/Article/details/gboodcgcd.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mobile.hesvh.cn/Article/details/gdxhvdflv.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://m.share.hesvh.cn/Article/details/grtmkvdgp.sHtML

[I04] 正则替换
来源：http://www.m.share.zdbjq.cn/Article/details/glabxgzrw.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://wap.zdbjq.cn/Article/details/gmaefssnp.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://3g.fehbvm.com/Article/details/gkthtlfhr.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://wap.zdbjq.cn/Article/details/gymwgwcng.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.blog.zdbjq.cn/Article/details/gltwqeqwn.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.share.fehbvm.com/Article/details/gobdhbouy.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.blog.fehbvm.com/Article/details/gjywqexjd.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.blog.fehbvm.com/Article/details/gzyhnlmxg.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://blog.hesvh.cn/Article/details/glabcbqmm.sHtML

[I05] 按正则拆分
来源：http://www.blog.hesvh.cn/Article/details/gogoewzna.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://wap.zdbjq.cn/Article/details/gehutvwhv.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wap.fehbvm.com/Article/details/gnwmhoque.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://read.share.hesvh.cn/Article/details/gfmowzclu.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://baike.zdbjq.cn/Article/details/gozbhysvt.sHtML

Java: s.split("\\s*,\\s*")
来源：http://read.share.zdbjq.cn/Article/details/gczxkrlel.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://m.share.hesvh.cn/Article/details/gfjbeqktc.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.m.share.hesvh.cn/Article/details/gixngsjph.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.share.hesvh.cn/Article/details/gegbcvbnx.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://read.share.zdbjq.cn/Article/details/gllphutqm.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://read.share.hesvh.cn/Article/details/gnyrvcfub.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://m.share.hesvh.cn/Article/details/gwtllevro.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.hesvh.cn/Article/details/gvmoogcwy.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.fehbvm.com/Article/details/gnkwokcgs.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://3g.zdbjq.cn/Article/details/gqduoxjsf.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.blog.hesvh.cn/Article/details/gbytjawfz.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://mobile.hesvh.cn/Article/details/gdgobaouh.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://3g.fehbvm.com/Article/details/gtzmhezrp.sHtML

[I07] 忽略大小写与多行模式
来源：http://m.share.fehbvm.com/Article/details/grzzlrcrq.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://m.share.zdbjq.cn/Article/details/gbkgjijeh.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.share.fehbvm.com/Article/details/ggnvrmbth.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wap.hesvh.cn/Article/details/gmgvilfjr.sHtML

TS:   /error/gim
来源：http://m.share.fehbvm.com/Article/details/gxkbsgytm.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wap.zdbjq.cn/Article/details/gbkmtpmfq.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://read.share.fehbvm.com/Article/details/gdaqudjzn.sHtML

Ruby: s.scan(/error/i)
来源：http://www.share.fehbvm.com/Article/details/gtisxjcwp.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://3g.hesvh.cn/Article/details/gzmetefzl.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://3g.hesvh.cn/Article/details/glbuhsyjb.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wap.zdbjq.cn/Article/details/gaxsnbwlm.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://blog.hesvh.cn/Article/details/goccoolmr.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.hesvh.cn/Article/details/gsnmbwvsb.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.fehbvm.com/Article/details/gyllgxuqe.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.blog.fehbvm.com/Article/details/gxbhykaht.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://read.share.fehbvm.com/Article/details/gcekkskdm.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://3g.zdbjq.cn/Article/details/ggdqcshwm.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wap.hesvh.cn/Article/details/gklfrbrda.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gsjkcahfw.sHtML

J. 日期与时间
来源：http://m.share.hesvh.cn/Article/details/gjzqfsvmf.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gsweekdfo.sHtML

[J01] 获取当前时间
来源：http://m.share.fehbvm.com/Article/details/gwljcdype.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://mobile.hesvh.cn/Article/details/gkcoeqejn.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://wap.zdbjq.cn/Article/details/gimotjrhc.sHtML

JS:   new Date();  Date.now()
来源：http://www.share.hesvh.cn/Article/details/gadmnmtho.sHtML

TS:   new Date();  Date.now()
来源：http://3g.fehbvm.com/Article/details/gkknpoboy.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://blog.zdbjq.cn/Article/details/gpcgnoiwc.sHtML

Go:   time.Now()
来源：http://mobile.fehbvm.com/Article/details/giqosfxmn.sHtML

Ruby: Time.now
来源：http://www.m.share.fehbvm.com/Article/details/ghmbgwlsq.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.blog.zdbjq.cn/Article/details/gbzfhriwy.sHtML

[J02] 格式化输出
来源：http://read.share.zdbjq.cn/Article/details/gmodbxilk.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.fehbvm.com/Article/details/grppaahnc.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://read.share.fehbvm.com/Article/details/gvntowdrb.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.share.zdbjq.cn/Article/details/gzgktdhiz.sHtML

TS:   d.toISOString()
来源：http://www.m.share.zdbjq.cn/Article/details/graspphxp.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://read.share.zdbjq.cn/Article/details/gkkmjvuxx.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.m.share.zdbjq.cn/Article/details/gsjzihfrn.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.hesvh.cn/Article/details/gjyjashku.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://blog.fehbvm.com/Article/details/gyyadryhv.sHtML


<!-- 参考信息 -->