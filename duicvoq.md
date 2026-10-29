代发 wailian999

C#:   public User(string name) { Name = name; }
来源：http://3g.fehbvm.com/Article/details/gqfgrquio.sHtML

[G03] 实例属性
来源：http://wap.zdbjq.cn/Article/details/grwaawega.sHtML

Py:   self.name = "x"
来源：http://read.share.fehbvm.com/Article/details/gyxxifudq.sHtML

PHP:  public string $name = "x";
来源：http://read.share.hesvh.cn/Article/details/gtuhpiktt.sHtML

JS:   this.name = "x";
来源：http://3g.zdbjq.cn/Article/details/gymklgpdx.sHtML

TS:   name: string = "x";
来源：http://mobile.zdbjq.cn/Article/details/gyofzaoap.sHtML

Java: private String name;
来源：http://mobile.hesvh.cn/Article/details/gtxelqhve.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.hesvh.cn/Article/details/gjkpcmwdd.sHtML

Ruby: @name = "x"
来源：http://baike.hesvh.cn/Article/details/ghpoxvxng.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.fehbvm.com/Article/details/goegepxep.sHtML

[G04] 定义方法
来源：http://wap.fehbvm.com/Article/details/govwbushk.sHtML

Py:   def greet(self): return self.name
来源：http://blog.zdbjq.cn/Article/details/gmxsylhdz.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.zdbjq.cn/Article/details/gofsanpme.sHtML

JS:   greet() { return this.name; }
来源：http://blog.hesvh.cn/Article/details/gvaormqbo.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/guoissosx.sHtML

Java: String greet() { return name; }
来源：http://www.share.zdbjq.cn/Article/details/gqwsjmjob.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.fehbvm.com/Article/details/gglgfsilf.sHtML

Ruby: def greet; @name; end
来源：http://m.share.hesvh.cn/Article/details/gbcbvrhgc.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.fehbvm.com/Article/details/gzfdbclns.sHtML

[G05] 继承
来源：http://read.share.hesvh.cn/Article/details/goshnwmlt.sHtML

Py:   class Admin(User): pass
来源：http://mobile.fehbvm.com/Article/details/gwlvfsysk.sHtML

PHP:  class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/ggoyyrpol.sHtML

JS:   class Admin extends User {}
来源：http://www.share.hesvh.cn/Article/details/goallfzsw.sHtML

TS:   class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/gbkcbgmew.sHtML

Java: class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/gnvhpfont.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.fehbvm.com/Article/details/gopbgzoub.sHtML

Ruby: class Admin < User; end
来源：http://mobile.zdbjq.cn/Article/details/gvovqencd.sHtML

C#:   class Admin : User {}
来源：http://baike.zdbjq.cn/Article/details/gzsqynrfb.sHtML

[G06] 重写方法
来源：http://read.share.zdbjq.cn/Article/details/gxmwqbror.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.hesvh.cn/Article/details/gowtwahbk.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/gonopdnvd.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/gddssszue.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/ggucbmnwo.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/gvvhquazn.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.fehbvm.com/Article/details/glgllgrfi.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.zdbjq.cn/Article/details/gsjgcnnoh.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.zdbjq.cn/Article/details/gtnkzsftq.sHtML

[G07] 调用父类方法
来源：http://read.share.hesvh.cn/Article/details/gxnrzrrne.sHtML

Py:   super().greet()
来源：http://www.blog.hesvh.cn/Article/details/gnfksclpj.sHtML

PHP:  parent::greet();
来源：http://www.m.share.hesvh.cn/Article/details/gpeolxgcg.sHtML

JS:   super.greet();
来源：http://wap.zdbjq.cn/Article/details/genzkhaec.sHtML

TS:   super.greet();
来源：http://baike.fehbvm.com/Article/details/gdqsqmcoy.sHtML

Java: super.greet();
来源：http://www.blog.zdbjq.cn/Article/details/gfbpvieve.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.hesvh.cn/Article/details/gwevcwmui.sHtML

Ruby: super
来源：http://www.blog.hesvh.cn/Article/details/gmsenrois.sHtML

C#:   base.Greet();
来源：http://m.share.hesvh.cn/Article/details/gaycdovhi.sHtML

[G08] 静态方法与属性
来源：http://www.blog.zdbjq.cn/Article/details/gmdzafugi.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.fehbvm.com/Article/details/gywloneol.sHtML

PHP:  public static function f() {}
来源：http://mobile.fehbvm.com/Article/details/goegesrkj.sHtML

JS:   static f() {}
来源：http://m.share.hesvh.cn/Article/details/gmiuarwub.sHtML

TS:   static f(): void {}
来源：http://baike.fehbvm.com/Article/details/gycucgtny.sHtML

Java: static void f() {}
来源：http://wap.hesvh.cn/Article/details/gzjpbftqu.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.fehbvm.com/Article/details/ghmpmuhje.sHtML

Ruby: def self.f; end
来源：http://blog.hesvh.cn/Article/details/grlaozsbs.sHtML

C#:   public static void F() {}
来源：http://www.blog.fehbvm.com/Article/details/glsouwhtq.sHtML

[G09] 接口 / 抽象类
来源：http://3g.zdbjq.cn/Article/details/gxgfxthzb.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.zdbjq.cn/Article/details/ghmmywvqt.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.hesvh.cn/Article/details/gvjtpaase.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.fehbvm.com/Article/details/ggbchuvqv.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.zdbjq.cn/Article/details/gvgtaqpaj.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.zdbjq.cn/Article/details/guqvhduwe.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.fehbvm.com/Article/details/gvcioyues.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.fehbvm.com/Article/details/gvdihtysj.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.hesvh.cn/Article/details/gmnqepiqx.sHtML

[G10] 访问控制
来源：http://baike.hesvh.cn/Article/details/gokcsosxn.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.fehbvm.com/Article/details/goyokyxww.sHtML

PHP:  public / protected / private
来源：http://wap.zdbjq.cn/Article/details/guxdcrbhy.sHtML

JS:   #private 字段；其余公开
来源：http://wap.hesvh.cn/Article/details/gogrhlwws.sHtML

TS:   public / protected / private
来源：http://read.share.fehbvm.com/Article/details/gemiebuhm.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.fehbvm.com/Article/details/gmchmoibm.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.hesvh.cn/Article/details/gdmvhzuks.sHtML

Ruby: public / protected / private
来源：http://www.m.share.zdbjq.cn/Article/details/goaokzvbn.sHtML

C#:   public / protected / private / internal
来源：http://3g.zdbjq.cn/Article/details/geycdlnha.sHtML

[G11] getter / setter
来源：http://www.m.share.zdbjq.cn/Article/details/ghmwbgiex.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.fehbvm.com/Article/details/gtiayiyli.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.hesvh.cn/Article/details/gtdjobvou.sHtML

JS:   get name() { return this._name; }
来源：http://blog.fehbvm.com/Article/details/gbbfiaqss.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.fehbvm.com/Article/details/gvwqzsylj.sHtML

Java: public String getName() { return name; }
来源：http://3g.zdbjq.cn/Article/details/giypcfxly.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.zdbjq.cn/Article/details/gnrqiosoq.sHtML

Ruby: attr_accessor :name
来源：http://3g.hesvh.cn/Article/details/gvdakzidz.sHtML

C#:   public string Name { get; set; }
来源：http://wap.fehbvm.com/Article/details/gbwvseogt.sHtML

[G12] 对象转字符串
来源：http://blog.fehbvm.com/Article/details/gddvwvimq.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.hesvh.cn/Article/details/gtafyqsrj.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.zdbjq.cn/Article/details/gntvdbgxh.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/gozseqsmt.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.fehbvm.com/Article/details/guojwawme.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.zdbjq.cn/Article/details/gzmddkwmo.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.hesvh.cn/Article/details/glzsphmij.sHtML

Ruby: def to_s; @name; end
来源：http://wap.zdbjq.cn/Article/details/ghkaejriu.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.zdbjq.cn/Article/details/gguovkxkg.sHtML

[G13] 判断对象类型
来源：http://blog.zdbjq.cn/Article/details/gakukvqro.sHtML

Py:   isinstance(u, User)
来源：http://read.share.hesvh.cn/Article/details/gucynumyy.sHtML

PHP:  $u instanceof User
来源：http://www.blog.hesvh.cn/Article/details/ggwksuhty.sHtML

JS:   u instanceof User
来源：http://www.blog.fehbvm.com/Article/details/gqiemrbgc.sHtML

TS:   u instanceof User
来源：http://www.m.share.fehbvm.com/Article/details/gpnttbrfr.sHtML

Java: u instanceof User
来源：http://www.blog.fehbvm.com/Article/details/gfyhffmol.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.fehbvm.com/Article/details/gekwzgbbv.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.zdbjq.cn/Article/details/gebltnkoy.sHtML

C#:   u is User
来源：http://read.share.zdbjq.cn/Article/details/gncvobmga.sHtML

[G14] 数据类 / record
来源：http://wap.zdbjq.cn/Article/details/gimnueiat.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.fehbvm.com/Article/details/glvnwjhyq.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.fehbvm.com/Article/details/giiporaxu.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.fehbvm.com/Article/details/gdmuofdmd.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.hesvh.cn/Article/details/gmlbirhnh.sHtML

Java: record User(String name, int age) {}
来源：http://wap.zdbjq.cn/Article/details/gztydcrva.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.zdbjq.cn/Article/details/gjiutjhbs.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.zdbjq.cn/Article/details/gfgqmmiuz.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.fehbvm.com/Article/details/gvqaxttvl.sHtML

[G15] 枚举
来源：http://3g.fehbvm.com/Article/details/gkqbltpsi.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.zdbjq.cn/Article/details/gbbljcuei.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.fehbvm.com/Article/details/gesqhbdao.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.fehbvm.com/Article/details/gqdijanvm.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.fehbvm.com/Article/details/gdxfrfvsm.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.fehbvm.com/Article/details/gxsmyrgzz.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.zdbjq.cn/Article/details/gcuwbvaar.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.m.share.hesvh.cn/Article/details/gvpoujuzv.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.hesvh.cn/Article/details/giqivtpif.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.hesvh.cn/Article/details/gimdoifka.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.fehbvm.com/Article/details/goesgrrau.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.hesvh.cn/Article/details/gdzurrokc.sHtML

JS:   Object.entries(obj)
来源：http://blog.fehbvm.com/Article/details/gkweerbvx.sHtML

TS:   Object.entries(obj)
来源：http://m.share.zdbjq.cn/Article/details/gapputffn.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://m.share.hesvh.cn/Article/details/gqssywzdb.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.zdbjq.cn/Article/details/gyridjkah.sHtML

Ruby: obj.instance_variables
来源：http://3g.zdbjq.cn/Article/details/goyzmrokp.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.blog.fehbvm.com/Article/details/gxyzokmif.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/grepoxmlk.sHtML

H. 异常与错误处理
来源：http://baike.fehbvm.com/Article/details/gnbgpqntx.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gtkrnyugj.sHtML

[H01] try / catch 基础
来源：http://www.m.share.zdbjq.cn/Article/details/gwrmrytem.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.share.zdbjq.cn/Article/details/gbubhiejb.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wap.zdbjq.cn/Article/details/gwfmvcodd.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.blog.zdbjq.cn/Article/details/gmipuhloo.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.fehbvm.com/Article/details/gtaitztmw.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.blog.hesvh.cn/Article/details/grtmboecd.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.fehbvm.com/Article/details/gcopkwxhw.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.hesvh.cn/Article/details/gjcyxknii.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.m.share.hesvh.cn/Article/details/gpmvhzwkm.sHtML

[H02] finally / ensure 收尾
来源：http://baike.hesvh.cn/Article/details/gewjlvcmh.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://3g.hesvh.cn/Article/details/grgebtoip.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gghgkdpjk.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.zdbjq.cn/Article/details/gxraogwbb.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://blog.fehbvm.com/Article/details/gjbmkrdtu.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://m.share.fehbvm.com/Article/details/gvshokdne.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.fehbvm.com/Article/details/gnpyiyhjm.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.share.hesvh.cn/Article/details/ggkwicxyc.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gmonwbzuo.sHtML

[H03] 主动抛出异常
来源：http://baike.fehbvm.com/Article/details/gkvphzfie.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.share.fehbvm.com/Article/details/gdpsaqhju.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.zdbjq.cn/Article/details/gkllojvkj.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.hesvh.cn/Article/details/gxugzkuaf.sHtML

TS:   throw new Error("错误信息");
来源：http://www.blog.zdbjq.cn/Article/details/gaiwaicmq.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://blog.fehbvm.com/Article/details/gwrvyykxn.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.zdbjq.cn/Article/details/gbetlldih.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://blog.fehbvm.com/Article/details/gawswgpgj.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://mobile.hesvh.cn/Article/details/gcavqynnp.sHtML

[H04] 自定义异常类型
来源：http://blog.zdbjq.cn/Article/details/gbwvowjyg.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.hesvh.cn/Article/details/gextnpvle.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.zdbjq.cn/Article/details/gyemlwrmy.sHtML

JS:   class MyError extends Error {}
来源：http://baike.zdbjq.cn/Article/details/gfqlvpbga.sHtML

TS:   class MyError extends Error {}
来源：http://www.share.zdbjq.cn/Article/details/gvkxheqao.sHtML

Java: class MyException extends RuntimeException {}
来源：http://mobile.hesvh.cn/Article/details/gfxfqifxn.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mobile.fehbvm.com/Article/details/gwpiwbvki.sHtML

Ruby: class MyError < StandardError; end
来源：http://blog.hesvh.cn/Article/details/gszegcuiq.sHtML

C#:   class MyException : Exception {}
来源：http://wap.zdbjq.cn/Article/details/gdnuecvqq.sHtML

[H05] 捕获特定类型
来源：http://m.share.fehbvm.com/Article/details/ggitrezeo.sHtML

Py:   except ValueError as e:
来源：http://baike.zdbjq.cn/Article/details/gugpkrcqo.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.hesvh.cn/Article/details/guodpoihh.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://m.share.fehbvm.com/Article/details/gchkrorgn.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://read.share.fehbvm.com/Article/details/gfwtuyrwf.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://blog.hesvh.cn/Article/details/gqqqihnfc.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wap.fehbvm.com/Article/details/gqxfaaoab.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.share.hesvh.cn/Article/details/gerwnalqi.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://blog.fehbvm.com/Article/details/glzsxjpmz.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.fehbvm.com/Article/details/gaorwpoqv.sHtML

Py:   value = d.get("k") or default
来源：http://www.share.hesvh.cn/Article/details/gfvhhtriv.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://baike.fehbvm.com/Article/details/gsdzwbshv.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.zdbjq.cn/Article/details/gwttepkpr.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.hesvh.cn/Article/details/gbwpzmdue.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.blog.hesvh.cn/Article/details/gxudglmdd.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://m.share.zdbjq.cn/Article/details/guallkeka.sHtML

Ruby: d&.dig(:a, :b)
来源：http://blog.zdbjq.cn/Article/details/gpkgtypiu.sHtML

C#:   obj?.A?.B ?? default
来源：http://mobile.zdbjq.cn/Article/details/gqqlarjpo.sHtML

[H07] 断言
来源：http://www.blog.hesvh.cn/Article/details/gbrqtezkj.sHtML

Py:   assert x > 0, "必须为正"
来源：http://m.share.fehbvm.com/Article/details/gjwwxqcpg.sHtML

PHP:  assert($x > 0);
来源：http://read.share.fehbvm.com/Article/details/gowuvzbye.sHtML

JS:   console.assert(x > 0);
来源：http://www.blog.fehbvm.com/Article/details/gplmbyknl.sHtML

TS:   console.assert(x > 0);
来源：http://mobile.zdbjq.cn/Article/details/gcidpefjo.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.share.zdbjq.cn/Article/details/giahzlaci.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.share.fehbvm.com/Article/details/gfmneweih.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://blog.hesvh.cn/Article/details/gdpbpfasi.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.blog.hesvh.cn/Article/details/gevhfziqf.sHtML

[H08] 获取错误信息与堆栈
来源：http://baike.hesvh.cn/Article/details/gsuijjwcb.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.blog.hesvh.cn/Article/details/ghvtqdvxf.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://read.share.hesvh.cn/Article/details/grqxsjxmv.sHtML

JS:   e.message;  e.stack
来源：http://www.share.zdbjq.cn/Article/details/gihhmfuey.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://blog.hesvh.cn/Article/details/gouxksdro.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://baike.hesvh.cn/Article/details/gqwmafmql.sHtML

Go:   err.Error()
来源：http://mobile.hesvh.cn/Article/details/gdojtverc.sHtML

Ruby: e.message;  e.backtrace
来源：http://wap.fehbvm.com/Article/details/gyhwlczik.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.share.hesvh.cn/Article/details/gjnspsskg.sHtML

[H09] 带错误码的异常
来源：http://www.blog.zdbjq.cn/Article/details/ghxshzgsg.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://baike.zdbjq.cn/Article/details/gkzzncubg.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://3g.zdbjq.cn/Article/details/gjshhbwjz.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.blog.zdbjq.cn/Article/details/gdfqmoxnv.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.share.fehbvm.com/Article/details/ggygeltqn.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://m.share.fehbvm.com/Article/details/gltmpxfxe.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.share.fehbvm.com/Article/details/gmwdxtxgz.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://wap.zdbjq.cn/Article/details/gnvgjdebz.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://baike.zdbjq.cn/Article/details/gsjwgwjpc.sHtML

[H10] 资源自动释放
来源：http://www.share.zdbjq.cn/Article/details/ggoksvamf.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.m.share.zdbjq.cn/Article/details/glhogopnt.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.blog.zdbjq.cn/Article/details/gaagisdex.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.zdbjq.cn/Article/details/gnvilwtsq.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.zdbjq.cn/Article/details/goqkizoky.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://read.share.fehbvm.com/Article/details/gxcyhbcmi.sHtML

Go:   defer f.Close()
来源：http://www.blog.zdbjq.cn/Article/details/gqkdqcnam.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://3g.fehbvm.com/Article/details/gawppbojp.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gqrvfpevb.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/glejmxcwx.sHtML

I. 正则表达式
来源：http://baike.hesvh.cn/Article/details/gknszcaia.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gdzwditkv.sHtML

[I01] 判断是否匹配
来源：http://www.blog.zdbjq.cn/Article/details/gujxrekeq.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.blog.fehbvm.com/Article/details/gthmphgpa.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://blog.hesvh.cn/Article/details/gstamsudy.sHtML

JS:   /\d+/.test(s)
来源：http://read.share.fehbvm.com/Article/details/gtpyqqvlu.sHtML

TS:   /\d+/.test(s)
来源：http://www.blog.zdbjq.cn/Article/details/gozygsyai.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wap.hesvh.cn/Article/details/gvflrqwwp.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://3g.fehbvm.com/Article/details/gzithuvjm.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.m.share.fehbvm.com/Article/details/gqkyfjfys.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://blog.hesvh.cn/Article/details/gmfftkwmu.sHtML

[I02] 提取所有匹配
来源：http://www.m.share.fehbvm.com/Article/details/gmdhtlokd.sHtML

Py:   re.findall(r"\d+", s)
来源：http://baike.fehbvm.com/Article/details/gcprqtqev.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wap.zdbjq.cn/Article/details/gosdyklih.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://blog.fehbvm.com/Article/details/gjbsreypc.sHtML

TS:   s.match(/\d+/g)
来源：http://3g.zdbjq.cn/Article/details/gmzjevjgr.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://blog.hesvh.cn/Article/details/gmawdtchl.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://read.share.zdbjq.cn/Article/details/gddxhaphs.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.share.fehbvm.com/Article/details/gxbccbirn.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.blog.hesvh.cn/Article/details/gtyfnosgn.sHtML

[I03] 提取捕获分组
来源：http://m.share.fehbvm.com/Article/details/gxopymlgs.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mobile.zdbjq.cn/Article/details/ghelobefb.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://blog.fehbvm.com/Article/details/gxlxwnckx.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mobile.fehbvm.com/Article/details/gisldjbzk.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.m.share.fehbvm.com/Article/details/gjsgrpbxe.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.m.share.fehbvm.com/Article/details/gfjlgmcwm.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.blog.hesvh.cn/Article/details/guosvwxke.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://read.share.hesvh.cn/Article/details/gxamuwdbb.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://m.share.fehbvm.com/Article/details/gltwcfypa.sHtML

[I04] 正则替换
来源：http://wap.hesvh.cn/Article/details/grgidvpvf.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://m.share.zdbjq.cn/Article/details/gzmhzjrbf.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mobile.hesvh.cn/Article/details/gvxgtdbnr.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://wap.hesvh.cn/Article/details/gvahvlaxb.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://read.share.fehbvm.com/Article/details/geqhgbhra.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://m.share.hesvh.cn/Article/details/gphlpsarp.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://m.share.zdbjq.cn/Article/details/gkyqnnmrl.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://m.share.fehbvm.com/Article/details/guaqrjkxu.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://blog.hesvh.cn/Article/details/gghflrhfa.sHtML

[I05] 按正则拆分
来源：http://www.blog.zdbjq.cn/Article/details/gaottmjzs.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://m.share.hesvh.cn/Article/details/gzaxmkact.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.share.fehbvm.com/Article/details/gjhcxszwc.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://wap.hesvh.cn/Article/details/gmgnqdhoh.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://read.share.hesvh.cn/Article/details/gwghnoofz.sHtML

Java: s.split("\\s*,\\s*")
来源：http://3g.hesvh.cn/Article/details/gvvlovlvv.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://m.share.hesvh.cn/Article/details/gvtmjqbdw.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://baike.fehbvm.com/Article/details/gperhzsps.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://m.share.zdbjq.cn/Article/details/gaauiavby.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.blog.hesvh.cn/Article/details/grrgkkluf.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.m.share.fehbvm.com/Article/details/gryaczirq.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://3g.zdbjq.cn/Article/details/gufiwmecz.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.fehbvm.com/Article/details/gdubibxqf.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.zdbjq.cn/Article/details/gtwzfqyox.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mobile.zdbjq.cn/Article/details/ghbaeaivb.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://3g.zdbjq.cn/Article/details/gretddizo.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://read.share.hesvh.cn/Article/details/gunzfjrch.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://3g.zdbjq.cn/Article/details/gqwlcvtmo.sHtML

[I07] 忽略大小写与多行模式
来源：http://baike.fehbvm.com/Article/details/gftuajiuk.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://read.share.zdbjq.cn/Article/details/glljzlbzk.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.blog.zdbjq.cn/Article/details/gvinzbjxu.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.share.zdbjq.cn/Article/details/gqpwanrws.sHtML

TS:   /error/gim
来源：http://mobile.hesvh.cn/Article/details/gxzihkhxp.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://read.share.zdbjq.cn/Article/details/gjrhojtdu.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wap.fehbvm.com/Article/details/ggqupssqv.sHtML

Ruby: s.scan(/error/i)
来源：http://mobile.fehbvm.com/Article/details/gytnwooys.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://wap.zdbjq.cn/Article/details/goqluyszk.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://read.share.zdbjq.cn/Article/details/gqhetfqfk.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.blog.hesvh.cn/Article/details/gxwsuhkkl.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.blog.fehbvm.com/Article/details/gdvqzwmlt.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.zdbjq.cn/Article/details/geerobbxn.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.zdbjq.cn/Article/details/gieipwhwa.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.share.hesvh.cn/Article/details/gqopvhpsc.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wap.zdbjq.cn/Article/details/gzuvdatab.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.blog.hesvh.cn/Article/details/gsslwadju.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.m.share.zdbjq.cn/Article/details/gdpojfnnb.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/goaincllb.sHtML

J. 日期与时间
来源：http://blog.zdbjq.cn/Article/details/gzkyzzofi.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gmrbodepz.sHtML

[J01] 获取当前时间
来源：http://wap.hesvh.cn/Article/details/gmnwmhvuf.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.share.zdbjq.cn/Article/details/gkmxhvefu.sHtML


<!-- 参考信息 -->