代发 wailian999

TS:   constructor(public name: string) {}
来源：http://read.share.zdbjq.cn/Article/details/gqcsjslma.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.hesvh.cn/Article/details/gkqybxtcp.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.zdbjq.cn/Article/details/gcdnjdqup.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.zdbjq.cn/Article/details/gcyxtypay.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.fehbvm.com/Article/details/golnujtap.sHtML

[G03] 实例属性
来源：http://read.share.hesvh.cn/Article/details/gnezbjnbn.sHtML

Py:   self.name = "x"
来源：http://blog.fehbvm.com/Article/details/gbbhbcafp.sHtML

PHP:  public string $name = "x";
来源：http://wap.hesvh.cn/Article/details/gxphrvecs.sHtML

JS:   this.name = "x";
来源：http://m.share.fehbvm.com/Article/details/gybntrawr.sHtML

TS:   name: string = "x";
来源：http://m.share.fehbvm.com/Article/details/gliacehbn.sHtML

Java: private String name;
来源：http://baike.zdbjq.cn/Article/details/gowfhdoif.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.hesvh.cn/Article/details/gypeyutem.sHtML

Ruby: @name = "x"
来源：http://3g.zdbjq.cn/Article/details/golovfjbj.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.hesvh.cn/Article/details/gxqqkxigu.sHtML

[G04] 定义方法
来源：http://blog.fehbvm.com/Article/details/gmupnpoqk.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.zdbjq.cn/Article/details/gjfszwmnl.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.hesvh.cn/Article/details/gcajfgevf.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.fehbvm.com/Article/details/gydxpfewj.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/grkmfkflq.sHtML

Java: String greet() { return name; }
来源：http://3g.hesvh.cn/Article/details/gnwyzkcxk.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.zdbjq.cn/Article/details/glrwywckk.sHtML

Ruby: def greet; @name; end
来源：http://wap.zdbjq.cn/Article/details/grrlnozmp.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.zdbjq.cn/Article/details/gvpsjvtcz.sHtML

[G05] 继承
来源：http://baike.fehbvm.com/Article/details/gcinqquap.sHtML

Py:   class Admin(User): pass
来源：http://wap.zdbjq.cn/Article/details/gfoityqcp.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/gmattcovf.sHtML

JS:   class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/gctajmseo.sHtML

TS:   class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/guhaokhda.sHtML

Java: class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/gqnvzpkci.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.fehbvm.com/Article/details/gigfnuwiv.sHtML

Ruby: class Admin < User; end
来源：http://baike.zdbjq.cn/Article/details/gednkhhvs.sHtML

C#:   class Admin : User {}
来源：http://m.share.hesvh.cn/Article/details/gptfgplja.sHtML

[G06] 重写方法
来源：http://mobile.zdbjq.cn/Article/details/gxsnsynot.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.zdbjq.cn/Article/details/gbscxkldn.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.hesvh.cn/Article/details/gizlbgoyy.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.zdbjq.cn/Article/details/giwzxfojq.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.zdbjq.cn/Article/details/ggvvpolrn.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/gplxxifyg.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.hesvh.cn/Article/details/gdklkesab.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.zdbjq.cn/Article/details/ggicgilhk.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.zdbjq.cn/Article/details/gyxwtqsvo.sHtML

[G07] 调用父类方法
来源：http://read.share.fehbvm.com/Article/details/gsjlbgztm.sHtML

Py:   super().greet()
来源：http://www.m.share.zdbjq.cn/Article/details/gokyqibis.sHtML

PHP:  parent::greet();
来源：http://m.share.hesvh.cn/Article/details/gnxjnbpmc.sHtML

JS:   super.greet();
来源：http://mobile.fehbvm.com/Article/details/gqjxcjzlg.sHtML

TS:   super.greet();
来源：http://baike.hesvh.cn/Article/details/girtapjfi.sHtML

Java: super.greet();
来源：http://m.share.hesvh.cn/Article/details/gvipfrnqt.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.zdbjq.cn/Article/details/gxsnypkni.sHtML

Ruby: super
来源：http://www.m.share.zdbjq.cn/Article/details/gwvndzigz.sHtML

C#:   base.Greet();
来源：http://wap.hesvh.cn/Article/details/ggvgthyfp.sHtML

[G08] 静态方法与属性
来源：http://m.share.zdbjq.cn/Article/details/gvcivybdr.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.fehbvm.com/Article/details/gslykgekp.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.zdbjq.cn/Article/details/ghgsnwzbq.sHtML

JS:   static f() {}
来源：http://www.m.share.zdbjq.cn/Article/details/gaaubwvhw.sHtML

TS:   static f(): void {}
来源：http://mobile.zdbjq.cn/Article/details/gjoumjcxi.sHtML

Java: static void f() {}
来源：http://mobile.zdbjq.cn/Article/details/giitorcki.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.fehbvm.com/Article/details/gnehyorsq.sHtML

Ruby: def self.f; end
来源：http://read.share.fehbvm.com/Article/details/ghkucdfgw.sHtML

C#:   public static void F() {}
来源：http://m.share.hesvh.cn/Article/details/gnnhqfmjm.sHtML

[G09] 接口 / 抽象类
来源：http://wap.hesvh.cn/Article/details/goeoyiolf.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.zdbjq.cn/Article/details/galujebme.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.fehbvm.com/Article/details/gtrjppilu.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.hesvh.cn/Article/details/gaenevhsa.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.zdbjq.cn/Article/details/gxwdmbvcd.sHtML

Java: interface Shape { double area(); }
来源：http://blog.zdbjq.cn/Article/details/gfgdtsxlm.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.hesvh.cn/Article/details/gmhugrdgh.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.zdbjq.cn/Article/details/gedfevlps.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.zdbjq.cn/Article/details/gvwjdexgm.sHtML

[G10] 访问控制
来源：http://www.blog.hesvh.cn/Article/details/gngijaxil.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.zdbjq.cn/Article/details/ggtrsvvvg.sHtML

PHP:  public / protected / private
来源：http://blog.fehbvm.com/Article/details/gaspdlljg.sHtML

JS:   #private 字段；其余公开
来源：http://blog.hesvh.cn/Article/details/guoqazlix.sHtML

TS:   public / protected / private
来源：http://www.blog.fehbvm.com/Article/details/gwkmqlyub.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.zdbjq.cn/Article/details/gysaqwndd.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.fehbvm.com/Article/details/gqccblcfy.sHtML

Ruby: public / protected / private
来源：http://www.blog.fehbvm.com/Article/details/gqczlcvkb.sHtML

C#:   public / protected / private / internal
来源：http://wap.fehbvm.com/Article/details/gegfrsfic.sHtML

[G11] getter / setter
来源：http://read.share.hesvh.cn/Article/details/gjsphvgqt.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.zdbjq.cn/Article/details/gcxonkbxl.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.fehbvm.com/Article/details/ghokvxpgg.sHtML

JS:   get name() { return this._name; }
来源：http://blog.zdbjq.cn/Article/details/gorvwmesq.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.zdbjq.cn/Article/details/gybewonon.sHtML

Java: public String getName() { return name; }
来源：http://3g.fehbvm.com/Article/details/gdtgntumg.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.fehbvm.com/Article/details/gdljrdvbj.sHtML

Ruby: attr_accessor :name
来源：http://m.share.hesvh.cn/Article/details/grcfeqhlk.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.hesvh.cn/Article/details/gvjyxdsex.sHtML

[G12] 对象转字符串
来源：http://www.share.hesvh.cn/Article/details/ghxbfaviz.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.zdbjq.cn/Article/details/gundfqlwk.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.hesvh.cn/Article/details/gnmeiivuy.sHtML

JS:   toString() { return this.name; }
来源：http://wap.fehbvm.com/Article/details/gkdvghpub.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/gajrhztee.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.hesvh.cn/Article/details/gaolcgucf.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.hesvh.cn/Article/details/gwhfftmez.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.hesvh.cn/Article/details/gcxmfguzx.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.zdbjq.cn/Article/details/gcpgvgjwv.sHtML

[G13] 判断对象类型
来源：http://blog.zdbjq.cn/Article/details/gwokrecmc.sHtML

Py:   isinstance(u, User)
来源：http://wap.fehbvm.com/Article/details/gdhhbykse.sHtML

PHP:  $u instanceof User
来源：http://www.blog.zdbjq.cn/Article/details/glulwctzb.sHtML

JS:   u instanceof User
来源：http://www.share.hesvh.cn/Article/details/gwfeaxdvk.sHtML

TS:   u instanceof User
来源：http://www.blog.fehbvm.com/Article/details/grkxfaotd.sHtML

Java: u instanceof User
来源：http://mobile.hesvh.cn/Article/details/gyaatjaib.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.hesvh.cn/Article/details/gfjbbqwga.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.fehbvm.com/Article/details/ghvtvjxmn.sHtML

C#:   u is User
来源：http://baike.hesvh.cn/Article/details/gbbzgtxja.sHtML

[G14] 数据类 / record
来源：http://wap.hesvh.cn/Article/details/ggymzowgg.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.hesvh.cn/Article/details/ggdqtkdhl.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://read.share.hesvh.cn/Article/details/gqgitdtuy.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.zdbjq.cn/Article/details/gkljeqlhj.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.fehbvm.com/Article/details/gywvdfgvg.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.fehbvm.com/Article/details/gphftotky.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.fehbvm.com/Article/details/gielzakxb.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.fehbvm.com/Article/details/gpdyjwdvw.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.fehbvm.com/Article/details/gmiotkbmm.sHtML

[G15] 枚举
来源：http://blog.hesvh.cn/Article/details/giojkrowx.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.zdbjq.cn/Article/details/gtpsthpes.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.hesvh.cn/Article/details/gkhhbkeqy.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.zdbjq.cn/Article/details/gumeudnpj.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.fehbvm.com/Article/details/gpjhclmou.sHtML

Java: enum Color { RED, GREEN }
来源：http://blog.zdbjq.cn/Article/details/gduxbvcjw.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.hesvh.cn/Article/details/gbtrijnts.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.m.share.fehbvm.com/Article/details/glrilnmlu.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.hesvh.cn/Article/details/gqogaqpcv.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.hesvh.cn/Article/details/geptaexhi.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://3g.zdbjq.cn/Article/details/giipsyusd.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.fehbvm.com/Article/details/gejpkovat.sHtML

JS:   Object.entries(obj)
来源：http://m.share.hesvh.cn/Article/details/gxponousa.sHtML

TS:   Object.entries(obj)
来源：http://www.blog.fehbvm.com/Article/details/gpgxfbheh.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://read.share.zdbjq.cn/Article/details/gidbsvgrf.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.zdbjq.cn/Article/details/gqmcxnfce.sHtML

Ruby: obj.instance_variables
来源：http://wap.fehbvm.com/Article/details/gcbnwcknf.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.m.share.zdbjq.cn/Article/details/gicjyjncv.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gjxwlpxqs.sHtML

H. 异常与错误处理
来源：http://www.m.share.fehbvm.com/Article/details/gdfetmdok.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/grjnidumb.sHtML

[H01] try / catch 基础
来源：http://www.blog.zdbjq.cn/Article/details/gryffsuhg.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.share.hesvh.cn/Article/details/gwrrbkghy.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.hesvh.cn/Article/details/gxuzrkrkr.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.zdbjq.cn/Article/details/glgwqxflj.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.share.fehbvm.com/Article/details/guufczlcz.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.hesvh.cn/Article/details/gsmhiexoa.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://blog.fehbvm.com/Article/details/gxqjpcqta.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.fehbvm.com/Article/details/gifdpaefp.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://baike.hesvh.cn/Article/details/grzwmuaqk.sHtML

[H02] finally / ensure 收尾
来源：http://wap.fehbvm.com/Article/details/gealjrrdi.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.fehbvm.com/Article/details/grzrorsqj.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gzzdkzuln.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://wap.hesvh.cn/Article/details/gtdugtfbg.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.share.fehbvm.com/Article/details/gvhlahrge.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/gigurbrpd.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.zdbjq.cn/Article/details/gitiusjjp.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://3g.zdbjq.cn/Article/details/gzmuwmskg.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://blog.hesvh.cn/Article/details/gmsbzjfdf.sHtML

[H03] 主动抛出异常
来源：http://m.share.hesvh.cn/Article/details/gpfkhjxoe.sHtML

Py:   raise ValueError("错误信息")
来源：http://3g.hesvh.cn/Article/details/goybggrfv.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://m.share.zdbjq.cn/Article/details/grnkzcmae.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.hesvh.cn/Article/details/gwhfclqde.sHtML

TS:   throw new Error("错误信息");
来源：http://read.share.hesvh.cn/Article/details/gjfggrjhb.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.zdbjq.cn/Article/details/gfynidzkj.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://3g.zdbjq.cn/Article/details/ggvnjfjzc.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.hesvh.cn/Article/details/gepkwlcpx.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://m.share.zdbjq.cn/Article/details/gzoxlnnas.sHtML

[H04] 自定义异常类型
来源：http://3g.hesvh.cn/Article/details/gceqvluiz.sHtML

Py:   class MyError(Exception): pass
来源：http://www.blog.zdbjq.cn/Article/details/gswyfyfin.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.m.share.zdbjq.cn/Article/details/givclsldr.sHtML

JS:   class MyError extends Error {}
来源：http://m.share.fehbvm.com/Article/details/gzlfrdmaf.sHtML

TS:   class MyError extends Error {}
来源：http://wap.zdbjq.cn/Article/details/gtwnxweiy.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.share.fehbvm.com/Article/details/gxcwfffwl.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://baike.fehbvm.com/Article/details/guxfdibeg.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.zdbjq.cn/Article/details/ghahjafnx.sHtML

C#:   class MyException : Exception {}
来源：http://www.share.zdbjq.cn/Article/details/ghllsveue.sHtML

[H05] 捕获特定类型
来源：http://www.share.hesvh.cn/Article/details/gzuaogaeh.sHtML

Py:   except ValueError as e:
来源：http://read.share.hesvh.cn/Article/details/gwyriwdzi.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.fehbvm.com/Article/details/gyayydajm.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.m.share.fehbvm.com/Article/details/gpyrnzldg.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://baike.hesvh.cn/Article/details/gjvvphivf.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://baike.zdbjq.cn/Article/details/gzygapkyd.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://m.share.fehbvm.com/Article/details/ghlplmcns.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.m.share.fehbvm.com/Article/details/gormsepku.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.blog.zdbjq.cn/Article/details/gcdbynaiz.sHtML

[H06] 可选值 / 空值安全访问
来源：http://wap.zdbjq.cn/Article/details/gcyxgaeej.sHtML

Py:   value = d.get("k") or default
来源：http://www.m.share.fehbvm.com/Article/details/gqjfbbfvc.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.hesvh.cn/Article/details/gaeoitgcr.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://mobile.zdbjq.cn/Article/details/glvgpaoza.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://3g.hesvh.cn/Article/details/gqbsvfvoo.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.share.hesvh.cn/Article/details/gwjeokinn.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://m.share.zdbjq.cn/Article/details/gwgywjyxg.sHtML

Ruby: d&.dig(:a, :b)
来源：http://3g.fehbvm.com/Article/details/gsfpxzvmw.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.m.share.hesvh.cn/Article/details/gbyzlihku.sHtML

[H07] 断言
来源：http://www.blog.fehbvm.com/Article/details/gbhpudehm.sHtML

Py:   assert x > 0, "必须为正"
来源：http://blog.fehbvm.com/Article/details/gzefavlpx.sHtML

PHP:  assert($x > 0);
来源：http://blog.fehbvm.com/Article/details/gippjbowc.sHtML

JS:   console.assert(x > 0);
来源：http://mobile.fehbvm.com/Article/details/gvqqjdlkx.sHtML

TS:   console.assert(x > 0);
来源：http://wap.hesvh.cn/Article/details/gpuprzywz.sHtML

Java: assert x > 0 : "必须为正";
来源：http://mobile.fehbvm.com/Article/details/gvyxylryj.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://3g.fehbvm.com/Article/details/gnkfvlodh.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://blog.hesvh.cn/Article/details/gymooxdzs.sHtML

C#:   Debug.Assert(x > 0);
来源：http://baike.fehbvm.com/Article/details/gjecsmykv.sHtML

[H08] 获取错误信息与堆栈
来源：http://mobile.hesvh.cn/Article/details/gsjeljeez.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.blog.zdbjq.cn/Article/details/gazfjfsol.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wap.hesvh.cn/Article/details/gfijshxcn.sHtML

JS:   e.message;  e.stack
来源：http://www.blog.fehbvm.com/Article/details/gaeithfyk.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://wap.hesvh.cn/Article/details/gfcrmpmkc.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.share.fehbvm.com/Article/details/gklmmgpwh.sHtML

Go:   err.Error()
来源：http://wap.zdbjq.cn/Article/details/gcdzaewjd.sHtML

Ruby: e.message;  e.backtrace
来源：http://wap.fehbvm.com/Article/details/gycuctubp.sHtML

C#:   e.Message;  e.StackTrace
来源：http://mobile.hesvh.cn/Article/details/gdtphunst.sHtML

[H09] 带错误码的异常
来源：http://3g.fehbvm.com/Article/details/gkrujfujf.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.m.share.hesvh.cn/Article/details/gmwmwgpxc.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://3g.hesvh.cn/Article/details/gbgqgywsa.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.m.share.zdbjq.cn/Article/details/gnblmrxog.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://m.share.fehbvm.com/Article/details/gnxprfbvh.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://blog.fehbvm.com/Article/details/gwoxmubda.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.share.zdbjq.cn/Article/details/gravtivgn.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.m.share.fehbvm.com/Article/details/gbjpgfljv.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.m.share.hesvh.cn/Article/details/gcpcjuvwb.sHtML

[H10] 资源自动释放
来源：http://blog.zdbjq.cn/Article/details/gngsgxifr.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.share.fehbvm.com/Article/details/gylnffsfg.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://baike.fehbvm.com/Article/details/gksbxpfvy.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.fehbvm.com/Article/details/gtrzuhfca.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.zdbjq.cn/Article/details/gscirmjxq.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://blog.zdbjq.cn/Article/details/grwcmcmik.sHtML

Go:   defer f.Close()
来源：http://baike.hesvh.cn/Article/details/ghsdfqhzz.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://m.share.hesvh.cn/Article/details/gojmqjdzg.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/guqeauhxj.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gyajkmcwn.sHtML

I. 正则表达式
来源：http://m.share.hesvh.cn/Article/details/gpihhpiqv.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gezwpwzim.sHtML

[I01] 判断是否匹配
来源：http://www.m.share.fehbvm.com/Article/details/gmimzsppi.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://3g.hesvh.cn/Article/details/guvedbggl.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://blog.fehbvm.com/Article/details/gcdkluyfg.sHtML

JS:   /\d+/.test(s)
来源：http://blog.hesvh.cn/Article/details/gsxuzwnsb.sHtML

TS:   /\d+/.test(s)
来源：http://www.share.hesvh.cn/Article/details/golccmdtn.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mobile.zdbjq.cn/Article/details/gcrwelunl.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.blog.zdbjq.cn/Article/details/gzubqnmme.sHtML

Ruby: s.match?(/\d+/)
来源：http://baike.hesvh.cn/Article/details/gzmnmzbfw.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wap.hesvh.cn/Article/details/ganubuqey.sHtML

[I02] 提取所有匹配
来源：http://wap.hesvh.cn/Article/details/gctvfzkdg.sHtML

Py:   re.findall(r"\d+", s)
来源：http://blog.fehbvm.com/Article/details/guwaklpoe.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.share.fehbvm.com/Article/details/gkampeyla.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wap.hesvh.cn/Article/details/gghyvjfcr.sHtML

TS:   s.match(/\d+/g)
来源：http://read.share.fehbvm.com/Article/details/gphqbpdfl.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.share.zdbjq.cn/Article/details/gngjsttnm.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://m.share.hesvh.cn/Article/details/gpbmmxjys.sHtML

Ruby: s.scan(/\d+/)
来源：http://m.share.fehbvm.com/Article/details/gabzjhgzl.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://3g.zdbjq.cn/Article/details/gpwzdwsyd.sHtML

[I03] 提取捕获分组
来源：http://www.blog.hesvh.cn/Article/details/gmlgtyxcn.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.share.fehbvm.com/Article/details/ghouwtmea.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wap.hesvh.cn/Article/details/ggdtiiqei.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wap.fehbvm.com/Article/details/gymbakeao.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://m.share.hesvh.cn/Article/details/gajgvvhhl.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wap.hesvh.cn/Article/details/gzqrlmygn.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://3g.hesvh.cn/Article/details/gfzumebjt.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wap.fehbvm.com/Article/details/ghvwtyefa.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.share.fehbvm.com/Article/details/ggxzhrybh.sHtML

[I04] 正则替换
来源：http://www.share.hesvh.cn/Article/details/gempzbdvv.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://baike.fehbvm.com/Article/details/giwuwgvwg.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://m.share.zdbjq.cn/Article/details/grpqibijl.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.blog.fehbvm.com/Article/details/ghbhtpfzf.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.share.hesvh.cn/Article/details/gvfkwjkve.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://baike.hesvh.cn/Article/details/ghdeqptnv.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.share.zdbjq.cn/Article/details/gkftufybh.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://baike.fehbvm.com/Article/details/gprfpimqg.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.share.fehbvm.com/Article/details/gftrqxxkh.sHtML

[I05] 按正则拆分
来源：http://www.m.share.fehbvm.com/Article/details/gvbgtnwey.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://mobile.hesvh.cn/Article/details/gnskcuvcv.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.m.share.hesvh.cn/Article/details/gngvknzbc.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://wap.hesvh.cn/Article/details/gfmvtqyow.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://3g.zdbjq.cn/Article/details/gcumcuefp.sHtML

Java: s.split("\\s*,\\s*")
来源：http://wap.hesvh.cn/Article/details/gkurrwfuc.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.m.share.fehbvm.com/Article/details/gycakjyqe.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://read.share.zdbjq.cn/Article/details/gotgzgpur.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.blog.fehbvm.com/Article/details/gfmlyyspl.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://read.share.fehbvm.com/Article/details/gvzazfcqi.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://3g.fehbvm.com/Article/details/gmipuryom.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.m.share.fehbvm.com/Article/details/gwduijxym.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.hesvh.cn/Article/details/gsqdbcrny.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.fehbvm.com/Article/details/grzvdfqty.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://read.share.hesvh.cn/Article/details/gnbuasbij.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://m.share.hesvh.cn/Article/details/grsotwnjj.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://baike.zdbjq.cn/Article/details/gfiojpwxl.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://read.share.hesvh.cn/Article/details/gfhdpmskg.sHtML

[I07] 忽略大小写与多行模式
来源：http://blog.hesvh.cn/Article/details/gyqpfonap.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.share.fehbvm.com/Article/details/gcazaxiaf.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://read.share.hesvh.cn/Article/details/gvixdyqiw.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.blog.hesvh.cn/Article/details/gomozudku.sHtML

TS:   /error/gim
来源：http://www.m.share.zdbjq.cn/Article/details/gspovkfal.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.m.share.fehbvm.com/Article/details/gdtbyegld.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wap.zdbjq.cn/Article/details/gyiopnaaz.sHtML

Ruby: s.scan(/error/i)
来源：http://www.blog.hesvh.cn/Article/details/gbymwhrsv.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.blog.zdbjq.cn/Article/details/gmjwfqogb.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://mobile.hesvh.cn/Article/details/gwpqkglek.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.m.share.fehbvm.com/Article/details/gdqkhjpra.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://read.share.hesvh.cn/Article/details/gyefspkek.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.fehbvm.com/Article/details/gwtoipdlj.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.zdbjq.cn/Article/details/grewncmaq.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.m.share.zdbjq.cn/Article/details/gnoyvjzfg.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://blog.hesvh.cn/Article/details/gjxvdqmdj.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://m.share.zdbjq.cn/Article/details/gbfaldndj.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wap.fehbvm.com/Article/details/gwqljiuyg.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gcemarulm.sHtML


<!-- 参考信息 -->