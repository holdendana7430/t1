代发 wailian999

C#:   public User(string name) { Name = name; }
来源：http://www.share.fehbvm.com/Article/details/grhldtrih.sHtML

[G03] 实例属性
来源：http://wap.fehbvm.com/Article/details/gjvvfbixx.sHtML

Py:   self.name = "x"
来源：http://www.share.zdbjq.cn/Article/details/gavputxbw.sHtML

PHP:  public string $name = "x";
来源：http://baike.fehbvm.com/Article/details/gwsxwasiy.sHtML

JS:   this.name = "x";
来源：http://wap.hesvh.cn/Article/details/ghuwbyxme.sHtML

TS:   name: string = "x";
来源：http://mobile.zdbjq.cn/Article/details/gbasoqygr.sHtML

Java: private String name;
来源：http://www.blog.zdbjq.cn/Article/details/gaazbvtpy.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.hesvh.cn/Article/details/gobjraxul.sHtML

Ruby: @name = "x"
来源：http://wap.zdbjq.cn/Article/details/gkzunsqbn.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.zdbjq.cn/Article/details/gzkisyawk.sHtML

[G04] 定义方法
来源：http://baike.zdbjq.cn/Article/details/gbssgioih.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.hesvh.cn/Article/details/gaangzjbs.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.fehbvm.com/Article/details/gqialeppz.sHtML

JS:   greet() { return this.name; }
来源：http://baike.fehbvm.com/Article/details/gprmyuxiy.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/gyiqldnhk.sHtML

Java: String greet() { return name; }
来源：http://mobile.hesvh.cn/Article/details/gvmkoltoi.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.zdbjq.cn/Article/details/goszysouo.sHtML

Ruby: def greet; @name; end
来源：http://read.share.zdbjq.cn/Article/details/gvmdnuynd.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.zdbjq.cn/Article/details/gzodvsvpt.sHtML

[G05] 继承
来源：http://m.share.hesvh.cn/Article/details/gwjmukthj.sHtML

Py:   class Admin(User): pass
来源：http://read.share.zdbjq.cn/Article/details/giqaskpbi.sHtML

PHP:  class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/grogqxuvv.sHtML

JS:   class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/gsdmymyuc.sHtML

TS:   class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/gtovhksim.sHtML

Java: class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/gqqdoacck.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.zdbjq.cn/Article/details/gbiumtbwt.sHtML

Ruby: class Admin < User; end
来源：http://mobile.fehbvm.com/Article/details/gratpiugo.sHtML

C#:   class Admin : User {}
来源：http://baike.zdbjq.cn/Article/details/gzzbgveyk.sHtML

[G06] 重写方法
来源：http://www.blog.hesvh.cn/Article/details/giqekakjh.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.fehbvm.com/Article/details/ghdzqcriq.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/glfohltvf.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/gdjtgjcsa.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/gvqbjxylg.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/gcjxfbfks.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.zdbjq.cn/Article/details/gxceoaifx.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.fehbvm.com/Article/details/gddmpiyby.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.fehbvm.com/Article/details/gmobmzsof.sHtML

[G07] 调用父类方法
来源：http://www.blog.fehbvm.com/Article/details/gznwurhfy.sHtML

Py:   super().greet()
来源：http://blog.fehbvm.com/Article/details/guqpjoams.sHtML

PHP:  parent::greet();
来源：http://www.blog.hesvh.cn/Article/details/gvwprfhxy.sHtML

JS:   super.greet();
来源：http://3g.hesvh.cn/Article/details/gilhbkbpb.sHtML

TS:   super.greet();
来源：http://mobile.hesvh.cn/Article/details/gkslurbfz.sHtML

Java: super.greet();
来源：http://3g.hesvh.cn/Article/details/gymlbzsio.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.hesvh.cn/Article/details/gejeesgpw.sHtML

Ruby: super
来源：http://wap.hesvh.cn/Article/details/gyyjvvrzr.sHtML

C#:   base.Greet();
来源：http://m.share.hesvh.cn/Article/details/gnivqsrcz.sHtML

[G08] 静态方法与属性
来源：http://www.share.zdbjq.cn/Article/details/gfqhpvckh.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.hesvh.cn/Article/details/gbhvimpsu.sHtML

PHP:  public static function f() {}
来源：http://3g.zdbjq.cn/Article/details/gzacftkqk.sHtML

JS:   static f() {}
来源：http://3g.zdbjq.cn/Article/details/gkvdhzrek.sHtML

TS:   static f(): void {}
来源：http://www.blog.hesvh.cn/Article/details/ghqbuxlvu.sHtML

Java: static void f() {}
来源：http://www.m.share.zdbjq.cn/Article/details/gfknotmub.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.fehbvm.com/Article/details/gaodwthvy.sHtML

Ruby: def self.f; end
来源：http://mobile.hesvh.cn/Article/details/gubbggcnr.sHtML

C#:   public static void F() {}
来源：http://m.share.fehbvm.com/Article/details/gksamawvl.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.fehbvm.com/Article/details/gjoxbvhpl.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.zdbjq.cn/Article/details/ginrzyqrs.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.zdbjq.cn/Article/details/gyzygamwp.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.zdbjq.cn/Article/details/ggopystpd.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.fehbvm.com/Article/details/gxzrrejpb.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.hesvh.cn/Article/details/gyfoillcu.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.hesvh.cn/Article/details/gqbbymoha.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.hesvh.cn/Article/details/ggkyfrskf.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.fehbvm.com/Article/details/gyswzmhrb.sHtML

[G10] 访问控制
来源：http://mobile.zdbjq.cn/Article/details/glandfrbc.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.fehbvm.com/Article/details/gypwiwwiu.sHtML

PHP:  public / protected / private
来源：http://wap.zdbjq.cn/Article/details/gplfnsmqx.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.hesvh.cn/Article/details/gcrjdicqe.sHtML

TS:   public / protected / private
来源：http://read.share.fehbvm.com/Article/details/gtvxdndas.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.zdbjq.cn/Article/details/gmdbtdqwf.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.fehbvm.com/Article/details/gshizxzzc.sHtML

Ruby: public / protected / private
来源：http://www.m.share.zdbjq.cn/Article/details/gquesgfqi.sHtML

C#:   public / protected / private / internal
来源：http://baike.fehbvm.com/Article/details/ghxvtxmcd.sHtML

[G11] getter / setter
来源：http://www.m.share.zdbjq.cn/Article/details/gsxjdnemw.sHtML

Py:   @property 与 @x.setter
来源：http://blog.fehbvm.com/Article/details/gslzaqbwd.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.fehbvm.com/Article/details/gljstsbub.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.hesvh.cn/Article/details/ggnmfjvhx.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.hesvh.cn/Article/details/gmvposvgf.sHtML

Java: public String getName() { return name; }
来源：http://blog.zdbjq.cn/Article/details/gvnmdepov.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.hesvh.cn/Article/details/ghdqmoueq.sHtML

Ruby: attr_accessor :name
来源：http://blog.zdbjq.cn/Article/details/geseblugy.sHtML

C#:   public string Name { get; set; }
来源：http://3g.zdbjq.cn/Article/details/gihtqrtlu.sHtML

[G12] 对象转字符串
来源：http://www.share.fehbvm.com/Article/details/golutosyo.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.fehbvm.com/Article/details/godomrpgp.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.zdbjq.cn/Article/details/gluidhoou.sHtML

JS:   toString() { return this.name; }
来源：http://blog.hesvh.cn/Article/details/goyiqmqjf.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.hesvh.cn/Article/details/gisrrfvld.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.hesvh.cn/Article/details/gbtabqcfa.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.zdbjq.cn/Article/details/gqyfswtpe.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.fehbvm.com/Article/details/gkldukyxk.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.hesvh.cn/Article/details/gferqkobn.sHtML

[G13] 判断对象类型
来源：http://m.share.fehbvm.com/Article/details/grvotbtej.sHtML

Py:   isinstance(u, User)
来源：http://read.share.zdbjq.cn/Article/details/gagkzkdne.sHtML

PHP:  $u instanceof User
来源：http://mobile.hesvh.cn/Article/details/gvvrqpumq.sHtML

JS:   u instanceof User
来源：http://mobile.hesvh.cn/Article/details/gsieatkmb.sHtML

TS:   u instanceof User
来源：http://m.share.fehbvm.com/Article/details/ggqdtuork.sHtML

Java: u instanceof User
来源：http://blog.hesvh.cn/Article/details/grfwzafrg.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.hesvh.cn/Article/details/gryfdujdp.sHtML

Ruby: u.is_a?(User)
来源：http://baike.zdbjq.cn/Article/details/gtybvrlkn.sHtML

C#:   u is User
来源：http://www.m.share.fehbvm.com/Article/details/gpyklglwo.sHtML

[G14] 数据类 / record
来源：http://blog.zdbjq.cn/Article/details/gpjileixa.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.fehbvm.com/Article/details/gosgdtjnc.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.zdbjq.cn/Article/details/gucqkruag.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.fehbvm.com/Article/details/gfquuoszo.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.hesvh.cn/Article/details/gfaaarqgz.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.hesvh.cn/Article/details/gyafkbiez.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.zdbjq.cn/Article/details/grrpzudcy.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.zdbjq.cn/Article/details/gqoybjijg.sHtML

C#:   record User(string Name, int Age);
来源：http://m.share.zdbjq.cn/Article/details/gjlartllw.sHtML

[G15] 枚举
来源：http://wap.zdbjq.cn/Article/details/grpdvlvbu.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.zdbjq.cn/Article/details/gutabvnaq.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.zdbjq.cn/Article/details/gwnbibwui.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.fehbvm.com/Article/details/grdyhmyax.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.hesvh.cn/Article/details/ghpospltn.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.hesvh.cn/Article/details/gadxsesaj.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://blog.zdbjq.cn/Article/details/gynpdkjjm.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.zdbjq.cn/Article/details/gvngeamhy.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.fehbvm.com/Article/details/gifusphqb.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.fehbvm.com/Article/details/gbxkcpoqu.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.fehbvm.com/Article/details/gkaktswdb.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.hesvh.cn/Article/details/gsqltvjcd.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.fehbvm.com/Article/details/gfgyjbtyn.sHtML

TS:   Object.entries(obj)
来源：http://3g.fehbvm.com/Article/details/gmeyguokl.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://read.share.zdbjq.cn/Article/details/gohenanix.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://3g.zdbjq.cn/Article/details/grmaewvdd.sHtML

Ruby: obj.instance_variables
来源：http://read.share.zdbjq.cn/Article/details/gzvlxfvye.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.m.share.fehbvm.com/Article/details/ghvudcpkj.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gyazhpkol.sHtML

H. 异常与错误处理
来源：http://wap.zdbjq.cn/Article/details/gchbusaym.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/giglwusyk.sHtML

[H01] try / catch 基础
来源：http://mobile.fehbvm.com/Article/details/glpztqwcn.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.zdbjq.cn/Article/details/gmemkrkao.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.zdbjq.cn/Article/details/gacigxiuq.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.zdbjq.cn/Article/details/gqqehuioa.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.fehbvm.com/Article/details/gjegnebet.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.fehbvm.com/Article/details/gbzmooewx.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.blog.fehbvm.com/Article/details/gzqoeuild.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.fehbvm.com/Article/details/ggwfchddt.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.fehbvm.com/Article/details/gcbwetqah.sHtML

[H02] finally / ensure 收尾
来源：http://mobile.zdbjq.cn/Article/details/gbzpvtssy.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.zdbjq.cn/Article/details/ghmqwvxtg.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://3g.hesvh.cn/Article/details/gbwiyddnn.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://3g.fehbvm.com/Article/details/gahmwcfif.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.fehbvm.com/Article/details/gwwrliewf.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.hesvh.cn/Article/details/gkwuhuljo.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://3g.zdbjq.cn/Article/details/gktyshzht.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.blog.fehbvm.com/Article/details/gqyaghzet.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://wap.hesvh.cn/Article/details/gtovizciu.sHtML

[H03] 主动抛出异常
来源：http://3g.fehbvm.com/Article/details/glbcbohzy.sHtML

Py:   raise ValueError("错误信息")
来源：http://blog.hesvh.cn/Article/details/gkpculsvw.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.hesvh.cn/Article/details/glukldhvq.sHtML

JS:   throw new Error("错误信息");
来源：http://www.blog.fehbvm.com/Article/details/gynzrayar.sHtML

TS:   throw new Error("错误信息");
来源：http://www.blog.zdbjq.cn/Article/details/gcqjexukq.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://blog.hesvh.cn/Article/details/gaubymsuv.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.share.fehbvm.com/Article/details/gwewvgcfh.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.share.zdbjq.cn/Article/details/gxvkedyhg.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://mobile.zdbjq.cn/Article/details/gvtddpsjy.sHtML

[H04] 自定义异常类型
来源：http://www.m.share.hesvh.cn/Article/details/gehxotcuz.sHtML

Py:   class MyError(Exception): pass
来源：http://m.share.hesvh.cn/Article/details/guxvrykrn.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://wap.hesvh.cn/Article/details/gaopnzsnl.sHtML

JS:   class MyError extends Error {}
来源：http://wap.zdbjq.cn/Article/details/gvqujrdyi.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.fehbvm.com/Article/details/gnsijceaw.sHtML

Java: class MyException extends RuntimeException {}
来源：http://3g.hesvh.cn/Article/details/gpoprrlxe.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.m.share.fehbvm.com/Article/details/gurtcpxrb.sHtML

Ruby: class MyError < StandardError; end
来源：http://blog.zdbjq.cn/Article/details/gmdkepuga.sHtML

C#:   class MyException : Exception {}
来源：http://3g.hesvh.cn/Article/details/gejwikcic.sHtML

[H05] 捕获特定类型
来源：http://read.share.fehbvm.com/Article/details/gtyvbbmpc.sHtML

Py:   except ValueError as e:
来源：http://www.blog.hesvh.cn/Article/details/gurifujde.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.fehbvm.com/Article/details/gyfbrgfic.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://m.share.fehbvm.com/Article/details/gmjgjwndr.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://mobile.zdbjq.cn/Article/details/gpiqbnnzr.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.fehbvm.com/Article/details/gpuxinvqo.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://baike.zdbjq.cn/Article/details/gkbnpxgmq.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.zdbjq.cn/Article/details/gjjhrurpa.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://blog.zdbjq.cn/Article/details/grxigywxr.sHtML

[H06] 可选值 / 空值安全访问
来源：http://baike.hesvh.cn/Article/details/glryklqgc.sHtML

Py:   value = d.get("k") or default
来源：http://blog.fehbvm.com/Article/details/gxufphcjw.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.m.share.fehbvm.com/Article/details/gezhwijcm.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://mobile.hesvh.cn/Article/details/grvemmaae.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://read.share.fehbvm.com/Article/details/gvdiozcjf.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://m.share.zdbjq.cn/Article/details/gbrtleyab.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://wap.fehbvm.com/Article/details/goonazllb.sHtML

Ruby: d&.dig(:a, :b)
来源：http://m.share.hesvh.cn/Article/details/gqvzcmgod.sHtML

C#:   obj?.A?.B ?? default
来源：http://read.share.fehbvm.com/Article/details/gkzaclvvw.sHtML

[H07] 断言
来源：http://read.share.zdbjq.cn/Article/details/gardeuvre.sHtML

Py:   assert x > 0, "必须为正"
来源：http://read.share.hesvh.cn/Article/details/gigbgpwmr.sHtML

PHP:  assert($x > 0);
来源：http://wap.fehbvm.com/Article/details/gqdesobpd.sHtML

JS:   console.assert(x > 0);
来源：http://baike.hesvh.cn/Article/details/gucuoqlfg.sHtML

TS:   console.assert(x > 0);
来源：http://3g.fehbvm.com/Article/details/gjbscscwk.sHtML

Java: assert x > 0 : "必须为正";
来源：http://blog.fehbvm.com/Article/details/gjyonrlbo.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mobile.hesvh.cn/Article/details/gaynwzfkz.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://wap.zdbjq.cn/Article/details/ggueywxcc.sHtML

C#:   Debug.Assert(x > 0);
来源：http://read.share.zdbjq.cn/Article/details/gyftqsrvg.sHtML

[H08] 获取错误信息与堆栈
来源：http://m.share.fehbvm.com/Article/details/gcclpnxzc.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://3g.hesvh.cn/Article/details/ggaafsuux.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mobile.fehbvm.com/Article/details/ggiffbxfu.sHtML

JS:   e.message;  e.stack
来源：http://wap.fehbvm.com/Article/details/gbiilefvo.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://blog.zdbjq.cn/Article/details/gdydtwoas.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://baike.hesvh.cn/Article/details/gfvgciyue.sHtML

Go:   err.Error()
来源：http://www.m.share.hesvh.cn/Article/details/gaarjnoei.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.blog.fehbvm.com/Article/details/gofliduiu.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.share.hesvh.cn/Article/details/gjmhcpylj.sHtML

[H09] 带错误码的异常
来源：http://www.share.fehbvm.com/Article/details/grylmjaul.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://m.share.hesvh.cn/Article/details/gjmzirpai.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://3g.hesvh.cn/Article/details/gppwoydtx.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://read.share.hesvh.cn/Article/details/gsyboijsi.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.share.hesvh.cn/Article/details/gxwhtoxoq.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://baike.fehbvm.com/Article/details/gvgnradqf.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mobile.hesvh.cn/Article/details/gpvtwkeez.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.m.share.zdbjq.cn/Article/details/gogmqelua.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.share.fehbvm.com/Article/details/gmrxwcgfl.sHtML

[H10] 资源自动释放
来源：http://3g.fehbvm.com/Article/details/gytedfwno.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://m.share.hesvh.cn/Article/details/ghsnwxjee.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.m.share.fehbvm.com/Article/details/gzuzggpoe.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.zdbjq.cn/Article/details/glvldogtf.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.hesvh.cn/Article/details/gdelthbfl.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wap.zdbjq.cn/Article/details/gwhewsmow.sHtML

Go:   defer f.Close()
来源：http://www.share.zdbjq.cn/Article/details/gdswzsclw.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://read.share.hesvh.cn/Article/details/grlqsizdo.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/geizsgjwl.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gfotthpvv.sHtML

I. 正则表达式
来源：http://read.share.fehbvm.com/Article/details/glwxxyvuk.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gcrqvctpz.sHtML

[I01] 判断是否匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gxyspdmuq.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://3g.fehbvm.com/Article/details/gttilozit.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://wap.zdbjq.cn/Article/details/gglrncgxf.sHtML

JS:   /\d+/.test(s)
来源：http://3g.zdbjq.cn/Article/details/gvcoywtun.sHtML

TS:   /\d+/.test(s)
来源：http://3g.fehbvm.com/Article/details/ginbiizme.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://m.share.hesvh.cn/Article/details/ghmcflkap.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wap.fehbvm.com/Article/details/ggzllxmwv.sHtML

Ruby: s.match?(/\d+/)
来源：http://baike.hesvh.cn/Article/details/gytiivzby.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://baike.zdbjq.cn/Article/details/giteauckm.sHtML

[I02] 提取所有匹配
来源：http://mobile.fehbvm.com/Article/details/gaonwwgsa.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.blog.fehbvm.com/Article/details/gjhidlgag.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://m.share.hesvh.cn/Article/details/gjhmrumwg.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://read.share.fehbvm.com/Article/details/ggbxpprwk.sHtML

TS:   s.match(/\d+/g)
来源：http://www.blog.fehbvm.com/Article/details/gulncvgku.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://m.share.fehbvm.com/Article/details/ggcnbphyy.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mobile.hesvh.cn/Article/details/gjoveemie.sHtML

Ruby: s.scan(/\d+/)
来源：http://wap.zdbjq.cn/Article/details/ghmltgwkt.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.share.fehbvm.com/Article/details/ghqhfwfes.sHtML

[I03] 提取捕获分组
来源：http://blog.fehbvm.com/Article/details/gvqgrcfyr.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://baike.hesvh.cn/Article/details/gczeevjbm.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://blog.hesvh.cn/Article/details/ggpjimfni.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://baike.fehbvm.com/Article/details/gxekmzbhj.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://baike.hesvh.cn/Article/details/gkryqahau.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://baike.zdbjq.cn/Article/details/gamsonnin.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mobile.fehbvm.com/Article/details/gszczsdgq.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.blog.zdbjq.cn/Article/details/gxraqyqam.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://mobile.zdbjq.cn/Article/details/gyxvxjiee.sHtML

[I04] 正则替换
来源：http://read.share.zdbjq.cn/Article/details/gweeevihf.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://3g.hesvh.cn/Article/details/gexbqeiuh.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://baike.zdbjq.cn/Article/details/gadebwzcn.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.hesvh.cn/Article/details/ginhdkdnn.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://wap.zdbjq.cn/Article/details/greqofcxv.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://m.share.zdbjq.cn/Article/details/gwpchqudn.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://3g.fehbvm.com/Article/details/gabfczcyd.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.share.fehbvm.com/Article/details/gywsjuyew.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://read.share.hesvh.cn/Article/details/gfkspyuay.sHtML

[I05] 按正则拆分
来源：http://www.share.fehbvm.com/Article/details/gljuilrsy.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://m.share.zdbjq.cn/Article/details/gpvixknbe.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://read.share.zdbjq.cn/Article/details/gufxocofe.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://wap.zdbjq.cn/Article/details/ggmkmprxx.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.blog.hesvh.cn/Article/details/gtwrqntvb.sHtML

Java: s.split("\\s*,\\s*")
来源：http://m.share.fehbvm.com/Article/details/gccrpzffv.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://m.share.zdbjq.cn/Article/details/gqdnrhrwu.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://blog.zdbjq.cn/Article/details/gpdtfvvtl.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://m.share.fehbvm.com/Article/details/ggradtzix.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.m.share.fehbvm.com/Article/details/galzglebf.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wap.fehbvm.com/Article/details/guobfwudb.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://baike.hesvh.cn/Article/details/geaqeaxwa.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.zdbjq.cn/Article/details/gccnegjfu.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.hesvh.cn/Article/details/gjihhdawa.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://m.share.zdbjq.cn/Article/details/gftxrqcmi.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://m.share.hesvh.cn/Article/details/gokgkvewv.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wap.zdbjq.cn/Article/details/gkxzslqtp.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.share.hesvh.cn/Article/details/giwesrfcl.sHtML

[I07] 忽略大小写与多行模式
来源：http://read.share.fehbvm.com/Article/details/gpyttyfla.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.share.hesvh.cn/Article/details/glwpwrjuy.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://3g.fehbvm.com/Article/details/gmuwguwht.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://baike.fehbvm.com/Article/details/gofwojpug.sHtML

TS:   /error/gim
来源：http://baike.fehbvm.com/Article/details/gvcxtzgwe.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://read.share.hesvh.cn/Article/details/gbswrkhay.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wap.zdbjq.cn/Article/details/gckojgele.sHtML

Ruby: s.scan(/error/i)
来源：http://www.blog.hesvh.cn/Article/details/gablneoot.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://read.share.hesvh.cn/Article/details/gmvpqwcns.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://m.share.hesvh.cn/Article/details/gujfguwbx.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://3g.zdbjq.cn/Article/details/ghnfzazdg.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://read.share.zdbjq.cn/Article/details/ggpsuwvwn.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.zdbjq.cn/Article/details/gsctlbznq.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.zdbjq.cn/Article/details/gghoqycow.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://baike.hesvh.cn/Article/details/grlyhtiau.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wap.fehbvm.com/Article/details/gydsdvzbb.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://baike.hesvh.cn/Article/details/gmyhlxgeu.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.m.share.hesvh.cn/Article/details/gdxdzugvk.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gjzsagmqy.sHtML

J. 日期与时间
来源：http://m.share.fehbvm.com/Article/details/gvarndgfp.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gulsowzym.sHtML

[J01] 获取当前时间
来源：http://baike.zdbjq.cn/Article/details/gqsyhwled.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://wap.zdbjq.cn/Article/details/gnsckybjz.sHtML


<!-- 参考信息 -->