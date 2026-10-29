代发 wailian999

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.fehbvm.com/Article/details/gwxjyzgge.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.zdbjq.cn/Article/details/gyeyzidwi.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.fehbvm.com/Article/details/gkedvyfuu.sHtML

Java: String greet() { return name; }
来源：http://mobile.fehbvm.com/Article/details/gokijnybg.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.hesvh.cn/Article/details/gmtxoatxi.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.hesvh.cn/Article/details/gcfiitvsj.sHtML

C#:   public string Greet() => Name;
来源：http://baike.fehbvm.com/Article/details/gnjosamlx.sHtML

[G05] 继承
来源：http://m.share.hesvh.cn/Article/details/gvlrtbweh.sHtML

Py:   class Admin(User): pass
来源：http://baike.zdbjq.cn/Article/details/giwkkyzed.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/ggygsddjd.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/gzxsezyvd.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/gcajdzhac.sHtML

Java: class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/gttiirerr.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.fehbvm.com/Article/details/gsujgnfzk.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.zdbjq.cn/Article/details/genfhqhwf.sHtML

C#:   class Admin : User {}
来源：http://www.share.hesvh.cn/Article/details/gvjbqbjyf.sHtML

[G06] 重写方法
来源：http://wap.fehbvm.com/Article/details/gikoojvzd.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.hesvh.cn/Article/details/gwgobgsuq.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/gpvojtfch.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/gutwitotw.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/gehnbjvcy.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/gclhtqosi.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.hesvh.cn/Article/details/gbruorrah.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.hesvh.cn/Article/details/gzsmjwkmb.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.zdbjq.cn/Article/details/gxakbqvdy.sHtML

[G07] 调用父类方法
来源：http://read.share.zdbjq.cn/Article/details/gghyycewd.sHtML

Py:   super().greet()
来源：http://www.share.hesvh.cn/Article/details/gaokchxmg.sHtML

PHP:  parent::greet();
来源：http://www.blog.hesvh.cn/Article/details/gnwygqdii.sHtML

JS:   super.greet();
来源：http://read.share.fehbvm.com/Article/details/gizpxkocc.sHtML

TS:   super.greet();
来源：http://baike.zdbjq.cn/Article/details/gkwdioxlg.sHtML

Java: super.greet();
来源：http://3g.fehbvm.com/Article/details/gsaxoystq.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.zdbjq.cn/Article/details/gysixsgrj.sHtML

Ruby: super
来源：http://wap.fehbvm.com/Article/details/gbsqtbfij.sHtML

C#:   base.Greet();
来源：http://blog.hesvh.cn/Article/details/grpwpewju.sHtML

[G08] 静态方法与属性
来源：http://mobile.fehbvm.com/Article/details/gwyrzuzrq.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.zdbjq.cn/Article/details/gdgftosue.sHtML

PHP:  public static function f() {}
来源：http://blog.zdbjq.cn/Article/details/gafqtincy.sHtML

JS:   static f() {}
来源：http://www.share.fehbvm.com/Article/details/guuqbwani.sHtML

TS:   static f(): void {}
来源：http://www.m.share.hesvh.cn/Article/details/ghtpvfwsb.sHtML

Java: static void f() {}
来源：http://www.m.share.zdbjq.cn/Article/details/gbgvusekf.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.fehbvm.com/Article/details/gubyosmtn.sHtML

Ruby: def self.f; end
来源：http://3g.hesvh.cn/Article/details/ggcozegbu.sHtML

C#:   public static void F() {}
来源：http://read.share.zdbjq.cn/Article/details/grcuxldul.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.hesvh.cn/Article/details/glqasjnqy.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.zdbjq.cn/Article/details/gtlxdejcl.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.zdbjq.cn/Article/details/gjgcjgfrj.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.fehbvm.com/Article/details/glwzkctdb.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.fehbvm.com/Article/details/gtalmniyq.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.zdbjq.cn/Article/details/gubpwcasp.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.hesvh.cn/Article/details/gadanjvhz.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.zdbjq.cn/Article/details/gbhbyirfv.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.fehbvm.com/Article/details/gujzjsffm.sHtML

[G10] 访问控制
来源：http://wap.hesvh.cn/Article/details/gvmvzmese.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.zdbjq.cn/Article/details/gicfnzuor.sHtML

PHP:  public / protected / private
来源：http://3g.fehbvm.com/Article/details/gkhqmysmd.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.hesvh.cn/Article/details/gixmlugvj.sHtML

TS:   public / protected / private
来源：http://www.m.share.zdbjq.cn/Article/details/gzwxwowwq.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.hesvh.cn/Article/details/gngtxevmj.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.zdbjq.cn/Article/details/gftyzzovi.sHtML

Ruby: public / protected / private
来源：http://baike.hesvh.cn/Article/details/ggpmervxs.sHtML

C#:   public / protected / private / internal
来源：http://baike.hesvh.cn/Article/details/gtgvpgtsj.sHtML

[G11] getter / setter
来源：http://3g.hesvh.cn/Article/details/gncvrdntc.sHtML

Py:   @property 与 @x.setter
来源：http://3g.hesvh.cn/Article/details/gsvjhtdni.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.zdbjq.cn/Article/details/gtllojshn.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.zdbjq.cn/Article/details/gmhhoughj.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.fehbvm.com/Article/details/gpkaeexsx.sHtML

Java: public String getName() { return name; }
来源：http://m.share.zdbjq.cn/Article/details/gsnxrjxnm.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.hesvh.cn/Article/details/grwzsoage.sHtML

Ruby: attr_accessor :name
来源：http://wap.zdbjq.cn/Article/details/gmuqviicy.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.fehbvm.com/Article/details/gfqchnzrt.sHtML

[G12] 对象转字符串
来源：http://baike.zdbjq.cn/Article/details/gczbirnnb.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.hesvh.cn/Article/details/gtiyrkuss.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.zdbjq.cn/Article/details/gcfyerqdm.sHtML

JS:   toString() { return this.name; }
来源：http://blog.fehbvm.com/Article/details/gsawhiwpb.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/gnpqwptwt.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.hesvh.cn/Article/details/gofhzzpvj.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.zdbjq.cn/Article/details/gujbygxhq.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.hesvh.cn/Article/details/gxuhvuykg.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.hesvh.cn/Article/details/gwcdvuyib.sHtML

[G13] 判断对象类型
来源：http://www.share.zdbjq.cn/Article/details/gwwsfqcbi.sHtML

Py:   isinstance(u, User)
来源：http://read.share.fehbvm.com/Article/details/gtznkaajx.sHtML

PHP:  $u instanceof User
来源：http://m.share.fehbvm.com/Article/details/gismdpwqc.sHtML

JS:   u instanceof User
来源：http://www.m.share.hesvh.cn/Article/details/gtnfxkwdf.sHtML

TS:   u instanceof User
来源：http://3g.fehbvm.com/Article/details/gkzbvtfxs.sHtML

Java: u instanceof User
来源：http://m.share.hesvh.cn/Article/details/gqmnpeqve.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.zdbjq.cn/Article/details/gnmvpaqpk.sHtML

Ruby: u.is_a?(User)
来源：http://3g.fehbvm.com/Article/details/guxivdnwj.sHtML

C#:   u is User
来源：http://mobile.fehbvm.com/Article/details/gqxapyezl.sHtML

[G14] 数据类 / record
来源：http://wap.zdbjq.cn/Article/details/ghxdqysgz.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.fehbvm.com/Article/details/gkeoxubha.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.zdbjq.cn/Article/details/gfrafowwx.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.zdbjq.cn/Article/details/gtepkqzcd.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.fehbvm.com/Article/details/gpdpionbm.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.fehbvm.com/Article/details/gmktffxvr.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.fehbvm.com/Article/details/gtacrgeks.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.fehbvm.com/Article/details/goomqwsmd.sHtML

C#:   record User(string Name, int Age);
来源：http://m.share.hesvh.cn/Article/details/gpzfpmole.sHtML

[G15] 枚举
来源：http://wap.hesvh.cn/Article/details/guywonsnj.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.zdbjq.cn/Article/details/gbehwecdl.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.zdbjq.cn/Article/details/gdcjditsa.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.fehbvm.com/Article/details/gtjdwtegg.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.fehbvm.com/Article/details/gvdqibakr.sHtML

Java: enum Color { RED, GREEN }
来源：http://m.share.zdbjq.cn/Article/details/gqbabrmmo.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.zdbjq.cn/Article/details/gsngkzwvl.sHtML

Ruby: Color = %i[red green].freeze
来源：http://read.share.zdbjq.cn/Article/details/ghdifnlyf.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.fehbvm.com/Article/details/gmkjnqgdd.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.hesvh.cn/Article/details/gdkrkfaug.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.fehbvm.com/Article/details/gpcavphio.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.zdbjq.cn/Article/details/gxstnflia.sHtML

JS:   Object.entries(obj)
来源：http://wap.zdbjq.cn/Article/details/ggsfbvhbl.sHtML

TS:   Object.entries(obj)
来源：http://mobile.hesvh.cn/Article/details/ghnjqtvtu.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.zdbjq.cn/Article/details/gkwsjvade.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.hesvh.cn/Article/details/gnnphdgwq.sHtML

Ruby: obj.instance_variables
来源：http://mobile.hesvh.cn/Article/details/ggqgxweam.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.hesvh.cn/Article/details/gvldqahah.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gvbnnlvrv.sHtML

H. 异常与错误处理
来源：http://www.blog.fehbvm.com/Article/details/gevtsmqcv.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gwcppgwkw.sHtML

[H01] try / catch 基础
来源：http://wap.hesvh.cn/Article/details/gvwwrjxdw.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.fehbvm.com/Article/details/giovvszmv.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.hesvh.cn/Article/details/gucjlvtcd.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.fehbvm.com/Article/details/gytvkqoff.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.blog.zdbjq.cn/Article/details/grhtavykc.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.share.hesvh.cn/Article/details/gmwmrerrx.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.fehbvm.com/Article/details/gqwossxjq.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://3g.zdbjq.cn/Article/details/gvghjgrkm.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://blog.fehbvm.com/Article/details/gchoeppsg.sHtML

[H02] finally / ensure 收尾
来源：http://baike.zdbjq.cn/Article/details/gwstpleib.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://read.share.fehbvm.com/Article/details/gpqnbzfjg.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://blog.zdbjq.cn/Article/details/gsjebrvuy.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.zdbjq.cn/Article/details/guycyqjhe.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.hesvh.cn/Article/details/gfiyhjiks.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.fehbvm.com/Article/details/gzdejhmue.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.fehbvm.com/Article/details/ghmrtpogz.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.hesvh.cn/Article/details/gzewkphlf.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/gglwmiqbz.sHtML

[H03] 主动抛出异常
来源：http://m.share.hesvh.cn/Article/details/gejbwqhhp.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.hesvh.cn/Article/details/gyhmaqgqi.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.blog.zdbjq.cn/Article/details/gowxypxmn.sHtML

JS:   throw new Error("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/gnuupevpi.sHtML

TS:   throw new Error("错误信息");
来源：http://blog.zdbjq.cn/Article/details/ggjdaxaha.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://read.share.fehbvm.com/Article/details/gptjcygvt.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://baike.fehbvm.com/Article/details/gsptpeyhl.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://wap.zdbjq.cn/Article/details/gjtaeytdo.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://blog.fehbvm.com/Article/details/ghoicnyec.sHtML

[H04] 自定义异常类型
来源：http://read.share.zdbjq.cn/Article/details/gcpztungl.sHtML

Py:   class MyError(Exception): pass
来源：http://3g.hesvh.cn/Article/details/ghrnxemxv.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://read.share.hesvh.cn/Article/details/gtipmbcaz.sHtML

JS:   class MyError extends Error {}
来源：http://wap.hesvh.cn/Article/details/gybakjexl.sHtML

TS:   class MyError extends Error {}
来源：http://3g.zdbjq.cn/Article/details/gbkfnnckl.sHtML

Java: class MyException extends RuntimeException {}
来源：http://mobile.zdbjq.cn/Article/details/gwlvighat.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://read.share.hesvh.cn/Article/details/ggunftfqw.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.share.fehbvm.com/Article/details/gutcoyduh.sHtML

C#:   class MyException : Exception {}
来源：http://www.share.hesvh.cn/Article/details/gevdipwnn.sHtML

[H05] 捕获特定类型
来源：http://m.share.zdbjq.cn/Article/details/gumgjzvzd.sHtML

Py:   except ValueError as e:
来源：http://www.blog.hesvh.cn/Article/details/gyaznjxjp.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.fehbvm.com/Article/details/gxtqhgkjo.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://m.share.hesvh.cn/Article/details/gthxxcpoz.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.share.fehbvm.com/Article/details/ggmwiljko.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://wap.hesvh.cn/Article/details/gupujbpmq.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.blog.hesvh.cn/Article/details/gpwcjkwhg.sHtML

Ruby: rescue ArgumentError => e
来源：http://m.share.fehbvm.com/Article/details/gbfbkguzf.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://blog.hesvh.cn/Article/details/gbdghxfzd.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.share.hesvh.cn/Article/details/gjoeqcosg.sHtML

Py:   value = d.get("k") or default
来源：http://baike.hesvh.cn/Article/details/gizhnrdfe.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://wap.fehbvm.com/Article/details/gswwdibyi.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.blog.fehbvm.com/Article/details/guowiqutc.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.blog.hesvh.cn/Article/details/gwllwkohj.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://m.share.zdbjq.cn/Article/details/guugffmlr.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://baike.fehbvm.com/Article/details/gabucomlq.sHtML

Ruby: d&.dig(:a, :b)
来源：http://read.share.hesvh.cn/Article/details/ghhppnpjm.sHtML

C#:   obj?.A?.B ?? default
来源：http://wap.hesvh.cn/Article/details/gaobanmaf.sHtML

[H07] 断言
来源：http://www.share.zdbjq.cn/Article/details/gajafpkcz.sHtML

Py:   assert x > 0, "必须为正"
来源：http://mobile.zdbjq.cn/Article/details/gjcqiegvk.sHtML

PHP:  assert($x > 0);
来源：http://m.share.hesvh.cn/Article/details/gorqyrrbw.sHtML

JS:   console.assert(x > 0);
来源：http://m.share.fehbvm.com/Article/details/ganvmxmjz.sHtML

TS:   console.assert(x > 0);
来源：http://www.blog.zdbjq.cn/Article/details/gaocyvcgm.sHtML

Java: assert x > 0 : "必须为正";
来源：http://baike.hesvh.cn/Article/details/gfqlopjao.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://blog.hesvh.cn/Article/details/gxzjplmoh.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://baike.zdbjq.cn/Article/details/guhtzmywz.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.m.share.fehbvm.com/Article/details/gsnfxsuea.sHtML

[H08] 获取错误信息与堆栈
来源：http://read.share.hesvh.cn/Article/details/gqvjeigsn.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://blog.fehbvm.com/Article/details/gyjguxkak.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wap.hesvh.cn/Article/details/grflvjnxr.sHtML

JS:   e.message;  e.stack
来源：http://wap.zdbjq.cn/Article/details/gbpnvqtfa.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://m.share.fehbvm.com/Article/details/gmeyqgsog.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://read.share.zdbjq.cn/Article/details/gvlcfsgai.sHtML

Go:   err.Error()
来源：http://mobile.hesvh.cn/Article/details/gpsyqsrtt.sHtML

Ruby: e.message;  e.backtrace
来源：http://read.share.fehbvm.com/Article/details/gqpjmjsrf.sHtML

C#:   e.Message;  e.StackTrace
来源：http://baike.zdbjq.cn/Article/details/gxejplaby.sHtML

[H09] 带错误码的异常
来源：http://baike.zdbjq.cn/Article/details/ggkvcohdc.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://m.share.zdbjq.cn/Article/details/gmcpvgbag.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.share.fehbvm.com/Article/details/gisdnnwyj.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://m.share.fehbvm.com/Article/details/gngypyukh.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://read.share.fehbvm.com/Article/details/ghxqvghjb.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://read.share.zdbjq.cn/Article/details/gpvvzcolo.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://blog.zdbjq.cn/Article/details/gbfuncsbx.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://wap.zdbjq.cn/Article/details/gsqubqbvm.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://read.share.zdbjq.cn/Article/details/gffpxbwry.sHtML

[H10] 资源自动释放
来源：http://baike.hesvh.cn/Article/details/gegxwtenu.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://m.share.zdbjq.cn/Article/details/gtmrodcxi.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://read.share.fehbvm.com/Article/details/gaotmxkhs.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.zdbjq.cn/Article/details/glyjugnei.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.hesvh.cn/Article/details/gubrfiflc.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.blog.fehbvm.com/Article/details/ghspnfgzu.sHtML

Go:   defer f.Close()
来源：http://blog.hesvh.cn/Article/details/grvnoniei.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.blog.fehbvm.com/Article/details/grpmaxvel.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gcwtxvueq.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gdzeytocv.sHtML

I. 正则表达式
来源：http://wap.hesvh.cn/Article/details/gthruaorm.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gdgwbkkmz.sHtML

[I01] 判断是否匹配
来源：http://3g.fehbvm.com/Article/details/gxxolglrg.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.blog.hesvh.cn/Article/details/gmhhrjref.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://m.share.zdbjq.cn/Article/details/gqzxlbyrc.sHtML

JS:   /\d+/.test(s)
来源：http://baike.fehbvm.com/Article/details/goqayodup.sHtML

TS:   /\d+/.test(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gxzttbmss.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://read.share.hesvh.cn/Article/details/gojnscosb.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://baike.hesvh.cn/Article/details/gjuvuzdhg.sHtML

Ruby: s.match?(/\d+/)
来源：http://blog.fehbvm.com/Article/details/gyjtjenzj.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.m.share.fehbvm.com/Article/details/gnzfrkjvo.sHtML

[I02] 提取所有匹配
来源：http://3g.zdbjq.cn/Article/details/ghvevtzsd.sHtML

Py:   re.findall(r"\d+", s)
来源：http://m.share.zdbjq.cn/Article/details/gavbztwkx.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.m.share.fehbvm.com/Article/details/guzxbgfkv.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wap.fehbvm.com/Article/details/gkzcxuofc.sHtML

TS:   s.match(/\d+/g)
来源：http://www.m.share.zdbjq.cn/Article/details/gpcupkjcw.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://read.share.zdbjq.cn/Article/details/gwsqxklpb.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://m.share.zdbjq.cn/Article/details/gmvmxpmxu.sHtML

Ruby: s.scan(/\d+/)
来源：http://read.share.fehbvm.com/Article/details/gtwivxloj.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://blog.hesvh.cn/Article/details/gvitkipcf.sHtML

[I03] 提取捕获分组
来源：http://www.share.fehbvm.com/Article/details/gkqygqakk.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.blog.fehbvm.com/Article/details/gxpmhvwaa.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://3g.zdbjq.cn/Article/details/goezahruc.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://m.share.fehbvm.com/Article/details/gmhkoyfev.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://read.share.hesvh.cn/Article/details/glshoybqq.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://blog.fehbvm.com/Article/details/gbvsqivvz.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://blog.hesvh.cn/Article/details/ghqyguwlh.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://blog.zdbjq.cn/Article/details/guqhlprnq.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.blog.hesvh.cn/Article/details/grptrvkoj.sHtML

[I04] 正则替换
来源：http://wap.hesvh.cn/Article/details/gtwqhtcbx.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://wap.hesvh.cn/Article/details/gmapzpvnk.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.share.hesvh.cn/Article/details/grlcdjijw.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://read.share.hesvh.cn/Article/details/gzprlqtjq.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://baike.zdbjq.cn/Article/details/gqwlilvuy.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.blog.hesvh.cn/Article/details/gbhytajii.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://mobile.hesvh.cn/Article/details/gousouxtf.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.m.share.hesvh.cn/Article/details/gxzbitsou.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.m.share.fehbvm.com/Article/details/gewhxquef.sHtML

[I05] 按正则拆分
来源：http://www.share.zdbjq.cn/Article/details/gneihzifv.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://blog.fehbvm.com/Article/details/grelxygwl.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gdtqrxzbh.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://wap.zdbjq.cn/Article/details/gopkwkcsz.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.share.fehbvm.com/Article/details/gwrkfzxdz.sHtML

Java: s.split("\\s*,\\s*")
来源：http://mobile.hesvh.cn/Article/details/gbaxbejax.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wap.hesvh.cn/Article/details/ghwqsulxp.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://mobile.fehbvm.com/Article/details/gbanrmhbi.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wap.fehbvm.com/Article/details/gtlfuodoj.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.share.fehbvm.com/Article/details/gomglsjrv.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://m.share.fehbvm.com/Article/details/gegkgpgge.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://baike.hesvh.cn/Article/details/gaiequbyl.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.fehbvm.com/Article/details/gwmxdyskt.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.hesvh.cn/Article/details/gpgfoiqii.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.blog.hesvh.cn/Article/details/gowoawcji.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://baike.zdbjq.cn/Article/details/gfpilqlbs.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://blog.zdbjq.cn/Article/details/gnifktfgz.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.share.zdbjq.cn/Article/details/gxvtnsnrf.sHtML

[I07] 忽略大小写与多行模式
来源：http://mobile.zdbjq.cn/Article/details/gkouobdwg.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://3g.zdbjq.cn/Article/details/giwdolxbw.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.blog.zdbjq.cn/Article/details/gabzpgucc.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://baike.zdbjq.cn/Article/details/gnfxbgbzd.sHtML

TS:   /error/gim
来源：http://www.share.zdbjq.cn/Article/details/gtftxfwio.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mobile.zdbjq.cn/Article/details/gfdmughsh.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://blog.fehbvm.com/Article/details/gencfsdqp.sHtML

Ruby: s.scan(/error/i)
来源：http://www.blog.fehbvm.com/Article/details/gxkbcbfba.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mobile.hesvh.cn/Article/details/gussxwgso.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.share.fehbvm.com/Article/details/gclzqjjbq.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.blog.zdbjq.cn/Article/details/gluvrglkg.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.blog.fehbvm.com/Article/details/gffyputop.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.fehbvm.com/Article/details/gnvyubbyd.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.fehbvm.com/Article/details/gsahnnuco.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.blog.fehbvm.com/Article/details/gcqtucecz.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.m.share.fehbvm.com/Article/details/gwjtbgvym.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://read.share.fehbvm.com/Article/details/gqhvaxsja.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.blog.zdbjq.cn/Article/details/guauckryr.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/greogzbhh.sHtML

J. 日期与时间
来源：http://www.share.zdbjq.cn/Article/details/gggciawpa.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gehwhssbi.sHtML

[J01] 获取当前时间
来源：http://3g.zdbjq.cn/Article/details/gcixycfbx.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://m.share.hesvh.cn/Article/details/gijeosdpk.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://blog.zdbjq.cn/Article/details/gvwrcyfxr.sHtML

JS:   new Date();  Date.now()
来源：http://baike.fehbvm.com/Article/details/gmpytudeu.sHtML

TS:   new Date();  Date.now()
来源：http://m.share.hesvh.cn/Article/details/gnfuacsqg.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://baike.hesvh.cn/Article/details/gxtgvszky.sHtML

Go:   time.Now()
来源：http://www.m.share.hesvh.cn/Article/details/gedyjbsbu.sHtML

Ruby: Time.now
来源：http://wap.hesvh.cn/Article/details/gsbhwzlqy.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://3g.fehbvm.com/Article/details/gzzkxloah.sHtML

[J02] 格式化输出
来源：http://www.m.share.fehbvm.com/Article/details/gjlwklisl.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.fehbvm.com/Article/details/gnqeqygxc.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://baike.hesvh.cn/Article/details/gludcyyek.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.blog.hesvh.cn/Article/details/gxvixjgqy.sHtML

TS:   d.toISOString()
来源：http://3g.hesvh.cn/Article/details/gncyufnfw.sHtML


<!-- 参考信息 -->