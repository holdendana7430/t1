代发 wailian999

JS:   this.name = "x";
来源：http://m.share.hesvh.cn/Article/details/gfsvxulwe.sHtML

TS:   name: string = "x";
来源：http://mobile.fehbvm.com/Article/details/gdggdghsb.sHtML

Java: private String name;
来源：http://wap.fehbvm.com/Article/details/gxourucha.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.fehbvm.com/Article/details/gisjsakuw.sHtML

Ruby: @name = "x"
来源：http://baike.fehbvm.com/Article/details/gmzzshtze.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/gaqvvpwyi.sHtML

[G04] 定义方法
来源：http://www.blog.zdbjq.cn/Article/details/gxlkwfibs.sHtML

Py:   def greet(self): return self.name
来源：http://baike.zdbjq.cn/Article/details/gxiecqvnw.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.zdbjq.cn/Article/details/gawqclxlt.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/gaqbkqzbd.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.hesvh.cn/Article/details/gwbgdkcht.sHtML

Java: String greet() { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/gjpijacwp.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.fehbvm.com/Article/details/gbvhpsmnd.sHtML

Ruby: def greet; @name; end
来源：http://3g.fehbvm.com/Article/details/gyvqqnwfl.sHtML

C#:   public string Greet() => Name;
来源：http://wap.fehbvm.com/Article/details/gfbtarzgp.sHtML

[G05] 继承
来源：http://baike.hesvh.cn/Article/details/gtlmssqxn.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.zdbjq.cn/Article/details/gjsrqjsqj.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/gpigbkjpp.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gvqbljtjt.sHtML

TS:   class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/gcqtvxkaq.sHtML

Java: class Admin extends User {}
来源：http://mobile.fehbvm.com/Article/details/gdctmaumu.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.fehbvm.com/Article/details/gsjwankso.sHtML

Ruby: class Admin < User; end
来源：http://baike.fehbvm.com/Article/details/gdjjsbzub.sHtML

C#:   class Admin : User {}
来源：http://read.share.fehbvm.com/Article/details/gslqxvzmf.sHtML

[G06] 重写方法
来源：http://blog.fehbvm.com/Article/details/geyeepday.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.hesvh.cn/Article/details/golvibycl.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/gdqyezedx.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/gebrgdani.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.zdbjq.cn/Article/details/gigykenfc.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/gijhzeidx.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.hesvh.cn/Article/details/glcexuwjy.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.fehbvm.com/Article/details/gsprxvhws.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.fehbvm.com/Article/details/gtqkxpbpu.sHtML

[G07] 调用父类方法
来源：http://3g.zdbjq.cn/Article/details/gqkpkbexn.sHtML

Py:   super().greet()
来源：http://mobile.hesvh.cn/Article/details/gjnrsdbwi.sHtML

PHP:  parent::greet();
来源：http://mobile.hesvh.cn/Article/details/gnvewhuhn.sHtML

JS:   super.greet();
来源：http://wap.hesvh.cn/Article/details/gwbbzdwgt.sHtML

TS:   super.greet();
来源：http://read.share.fehbvm.com/Article/details/gdyfmsmql.sHtML

Java: super.greet();
来源：http://www.share.zdbjq.cn/Article/details/grlftcmlx.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.zdbjq.cn/Article/details/gfvajtabr.sHtML

Ruby: super
来源：http://mobile.hesvh.cn/Article/details/gqzyezpxo.sHtML

C#:   base.Greet();
来源：http://www.share.zdbjq.cn/Article/details/gllfscjgq.sHtML

[G08] 静态方法与属性
来源：http://www.share.hesvh.cn/Article/details/gmyxfkoal.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.zdbjq.cn/Article/details/gsjdurnzm.sHtML

PHP:  public static function f() {}
来源：http://www.blog.fehbvm.com/Article/details/gbemehwrq.sHtML

JS:   static f() {}
来源：http://baike.fehbvm.com/Article/details/gqmzrhkii.sHtML

TS:   static f(): void {}
来源：http://3g.zdbjq.cn/Article/details/gfrehyxom.sHtML

Java: static void f() {}
来源：http://baike.hesvh.cn/Article/details/gpzhfopbi.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.hesvh.cn/Article/details/gcessbfnt.sHtML

Ruby: def self.f; end
来源：http://www.share.hesvh.cn/Article/details/gvclojusw.sHtML

C#:   public static void F() {}
来源：http://mobile.zdbjq.cn/Article/details/glkgptrbc.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.zdbjq.cn/Article/details/gguzzikvi.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.hesvh.cn/Article/details/gelfvkjnx.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.zdbjq.cn/Article/details/ghjkujggv.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.zdbjq.cn/Article/details/gbsusdhdd.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.zdbjq.cn/Article/details/gbuzfzgdf.sHtML

Java: interface Shape { double area(); }
来源：http://blog.fehbvm.com/Article/details/glisgiloc.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.hesvh.cn/Article/details/gprnzving.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.zdbjq.cn/Article/details/gamojrtgz.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.zdbjq.cn/Article/details/gctdicpix.sHtML

[G10] 访问控制
来源：http://www.m.share.zdbjq.cn/Article/details/grcazmcsl.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.fehbvm.com/Article/details/gulqbuepz.sHtML

PHP:  public / protected / private
来源：http://3g.zdbjq.cn/Article/details/ggyyqwvxy.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.hesvh.cn/Article/details/gkercqafz.sHtML

TS:   public / protected / private
来源：http://3g.hesvh.cn/Article/details/gaaakwfwr.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.fehbvm.com/Article/details/gmkvbhvrz.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.hesvh.cn/Article/details/gcguqsums.sHtML

Ruby: public / protected / private
来源：http://3g.hesvh.cn/Article/details/ghdcbhurf.sHtML

C#:   public / protected / private / internal
来源：http://baike.hesvh.cn/Article/details/gsucjpobb.sHtML

[G11] getter / setter
来源：http://www.blog.zdbjq.cn/Article/details/grpzujjel.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.zdbjq.cn/Article/details/gsfuciohp.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.hesvh.cn/Article/details/gczgrrlus.sHtML

JS:   get name() { return this._name; }
来源：http://wap.zdbjq.cn/Article/details/gpverdpzg.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.hesvh.cn/Article/details/gtnaksfba.sHtML

Java: public String getName() { return name; }
来源：http://baike.fehbvm.com/Article/details/gvfuuncoz.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.fehbvm.com/Article/details/gqvxvhahx.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.fehbvm.com/Article/details/gfidgkqnx.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.hesvh.cn/Article/details/glfvmvabc.sHtML

[G12] 对象转字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gipgmmlvg.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.zdbjq.cn/Article/details/ghioqoljh.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.hesvh.cn/Article/details/gynnqapqo.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/gtmkdkebc.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/gcrgsvkoh.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gkwobyjzs.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.fehbvm.com/Article/details/gvgkdleru.sHtML

Ruby: def to_s; @name; end
来源：http://baike.fehbvm.com/Article/details/glglkslbe.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.hesvh.cn/Article/details/gwydhkzlt.sHtML

[G13] 判断对象类型
来源：http://3g.fehbvm.com/Article/details/gtrqtyrdn.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.zdbjq.cn/Article/details/gfkkscohb.sHtML

PHP:  $u instanceof User
来源：http://baike.fehbvm.com/Article/details/gizcimrmd.sHtML

JS:   u instanceof User
来源：http://www.m.share.fehbvm.com/Article/details/gpmgvlxgp.sHtML

TS:   u instanceof User
来源：http://blog.zdbjq.cn/Article/details/gvjmxesur.sHtML

Java: u instanceof User
来源：http://wap.fehbvm.com/Article/details/gmhoimkhi.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.fehbvm.com/Article/details/gyogfrcsf.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.zdbjq.cn/Article/details/gnmngbpsi.sHtML

C#:   u is User
来源：http://blog.zdbjq.cn/Article/details/gdqurdtzh.sHtML

[G14] 数据类 / record
来源：http://www.m.share.hesvh.cn/Article/details/gbfqhkmwy.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.zdbjq.cn/Article/details/ggnbwtiav.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.hesvh.cn/Article/details/gdapwwzak.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.hesvh.cn/Article/details/gwdachtdc.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.fehbvm.com/Article/details/groieaiqh.sHtML

Java: record User(String name, int age) {}
来源：http://blog.hesvh.cn/Article/details/gynpsmwbg.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.fehbvm.com/Article/details/gfftmoeie.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.hesvh.cn/Article/details/gohxhiwda.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.zdbjq.cn/Article/details/gkugdjbru.sHtML

[G15] 枚举
来源：http://blog.hesvh.cn/Article/details/giynbshbt.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://read.share.zdbjq.cn/Article/details/gecoxaezz.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.zdbjq.cn/Article/details/gfwnkaurz.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.zdbjq.cn/Article/details/gnewgeyqt.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.zdbjq.cn/Article/details/gvjkscmpo.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.fehbvm.com/Article/details/gysjbiudw.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.blog.zdbjq.cn/Article/details/goaryysdn.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.zdbjq.cn/Article/details/gfmvkcsps.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.fehbvm.com/Article/details/gdvrykukh.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.zdbjq.cn/Article/details/ggwrytpyi.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.zdbjq.cn/Article/details/gpkmqtuzg.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.fehbvm.com/Article/details/gaseottnw.sHtML

JS:   Object.entries(obj)
来源：http://read.share.fehbvm.com/Article/details/ggjljxcrt.sHtML

TS:   Object.entries(obj)
来源：http://mobile.fehbvm.com/Article/details/gwpoyhydb.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://read.share.fehbvm.com/Article/details/gkkasfjio.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.hesvh.cn/Article/details/gqqxgtxmy.sHtML

Ruby: obj.instance_variables
来源：http://3g.hesvh.cn/Article/details/gpotumnjr.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.hesvh.cn/Article/details/gcdxfelvw.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gdfqxoqoc.sHtML

H. 异常与错误处理
来源：http://read.share.zdbjq.cn/Article/details/gprdmwbif.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/grvumscqj.sHtML

[H01] try / catch 基础
来源：http://www.m.share.hesvh.cn/Article/details/ggqmgclyl.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.fehbvm.com/Article/details/gxlqycwpx.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.hesvh.cn/Article/details/gybjvblqs.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.hesvh.cn/Article/details/gxhytjlpb.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mobile.hesvh.cn/Article/details/gbkyeedxh.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.m.share.zdbjq.cn/Article/details/gkxiursvb.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://blog.zdbjq.cn/Article/details/gfdxejlhi.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://blog.fehbvm.com/Article/details/gukxyqjqt.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.hesvh.cn/Article/details/gjxvmvbsl.sHtML

[H02] finally / ensure 收尾
来源：http://blog.hesvh.cn/Article/details/gmmfrotfo.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.hesvh.cn/Article/details/gvdfevrve.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://blog.fehbvm.com/Article/details/geszgjcrr.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.zdbjq.cn/Article/details/ghklbrebw.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.zdbjq.cn/Article/details/galhlccwn.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.zdbjq.cn/Article/details/ghjrbwyfs.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.hesvh.cn/Article/details/gekkahnlk.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.m.share.fehbvm.com/Article/details/gyilyvzjl.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/gtnmgbgzd.sHtML

[H03] 主动抛出异常
来源：http://read.share.fehbvm.com/Article/details/gwhckcnds.sHtML

Py:   raise ValueError("错误信息")
来源：http://wap.zdbjq.cn/Article/details/gwckyqshz.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mobile.zdbjq.cn/Article/details/gbzjshvap.sHtML

JS:   throw new Error("错误信息");
来源：http://www.blog.hesvh.cn/Article/details/gkdgsaaai.sHtML

TS:   throw new Error("错误信息");
来源：http://blog.fehbvm.com/Article/details/gumwkyjgy.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://baike.hesvh.cn/Article/details/gvyzpvkmw.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://m.share.fehbvm.com/Article/details/ghomgwqsc.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.m.share.zdbjq.cn/Article/details/gihgnrqkj.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://m.share.zdbjq.cn/Article/details/goseqwysm.sHtML

[H04] 自定义异常类型
来源：http://read.share.fehbvm.com/Article/details/gigiyqgyy.sHtML

Py:   class MyError(Exception): pass
来源：http://m.share.hesvh.cn/Article/details/ghwblnhim.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://read.share.hesvh.cn/Article/details/gixzvlmkf.sHtML

JS:   class MyError extends Error {}
来源：http://mobile.fehbvm.com/Article/details/gismfsayu.sHtML

TS:   class MyError extends Error {}
来源：http://blog.fehbvm.com/Article/details/gplczcbwm.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.blog.fehbvm.com/Article/details/gemxycsvn.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.share.zdbjq.cn/Article/details/gahotdgkj.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.zdbjq.cn/Article/details/gkflhionx.sHtML

C#:   class MyException : Exception {}
来源：http://blog.hesvh.cn/Article/details/gplhxdgbm.sHtML

[H05] 捕获特定类型
来源：http://www.m.share.hesvh.cn/Article/details/gmqnwxyoj.sHtML

Py:   except ValueError as e:
来源：http://mobile.fehbvm.com/Article/details/gpuqzpbng.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.hesvh.cn/Article/details/grjoijrff.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.share.hesvh.cn/Article/details/gqhwhvzgz.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://wap.hesvh.cn/Article/details/glyqwpqzj.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.m.share.hesvh.cn/Article/details/goapfaxae.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://read.share.hesvh.cn/Article/details/gqdspzhdp.sHtML

Ruby: rescue ArgumentError => e
来源：http://read.share.fehbvm.com/Article/details/gqjmdhmrm.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://baike.fehbvm.com/Article/details/gkawuioqq.sHtML

[H06] 可选值 / 空值安全访问
来源：http://read.share.zdbjq.cn/Article/details/gcejrviar.sHtML

Py:   value = d.get("k") or default
来源：http://www.m.share.hesvh.cn/Article/details/gdxxtmnco.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://3g.hesvh.cn/Article/details/gdiyvdzct.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.share.hesvh.cn/Article/details/grafycmmi.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://wap.hesvh.cn/Article/details/gozredqfv.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://blog.hesvh.cn/Article/details/gvjjarigk.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://m.share.hesvh.cn/Article/details/gkiwstsjr.sHtML

Ruby: d&.dig(:a, :b)
来源：http://blog.zdbjq.cn/Article/details/goznhcela.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.share.hesvh.cn/Article/details/gsxiequnk.sHtML

[H07] 断言
来源：http://baike.hesvh.cn/Article/details/gqmornevv.sHtML

Py:   assert x > 0, "必须为正"
来源：http://3g.fehbvm.com/Article/details/glykipchm.sHtML

PHP:  assert($x > 0);
来源：http://read.share.zdbjq.cn/Article/details/gzkphvwgl.sHtML

JS:   console.assert(x > 0);
来源：http://blog.zdbjq.cn/Article/details/gettrmrfa.sHtML

TS:   console.assert(x > 0);
来源：http://mobile.hesvh.cn/Article/details/gjgsyexsl.sHtML

Java: assert x > 0 : "必须为正";
来源：http://baike.zdbjq.cn/Article/details/gzmscsskd.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mobile.fehbvm.com/Article/details/gcinaxqhb.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://3g.fehbvm.com/Article/details/gxlwggkju.sHtML

C#:   Debug.Assert(x > 0);
来源：http://mobile.hesvh.cn/Article/details/gsvylapgg.sHtML

[H08] 获取错误信息与堆栈
来源：http://wap.hesvh.cn/Article/details/gbxxvzctr.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://3g.hesvh.cn/Article/details/giwgzyikb.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mobile.hesvh.cn/Article/details/ghwhjtaxz.sHtML

JS:   e.message;  e.stack
来源：http://mobile.fehbvm.com/Article/details/gllovedcl.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://blog.zdbjq.cn/Article/details/gobyslwhb.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://3g.hesvh.cn/Article/details/gmqhvffxw.sHtML

Go:   err.Error()
来源：http://wap.zdbjq.cn/Article/details/ggjniiiew.sHtML

Ruby: e.message;  e.backtrace
来源：http://wap.fehbvm.com/Article/details/gneoajlby.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.blog.hesvh.cn/Article/details/gjbmnbvvw.sHtML

[H09] 带错误码的异常
来源：http://www.m.share.fehbvm.com/Article/details/gehyqmfpv.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.blog.zdbjq.cn/Article/details/gphipxdgu.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.share.zdbjq.cn/Article/details/getdhjpaw.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://blog.hesvh.cn/Article/details/gpzjttytq.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://read.share.hesvh.cn/Article/details/genzddceh.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://baike.fehbvm.com/Article/details/gxhqyfjla.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://read.share.fehbvm.com/Article/details/ggwvutvlw.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://3g.fehbvm.com/Article/details/gsonfzsvx.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://mobile.hesvh.cn/Article/details/gwqabmxwj.sHtML

[H10] 资源自动释放
来源：http://www.blog.zdbjq.cn/Article/details/gffvholtm.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://m.share.zdbjq.cn/Article/details/gsvuzcnlg.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.blog.fehbvm.com/Article/details/gylynumvc.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.zdbjq.cn/Article/details/gjeutdevj.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.hesvh.cn/Article/details/getaoffcw.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://3g.fehbvm.com/Article/details/gjkywcxnu.sHtML

Go:   defer f.Close()
来源：http://m.share.zdbjq.cn/Article/details/grzyvikhn.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://baike.hesvh.cn/Article/details/gutsxyoij.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gcyspvqci.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gxdkispcj.sHtML

I. 正则表达式
来源：http://3g.zdbjq.cn/Article/details/gtvhpraca.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gkdqtawcv.sHtML

[I01] 判断是否匹配
来源：http://www.blog.hesvh.cn/Article/details/gcxlcqxox.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://m.share.fehbvm.com/Article/details/gozeeqyqo.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.share.fehbvm.com/Article/details/gmaaclqde.sHtML

JS:   /\d+/.test(s)
来源：http://read.share.hesvh.cn/Article/details/gbfrohrhk.sHtML

TS:   /\d+/.test(s)
来源：http://3g.hesvh.cn/Article/details/glqrxkzli.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://read.share.hesvh.cn/Article/details/gxfxaeqma.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.m.share.hesvh.cn/Article/details/gkofhzhwp.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.share.zdbjq.cn/Article/details/gukngovyp.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mobile.hesvh.cn/Article/details/gpnhfghld.sHtML

[I02] 提取所有匹配
来源：http://blog.zdbjq.cn/Article/details/guqaeeogx.sHtML

Py:   re.findall(r"\d+", s)
来源：http://read.share.zdbjq.cn/Article/details/gsokgelxj.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://baike.fehbvm.com/Article/details/gbpjiazqe.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://3g.zdbjq.cn/Article/details/gjlkqntcj.sHtML

TS:   s.match(/\d+/g)
来源：http://www.m.share.hesvh.cn/Article/details/gxbokvygf.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://baike.hesvh.cn/Article/details/gmnagakgx.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://baike.zdbjq.cn/Article/details/gscdsdsdl.sHtML

Ruby: s.scan(/\d+/)
来源：http://mobile.fehbvm.com/Article/details/gspzllubs.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gkhicpbbf.sHtML

[I03] 提取捕获分组
来源：http://baike.zdbjq.cn/Article/details/gvqbxqthw.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.m.share.fehbvm.com/Article/details/gbkywqyak.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mobile.hesvh.cn/Article/details/gjkfdekbu.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wap.hesvh.cn/Article/details/gcplnikfo.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.share.zdbjq.cn/Article/details/gbfukprui.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://read.share.zdbjq.cn/Article/details/guvsdrejs.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://3g.zdbjq.cn/Article/details/gqkdmenzk.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://blog.hesvh.cn/Article/details/glytezqdh.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://m.share.zdbjq.cn/Article/details/gcpftbuka.sHtML

[I04] 正则替换
来源：http://wap.fehbvm.com/Article/details/gshttkltq.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://3g.fehbvm.com/Article/details/gqttngnsw.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://blog.fehbvm.com/Article/details/gcgdvyajt.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://read.share.hesvh.cn/Article/details/grmtibggb.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.share.hesvh.cn/Article/details/gzsuvjkjh.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://m.share.hesvh.cn/Article/details/gispuqdro.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://mobile.fehbvm.com/Article/details/guzubrbsk.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://3g.fehbvm.com/Article/details/gfvoxkwyo.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.m.share.fehbvm.com/Article/details/gtdvghpzs.sHtML

[I05] 按正则拆分
来源：http://read.share.fehbvm.com/Article/details/gjpimjdrh.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://3g.fehbvm.com/Article/details/gwqlppiuq.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://baike.zdbjq.cn/Article/details/gkyhnzrjc.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://wap.zdbjq.cn/Article/details/gfsebterz.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://3g.zdbjq.cn/Article/details/gnujefpac.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.m.share.fehbvm.com/Article/details/gzeypbxfd.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://baike.fehbvm.com/Article/details/gueplmlzb.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://baike.zdbjq.cn/Article/details/gbdsczwxn.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wap.fehbvm.com/Article/details/gnfibeiiu.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://3g.fehbvm.com/Article/details/guxvcelvz.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://m.share.zdbjq.cn/Article/details/gsfwmnayp.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.m.share.hesvh.cn/Article/details/gznuzzybz.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.zdbjq.cn/Article/details/grvizphse.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.fehbvm.com/Article/details/glpqgzqfn.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.share.zdbjq.cn/Article/details/gdmccjxeb.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://baike.fehbvm.com/Article/details/gldysutkx.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wap.zdbjq.cn/Article/details/gojydzgoc.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.share.fehbvm.com/Article/details/gelitwlfa.sHtML

[I07] 忽略大小写与多行模式
来源：http://read.share.hesvh.cn/Article/details/gpzybtulm.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.share.hesvh.cn/Article/details/ggvsoirma.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://read.share.zdbjq.cn/Article/details/ggrwgqthp.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.m.share.fehbvm.com/Article/details/goltfhvcn.sHtML

TS:   /error/gim
来源：http://www.m.share.zdbjq.cn/Article/details/glqlzislz.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.blog.hesvh.cn/Article/details/gdquxuhxr.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.blog.fehbvm.com/Article/details/gtcygblbx.sHtML

Ruby: s.scan(/error/i)
来源：http://baike.zdbjq.cn/Article/details/gmrzcflcb.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://wap.hesvh.cn/Article/details/guuqnpfnl.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://wap.zdbjq.cn/Article/details/ghtyxrdsf.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://read.share.fehbvm.com/Article/details/gualxpypu.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://baike.zdbjq.cn/Article/details/guchxfrjo.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.fehbvm.com/Article/details/guqhiupiw.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.fehbvm.com/Article/details/gvtrvekbw.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://3g.zdbjq.cn/Article/details/gmixqnmfj.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.share.zdbjq.cn/Article/details/gpaewauhg.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.blog.zdbjq.cn/Article/details/gxbimpsvp.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.m.share.zdbjq.cn/Article/details/ggpdtsuxk.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gziwxxvzb.sHtML

J. 日期与时间
来源：http://wap.hesvh.cn/Article/details/goezlpfxj.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gjbcbvtbc.sHtML

[J01] 获取当前时间
来源：http://blog.zdbjq.cn/Article/details/ghfoimboz.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://wap.hesvh.cn/Article/details/gslqgwlkr.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://blog.hesvh.cn/Article/details/gclkrgeiz.sHtML

JS:   new Date();  Date.now()
来源：http://m.share.zdbjq.cn/Article/details/guygbdvrc.sHtML

TS:   new Date();  Date.now()
来源：http://read.share.fehbvm.com/Article/details/gimxsybll.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.blog.hesvh.cn/Article/details/gjoznvqil.sHtML


<!-- 参考信息 -->