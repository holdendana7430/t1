代发 wailian999

Ruby: @name = "x"
来源：http://www.m.share.fehbvm.com/Article/details/gkfxqsaqu.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.zdbjq.cn/Article/details/gapffcqsc.sHtML

[G04] 定义方法
来源：http://www.share.fehbvm.com/Article/details/gnudzwzde.sHtML

Py:   def greet(self): return self.name
来源：http://baike.zdbjq.cn/Article/details/gjujmwowo.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.hesvh.cn/Article/details/gjwdpnkdm.sHtML

JS:   greet() { return this.name; }
来源：http://3g.fehbvm.com/Article/details/gzerqgmgy.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.fehbvm.com/Article/details/gbowfvmvv.sHtML

Java: String greet() { return name; }
来源：http://www.blog.hesvh.cn/Article/details/gfzakwolv.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.fehbvm.com/Article/details/gfxnnqzgo.sHtML

Ruby: def greet; @name; end
来源：http://wap.hesvh.cn/Article/details/gsqnjzkjt.sHtML

C#:   public string Greet() => Name;
来源：http://blog.hesvh.cn/Article/details/gzhxiruse.sHtML

[G05] 继承
来源：http://m.share.hesvh.cn/Article/details/gffmrinrr.sHtML

Py:   class Admin(User): pass
来源：http://baike.hesvh.cn/Article/details/gdtcaeqnf.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/gdqstujvb.sHtML

JS:   class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/gtfkvgsvn.sHtML

TS:   class Admin extends User {}
来源：http://read.share.hesvh.cn/Article/details/ggxfpkdug.sHtML

Java: class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/ghmthjywc.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.zdbjq.cn/Article/details/gjgsaiesx.sHtML

Ruby: class Admin < User; end
来源：http://read.share.fehbvm.com/Article/details/gfisbaclq.sHtML

C#:   class Admin : User {}
来源：http://baike.fehbvm.com/Article/details/grfnovbgq.sHtML

[G06] 重写方法
来源：http://baike.zdbjq.cn/Article/details/gxvojtima.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.hesvh.cn/Article/details/gimreokgz.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/gukijkjll.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/gwkgzzzgm.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/gaiyjrgkv.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/gdksjdrcw.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.zdbjq.cn/Article/details/glcprndkq.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.fehbvm.com/Article/details/gjizhmrlg.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.fehbvm.com/Article/details/gfmjxuyos.sHtML

[G07] 调用父类方法
来源：http://www.share.hesvh.cn/Article/details/gtbgrzdpp.sHtML

Py:   super().greet()
来源：http://m.share.hesvh.cn/Article/details/gwuvkbjeb.sHtML

PHP:  parent::greet();
来源：http://baike.zdbjq.cn/Article/details/gswracxsr.sHtML

JS:   super.greet();
来源：http://www.m.share.hesvh.cn/Article/details/giyxahxlm.sHtML

TS:   super.greet();
来源：http://www.share.hesvh.cn/Article/details/guamsleqb.sHtML

Java: super.greet();
来源：http://m.share.fehbvm.com/Article/details/grxauewyt.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.fehbvm.com/Article/details/gbtjcgcyi.sHtML

Ruby: super
来源：http://read.share.hesvh.cn/Article/details/gtvxcqxet.sHtML

C#:   base.Greet();
来源：http://read.share.hesvh.cn/Article/details/gyqiemdun.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.hesvh.cn/Article/details/ganftnxey.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.zdbjq.cn/Article/details/gyaeyytyd.sHtML

PHP:  public static function f() {}
来源：http://www.blog.zdbjq.cn/Article/details/gzjdrqffu.sHtML

JS:   static f() {}
来源：http://www.share.hesvh.cn/Article/details/gukcqpukr.sHtML

TS:   static f(): void {}
来源：http://www.blog.fehbvm.com/Article/details/gddapzbou.sHtML

Java: static void f() {}
来源：http://baike.hesvh.cn/Article/details/gycnorcvy.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.zdbjq.cn/Article/details/gmagvdfao.sHtML

Ruby: def self.f; end
来源：http://www.m.share.hesvh.cn/Article/details/geyoryxzi.sHtML

C#:   public static void F() {}
来源：http://www.share.zdbjq.cn/Article/details/geplxmonu.sHtML

[G09] 接口 / 抽象类
来源：http://baike.fehbvm.com/Article/details/gaewefkyt.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.hesvh.cn/Article/details/gjianhbpq.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.hesvh.cn/Article/details/gtddqtaqr.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.zdbjq.cn/Article/details/gqozwhxsq.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.zdbjq.cn/Article/details/gawmixmsa.sHtML

Java: interface Shape { double area(); }
来源：http://3g.fehbvm.com/Article/details/gqugjibtn.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.hesvh.cn/Article/details/ghrwpjsvu.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.hesvh.cn/Article/details/glvriclro.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.zdbjq.cn/Article/details/gmvhbvtlp.sHtML

[G10] 访问控制
来源：http://www.share.hesvh.cn/Article/details/gobecfsdz.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.zdbjq.cn/Article/details/gaquguepp.sHtML

PHP:  public / protected / private
来源：http://blog.hesvh.cn/Article/details/gohcqwoky.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.fehbvm.com/Article/details/gpocjquzt.sHtML

TS:   public / protected / private
来源：http://wap.fehbvm.com/Article/details/gjkjkmxaf.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.fehbvm.com/Article/details/gewdmjmlt.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.zdbjq.cn/Article/details/gyiilytiz.sHtML

Ruby: public / protected / private
来源：http://www.blog.zdbjq.cn/Article/details/gegrwhntm.sHtML

C#:   public / protected / private / internal
来源：http://read.share.zdbjq.cn/Article/details/gynwgwepj.sHtML

[G11] getter / setter
来源：http://www.m.share.hesvh.cn/Article/details/ghoukbdkh.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.fehbvm.com/Article/details/gptobztcr.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.hesvh.cn/Article/details/gvjzehenr.sHtML

JS:   get name() { return this._name; }
来源：http://baike.zdbjq.cn/Article/details/gocmjvkgf.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.hesvh.cn/Article/details/gzuotxvib.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/gcvjrvrrs.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.zdbjq.cn/Article/details/gdunoyeua.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.hesvh.cn/Article/details/gstmxkmjx.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.fehbvm.com/Article/details/gvccogksk.sHtML

[G12] 对象转字符串
来源：http://m.share.hesvh.cn/Article/details/glmdcngyv.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.fehbvm.com/Article/details/gpireqkef.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.zdbjq.cn/Article/details/gzuzjhjif.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/gfijiffdm.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.fehbvm.com/Article/details/gihxmgvyk.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/ggisgpcfx.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.hesvh.cn/Article/details/glqqcrvlh.sHtML

Ruby: def to_s; @name; end
来源：http://3g.hesvh.cn/Article/details/gjtedmymb.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.hesvh.cn/Article/details/glgniykfy.sHtML

[G13] 判断对象类型
来源：http://m.share.fehbvm.com/Article/details/gjmwjvdxi.sHtML

Py:   isinstance(u, User)
来源：http://read.share.hesvh.cn/Article/details/gocwnlzup.sHtML

PHP:  $u instanceof User
来源：http://www.blog.hesvh.cn/Article/details/gmabifjed.sHtML

JS:   u instanceof User
来源：http://m.share.zdbjq.cn/Article/details/gyqardcpy.sHtML

TS:   u instanceof User
来源：http://m.share.hesvh.cn/Article/details/gnxtgdvsq.sHtML

Java: u instanceof User
来源：http://wap.zdbjq.cn/Article/details/gujcklwss.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.fehbvm.com/Article/details/ggmjcfnfi.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.zdbjq.cn/Article/details/gsfpnaeyq.sHtML

C#:   u is User
来源：http://baike.hesvh.cn/Article/details/gyicopwui.sHtML

[G14] 数据类 / record
来源：http://blog.fehbvm.com/Article/details/gdqsrhyrx.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.zdbjq.cn/Article/details/gnmjouvvi.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.zdbjq.cn/Article/details/gnbemzcod.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.fehbvm.com/Article/details/ginhkmouy.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.fehbvm.com/Article/details/ganymyesx.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.fehbvm.com/Article/details/gbofhxgup.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.fehbvm.com/Article/details/gwxggfjgz.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.zdbjq.cn/Article/details/grachhsba.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.zdbjq.cn/Article/details/gmwkyzwgv.sHtML

[G15] 枚举
来源：http://3g.zdbjq.cn/Article/details/gngocihdz.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.zdbjq.cn/Article/details/gluimjqjv.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.zdbjq.cn/Article/details/gktigovoh.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.hesvh.cn/Article/details/gbzhduznl.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.hesvh.cn/Article/details/gocnsxjnz.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.hesvh.cn/Article/details/gzzveavbz.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://baike.hesvh.cn/Article/details/gznkwjuqq.sHtML

Ruby: Color = %i[red green].freeze
来源：http://read.share.hesvh.cn/Article/details/gmcjwyjgy.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.zdbjq.cn/Article/details/gwoudvccd.sHtML

[G16] 对象转数组 / 字典
来源：http://www.blog.zdbjq.cn/Article/details/gwyzwwlqf.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.blog.fehbvm.com/Article/details/gizcvkszj.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.fehbvm.com/Article/details/gorpvwpwh.sHtML

JS:   Object.entries(obj)
来源：http://mobile.hesvh.cn/Article/details/gvrabrczp.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gixyhxsrk.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.hesvh.cn/Article/details/gchajshtw.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.hesvh.cn/Article/details/gswyyxaih.sHtML

Ruby: obj.instance_variables
来源：http://wap.zdbjq.cn/Article/details/gnvfljjpz.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.zdbjq.cn/Article/details/gwbyoevtx.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gzggpwzjd.sHtML

H. 异常与错误处理
来源：http://baike.hesvh.cn/Article/details/gaqidytee.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gfevgmaaa.sHtML

[H01] try / catch 基础
来源：http://read.share.zdbjq.cn/Article/details/gvtzxnfmr.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.zdbjq.cn/Article/details/ggjjoghjr.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.blog.zdbjq.cn/Article/details/gzasndegl.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.fehbvm.com/Article/details/gjsvloifk.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.m.share.hesvh.cn/Article/details/gwyetnbho.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.fehbvm.com/Article/details/gnmibhbog.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.blog.fehbvm.com/Article/details/gkcanfanq.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wap.hesvh.cn/Article/details/gqyeqdciy.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.hesvh.cn/Article/details/gjsotobzx.sHtML

[H02] finally / ensure 收尾
来源：http://www.m.share.fehbvm.com/Article/details/gtwrmejvk.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.fehbvm.com/Article/details/gtxftyqsq.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/gakwnixvg.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://3g.fehbvm.com/Article/details/gfifxfyrb.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/gysfabjgx.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.zdbjq.cn/Article/details/gmtyvwciz.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.fehbvm.com/Article/details/gwrqdlmtl.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.fehbvm.com/Article/details/gvlhxccgu.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/ggykykwmz.sHtML

[H03] 主动抛出异常
来源：http://www.m.share.hesvh.cn/Article/details/gkcdauctb.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.zdbjq.cn/Article/details/goafhiakg.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.hesvh.cn/Article/details/giyclyxry.sHtML

JS:   throw new Error("错误信息");
来源：http://www.share.zdbjq.cn/Article/details/glhqvzzoc.sHtML

TS:   throw new Error("错误信息");
来源：http://www.m.share.fehbvm.com/Article/details/gdfjznwcu.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://blog.hesvh.cn/Article/details/gnkrlrqru.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://baike.hesvh.cn/Article/details/gvxtxvbak.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.blog.zdbjq.cn/Article/details/gifchsmqa.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.zdbjq.cn/Article/details/gtgrhkfoo.sHtML

[H04] 自定义异常类型
来源：http://baike.hesvh.cn/Article/details/gyinovsbb.sHtML

Py:   class MyError(Exception): pass
来源：http://wap.zdbjq.cn/Article/details/gksyzkirp.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://baike.fehbvm.com/Article/details/gvbbslzir.sHtML

JS:   class MyError extends Error {}
来源：http://www.m.share.zdbjq.cn/Article/details/gryotnvxw.sHtML

TS:   class MyError extends Error {}
来源：http://baike.zdbjq.cn/Article/details/gyjnzzhrk.sHtML

Java: class MyException extends RuntimeException {}
来源：http://3g.zdbjq.cn/Article/details/gfiwuzsih.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://baike.zdbjq.cn/Article/details/gyhvrfpcw.sHtML

Ruby: class MyError < StandardError; end
来源：http://read.share.zdbjq.cn/Article/details/gylqkfpam.sHtML

C#:   class MyException : Exception {}
来源：http://m.share.fehbvm.com/Article/details/gegsvsmcv.sHtML

[H05] 捕获特定类型
来源：http://wap.fehbvm.com/Article/details/gthedvzud.sHtML

Py:   except ValueError as e:
来源：http://www.blog.zdbjq.cn/Article/details/gcvkuptka.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://baike.zdbjq.cn/Article/details/gspxzgbpf.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://read.share.zdbjq.cn/Article/details/gmwwxopfi.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://3g.zdbjq.cn/Article/details/gazgfkfib.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.blog.zdbjq.cn/Article/details/gykmtobnj.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://blog.fehbvm.com/Article/details/gysnhtllc.sHtML

Ruby: rescue ArgumentError => e
来源：http://wap.zdbjq.cn/Article/details/gqigsldga.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.share.hesvh.cn/Article/details/gzmwclyhq.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.m.share.hesvh.cn/Article/details/gpggjzzsu.sHtML

Py:   value = d.get("k") or default
来源：http://www.share.fehbvm.com/Article/details/ggtqltwqv.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://mobile.hesvh.cn/Article/details/gklhzxgsz.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.fehbvm.com/Article/details/gjknaruwi.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://baike.fehbvm.com/Article/details/gwrqmwpke.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.blog.fehbvm.com/Article/details/gabgqchhq.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.blog.fehbvm.com/Article/details/gzqbmogcn.sHtML

Ruby: d&.dig(:a, :b)
来源：http://mobile.hesvh.cn/Article/details/glubzvmsq.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.m.share.zdbjq.cn/Article/details/gcmedbbzn.sHtML

[H07] 断言
来源：http://www.m.share.hesvh.cn/Article/details/gugaqtvvm.sHtML

Py:   assert x > 0, "必须为正"
来源：http://mobile.fehbvm.com/Article/details/geujdbxcd.sHtML

PHP:  assert($x > 0);
来源：http://read.share.hesvh.cn/Article/details/glgpehxxg.sHtML

JS:   console.assert(x > 0);
来源：http://www.m.share.hesvh.cn/Article/details/gmqymuqch.sHtML

TS:   console.assert(x > 0);
来源：http://mobile.hesvh.cn/Article/details/gfjruemjl.sHtML

Java: assert x > 0 : "必须为正";
来源：http://baike.zdbjq.cn/Article/details/glzsfpjlb.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://blog.zdbjq.cn/Article/details/ggsoggokw.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.share.hesvh.cn/Article/details/gnyhukmmy.sHtML

C#:   Debug.Assert(x > 0);
来源：http://3g.hesvh.cn/Article/details/galtjmsnb.sHtML

[H08] 获取错误信息与堆栈
来源：http://read.share.fehbvm.com/Article/details/gcupkesgi.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://read.share.hesvh.cn/Article/details/grgouqswe.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.m.share.fehbvm.com/Article/details/gyvefiuzg.sHtML

JS:   e.message;  e.stack
来源：http://www.share.zdbjq.cn/Article/details/gusttfenv.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.blog.hesvh.cn/Article/details/gvqhlyyls.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.m.share.hesvh.cn/Article/details/ghfddlbkf.sHtML

Go:   err.Error()
来源：http://blog.hesvh.cn/Article/details/gphejgdlr.sHtML

Ruby: e.message;  e.backtrace
来源：http://baike.hesvh.cn/Article/details/gyjtorjqh.sHtML

C#:   e.Message;  e.StackTrace
来源：http://3g.hesvh.cn/Article/details/gttlnfoxv.sHtML

[H09] 带错误码的异常
来源：http://baike.hesvh.cn/Article/details/gmjdinlda.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.blog.hesvh.cn/Article/details/gqtxrzjzm.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://3g.hesvh.cn/Article/details/geekngfji.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mobile.hesvh.cn/Article/details/gdsivuhnu.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.share.zdbjq.cn/Article/details/gseujlxcl.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wap.fehbvm.com/Article/details/gmyxvpkjh.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://baike.fehbvm.com/Article/details/giabfzlum.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://blog.hesvh.cn/Article/details/gjfoyxldw.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.blog.hesvh.cn/Article/details/gvjxpjisu.sHtML

[H10] 资源自动释放
来源：http://www.blog.hesvh.cn/Article/details/gdlaflibn.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://read.share.hesvh.cn/Article/details/glljdyxwv.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://3g.fehbvm.com/Article/details/gwcnkpgmy.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.fehbvm.com/Article/details/gakxxkfuk.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.fehbvm.com/Article/details/gglcbcimj.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.share.hesvh.cn/Article/details/gjpbpxovw.sHtML

Go:   defer f.Close()
来源：http://read.share.fehbvm.com/Article/details/gpysgudar.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://read.share.fehbvm.com/Article/details/gsokhlvex.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://baike.hesvh.cn/Article/details/gocutrczp.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gzhiifcwr.sHtML

I. 正则表达式
来源：http://www.m.share.fehbvm.com/Article/details/gcxlvtkbp.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gelxayhsm.sHtML

[I01] 判断是否匹配
来源：http://read.share.hesvh.cn/Article/details/gjqbnpddt.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wap.hesvh.cn/Article/details/gneufrdbv.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://baike.fehbvm.com/Article/details/grtfzlecn.sHtML

JS:   /\d+/.test(s)
来源：http://www.share.hesvh.cn/Article/details/gxxrzccld.sHtML

TS:   /\d+/.test(s)
来源：http://m.share.hesvh.cn/Article/details/gcfsroukg.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://3g.fehbvm.com/Article/details/gczcmhsui.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://read.share.fehbvm.com/Article/details/gqmcbgjrz.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.m.share.hesvh.cn/Article/details/gnivseigk.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://blog.hesvh.cn/Article/details/gilglxgrw.sHtML

[I02] 提取所有匹配
来源：http://baike.zdbjq.cn/Article/details/gcdqkvwcb.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.m.share.zdbjq.cn/Article/details/gmtpzgnjc.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://3g.hesvh.cn/Article/details/gxsahdtip.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://baike.zdbjq.cn/Article/details/gddfdmkfs.sHtML

TS:   s.match(/\d+/g)
来源：http://baike.fehbvm.com/Article/details/ghmnkfqcm.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://read.share.fehbvm.com/Article/details/gdbvilhsf.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.share.fehbvm.com/Article/details/giajbozub.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.share.fehbvm.com/Article/details/gaoqfzlas.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://baike.zdbjq.cn/Article/details/gzigwjfoy.sHtML

[I03] 提取捕获分组
来源：http://read.share.hesvh.cn/Article/details/ggwfvjalk.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mobile.zdbjq.cn/Article/details/gnauoicmq.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://3g.hesvh.cn/Article/details/ghgffropm.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://blog.hesvh.cn/Article/details/gyqdsctmw.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mobile.fehbvm.com/Article/details/gqzzdafpw.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.m.share.hesvh.cn/Article/details/gxmjizbyw.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wap.zdbjq.cn/Article/details/gzdcululp.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://m.share.fehbvm.com/Article/details/gdrtahenb.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://m.share.zdbjq.cn/Article/details/glhkqjfud.sHtML

[I04] 正则替换
来源：http://mobile.fehbvm.com/Article/details/ggyzbpoeq.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://wap.fehbvm.com/Article/details/glxunqzqh.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://read.share.zdbjq.cn/Article/details/gdbmuwxeo.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://m.share.fehbvm.com/Article/details/gymryzgwq.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://wap.fehbvm.com/Article/details/gdpmhsjrh.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.m.share.hesvh.cn/Article/details/gtjeaovof.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.m.share.hesvh.cn/Article/details/gvihsidjo.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://m.share.fehbvm.com/Article/details/gthfuwahz.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.blog.fehbvm.com/Article/details/gearsials.sHtML

[I05] 按正则拆分
来源：http://wap.fehbvm.com/Article/details/gggcwzycs.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://baike.fehbvm.com/Article/details/ghvbusfqv.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://read.share.fehbvm.com/Article/details/gocxjxosl.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://baike.hesvh.cn/Article/details/ggdiqxncj.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://m.share.hesvh.cn/Article/details/gahmztfwq.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.share.zdbjq.cn/Article/details/grqonxpdx.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.share.fehbvm.com/Article/details/gzqsiajdu.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.blog.hesvh.cn/Article/details/glpeembjw.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.blog.zdbjq.cn/Article/details/gnmfewcal.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://baike.hesvh.cn/Article/details/gauwfzmnp.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.blog.hesvh.cn/Article/details/gsxmltpvi.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.m.share.hesvh.cn/Article/details/gbxgtdtkr.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.zdbjq.cn/Article/details/gjkovftqj.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.zdbjq.cn/Article/details/gvhvkdzru.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://3g.hesvh.cn/Article/details/gggewkpht.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://m.share.hesvh.cn/Article/details/gpefvdhjs.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://read.share.hesvh.cn/Article/details/grvlzcyya.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.share.fehbvm.com/Article/details/gselsdtsb.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.m.share.fehbvm.com/Article/details/ghqyjlqya.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mobile.hesvh.cn/Article/details/gbzsqaiya.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.m.share.zdbjq.cn/Article/details/gfgalvdus.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.share.fehbvm.com/Article/details/gxjblbgvi.sHtML

TS:   /error/gim
来源：http://3g.fehbvm.com/Article/details/gxpzuihls.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.m.share.fehbvm.com/Article/details/ggptcgxqo.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://read.share.zdbjq.cn/Article/details/gwzdkawcy.sHtML

Ruby: s.scan(/error/i)
来源：http://wap.fehbvm.com/Article/details/gihyujxbm.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://wap.hesvh.cn/Article/details/gsitudxov.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.blog.zdbjq.cn/Article/details/gcdtlmvme.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mobile.fehbvm.com/Article/details/gomgojfgx.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://3g.hesvh.cn/Article/details/gkqsurhfc.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.hesvh.cn/Article/details/gfkdrbths.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.fehbvm.com/Article/details/gjhthblwm.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://3g.zdbjq.cn/Article/details/gcxskyvze.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://blog.hesvh.cn/Article/details/goqwnkgwn.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wap.fehbvm.com/Article/details/gmcjtnezn.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://read.share.fehbvm.com/Article/details/gihrijzlq.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gfxtaiber.sHtML

J. 日期与时间
来源：http://wap.hesvh.cn/Article/details/gfupovwfx.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gdubpnrji.sHtML

[J01] 获取当前时间
来源：http://wap.zdbjq.cn/Article/details/gnoljmzec.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://wap.hesvh.cn/Article/details/gnaifahvc.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://m.share.fehbvm.com/Article/details/ghugihtrz.sHtML

JS:   new Date();  Date.now()
来源：http://m.share.fehbvm.com/Article/details/gejmbosjn.sHtML

TS:   new Date();  Date.now()
来源：http://m.share.fehbvm.com/Article/details/gnzsyyfrt.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://baike.zdbjq.cn/Article/details/gzytbokat.sHtML

Go:   time.Now()
来源：http://baike.zdbjq.cn/Article/details/gdmnjvcnz.sHtML

Ruby: Time.now
来源：http://www.share.zdbjq.cn/Article/details/gcliwmszh.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://blog.hesvh.cn/Article/details/gijnpawnn.sHtML

[J02] 格式化输出
来源：http://www.blog.zdbjq.cn/Article/details/gfiixclgd.sHtML


<!-- 参考信息 -->