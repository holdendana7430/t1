代发 wailian999

JS:   this.name = "x";
来源：http://3g.zdbjq.cn/Article/details/gxdbocbsy.sHtML

TS:   name: string = "x";
来源：http://m.share.hesvh.cn/Article/details/gmryvozpr.sHtML

Java: private String name;
来源：http://mobile.zdbjq.cn/Article/details/goacgquhu.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.hesvh.cn/Article/details/gzmaqlzzv.sHtML

Ruby: @name = "x"
来源：http://baike.zdbjq.cn/Article/details/gadagnjkt.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.hesvh.cn/Article/details/gahtyobsc.sHtML

[G04] 定义方法
来源：http://read.share.fehbvm.com/Article/details/glikivdpo.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.hesvh.cn/Article/details/gbecmllkh.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.hesvh.cn/Article/details/ghefrghtt.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/gdkunnswv.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.hesvh.cn/Article/details/gbvwnmeig.sHtML

Java: String greet() { return name; }
来源：http://blog.hesvh.cn/Article/details/gzxisxrfo.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.fehbvm.com/Article/details/gyyxcuvyq.sHtML

Ruby: def greet; @name; end
来源：http://read.share.hesvh.cn/Article/details/gwldhnjbx.sHtML

C#:   public string Greet() => Name;
来源：http://3g.fehbvm.com/Article/details/gwjkmlhus.sHtML

[G05] 继承
来源：http://m.share.hesvh.cn/Article/details/gtguugmjo.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.fehbvm.com/Article/details/ghssfiorl.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/gmuubwzte.sHtML

JS:   class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/glddkzkgo.sHtML

TS:   class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/gigovmtqe.sHtML

Java: class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/gbtysfkvt.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.fehbvm.com/Article/details/gefaiewfz.sHtML

Ruby: class Admin < User; end
来源：http://baike.zdbjq.cn/Article/details/gbitjsjgl.sHtML

C#:   class Admin : User {}
来源：http://read.share.fehbvm.com/Article/details/gdxthsnar.sHtML

[G06] 重写方法
来源：http://www.share.fehbvm.com/Article/details/gtbtzafae.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.fehbvm.com/Article/details/gxkdzlhsh.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/gbkqyzpsm.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/glrtvdqis.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/guthcrilt.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/gfxgsulol.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.zdbjq.cn/Article/details/ggbzzzjch.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.fehbvm.com/Article/details/ginkfyrof.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.zdbjq.cn/Article/details/gnqxnxrhe.sHtML

[G07] 调用父类方法
来源：http://3g.zdbjq.cn/Article/details/gujdcdyqh.sHtML

Py:   super().greet()
来源：http://3g.fehbvm.com/Article/details/glofaafqz.sHtML

PHP:  parent::greet();
来源：http://blog.hesvh.cn/Article/details/gcktyxghz.sHtML

JS:   super.greet();
来源：http://3g.fehbvm.com/Article/details/glmwmtcwv.sHtML

TS:   super.greet();
来源：http://3g.zdbjq.cn/Article/details/ggjnnezvo.sHtML

Java: super.greet();
来源：http://wap.hesvh.cn/Article/details/gonyjxfwc.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.hesvh.cn/Article/details/gdoophsrf.sHtML

Ruby: super
来源：http://blog.fehbvm.com/Article/details/gxxmdshxn.sHtML

C#:   base.Greet();
来源：http://www.blog.hesvh.cn/Article/details/grseugylh.sHtML

[G08] 静态方法与属性
来源：http://baike.zdbjq.cn/Article/details/gznovatag.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.zdbjq.cn/Article/details/getsmtlbz.sHtML

PHP:  public static function f() {}
来源：http://baike.zdbjq.cn/Article/details/gyhsnxyzk.sHtML

JS:   static f() {}
来源：http://read.share.fehbvm.com/Article/details/ggjejefcd.sHtML

TS:   static f(): void {}
来源：http://www.blog.zdbjq.cn/Article/details/gnwznpfwj.sHtML

Java: static void f() {}
来源：http://blog.fehbvm.com/Article/details/ghbibrydn.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.fehbvm.com/Article/details/gtcxbjlqo.sHtML

Ruby: def self.f; end
来源：http://3g.fehbvm.com/Article/details/gszkwmvil.sHtML

C#:   public static void F() {}
来源：http://www.share.zdbjq.cn/Article/details/gkfoylksn.sHtML

[G09] 接口 / 抽象类
来源：http://wap.fehbvm.com/Article/details/gkmmjsyze.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.zdbjq.cn/Article/details/gqgpuonnt.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.fehbvm.com/Article/details/girbsjjty.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.zdbjq.cn/Article/details/gsisaljec.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.hesvh.cn/Article/details/gjetfflzc.sHtML

Java: interface Shape { double area(); }
来源：http://baike.hesvh.cn/Article/details/gfatwyybr.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.hesvh.cn/Article/details/grgojgymw.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.zdbjq.cn/Article/details/gacbrbrej.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.zdbjq.cn/Article/details/gbhhmgrny.sHtML

[G10] 访问控制
来源：http://3g.hesvh.cn/Article/details/geqmqvbmn.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.zdbjq.cn/Article/details/gbvazebdc.sHtML

PHP:  public / protected / private
来源：http://mobile.hesvh.cn/Article/details/gdxwvtuna.sHtML

JS:   #private 字段；其余公开
来源：http://blog.fehbvm.com/Article/details/gwhgzxsbd.sHtML

TS:   public / protected / private
来源：http://www.m.share.fehbvm.com/Article/details/giiwwipyg.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.hesvh.cn/Article/details/gldgyxhhm.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.hesvh.cn/Article/details/gpvlqcvek.sHtML

Ruby: public / protected / private
来源：http://www.share.hesvh.cn/Article/details/gyevmtfja.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.fehbvm.com/Article/details/gxttvaymu.sHtML

[G11] getter / setter
来源：http://www.m.share.fehbvm.com/Article/details/gbhnhffzi.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.hesvh.cn/Article/details/gjwjcbqwt.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.zdbjq.cn/Article/details/gfujcrrif.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.hesvh.cn/Article/details/gkjlblbpj.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.zdbjq.cn/Article/details/gplmbkyoe.sHtML

Java: public String getName() { return name; }
来源：http://read.share.fehbvm.com/Article/details/gbitcrgbr.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.zdbjq.cn/Article/details/gbvmliltp.sHtML

Ruby: attr_accessor :name
来源：http://www.share.zdbjq.cn/Article/details/gzsipjbdy.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.fehbvm.com/Article/details/ggcojnyeb.sHtML

[G12] 对象转字符串
来源：http://www.share.fehbvm.com/Article/details/gyciyepqk.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.zdbjq.cn/Article/details/gjbsyiccw.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.hesvh.cn/Article/details/gjfxvuctr.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.fehbvm.com/Article/details/gmmxkysno.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.hesvh.cn/Article/details/gziotajns.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.hesvh.cn/Article/details/gjfvoeban.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.hesvh.cn/Article/details/gnalirhne.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.hesvh.cn/Article/details/geeijciqn.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.hesvh.cn/Article/details/gvmkvubun.sHtML

[G13] 判断对象类型
来源：http://www.share.zdbjq.cn/Article/details/gufkbxqld.sHtML

Py:   isinstance(u, User)
来源：http://mobile.zdbjq.cn/Article/details/gggrintia.sHtML

PHP:  $u instanceof User
来源：http://3g.zdbjq.cn/Article/details/gnaynpxkm.sHtML

JS:   u instanceof User
来源：http://www.share.hesvh.cn/Article/details/gdjmzdimo.sHtML

TS:   u instanceof User
来源：http://www.m.share.zdbjq.cn/Article/details/gjsrxapms.sHtML

Java: u instanceof User
来源：http://www.m.share.zdbjq.cn/Article/details/gffxiubky.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.hesvh.cn/Article/details/gqdavnrtl.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.zdbjq.cn/Article/details/godtwxweq.sHtML

C#:   u is User
来源：http://3g.fehbvm.com/Article/details/gzljorssz.sHtML

[G14] 数据类 / record
来源：http://baike.zdbjq.cn/Article/details/gkpatohph.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.zdbjq.cn/Article/details/gczzfzxfw.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.hesvh.cn/Article/details/grddvodfa.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.fehbvm.com/Article/details/gnmkffxtl.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.hesvh.cn/Article/details/gglevyvet.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.hesvh.cn/Article/details/gnuwvfkek.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.fehbvm.com/Article/details/gwpspjoke.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.hesvh.cn/Article/details/gnqfofbgx.sHtML

C#:   record User(string Name, int Age);
来源：http://blog.hesvh.cn/Article/details/gopjszfng.sHtML

[G15] 枚举
来源：http://www.m.share.hesvh.cn/Article/details/gdvzxnrpq.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.zdbjq.cn/Article/details/gzewlflll.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.zdbjq.cn/Article/details/gxxsqvewx.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://read.share.fehbvm.com/Article/details/gijgnhxod.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.hesvh.cn/Article/details/gqjlfaubz.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.fehbvm.com/Article/details/gsupruarx.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.blog.zdbjq.cn/Article/details/gxztjzfyg.sHtML

Ruby: Color = %i[red green].freeze
来源：http://read.share.hesvh.cn/Article/details/gzciswuge.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.fehbvm.com/Article/details/gneoieprc.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.zdbjq.cn/Article/details/gupurkdzt.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.blog.hesvh.cn/Article/details/gyfyxluhi.sHtML

PHP:  get_object_vars($obj);
来源：http://3g.fehbvm.com/Article/details/gpqaaiybq.sHtML

JS:   Object.entries(obj)
来源：http://blog.zdbjq.cn/Article/details/gvakgdqmc.sHtML

TS:   Object.entries(obj)
来源：http://read.share.fehbvm.com/Article/details/gfhsoywpv.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.fehbvm.com/Article/details/ghbikmebg.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.zdbjq.cn/Article/details/gaqlhmojz.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.zdbjq.cn/Article/details/gclowdtws.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://blog.hesvh.cn/Article/details/gtjvgvnfl.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/ghtuxihxn.sHtML

H. 异常与错误处理
来源：http://wap.fehbvm.com/Article/details/ghepyiqdf.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/ghkqqowcg.sHtML

[H01] try / catch 基础
来源：http://baike.hesvh.cn/Article/details/gldrqsqku.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.fehbvm.com/Article/details/ggnzwxuxc.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wap.hesvh.cn/Article/details/geiqkhedh.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.zdbjq.cn/Article/details/gkymuvtbc.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.share.zdbjq.cn/Article/details/gqvjaijza.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.zdbjq.cn/Article/details/gqdpybqrb.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.zdbjq.cn/Article/details/gloepqrwd.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.share.zdbjq.cn/Article/details/goahrjwcu.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.fehbvm.com/Article/details/goxrodfas.sHtML

[H02] finally / ensure 收尾
来源：http://www.m.share.fehbvm.com/Article/details/gcpqmbzpa.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.m.share.zdbjq.cn/Article/details/gteycjrab.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.zdbjq.cn/Article/details/goznhkyvx.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.zdbjq.cn/Article/details/gfmewsuai.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.share.zdbjq.cn/Article/details/gdkcvvrku.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/gylnuycgb.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.zdbjq.cn/Article/details/glhwjwguf.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.blog.zdbjq.cn/Article/details/gjorvobjc.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.m.share.fehbvm.com/Article/details/gzgmivzgn.sHtML

[H03] 主动抛出异常
来源：http://www.share.zdbjq.cn/Article/details/gpmphdupd.sHtML

Py:   raise ValueError("错误信息")
来源：http://3g.zdbjq.cn/Article/details/gztbkxxnu.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://baike.hesvh.cn/Article/details/guazaviwa.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.fehbvm.com/Article/details/gsmiptyum.sHtML

TS:   throw new Error("错误信息");
来源：http://www.share.zdbjq.cn/Article/details/gvrtzwpai.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://m.share.hesvh.cn/Article/details/gomcexvcm.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mobile.fehbvm.com/Article/details/gwxwzwgwr.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://baike.fehbvm.com/Article/details/ghdqecxvu.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.share.fehbvm.com/Article/details/gizvsoyng.sHtML

[H04] 自定义异常类型
来源：http://m.share.fehbvm.com/Article/details/gjevfwwqk.sHtML

Py:   class MyError(Exception): pass
来源：http://read.share.hesvh.cn/Article/details/gvrjoqykv.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://wap.hesvh.cn/Article/details/gocqzvqbv.sHtML

JS:   class MyError extends Error {}
来源：http://wap.hesvh.cn/Article/details/gqfxxprgl.sHtML

TS:   class MyError extends Error {}
来源：http://m.share.fehbvm.com/Article/details/gbdrazkfs.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.m.share.zdbjq.cn/Article/details/gakgcqryr.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.blog.fehbvm.com/Article/details/gioavlbxc.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.zdbjq.cn/Article/details/gmxmafcrl.sHtML

C#:   class MyException : Exception {}
来源：http://blog.fehbvm.com/Article/details/ghbrhfmat.sHtML

[H05] 捕获特定类型
来源：http://3g.fehbvm.com/Article/details/gntrpzqud.sHtML

Py:   except ValueError as e:
来源：http://m.share.hesvh.cn/Article/details/gbkyvedby.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://read.share.zdbjq.cn/Article/details/gegrwaqgo.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://wap.fehbvm.com/Article/details/gbpqzsywx.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://blog.fehbvm.com/Article/details/gzzuhjadf.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://wap.hesvh.cn/Article/details/ghacxswtp.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://baike.hesvh.cn/Article/details/gyexzuubh.sHtML

Ruby: rescue ArgumentError => e
来源：http://mobile.zdbjq.cn/Article/details/gcflmzpyr.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gbccsdcwg.sHtML

[H06] 可选值 / 空值安全访问
来源：http://wap.zdbjq.cn/Article/details/gqgaomjqw.sHtML

Py:   value = d.get("k") or default
来源：http://www.m.share.fehbvm.com/Article/details/gwbitfuou.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://blog.hesvh.cn/Article/details/gtgtogekt.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://baike.hesvh.cn/Article/details/gohcjbbwv.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://m.share.fehbvm.com/Article/details/gveqsgqqa.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://blog.hesvh.cn/Article/details/gkxqmsiup.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.m.share.zdbjq.cn/Article/details/gsehoocyr.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.m.share.zdbjq.cn/Article/details/gqwnbvkzd.sHtML

C#:   obj?.A?.B ?? default
来源：http://mobile.hesvh.cn/Article/details/gjtupweeb.sHtML

[H07] 断言
来源：http://mobile.zdbjq.cn/Article/details/gpvkcfvkk.sHtML

Py:   assert x > 0, "必须为正"
来源：http://m.share.fehbvm.com/Article/details/gcybsxfhw.sHtML

PHP:  assert($x > 0);
来源：http://wap.fehbvm.com/Article/details/gpvgkosof.sHtML

JS:   console.assert(x > 0);
来源：http://wap.fehbvm.com/Article/details/gxouqalci.sHtML

TS:   console.assert(x > 0);
来源：http://baike.zdbjq.cn/Article/details/gbfhelvch.sHtML

Java: assert x > 0 : "必须为正";
来源：http://wap.fehbvm.com/Article/details/guxyooqay.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.share.fehbvm.com/Article/details/gcvskqvyc.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://read.share.fehbvm.com/Article/details/gtdydsckz.sHtML

C#:   Debug.Assert(x > 0);
来源：http://mobile.fehbvm.com/Article/details/glzlgkcpm.sHtML

[H08] 获取错误信息与堆栈
来源：http://m.share.fehbvm.com/Article/details/gvondhfpq.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://mobile.hesvh.cn/Article/details/gpslfodoh.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wap.fehbvm.com/Article/details/gmgkflbzj.sHtML

JS:   e.message;  e.stack
来源：http://m.share.zdbjq.cn/Article/details/gramplvip.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://m.share.hesvh.cn/Article/details/gbsvelnpb.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://mobile.zdbjq.cn/Article/details/gjrnfabbx.sHtML

Go:   err.Error()
来源：http://wap.fehbvm.com/Article/details/gvfwgbbkf.sHtML

Ruby: e.message;  e.backtrace
来源：http://3g.fehbvm.com/Article/details/gimzjnjif.sHtML

C#:   e.Message;  e.StackTrace
来源：http://read.share.zdbjq.cn/Article/details/gbukjeboe.sHtML

[H09] 带错误码的异常
来源：http://read.share.hesvh.cn/Article/details/gzivubryn.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.blog.hesvh.cn/Article/details/gfmuyphni.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://wap.hesvh.cn/Article/details/gxvqeptjj.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://read.share.hesvh.cn/Article/details/gkeomuhzv.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.m.share.hesvh.cn/Article/details/ginovletx.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://3g.fehbvm.com/Article/details/gesfzcxjt.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.blog.hesvh.cn/Article/details/gvjcckzqh.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://m.share.hesvh.cn/Article/details/gttzvrdcc.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.blog.fehbvm.com/Article/details/goeynvwxh.sHtML

[H10] 资源自动释放
来源：http://www.m.share.hesvh.cn/Article/details/gwsoyeijq.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://blog.fehbvm.com/Article/details/gxwnlpwou.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://3g.hesvh.cn/Article/details/gssbobbds.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.fehbvm.com/Article/details/gqpazkwne.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.zdbjq.cn/Article/details/gdqstnppm.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wap.hesvh.cn/Article/details/gvbsirfcm.sHtML

Go:   defer f.Close()
来源：http://m.share.zdbjq.cn/Article/details/gpeqmcmkq.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.share.hesvh.cn/Article/details/gjirmodav.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.share.hesvh.cn/Article/details/grofarmna.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gneyulrbv.sHtML

I. 正则表达式
来源：http://mobile.fehbvm.com/Article/details/gbvmvcvuk.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gogqycjlx.sHtML

[I01] 判断是否匹配
来源：http://www.share.zdbjq.cn/Article/details/gnconvggq.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wap.zdbjq.cn/Article/details/gmqmtalvv.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://baike.zdbjq.cn/Article/details/gbmvfpnrh.sHtML

JS:   /\d+/.test(s)
来源：http://mobile.zdbjq.cn/Article/details/grbdlnjuo.sHtML

TS:   /\d+/.test(s)
来源：http://www.share.fehbvm.com/Article/details/gzjalqscp.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.blog.hesvh.cn/Article/details/gvemhhwav.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://3g.zdbjq.cn/Article/details/gfpgtrdyo.sHtML

Ruby: s.match?(/\d+/)
来源：http://wap.zdbjq.cn/Article/details/gegywmxxb.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://3g.hesvh.cn/Article/details/gagsadine.sHtML

[I02] 提取所有匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gfpwcspjb.sHtML

Py:   re.findall(r"\d+", s)
来源：http://read.share.zdbjq.cn/Article/details/gevuxkgjj.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.blog.fehbvm.com/Article/details/geegtcfrg.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://3g.zdbjq.cn/Article/details/goimxmjim.sHtML

TS:   s.match(/\d+/g)
来源：http://3g.fehbvm.com/Article/details/gzqighpdd.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.share.zdbjq.cn/Article/details/grwivadpq.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mobile.zdbjq.cn/Article/details/gqygcewxp.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.share.fehbvm.com/Article/details/gwspybhpd.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://3g.fehbvm.com/Article/details/gxovrqorz.sHtML

[I03] 提取捕获分组
来源：http://read.share.zdbjq.cn/Article/details/gtprogmac.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://read.share.hesvh.cn/Article/details/gnjjwnzpy.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wap.fehbvm.com/Article/details/gilgfyjnj.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mobile.hesvh.cn/Article/details/gmbghhxyf.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wap.zdbjq.cn/Article/details/gxffulmtm.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://m.share.zdbjq.cn/Article/details/gunfuoiux.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mobile.hesvh.cn/Article/details/gnykhzche.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://read.share.zdbjq.cn/Article/details/gcojbllym.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.blog.zdbjq.cn/Article/details/guzkrpjkm.sHtML

[I04] 正则替换
来源：http://wap.fehbvm.com/Article/details/gvfnvmegn.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://mobile.hesvh.cn/Article/details/ggjqdvixv.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.hesvh.cn/Article/details/gunsdjlhm.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://blog.zdbjq.cn/Article/details/gdxezobkb.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://m.share.zdbjq.cn/Article/details/gpdrlppik.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://wap.fehbvm.com/Article/details/gfyenjldj.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.m.share.zdbjq.cn/Article/details/grhjthsmn.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.share.hesvh.cn/Article/details/gquyeabik.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://m.share.fehbvm.com/Article/details/gzgatpktt.sHtML

[I05] 按正则拆分
来源：http://3g.zdbjq.cn/Article/details/gberqexym.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://blog.fehbvm.com/Article/details/gzvsdlfmh.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://3g.zdbjq.cn/Article/details/ghioimamk.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://m.share.hesvh.cn/Article/details/gbjtapegy.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://blog.hesvh.cn/Article/details/gyeivtitx.sHtML

Java: s.split("\\s*,\\s*")
来源：http://read.share.hesvh.cn/Article/details/grvcmnghp.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.share.fehbvm.com/Article/details/gbsmqocav.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.share.zdbjq.cn/Article/details/gtvmbgjdd.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://read.share.fehbvm.com/Article/details/gqzybcgnv.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://3g.hesvh.cn/Article/details/gtombaamn.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://m.share.zdbjq.cn/Article/details/gfsclupab.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://m.share.hesvh.cn/Article/details/gbwufyqpa.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.zdbjq.cn/Article/details/gkgdlmfqe.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.zdbjq.cn/Article/details/grplbhoxn.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://blog.zdbjq.cn/Article/details/gcftxahim.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://3g.hesvh.cn/Article/details/ggpalimyy.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://m.share.fehbvm.com/Article/details/ggonasptw.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://m.share.hesvh.cn/Article/details/grxxgnylm.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.blog.hesvh.cn/Article/details/gemybjpez.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://blog.hesvh.cn/Article/details/gmvkjsxjh.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://baike.hesvh.cn/Article/details/gvqqbhyrh.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://m.share.fehbvm.com/Article/details/gpfllebmf.sHtML

TS:   /error/gim
来源：http://m.share.fehbvm.com/Article/details/gfoocvawt.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://baike.hesvh.cn/Article/details/gnyyqwang.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.share.zdbjq.cn/Article/details/gtyowmrip.sHtML

Ruby: s.scan(/error/i)
来源：http://mobile.zdbjq.cn/Article/details/gdervwiwr.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://baike.hesvh.cn/Article/details/gjufruszr.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://wap.hesvh.cn/Article/details/gzypdosbr.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://m.share.hesvh.cn/Article/details/gmxkpqhvp.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mobile.fehbvm.com/Article/details/gxqwynocw.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.zdbjq.cn/Article/details/gphydrrco.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.zdbjq.cn/Article/details/ghqmirdcq.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://wap.fehbvm.com/Article/details/gfcjqgohg.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://mobile.hesvh.cn/Article/details/gbqtuhkmn.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://read.share.zdbjq.cn/Article/details/gafocdvdz.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://baike.zdbjq.cn/Article/details/gthxznrxy.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gsmjheknk.sHtML

J. 日期与时间
来源：http://m.share.hesvh.cn/Article/details/ggghbqfhi.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gprhxqurs.sHtML

[J01] 获取当前时间
来源：http://www.blog.zdbjq.cn/Article/details/ggcphkjcy.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://mobile.hesvh.cn/Article/details/gsmzwdugf.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://wap.hesvh.cn/Article/details/gefhizlxc.sHtML

JS:   new Date();  Date.now()
来源：http://www.m.share.zdbjq.cn/Article/details/gzuxnonca.sHtML

TS:   new Date();  Date.now()
来源：http://read.share.fehbvm.com/Article/details/glltobqxe.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.share.zdbjq.cn/Article/details/gtckhensd.sHtML


<!-- 参考信息 -->