代发 wailian999

Ruby: @name = "x"
来源：http://wap.hesvh.cn/Article/details/gelcizbce.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.fehbvm.com/Article/details/gtornapty.sHtML

[G04] 定义方法
来源：http://blog.hesvh.cn/Article/details/gamcqffcq.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.fehbvm.com/Article/details/gvxpnvsyz.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.zdbjq.cn/Article/details/gxpaeoqaa.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.zdbjq.cn/Article/details/grnznluxk.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/gxeuebzzz.sHtML

Java: String greet() { return name; }
来源：http://m.share.zdbjq.cn/Article/details/gvshturli.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.hesvh.cn/Article/details/gsojkgxfg.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.hesvh.cn/Article/details/gbievbkvr.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.zdbjq.cn/Article/details/gzfaesgyb.sHtML

[G05] 继承
来源：http://wap.zdbjq.cn/Article/details/gzrzxgnbr.sHtML

Py:   class Admin(User): pass
来源：http://www.share.zdbjq.cn/Article/details/gxaabqjfh.sHtML

PHP:  class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/gbiqvpqmy.sHtML

JS:   class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/gypqgoakd.sHtML

TS:   class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/gsklbznnr.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gkbtyebje.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.fehbvm.com/Article/details/gbqauibfk.sHtML

Ruby: class Admin < User; end
来源：http://3g.zdbjq.cn/Article/details/gcebldwts.sHtML

C#:   class Admin : User {}
来源：http://www.share.zdbjq.cn/Article/details/gdgpsihhe.sHtML

[G06] 重写方法
来源：http://read.share.hesvh.cn/Article/details/gqtsdkbsm.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.hesvh.cn/Article/details/gjvhhzjcg.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/gjpswupge.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/gsksoqgjb.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/gfaocbzmj.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/grdkjtaht.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.fehbvm.com/Article/details/gvzibhqsx.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.hesvh.cn/Article/details/gijfqouqg.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.hesvh.cn/Article/details/ghlxdzqpy.sHtML

[G07] 调用父类方法
来源：http://www.m.share.zdbjq.cn/Article/details/gejiepqsf.sHtML

Py:   super().greet()
来源：http://wap.zdbjq.cn/Article/details/grgzmbmaz.sHtML

PHP:  parent::greet();
来源：http://m.share.zdbjq.cn/Article/details/gnbkeoadb.sHtML

JS:   super.greet();
来源：http://m.share.fehbvm.com/Article/details/gdukekzum.sHtML

TS:   super.greet();
来源：http://wap.fehbvm.com/Article/details/ghmvgrfgq.sHtML

Java: super.greet();
来源：http://www.share.fehbvm.com/Article/details/gnzfqywnm.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.fehbvm.com/Article/details/ghemglcpk.sHtML

Ruby: super
来源：http://baike.zdbjq.cn/Article/details/goyxirnnq.sHtML

C#:   base.Greet();
来源：http://baike.hesvh.cn/Article/details/ggfvwnies.sHtML

[G08] 静态方法与属性
来源：http://mobile.hesvh.cn/Article/details/gvxwclynx.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.hesvh.cn/Article/details/ghdlqnpct.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.fehbvm.com/Article/details/gqmdydmcv.sHtML

JS:   static f() {}
来源：http://3g.zdbjq.cn/Article/details/gtlduabzr.sHtML

TS:   static f(): void {}
来源：http://baike.fehbvm.com/Article/details/gmtxyyckf.sHtML

Java: static void f() {}
来源：http://www.share.zdbjq.cn/Article/details/gfkrjcfeu.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.fehbvm.com/Article/details/gcarqtcrv.sHtML

Ruby: def self.f; end
来源：http://3g.hesvh.cn/Article/details/glycsranw.sHtML

C#:   public static void F() {}
来源：http://wap.zdbjq.cn/Article/details/gtkhtmbaq.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.fehbvm.com/Article/details/gkcuocnuh.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.hesvh.cn/Article/details/gbzcwxhfn.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.fehbvm.com/Article/details/gbizhiwhu.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.hesvh.cn/Article/details/guokrcddk.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.hesvh.cn/Article/details/ghjpgxciu.sHtML

Java: interface Shape { double area(); }
来源：http://baike.zdbjq.cn/Article/details/gyrigamvk.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.hesvh.cn/Article/details/gxnqospan.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.zdbjq.cn/Article/details/gemqllmrf.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.hesvh.cn/Article/details/guwwznjwp.sHtML

[G10] 访问控制
来源：http://baike.hesvh.cn/Article/details/gmwncwmyz.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.hesvh.cn/Article/details/gqvjdutaa.sHtML

PHP:  public / protected / private
来源：http://mobile.hesvh.cn/Article/details/guiluucio.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.hesvh.cn/Article/details/gzwsqjfic.sHtML

TS:   public / protected / private
来源：http://www.share.hesvh.cn/Article/details/gnizehsrz.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.fehbvm.com/Article/details/glmamryxt.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.fehbvm.com/Article/details/guujnuoje.sHtML

Ruby: public / protected / private
来源：http://baike.zdbjq.cn/Article/details/ghyyazuax.sHtML

C#:   public / protected / private / internal
来源：http://wap.hesvh.cn/Article/details/gppkbvxfb.sHtML

[G11] getter / setter
来源：http://3g.hesvh.cn/Article/details/gmqlgexbm.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.fehbvm.com/Article/details/gxpnwphpr.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.hesvh.cn/Article/details/gnjfcznjh.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.hesvh.cn/Article/details/giekpegeo.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.zdbjq.cn/Article/details/gksaxqhtf.sHtML

Java: public String getName() { return name; }
来源：http://read.share.fehbvm.com/Article/details/gzjhfneax.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.fehbvm.com/Article/details/ghwnbgvla.sHtML

Ruby: attr_accessor :name
来源：http://blog.hesvh.cn/Article/details/gjqrohmqt.sHtML

C#:   public string Name { get; set; }
来源：http://wap.hesvh.cn/Article/details/gakmwrnra.sHtML

[G12] 对象转字符串
来源：http://m.share.hesvh.cn/Article/details/gthnhxxcc.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.hesvh.cn/Article/details/gbrsxglxg.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.hesvh.cn/Article/details/gxcwuiuys.sHtML

JS:   toString() { return this.name; }
来源：http://wap.hesvh.cn/Article/details/ggdkodili.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/gvfqgpswa.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/gdkbrmrcn.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.zdbjq.cn/Article/details/gpisvavph.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.hesvh.cn/Article/details/gmlhfnyca.sHtML

C#:   public override string ToString() => Name;
来源：http://www.share.zdbjq.cn/Article/details/gsptvcplq.sHtML

[G13] 判断对象类型
来源：http://m.share.hesvh.cn/Article/details/gyizypupq.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.fehbvm.com/Article/details/gzgbjpgen.sHtML

PHP:  $u instanceof User
来源：http://m.share.fehbvm.com/Article/details/gktrqoxcq.sHtML

JS:   u instanceof User
来源：http://blog.zdbjq.cn/Article/details/gxhcgqqec.sHtML

TS:   u instanceof User
来源：http://baike.hesvh.cn/Article/details/gdwcgjvag.sHtML

Java: u instanceof User
来源：http://wap.hesvh.cn/Article/details/gwoayxoae.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.fehbvm.com/Article/details/gqqkvbgec.sHtML

Ruby: u.is_a?(User)
来源：http://blog.fehbvm.com/Article/details/gsyreyipu.sHtML

C#:   u is User
来源：http://baike.hesvh.cn/Article/details/gvrhsojwe.sHtML

[G14] 数据类 / record
来源：http://m.share.zdbjq.cn/Article/details/gwvzvpwpe.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.fehbvm.com/Article/details/ghktcklip.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.zdbjq.cn/Article/details/gbllufsya.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.fehbvm.com/Article/details/ghjmlrgkp.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.zdbjq.cn/Article/details/gajkredms.sHtML

Java: record User(String name, int age) {}
来源：http://baike.fehbvm.com/Article/details/gspmwiutf.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.hesvh.cn/Article/details/gffphsbpv.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.fehbvm.com/Article/details/gdfffvocz.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.zdbjq.cn/Article/details/gmjvsycfk.sHtML

[G15] 枚举
来源：http://blog.fehbvm.com/Article/details/gdrkyimfq.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.zdbjq.cn/Article/details/gxrnaradr.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.hesvh.cn/Article/details/gugxtolzg.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.hesvh.cn/Article/details/gmneikzky.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.hesvh.cn/Article/details/gqjtnyyzo.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.zdbjq.cn/Article/details/gbahstxjc.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.zdbjq.cn/Article/details/gvlqcfkzb.sHtML

Ruby: Color = %i[red green].freeze
来源：http://m.share.zdbjq.cn/Article/details/gyocflfcl.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.zdbjq.cn/Article/details/guwkqassq.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.hesvh.cn/Article/details/gmypjoovf.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.hesvh.cn/Article/details/ggrtlnhkk.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.zdbjq.cn/Article/details/gmvzyubqs.sHtML

JS:   Object.entries(obj)
来源：http://read.share.fehbvm.com/Article/details/ghfdimyjt.sHtML

TS:   Object.entries(obj)
来源：http://m.share.hesvh.cn/Article/details/gauukljub.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.fehbvm.com/Article/details/gjzskvykf.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.zdbjq.cn/Article/details/gvalwrhac.sHtML

Ruby: obj.instance_variables
来源：http://baike.hesvh.cn/Article/details/gitnqxbpl.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.hesvh.cn/Article/details/gjcjhjyeb.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gikljcyuw.sHtML

H. 异常与错误处理
来源：http://3g.zdbjq.cn/Article/details/gmtqmmmjy.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gpxdocihd.sHtML

[H01] try / catch 基础
来源：http://baike.hesvh.cn/Article/details/gocrgfmci.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.hesvh.cn/Article/details/gbjmxewuj.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.hesvh.cn/Article/details/gminuxfak.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://blog.hesvh.cn/Article/details/gvzycqobo.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.fehbvm.com/Article/details/gjstzavrp.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.hesvh.cn/Article/details/gkyiajhlj.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.fehbvm.com/Article/details/grobhzjrj.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://blog.zdbjq.cn/Article/details/gooyzyury.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.fehbvm.com/Article/details/gjaltyqoe.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.fehbvm.com/Article/details/gqrnxfoia.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.share.fehbvm.com/Article/details/gaqwerdaz.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.m.share.fehbvm.com/Article/details/gyjerjuti.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://baike.fehbvm.com/Article/details/ghwyvjhxp.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.fehbvm.com/Article/details/gtaegruvy.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/gpeybrhiw.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.zdbjq.cn/Article/details/gfhmgiqib.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.fehbvm.com/Article/details/gjuwndnay.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.share.zdbjq.cn/Article/details/ganugenif.sHtML

[H03] 主动抛出异常
来源：http://www.m.share.zdbjq.cn/Article/details/gbnrmobbl.sHtML

Py:   raise ValueError("错误信息")
来源：http://3g.hesvh.cn/Article/details/gjfeilsie.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.fehbvm.com/Article/details/gpykiiegp.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.zdbjq.cn/Article/details/ghiuwovbk.sHtML

TS:   throw new Error("错误信息");
来源：http://baike.zdbjq.cn/Article/details/gfgzxyfyn.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/gnfovvahw.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.blog.hesvh.cn/Article/details/gtmjhwehr.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://wap.fehbvm.com/Article/details/glvpvrpgy.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.fehbvm.com/Article/details/glghcbcwj.sHtML

[H04] 自定义异常类型
来源：http://www.blog.hesvh.cn/Article/details/gzjqmnwcn.sHtML

Py:   class MyError(Exception): pass
来源：http://m.share.hesvh.cn/Article/details/gqbeuoioc.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://wap.hesvh.cn/Article/details/gfilctpkd.sHtML

JS:   class MyError extends Error {}
来源：http://m.share.hesvh.cn/Article/details/gqrdiveiv.sHtML

TS:   class MyError extends Error {}
来源：http://mobile.zdbjq.cn/Article/details/ghkjqvthc.sHtML

Java: class MyException extends RuntimeException {}
来源：http://3g.hesvh.cn/Article/details/glwukkovv.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://baike.zdbjq.cn/Article/details/gncaxkvuh.sHtML

Ruby: class MyError < StandardError; end
来源：http://blog.zdbjq.cn/Article/details/gyxzljadm.sHtML

C#:   class MyException : Exception {}
来源：http://www.share.fehbvm.com/Article/details/ghwvscike.sHtML

[H05] 捕获特定类型
来源：http://m.share.hesvh.cn/Article/details/gmjitkquc.sHtML

Py:   except ValueError as e:
来源：http://www.blog.hesvh.cn/Article/details/gtqbywmpf.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://read.share.zdbjq.cn/Article/details/gqxvprhmd.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.m.share.fehbvm.com/Article/details/gbeecxnme.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://blog.hesvh.cn/Article/details/gorelcgss.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://blog.zdbjq.cn/Article/details/gcmsixnpr.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.m.share.hesvh.cn/Article/details/gumqugjuy.sHtML

Ruby: rescue ArgumentError => e
来源：http://blog.zdbjq.cn/Article/details/gatvmntbf.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.m.share.fehbvm.com/Article/details/gybpgsvtz.sHtML

[H06] 可选值 / 空值安全访问
来源：http://wap.hesvh.cn/Article/details/gizxwgadi.sHtML

Py:   value = d.get("k") or default
来源：http://mobile.hesvh.cn/Article/details/geryvwres.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://wap.zdbjq.cn/Article/details/gvuxocavx.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.share.fehbvm.com/Article/details/gufbhwzuv.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://wap.fehbvm.com/Article/details/ghmngvllq.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://m.share.zdbjq.cn/Article/details/gltgamarv.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://3g.fehbvm.com/Article/details/grzqpzygx.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.m.share.fehbvm.com/Article/details/gsooxjheh.sHtML

C#:   obj?.A?.B ?? default
来源：http://baike.hesvh.cn/Article/details/gpiznyykq.sHtML

[H07] 断言
来源：http://wap.zdbjq.cn/Article/details/gynankolo.sHtML

Py:   assert x > 0, "必须为正"
来源：http://baike.fehbvm.com/Article/details/ggvkfqxrb.sHtML

PHP:  assert($x > 0);
来源：http://blog.zdbjq.cn/Article/details/gsvwmvyqe.sHtML

JS:   console.assert(x > 0);
来源：http://wap.fehbvm.com/Article/details/gnmerlkun.sHtML

TS:   console.assert(x > 0);
来源：http://m.share.zdbjq.cn/Article/details/gchynjpxh.sHtML

Java: assert x > 0 : "必须为正";
来源：http://read.share.zdbjq.cn/Article/details/gqsvtlulm.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://blog.zdbjq.cn/Article/details/ghcdwtehc.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://blog.fehbvm.com/Article/details/glifecgdc.sHtML

C#:   Debug.Assert(x > 0);
来源：http://mobile.zdbjq.cn/Article/details/glmlgqdjf.sHtML

[H08] 获取错误信息与堆栈
来源：http://blog.fehbvm.com/Article/details/gmocsuppy.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://wap.zdbjq.cn/Article/details/golpujizd.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.share.hesvh.cn/Article/details/gtmfhcmih.sHtML

JS:   e.message;  e.stack
来源：http://mobile.zdbjq.cn/Article/details/gxdnryrxk.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://m.share.hesvh.cn/Article/details/gjabxmagd.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.m.share.fehbvm.com/Article/details/gcsdlhbiq.sHtML

Go:   err.Error()
来源：http://www.blog.hesvh.cn/Article/details/gzmeocexz.sHtML

Ruby: e.message;  e.backtrace
来源：http://mobile.hesvh.cn/Article/details/gwwqgcjqk.sHtML

C#:   e.Message;  e.StackTrace
来源：http://baike.fehbvm.com/Article/details/gsrmrimfu.sHtML

[H09] 带错误码的异常
来源：http://www.m.share.fehbvm.com/Article/details/gtnbrftcn.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://baike.fehbvm.com/Article/details/gxgsavbyd.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://baike.hesvh.cn/Article/details/gfquiiisr.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://blog.hesvh.cn/Article/details/gksqdvsxn.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.share.fehbvm.com/Article/details/gsteeydtf.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://m.share.hesvh.cn/Article/details/ghcyvistl.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mobile.fehbvm.com/Article/details/gqfrpodkt.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.share.fehbvm.com/Article/details/gbulznhni.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://blog.zdbjq.cn/Article/details/gwdoabaqa.sHtML

[H10] 资源自动释放
来源：http://mobile.hesvh.cn/Article/details/gwheixbha.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://blog.zdbjq.cn/Article/details/gqikjcqmq.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://baike.hesvh.cn/Article/details/gfahmfhtl.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.fehbvm.com/Article/details/gdcprzfhv.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.hesvh.cn/Article/details/gxznoxrzj.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://m.share.hesvh.cn/Article/details/gxyvsjxqo.sHtML

Go:   defer f.Close()
来源：http://www.share.zdbjq.cn/Article/details/ggavvidac.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wap.fehbvm.com/Article/details/gknbxwmjw.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gcxvwsmlm.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/giueazppu.sHtML

I. 正则表达式
来源：http://baike.fehbvm.com/Article/details/gjbllsrcq.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gnliacfgt.sHtML

[I01] 判断是否匹配
来源：http://m.share.fehbvm.com/Article/details/gwxxiexlw.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.m.share.zdbjq.cn/Article/details/gqbuidkvj.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://read.share.hesvh.cn/Article/details/glgdayiul.sHtML

JS:   /\d+/.test(s)
来源：http://mobile.fehbvm.com/Article/details/gtxqnacbi.sHtML

TS:   /\d+/.test(s)
来源：http://mobile.hesvh.cn/Article/details/gmnokzrwr.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://baike.fehbvm.com/Article/details/gikclwqni.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.blog.hesvh.cn/Article/details/gnptlktre.sHtML

Ruby: s.match?(/\d+/)
来源：http://3g.hesvh.cn/Article/details/ghdyvncxg.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://m.share.zdbjq.cn/Article/details/gcioovncw.sHtML

[I02] 提取所有匹配
来源：http://www.blog.hesvh.cn/Article/details/gipjrbrzk.sHtML

Py:   re.findall(r"\d+", s)
来源：http://wap.zdbjq.cn/Article/details/godpklhqx.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.share.fehbvm.com/Article/details/gxfjqfmpb.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.m.share.hesvh.cn/Article/details/gxjlbuzhs.sHtML

TS:   s.match(/\d+/g)
来源：http://www.share.fehbvm.com/Article/details/gkbnhmtmg.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.blog.hesvh.cn/Article/details/grsbgwhda.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.share.hesvh.cn/Article/details/ggompcucy.sHtML

Ruby: s.scan(/\d+/)
来源：http://baike.hesvh.cn/Article/details/gvlsgauaw.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://read.share.fehbvm.com/Article/details/grxhpgrdf.sHtML

[I03] 提取捕获分组
来源：http://mobile.hesvh.cn/Article/details/gkldwderx.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://3g.hesvh.cn/Article/details/gksoqfzcs.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.m.share.zdbjq.cn/Article/details/gqmfbvpto.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wap.fehbvm.com/Article/details/gwtnhshzr.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://m.share.fehbvm.com/Article/details/gnpfjeifu.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://mobile.zdbjq.cn/Article/details/gfdrvgzur.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://m.share.zdbjq.cn/Article/details/gxbdhvyzr.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mobile.fehbvm.com/Article/details/gitieidia.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.m.share.zdbjq.cn/Article/details/gpsqynnvf.sHtML

[I04] 正则替换
来源：http://baike.zdbjq.cn/Article/details/gaemtegty.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://mobile.fehbvm.com/Article/details/gwrfivctw.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.hesvh.cn/Article/details/gubbdzbuz.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.share.hesvh.cn/Article/details/gyayacqqk.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://3g.zdbjq.cn/Article/details/gjxkcysso.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://wap.hesvh.cn/Article/details/ggdambpqc.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://blog.zdbjq.cn/Article/details/gzjmcncdq.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://read.share.fehbvm.com/Article/details/glouqaxco.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://read.share.hesvh.cn/Article/details/gmfeyqsva.sHtML

[I05] 按正则拆分
来源：http://read.share.hesvh.cn/Article/details/gtosdqnzq.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://wap.fehbvm.com/Article/details/gskvrxujo.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.blog.zdbjq.cn/Article/details/gpzlvyvom.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://read.share.hesvh.cn/Article/details/gcjujxjyp.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://baike.fehbvm.com/Article/details/gumwettqe.sHtML

Java: s.split("\\s*,\\s*")
来源：http://blog.zdbjq.cn/Article/details/gvcfxdxvf.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wap.zdbjq.cn/Article/details/guztmgedq.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.blog.fehbvm.com/Article/details/gskmyoyec.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.share.zdbjq.cn/Article/details/guyrqhhcf.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.share.hesvh.cn/Article/details/ghtankavo.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://read.share.fehbvm.com/Article/details/gdqmeioya.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://baike.hesvh.cn/Article/details/gsapavvhz.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.zdbjq.cn/Article/details/gepmwvuuv.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.zdbjq.cn/Article/details/gichyoqqu.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://3g.fehbvm.com/Article/details/gozvfutes.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://read.share.hesvh.cn/Article/details/gtdlqvhbz.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://baike.zdbjq.cn/Article/details/gltormobl.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.blog.fehbvm.com/Article/details/goiejhaem.sHtML

[I07] 忽略大小写与多行模式
来源：http://3g.fehbvm.com/Article/details/gycgxdtrv.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://read.share.zdbjq.cn/Article/details/gruteoubg.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.share.zdbjq.cn/Article/details/gzlfvgwcv.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://m.share.zdbjq.cn/Article/details/gcxfjyylr.sHtML

TS:   /error/gim
来源：http://baike.zdbjq.cn/Article/details/gtxtaaxba.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.blog.zdbjq.cn/Article/details/goawtufni.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wap.zdbjq.cn/Article/details/gpzmmmlgc.sHtML

Ruby: s.scan(/error/i)
来源：http://m.share.hesvh.cn/Article/details/gsptyfucr.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mobile.fehbvm.com/Article/details/gxjcijpwl.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://baike.fehbvm.com/Article/details/gqoatyhpg.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wap.zdbjq.cn/Article/details/gradhiaeh.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.blog.hesvh.cn/Article/details/ghipclimt.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.zdbjq.cn/Article/details/gdkpxnybs.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.zdbjq.cn/Article/details/gzkzslzfj.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://baike.hesvh.cn/Article/details/ggufqszou.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://m.share.hesvh.cn/Article/details/gtfuhdmkt.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mobile.hesvh.cn/Article/details/gnnevilld.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://baike.zdbjq.cn/Article/details/gccnlsxjz.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/grmenkuvs.sHtML

J. 日期与时间
来源：http://www.share.zdbjq.cn/Article/details/ghtmraefs.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gammqahqr.sHtML

[J01] 获取当前时间
来源：http://wap.hesvh.cn/Article/details/gvmmrvjnn.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://baike.zdbjq.cn/Article/details/gfpqewmmg.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.blog.zdbjq.cn/Article/details/glqrouvmq.sHtML

JS:   new Date();  Date.now()
来源：http://www.share.zdbjq.cn/Article/details/gppxhblao.sHtML

TS:   new Date();  Date.now()
来源：http://mobile.hesvh.cn/Article/details/gposjiflz.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://baike.hesvh.cn/Article/details/gosgsvsnj.sHtML

Go:   time.Now()
来源：http://blog.zdbjq.cn/Article/details/gfanwzolw.sHtML

Ruby: Time.now
来源：http://mobile.zdbjq.cn/Article/details/gsptzdaoo.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://blog.zdbjq.cn/Article/details/gkslusmkx.sHtML

[J02] 格式化输出
来源：http://read.share.fehbvm.com/Article/details/gwpgkrqqw.sHtML


<!-- 参考信息 -->