代发 wailian999

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.hesvh.cn/Article/details/gbocfdmkj.sHtML

Ruby: def greet; @name; end
来源：http://3g.fehbvm.com/Article/details/ghgatxxhr.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.hesvh.cn/Article/details/gvgtkyhgu.sHtML

[G05] 继承
来源：http://m.share.fehbvm.com/Article/details/gzovlmxyj.sHtML

Py:   class Admin(User): pass
来源：http://wap.zdbjq.cn/Article/details/gaqalxckj.sHtML

PHP:  class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/gmproyviz.sHtML

JS:   class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/gmhpondpt.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/gebwlsjtf.sHtML

Java: class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/gzcboepxz.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.zdbjq.cn/Article/details/gfrrzpxwe.sHtML

Ruby: class Admin < User; end
来源：http://mobile.fehbvm.com/Article/details/gnfpkkyub.sHtML

C#:   class Admin : User {}
来源：http://mobile.hesvh.cn/Article/details/gvicqufmg.sHtML

[G06] 重写方法
来源：http://www.blog.fehbvm.com/Article/details/glqyxskef.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.zdbjq.cn/Article/details/gxohgmdzh.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/glwrtjjjm.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/gxmazxlju.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/gmtyneelb.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/grtzhssxc.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.zdbjq.cn/Article/details/gqrhtzszp.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.fehbvm.com/Article/details/gwhogdadu.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.hesvh.cn/Article/details/glesuungr.sHtML

[G07] 调用父类方法
来源：http://read.share.zdbjq.cn/Article/details/gdtioifsx.sHtML

Py:   super().greet()
来源：http://3g.hesvh.cn/Article/details/gielrzgmn.sHtML

PHP:  parent::greet();
来源：http://mobile.zdbjq.cn/Article/details/gqydoclrf.sHtML

JS:   super.greet();
来源：http://3g.fehbvm.com/Article/details/gzchrvgnd.sHtML

TS:   super.greet();
来源：http://baike.hesvh.cn/Article/details/gcmvvvboh.sHtML

Java: super.greet();
来源：http://www.m.share.fehbvm.com/Article/details/gsfsmrldw.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.zdbjq.cn/Article/details/grpoeldjv.sHtML

Ruby: super
来源：http://www.m.share.fehbvm.com/Article/details/gilpdknxp.sHtML

C#:   base.Greet();
来源：http://read.share.fehbvm.com/Article/details/gpaamnxwp.sHtML

[G08] 静态方法与属性
来源：http://3g.zdbjq.cn/Article/details/gqgociwes.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.fehbvm.com/Article/details/gefkrelas.sHtML

PHP:  public static function f() {}
来源：http://baike.fehbvm.com/Article/details/ggyizhdya.sHtML

JS:   static f() {}
来源：http://m.share.fehbvm.com/Article/details/galgziotv.sHtML

TS:   static f(): void {}
来源：http://read.share.hesvh.cn/Article/details/gchocecvf.sHtML

Java: static void f() {}
来源：http://baike.hesvh.cn/Article/details/gdhpihpaz.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.fehbvm.com/Article/details/gyeavyliv.sHtML

Ruby: def self.f; end
来源：http://www.share.zdbjq.cn/Article/details/gtnyrjztr.sHtML

C#:   public static void F() {}
来源：http://read.share.zdbjq.cn/Article/details/gcnoumzuv.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.zdbjq.cn/Article/details/gmbcqezyg.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.fehbvm.com/Article/details/gskhsimuw.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.hesvh.cn/Article/details/gnmpcrvir.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.hesvh.cn/Article/details/gotumwcfi.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.zdbjq.cn/Article/details/gedgqqpfh.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gjzllcosh.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.zdbjq.cn/Article/details/gribsfahe.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.zdbjq.cn/Article/details/gmxkvwapf.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.zdbjq.cn/Article/details/gfidkpbuc.sHtML

[G10] 访问控制
来源：http://baike.hesvh.cn/Article/details/gkfutakse.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.zdbjq.cn/Article/details/gfdlstrut.sHtML

PHP:  public / protected / private
来源：http://www.share.hesvh.cn/Article/details/gxpehegfe.sHtML

JS:   #private 字段；其余公开
来源：http://3g.hesvh.cn/Article/details/gcravzibv.sHtML

TS:   public / protected / private
来源：http://www.blog.fehbvm.com/Article/details/gdmuhfabe.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.hesvh.cn/Article/details/gbgcomcxg.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.hesvh.cn/Article/details/gisjkdgax.sHtML

Ruby: public / protected / private
来源：http://m.share.hesvh.cn/Article/details/grikujzfc.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.hesvh.cn/Article/details/gleuhkmmi.sHtML

[G11] getter / setter
来源：http://wap.zdbjq.cn/Article/details/gsgbcdpbq.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.zdbjq.cn/Article/details/gwcitdfpe.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.fehbvm.com/Article/details/gnkwneyth.sHtML

JS:   get name() { return this._name; }
来源：http://wap.zdbjq.cn/Article/details/goswoicxq.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.hesvh.cn/Article/details/gbfwjsaxa.sHtML

Java: public String getName() { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gogbgteje.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.fehbvm.com/Article/details/gdlbqbzbz.sHtML

Ruby: attr_accessor :name
来源：http://blog.hesvh.cn/Article/details/gwxmcwqnb.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.fehbvm.com/Article/details/gmfmpvchb.sHtML

[G12] 对象转字符串
来源：http://m.share.hesvh.cn/Article/details/gefxqwqhs.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.zdbjq.cn/Article/details/gdvcnkxen.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.hesvh.cn/Article/details/ghyhwudqz.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.hesvh.cn/Article/details/gpnwmcdsx.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.hesvh.cn/Article/details/gsqrmkjqj.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.zdbjq.cn/Article/details/gchgweamu.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.hesvh.cn/Article/details/gkbshrprf.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.fehbvm.com/Article/details/gdbcdlemf.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.fehbvm.com/Article/details/gcuoslyjg.sHtML

[G13] 判断对象类型
来源：http://m.share.zdbjq.cn/Article/details/gftigokvi.sHtML

Py:   isinstance(u, User)
来源：http://www.share.fehbvm.com/Article/details/gjmzinjwh.sHtML

PHP:  $u instanceof User
来源：http://blog.fehbvm.com/Article/details/gdqvnsmhp.sHtML

JS:   u instanceof User
来源：http://www.m.share.zdbjq.cn/Article/details/ghmzkglsh.sHtML

TS:   u instanceof User
来源：http://3g.hesvh.cn/Article/details/ghylwsiog.sHtML

Java: u instanceof User
来源：http://blog.zdbjq.cn/Article/details/gkeyeajwi.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.fehbvm.com/Article/details/gwbhlcbya.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.fehbvm.com/Article/details/gaklnojaq.sHtML

C#:   u is User
来源：http://www.blog.hesvh.cn/Article/details/gjjgnploz.sHtML

[G14] 数据类 / record
来源：http://3g.zdbjq.cn/Article/details/gktmgdbis.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.fehbvm.com/Article/details/gapfbvttt.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.zdbjq.cn/Article/details/gnritetnl.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.hesvh.cn/Article/details/gnbzvlnpv.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.zdbjq.cn/Article/details/gisfxbvzr.sHtML

Java: record User(String name, int age) {}
来源：http://3g.zdbjq.cn/Article/details/gxoycwrqx.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.hesvh.cn/Article/details/gathxzwgq.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.zdbjq.cn/Article/details/ggfidrmdw.sHtML

C#:   record User(string Name, int Age);
来源：http://wap.hesvh.cn/Article/details/gezugfbwn.sHtML

[G15] 枚举
来源：http://baike.zdbjq.cn/Article/details/gzlkbpddo.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.zdbjq.cn/Article/details/gtpketngp.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.zdbjq.cn/Article/details/guxzvyaqs.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.hesvh.cn/Article/details/gungxekau.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.fehbvm.com/Article/details/gqzyikxix.sHtML

Java: enum Color { RED, GREEN }
来源：http://blog.fehbvm.com/Article/details/gzmopdnqf.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.hesvh.cn/Article/details/golzwnkkx.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.fehbvm.com/Article/details/gxtcfwmju.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.hesvh.cn/Article/details/gxkajdxkz.sHtML

[G16] 对象转数组 / 字典
来源：http://www.blog.fehbvm.com/Article/details/gxektprdz.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://3g.fehbvm.com/Article/details/gbnlbyndn.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.hesvh.cn/Article/details/gxtqpgozz.sHtML

JS:   Object.entries(obj)
来源：http://www.share.fehbvm.com/Article/details/ggvsbveqm.sHtML

TS:   Object.entries(obj)
来源：http://mobile.zdbjq.cn/Article/details/gaduuyfdm.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.fehbvm.com/Article/details/gozoufcgm.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.fehbvm.com/Article/details/ggvvebhmm.sHtML

Ruby: obj.instance_variables
来源：http://3g.zdbjq.cn/Article/details/gsxgrgwtw.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.m.share.zdbjq.cn/Article/details/gcjdndhsb.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gggtjehic.sHtML

H. 异常与错误处理
来源：http://baike.hesvh.cn/Article/details/gbvwtskhh.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gfaupguca.sHtML

[H01] try / catch 基础
来源：http://3g.fehbvm.com/Article/details/gmokgsojy.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.fehbvm.com/Article/details/gxgbhkrcd.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.fehbvm.com/Article/details/glvkokufv.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.fehbvm.com/Article/details/glddbydkg.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.m.share.zdbjq.cn/Article/details/gwvvpymnp.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.blog.zdbjq.cn/Article/details/gnxqunhyi.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://read.share.zdbjq.cn/Article/details/gbdidaqak.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.zdbjq.cn/Article/details/gjpdjqpyx.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://blog.zdbjq.cn/Article/details/gufupwsqn.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.hesvh.cn/Article/details/giwgyvvuz.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://baike.hesvh.cn/Article/details/grmxjjeka.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://mobile.zdbjq.cn/Article/details/gbsyzodtb.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.fehbvm.com/Article/details/gnimrpikm.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.fehbvm.com/Article/details/gyxyheqlv.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.blog.hesvh.cn/Article/details/ggaemlegv.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.fehbvm.com/Article/details/gdpextyau.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://read.share.fehbvm.com/Article/details/glcvvwhkv.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://read.share.zdbjq.cn/Article/details/gwjxmcwar.sHtML

[H03] 主动抛出异常
来源：http://baike.hesvh.cn/Article/details/gmasjqdyq.sHtML

Py:   raise ValueError("错误信息")
来源：http://wap.zdbjq.cn/Article/details/gpqvmsswj.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.blog.fehbvm.com/Article/details/gwibroyqz.sHtML

JS:   throw new Error("错误信息");
来源：http://baike.zdbjq.cn/Article/details/ggagmocdm.sHtML

TS:   throw new Error("错误信息");
来源：http://wap.zdbjq.cn/Article/details/gmrflloio.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://read.share.hesvh.cn/Article/details/gumabicjl.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://read.share.hesvh.cn/Article/details/gxfguyuua.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.blog.hesvh.cn/Article/details/gmxbunpcy.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://mobile.fehbvm.com/Article/details/gdelzngvk.sHtML

[H04] 自定义异常类型
来源：http://mobile.zdbjq.cn/Article/details/guqffcktl.sHtML

Py:   class MyError(Exception): pass
来源：http://wap.hesvh.cn/Article/details/gjvogkbts.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://mobile.fehbvm.com/Article/details/glpocwxwt.sHtML

JS:   class MyError extends Error {}
来源：http://m.share.fehbvm.com/Article/details/gghajkvlu.sHtML

TS:   class MyError extends Error {}
来源：http://www.blog.hesvh.cn/Article/details/gwglmwwjd.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.share.hesvh.cn/Article/details/gyklpchzi.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.m.share.fehbvm.com/Article/details/gqzblqxvr.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.fehbvm.com/Article/details/glcyjvsaq.sHtML

C#:   class MyException : Exception {}
来源：http://baike.zdbjq.cn/Article/details/glcicngje.sHtML

[H05] 捕获特定类型
来源：http://3g.hesvh.cn/Article/details/gpxlxunzs.sHtML

Py:   except ValueError as e:
来源：http://www.blog.fehbvm.com/Article/details/gqdinfxdx.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://blog.hesvh.cn/Article/details/goncjgkoi.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://mobile.hesvh.cn/Article/details/gfkbulfmp.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.blog.hesvh.cn/Article/details/gceihlnxt.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://mobile.hesvh.cn/Article/details/gdetreusq.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.m.share.fehbvm.com/Article/details/gecubtkrm.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.m.share.hesvh.cn/Article/details/gcqymvoxa.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://blog.hesvh.cn/Article/details/ghmodijjz.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.blog.fehbvm.com/Article/details/gensqepwl.sHtML

Py:   value = d.get("k") or default
来源：http://m.share.zdbjq.cn/Article/details/gtuaqmlzq.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://wap.hesvh.cn/Article/details/gyobpznze.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.blog.hesvh.cn/Article/details/gdazjdclo.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://wap.zdbjq.cn/Article/details/gnrcbpdlv.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://baike.zdbjq.cn/Article/details/getegjfha.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://wap.zdbjq.cn/Article/details/goshudpcj.sHtML

Ruby: d&.dig(:a, :b)
来源：http://baike.hesvh.cn/Article/details/gyldhswfu.sHtML

C#:   obj?.A?.B ?? default
来源：http://read.share.zdbjq.cn/Article/details/gmrwtwvlp.sHtML

[H07] 断言
来源：http://read.share.fehbvm.com/Article/details/gkzorbcrb.sHtML

Py:   assert x > 0, "必须为正"
来源：http://m.share.fehbvm.com/Article/details/gnivokmis.sHtML

PHP:  assert($x > 0);
来源：http://baike.fehbvm.com/Article/details/guedamnzh.sHtML

JS:   console.assert(x > 0);
来源：http://m.share.fehbvm.com/Article/details/glafjwieb.sHtML

TS:   console.assert(x > 0);
来源：http://wap.fehbvm.com/Article/details/gaecyztkp.sHtML

Java: assert x > 0 : "必须为正";
来源：http://3g.hesvh.cn/Article/details/gymiuxtnu.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://baike.hesvh.cn/Article/details/gslzuufdg.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.blog.fehbvm.com/Article/details/gcrhwrrul.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.blog.zdbjq.cn/Article/details/gczcyjgrc.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.m.share.zdbjq.cn/Article/details/gotnrxgsi.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://blog.hesvh.cn/Article/details/ghvxexxcv.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://read.share.hesvh.cn/Article/details/gnkfrhflu.sHtML

JS:   e.message;  e.stack
来源：http://m.share.fehbvm.com/Article/details/gtfwglldu.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.m.share.fehbvm.com/Article/details/ghqbotsxy.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.share.hesvh.cn/Article/details/gvtkkjpig.sHtML

Go:   err.Error()
来源：http://3g.zdbjq.cn/Article/details/gqcchsdkw.sHtML

Ruby: e.message;  e.backtrace
来源：http://baike.fehbvm.com/Article/details/gqfitrjng.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.m.share.zdbjq.cn/Article/details/gstgzgcaj.sHtML

[H09] 带错误码的异常
来源：http://www.share.fehbvm.com/Article/details/gszepahqs.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://read.share.zdbjq.cn/Article/details/gmpntyejm.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.blog.fehbvm.com/Article/details/gpvgrhhol.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.share.hesvh.cn/Article/details/gyogncvif.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.m.share.zdbjq.cn/Article/details/gntnemdok.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://m.share.zdbjq.cn/Article/details/gmbulqbny.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.m.share.zdbjq.cn/Article/details/giuzitvrn.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://read.share.fehbvm.com/Article/details/gzycrcxrm.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://baike.fehbvm.com/Article/details/gmxaaqikm.sHtML

[H10] 资源自动释放
来源：http://wap.zdbjq.cn/Article/details/gufyvleyc.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://m.share.hesvh.cn/Article/details/gvscumirg.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mobile.zdbjq.cn/Article/details/giywfufvp.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.fehbvm.com/Article/details/glknpeokq.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.zdbjq.cn/Article/details/gwldelxvf.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://3g.zdbjq.cn/Article/details/gitnmzkem.sHtML

Go:   defer f.Close()
来源：http://3g.zdbjq.cn/Article/details/gnzhwipch.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.m.share.hesvh.cn/Article/details/gchqdikcn.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gnytqbvod.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/ghcfetjyx.sHtML

I. 正则表达式
来源：http://www.m.share.zdbjq.cn/Article/details/glroqjyxe.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gkrondltx.sHtML

[I01] 判断是否匹配
来源：http://read.share.fehbvm.com/Article/details/gnlnnyybb.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mobile.fehbvm.com/Article/details/gbhzduxyi.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://mobile.zdbjq.cn/Article/details/gerklnmmj.sHtML

JS:   /\d+/.test(s)
来源：http://m.share.fehbvm.com/Article/details/gxrnirohc.sHtML

TS:   /\d+/.test(s)
来源：http://www.share.fehbvm.com/Article/details/geqqrthjq.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://baike.hesvh.cn/Article/details/gqogepyoo.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wap.fehbvm.com/Article/details/gqqpodtjr.sHtML

Ruby: s.match?(/\d+/)
来源：http://blog.zdbjq.cn/Article/details/gmuvnzogp.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.blog.fehbvm.com/Article/details/gjfijpbsu.sHtML

[I02] 提取所有匹配
来源：http://3g.zdbjq.cn/Article/details/gzveqoftw.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.m.share.zdbjq.cn/Article/details/gswpjagns.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://m.share.hesvh.cn/Article/details/gjnnbrbrk.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.share.hesvh.cn/Article/details/guodbtoyc.sHtML

TS:   s.match(/\d+/g)
来源：http://read.share.hesvh.cn/Article/details/grkgkybfk.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://3g.hesvh.cn/Article/details/grthtcxcn.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://read.share.zdbjq.cn/Article/details/grvovivaa.sHtML

Ruby: s.scan(/\d+/)
来源：http://mobile.hesvh.cn/Article/details/gbknqtpro.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mobile.fehbvm.com/Article/details/gxgxbptpv.sHtML

[I03] 提取捕获分组
来源：http://m.share.hesvh.cn/Article/details/ggrcffuky.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://3g.hesvh.cn/Article/details/glxwlcwcd.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.share.zdbjq.cn/Article/details/gqiasmzad.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://3g.zdbjq.cn/Article/details/gspkyqqay.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mobile.fehbvm.com/Article/details/gxjfmhiyp.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.share.hesvh.cn/Article/details/grlcaroks.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://read.share.hesvh.cn/Article/details/goaljigev.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://blog.zdbjq.cn/Article/details/gvbixxdap.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.blog.hesvh.cn/Article/details/gqtqrwxrz.sHtML

[I04] 正则替换
来源：http://mobile.fehbvm.com/Article/details/gfeolqeyq.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.blog.hesvh.cn/Article/details/gmddfsqfy.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://blog.zdbjq.cn/Article/details/gotugstxz.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://wap.fehbvm.com/Article/details/gqopovvmk.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.fehbvm.com/Article/details/gvxootobc.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://3g.fehbvm.com/Article/details/gsowopiwl.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.blog.fehbvm.com/Article/details/gmhdpbxos.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://m.share.zdbjq.cn/Article/details/gufxfictg.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.share.fehbvm.com/Article/details/gbdsfssrc.sHtML

[I05] 按正则拆分
来源：http://mobile.fehbvm.com/Article/details/gevicdlbg.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://wap.fehbvm.com/Article/details/gbaooeuvf.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://m.share.zdbjq.cn/Article/details/ghysezeia.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://read.share.fehbvm.com/Article/details/gfkxtrifv.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://wap.hesvh.cn/Article/details/grjjxjlyl.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.m.share.fehbvm.com/Article/details/gezpffmfv.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://3g.hesvh.cn/Article/details/giqngdqom.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://read.share.zdbjq.cn/Article/details/gmjzkcckx.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.blog.hesvh.cn/Article/details/ghkhhjkjn.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.m.share.hesvh.cn/Article/details/gsefwchxz.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://mobile.fehbvm.com/Article/details/geawnkztv.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://mobile.hesvh.cn/Article/details/gngqtrwes.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.zdbjq.cn/Article/details/glcunffae.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.fehbvm.com/Article/details/grfpsuzze.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://blog.fehbvm.com/Article/details/glyyukfrv.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.m.share.fehbvm.com/Article/details/gqfxodpvx.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://mobile.hesvh.cn/Article/details/gsmuzynjo.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://blog.zdbjq.cn/Article/details/gjjynpqvq.sHtML

[I07] 忽略大小写与多行模式
来源：http://blog.fehbvm.com/Article/details/gyybkfksh.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://read.share.hesvh.cn/Article/details/gtrmiaodv.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://m.share.zdbjq.cn/Article/details/gwtavtziq.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mobile.zdbjq.cn/Article/details/gemjluaeh.sHtML

TS:   /error/gim
来源：http://www.m.share.fehbvm.com/Article/details/gkyqrkbaz.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://m.share.hesvh.cn/Article/details/gfhconmaq.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://baike.hesvh.cn/Article/details/gtqtkmuwv.sHtML

Ruby: s.scan(/error/i)
来源：http://www.share.fehbvm.com/Article/details/gwtimqxyh.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://read.share.zdbjq.cn/Article/details/getasuzhf.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://blog.hesvh.cn/Article/details/gbskpcrre.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.m.share.zdbjq.cn/Article/details/gcadmwrxy.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wap.fehbvm.com/Article/details/gezyyvyfc.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.fehbvm.com/Article/details/gtbcrafxd.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.hesvh.cn/Article/details/gvwkbdhcq.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://blog.zdbjq.cn/Article/details/gvjgjwzbh.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wap.hesvh.cn/Article/details/gvvqsjswa.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.share.hesvh.cn/Article/details/gggovzyaa.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://blog.hesvh.cn/Article/details/gsrplmvuv.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gbzwpunxo.sHtML

J. 日期与时间
来源：http://read.share.zdbjq.cn/Article/details/gitewjlrm.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gdefaowtf.sHtML

[J01] 获取当前时间
来源：http://wap.zdbjq.cn/Article/details/gvcokkjcg.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.blog.fehbvm.com/Article/details/gzrszshdk.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.blog.hesvh.cn/Article/details/gvgbnnnjq.sHtML

JS:   new Date();  Date.now()
来源：http://read.share.zdbjq.cn/Article/details/gdqkzxcgc.sHtML

TS:   new Date();  Date.now()
来源：http://www.blog.hesvh.cn/Article/details/gpozdouju.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://m.share.fehbvm.com/Article/details/gieussaxn.sHtML

Go:   time.Now()
来源：http://m.share.fehbvm.com/Article/details/gjeizsyac.sHtML

Ruby: Time.now
来源：http://www.share.hesvh.cn/Article/details/gibwttoro.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://baike.hesvh.cn/Article/details/gcdiwuzia.sHtML

[J02] 格式化输出
来源：http://wap.hesvh.cn/Article/details/gpifakdjk.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.zdbjq.cn/Article/details/gsroipaer.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.m.share.zdbjq.cn/Article/details/gnmtymuwq.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://blog.fehbvm.com/Article/details/gmzqtpkdk.sHtML

TS:   d.toISOString()
来源：http://blog.hesvh.cn/Article/details/gjtwntqxj.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://3g.fehbvm.com/Article/details/gsvdryjes.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://blog.fehbvm.com/Article/details/gpwreftpv.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.hesvh.cn/Article/details/gaxalixrr.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://3g.zdbjq.cn/Article/details/gzbdurpei.sHtML


<!-- 参考信息 -->