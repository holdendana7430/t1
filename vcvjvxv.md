代发 wailian999

C#:   public User(string name) { Name = name; }
来源：http://3g.fehbvm.com/Article/details/gdeipsfql.sHtML

[G03] 实例属性
来源：http://m.share.zdbjq.cn/Article/details/gxcuraryd.sHtML

Py:   self.name = "x"
来源：http://wap.fehbvm.com/Article/details/gawdocfmh.sHtML

PHP:  public string $name = "x";
来源：http://www.share.hesvh.cn/Article/details/gfwprzwke.sHtML

JS:   this.name = "x";
来源：http://mobile.fehbvm.com/Article/details/gstlztewz.sHtML

TS:   name: string = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/gqzwwhkez.sHtML

Java: private String name;
来源：http://wap.hesvh.cn/Article/details/gmblmfjxp.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.hesvh.cn/Article/details/ggamwstyn.sHtML

Ruby: @name = "x"
来源：http://blog.zdbjq.cn/Article/details/gpgcqtkmf.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.zdbjq.cn/Article/details/geppgyxxn.sHtML

[G04] 定义方法
来源：http://www.m.share.fehbvm.com/Article/details/gtzqkmpkz.sHtML

Py:   def greet(self): return self.name
来源：http://3g.hesvh.cn/Article/details/gyyfwtvjf.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.hesvh.cn/Article/details/gkpcgbzno.sHtML

JS:   greet() { return this.name; }
来源：http://blog.fehbvm.com/Article/details/gjjhqydic.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.fehbvm.com/Article/details/gkscnlexc.sHtML

Java: String greet() { return name; }
来源：http://www.blog.hesvh.cn/Article/details/gmwpleysw.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.hesvh.cn/Article/details/gwtkhjzth.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.zdbjq.cn/Article/details/gmcgoowsa.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.fehbvm.com/Article/details/goyqgubce.sHtML

[G05] 继承
来源：http://3g.zdbjq.cn/Article/details/gtbqqchnk.sHtML

Py:   class Admin(User): pass
来源：http://3g.fehbvm.com/Article/details/gntswzsic.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/gwfrzkmwk.sHtML

JS:   class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/gkoxoxsbt.sHtML

TS:   class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/gamyvbhnc.sHtML

Java: class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/gnjcmgeuy.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.zdbjq.cn/Article/details/gzwpqcrnd.sHtML

Ruby: class Admin < User; end
来源：http://baike.zdbjq.cn/Article/details/gxlvkywbm.sHtML

C#:   class Admin : User {}
来源：http://www.share.zdbjq.cn/Article/details/gqhonjgtr.sHtML

[G06] 重写方法
来源：http://3g.zdbjq.cn/Article/details/gjsdgzrlw.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.fehbvm.com/Article/details/glpajrhfw.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/gstlwdlqe.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/goesxdnal.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/geijnspfw.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/gkvbgcekb.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.zdbjq.cn/Article/details/gxpojpprz.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.hesvh.cn/Article/details/gwrdeeofs.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.zdbjq.cn/Article/details/gncorzpfx.sHtML

[G07] 调用父类方法
来源：http://blog.fehbvm.com/Article/details/gjyfnceeg.sHtML

Py:   super().greet()
来源：http://www.blog.fehbvm.com/Article/details/gyplrjmlh.sHtML

PHP:  parent::greet();
来源：http://www.blog.hesvh.cn/Article/details/gtpipxihs.sHtML

JS:   super.greet();
来源：http://blog.fehbvm.com/Article/details/gqbryaotx.sHtML

TS:   super.greet();
来源：http://www.blog.hesvh.cn/Article/details/geneqgcim.sHtML

Java: super.greet();
来源：http://blog.hesvh.cn/Article/details/ggagouudh.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.zdbjq.cn/Article/details/gtftpnetn.sHtML

Ruby: super
来源：http://blog.hesvh.cn/Article/details/glzqdraqh.sHtML

C#:   base.Greet();
来源：http://baike.hesvh.cn/Article/details/ghavivxwm.sHtML

[G08] 静态方法与属性
来源：http://baike.zdbjq.cn/Article/details/gxlgnvewu.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.zdbjq.cn/Article/details/ghvkypoxg.sHtML

PHP:  public static function f() {}
来源：http://m.share.zdbjq.cn/Article/details/gyefplmey.sHtML

JS:   static f() {}
来源：http://m.share.fehbvm.com/Article/details/gwhmnqzgu.sHtML

TS:   static f(): void {}
来源：http://baike.zdbjq.cn/Article/details/gksjxbtwn.sHtML

Java: static void f() {}
来源：http://wap.zdbjq.cn/Article/details/ggidwnglz.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.fehbvm.com/Article/details/gvxuwthte.sHtML

Ruby: def self.f; end
来源：http://m.share.hesvh.cn/Article/details/gdghnxygr.sHtML

C#:   public static void F() {}
来源：http://read.share.zdbjq.cn/Article/details/gpsijybew.sHtML

[G09] 接口 / 抽象类
来源：http://wap.hesvh.cn/Article/details/gamkgptpl.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.hesvh.cn/Article/details/ggoxmalwt.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.hesvh.cn/Article/details/gqkasjlrj.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.hesvh.cn/Article/details/gslzgbmuw.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.zdbjq.cn/Article/details/gbylzyubr.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.fehbvm.com/Article/details/ghwosrasv.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.fehbvm.com/Article/details/gddfawnwd.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.zdbjq.cn/Article/details/gsyprgqce.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gzxoymvcf.sHtML

[G10] 访问控制
来源：http://mobile.hesvh.cn/Article/details/gjmhjgykl.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.fehbvm.com/Article/details/gkiwqlemz.sHtML

PHP:  public / protected / private
来源：http://www.share.zdbjq.cn/Article/details/gsunrdkvq.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.hesvh.cn/Article/details/gniaqtorz.sHtML

TS:   public / protected / private
来源：http://blog.fehbvm.com/Article/details/gjjzcbfyc.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.zdbjq.cn/Article/details/gzziwbjnx.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.zdbjq.cn/Article/details/grxoriyra.sHtML

Ruby: public / protected / private
来源：http://wap.zdbjq.cn/Article/details/gahtriegl.sHtML

C#:   public / protected / private / internal
来源：http://baike.hesvh.cn/Article/details/ggplxmhvr.sHtML

[G11] getter / setter
来源：http://www.m.share.fehbvm.com/Article/details/grpalamrz.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.hesvh.cn/Article/details/gkhkjqvwc.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.fehbvm.com/Article/details/gbzlumxal.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.zdbjq.cn/Article/details/gjeytvkde.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.fehbvm.com/Article/details/gpuwojnok.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.hesvh.cn/Article/details/gjsuoeleq.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.hesvh.cn/Article/details/ggxckoqll.sHtML

Ruby: attr_accessor :name
来源：http://www.share.zdbjq.cn/Article/details/gdkmrsmxi.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.zdbjq.cn/Article/details/grggqkmuv.sHtML

[G12] 对象转字符串
来源：http://mobile.fehbvm.com/Article/details/gzpegixwr.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.hesvh.cn/Article/details/gexrxvypd.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.fehbvm.com/Article/details/gzqfnpujt.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gliaydadp.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.hesvh.cn/Article/details/gxqjhtjwr.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.zdbjq.cn/Article/details/gbchzdcju.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.fehbvm.com/Article/details/gwfgjhxyp.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.fehbvm.com/Article/details/gaxzetkza.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.zdbjq.cn/Article/details/gsdturgac.sHtML

[G13] 判断对象类型
来源：http://www.m.share.hesvh.cn/Article/details/gxxkptocv.sHtML

Py:   isinstance(u, User)
来源：http://m.share.fehbvm.com/Article/details/gnifkkryo.sHtML

PHP:  $u instanceof User
来源：http://wap.hesvh.cn/Article/details/gxvsnidns.sHtML

JS:   u instanceof User
来源：http://blog.hesvh.cn/Article/details/gsdgeyqsv.sHtML

TS:   u instanceof User
来源：http://blog.hesvh.cn/Article/details/ghfyhovrp.sHtML

Java: u instanceof User
来源：http://wap.fehbvm.com/Article/details/gtuunniby.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.share.fehbvm.com/Article/details/ghmxqtvax.sHtML

Ruby: u.is_a?(User)
来源：http://baike.fehbvm.com/Article/details/grpzmirsy.sHtML

C#:   u is User
来源：http://m.share.hesvh.cn/Article/details/gjmukmpeh.sHtML

[G14] 数据类 / record
来源：http://m.share.zdbjq.cn/Article/details/ghscgjbth.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://3g.hesvh.cn/Article/details/gfsfqkzpk.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.hesvh.cn/Article/details/gtqviyxtb.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.zdbjq.cn/Article/details/gyrspillk.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.hesvh.cn/Article/details/geqaydbdm.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.fehbvm.com/Article/details/gboxinetc.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.zdbjq.cn/Article/details/gsycipppn.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.hesvh.cn/Article/details/gtteylptc.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.hesvh.cn/Article/details/goftgghrm.sHtML

[G15] 枚举
来源：http://mobile.hesvh.cn/Article/details/gkwviggab.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://read.share.fehbvm.com/Article/details/ggyvevzgr.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.m.share.fehbvm.com/Article/details/gdydsbqja.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://read.share.hesvh.cn/Article/details/gjvgwntys.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.hesvh.cn/Article/details/gadpyycpe.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.zdbjq.cn/Article/details/gujygzuvq.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://baike.zdbjq.cn/Article/details/gkpygbjxj.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.zdbjq.cn/Article/details/gvtywkwmx.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.zdbjq.cn/Article/details/gsoehhduj.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.fehbvm.com/Article/details/gwdcslumm.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.zdbjq.cn/Article/details/gccrystpg.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.fehbvm.com/Article/details/gyslhtilp.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.hesvh.cn/Article/details/gegraszsw.sHtML

TS:   Object.entries(obj)
来源：http://3g.fehbvm.com/Article/details/ghyabyvln.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://m.share.fehbvm.com/Article/details/gcaxyaitn.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://wap.zdbjq.cn/Article/details/gujbcstaj.sHtML

Ruby: obj.instance_variables
来源：http://3g.fehbvm.com/Article/details/gkaankqxn.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.zdbjq.cn/Article/details/gpqugfhey.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gdjwneejm.sHtML

H. 异常与错误处理
来源：http://www.share.zdbjq.cn/Article/details/gaxmkdeng.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/glckhimyw.sHtML

[H01] try / catch 基础
来源：http://www.blog.fehbvm.com/Article/details/gqlgerbni.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.zdbjq.cn/Article/details/gmoikrong.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.blog.zdbjq.cn/Article/details/gsueeupce.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.share.zdbjq.cn/Article/details/gbezvqdip.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.zdbjq.cn/Article/details/gfelqeknd.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.share.hesvh.cn/Article/details/gzynjhgxq.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.zdbjq.cn/Article/details/grpeeihhh.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.hesvh.cn/Article/details/gldrfjxmr.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.hesvh.cn/Article/details/gnjihrbjn.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.hesvh.cn/Article/details/gnfqqjhxp.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.fehbvm.com/Article/details/gyixuvynw.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/gqlfucuks.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.fehbvm.com/Article/details/gwliqajfu.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.fehbvm.com/Article/details/ggfabtild.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.fehbvm.com/Article/details/gwdykoiez.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.hesvh.cn/Article/details/gjiqnurck.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.zdbjq.cn/Article/details/gfrtibpvr.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://mobile.zdbjq.cn/Article/details/glqtxxdxm.sHtML

[H03] 主动抛出异常
来源：http://www.share.zdbjq.cn/Article/details/gowyxlbnf.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.hesvh.cn/Article/details/gtkqyrmvv.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://baike.zdbjq.cn/Article/details/gfmcwtvgm.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.zdbjq.cn/Article/details/gqgfvgarr.sHtML

TS:   throw new Error("错误信息");
来源：http://read.share.fehbvm.com/Article/details/gtkrdafer.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.zdbjq.cn/Article/details/gimeftyak.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wap.fehbvm.com/Article/details/grvjfcgci.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://m.share.hesvh.cn/Article/details/gbndijmrj.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://m.share.fehbvm.com/Article/details/gpblbutfp.sHtML

[H04] 自定义异常类型
来源：http://mobile.fehbvm.com/Article/details/grcuwpryj.sHtML

Py:   class MyError(Exception): pass
来源：http://blog.fehbvm.com/Article/details/gagywkymr.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://baike.hesvh.cn/Article/details/ghekecrir.sHtML

JS:   class MyError extends Error {}
来源：http://baike.zdbjq.cn/Article/details/gtmhnvpol.sHtML

TS:   class MyError extends Error {}
来源：http://m.share.zdbjq.cn/Article/details/gtciaogmv.sHtML

Java: class MyException extends RuntimeException {}
来源：http://mobile.hesvh.cn/Article/details/gzcpgeudc.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.fehbvm.com/Article/details/gstaqqvmx.sHtML

Ruby: class MyError < StandardError; end
来源：http://mobile.fehbvm.com/Article/details/gqfqqtgyt.sHtML

C#:   class MyException : Exception {}
来源：http://baike.zdbjq.cn/Article/details/guwzvrnlp.sHtML

[H05] 捕获特定类型
来源：http://wap.hesvh.cn/Article/details/gqvwfcebg.sHtML

Py:   except ValueError as e:
来源：http://mobile.fehbvm.com/Article/details/gcgjltdch.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.blog.zdbjq.cn/Article/details/gjssolddd.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.share.zdbjq.cn/Article/details/gmyscyzua.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.blog.zdbjq.cn/Article/details/gnfrmucol.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://mobile.fehbvm.com/Article/details/gdmiibbup.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wap.fehbvm.com/Article/details/goxgdtbmq.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.zdbjq.cn/Article/details/gtqmeizgz.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://blog.fehbvm.com/Article/details/gxsowljai.sHtML

[H06] 可选值 / 空值安全访问
来源：http://wap.fehbvm.com/Article/details/gnlmtfgtl.sHtML

Py:   value = d.get("k") or default
来源：http://www.share.hesvh.cn/Article/details/gkdqvfand.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.share.hesvh.cn/Article/details/gunndytgr.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.zdbjq.cn/Article/details/gckmvkhvb.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.fehbvm.com/Article/details/ghkdysmql.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wap.zdbjq.cn/Article/details/gwzivokqf.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://read.share.hesvh.cn/Article/details/glnwaxjzc.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.blog.fehbvm.com/Article/details/gotejmcup.sHtML

C#:   obj?.A?.B ?? default
来源：http://m.share.fehbvm.com/Article/details/gcjhpvika.sHtML

[H07] 断言
来源：http://wap.hesvh.cn/Article/details/glqgszwke.sHtML

Py:   assert x > 0, "必须为正"
来源：http://mobile.fehbvm.com/Article/details/gvdngziqo.sHtML

PHP:  assert($x > 0);
来源：http://baike.hesvh.cn/Article/details/glyfnfqfc.sHtML

JS:   console.assert(x > 0);
来源：http://baike.zdbjq.cn/Article/details/gsvvifdpw.sHtML

TS:   console.assert(x > 0);
来源：http://www.share.hesvh.cn/Article/details/gjpacffyi.sHtML

Java: assert x > 0 : "必须为正";
来源：http://mobile.zdbjq.cn/Article/details/ghzxlddaj.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://read.share.zdbjq.cn/Article/details/gkcyumnrl.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://3g.fehbvm.com/Article/details/gthxzcatf.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.blog.zdbjq.cn/Article/details/gmjmkrdyz.sHtML

[H08] 获取错误信息与堆栈
来源：http://3g.hesvh.cn/Article/details/gvyxacvxe.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://mobile.fehbvm.com/Article/details/gbiqdgprp.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.m.share.fehbvm.com/Article/details/gzskexgzg.sHtML

JS:   e.message;  e.stack
来源：http://wap.hesvh.cn/Article/details/gdtcrqysh.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://read.share.hesvh.cn/Article/details/gsehjihuy.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://m.share.hesvh.cn/Article/details/glrhwcygv.sHtML

Go:   err.Error()
来源：http://baike.zdbjq.cn/Article/details/gmnleyucd.sHtML

Ruby: e.message;  e.backtrace
来源：http://m.share.hesvh.cn/Article/details/gdyttthjn.sHtML

C#:   e.Message;  e.StackTrace
来源：http://wap.hesvh.cn/Article/details/gqkxvpwdy.sHtML

[H09] 带错误码的异常
来源：http://www.blog.zdbjq.cn/Article/details/gwzzslrtn.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://baike.fehbvm.com/Article/details/gtyskboju.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://read.share.hesvh.cn/Article/details/goiovnadu.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://m.share.zdbjq.cn/Article/details/glncjibpy.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.share.hesvh.cn/Article/details/gzowxbrdm.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mobile.zdbjq.cn/Article/details/gnyjjvuad.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://3g.zdbjq.cn/Article/details/gqpwhutfz.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://wap.hesvh.cn/Article/details/gxpcyibsr.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://read.share.hesvh.cn/Article/details/gqkxeoowu.sHtML

[H10] 资源自动释放
来源：http://www.blog.hesvh.cn/Article/details/gdzsgxtqb.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://read.share.hesvh.cn/Article/details/gwznwixtu.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.share.zdbjq.cn/Article/details/gcqyhpidu.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.zdbjq.cn/Article/details/gutwwsbca.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.hesvh.cn/Article/details/genvczmwp.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.m.share.fehbvm.com/Article/details/guuoeowkx.sHtML

Go:   defer f.Close()
来源：http://baike.zdbjq.cn/Article/details/gaciexrpd.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.blog.hesvh.cn/Article/details/gtuveonqb.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gufniszfh.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gvldgjhmn.sHtML

I. 正则表达式
来源：http://www.m.share.hesvh.cn/Article/details/gprzhlhxp.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gqwqrmrka.sHtML

[I01] 判断是否匹配
来源：http://read.share.fehbvm.com/Article/details/gvyywqwxq.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://3g.fehbvm.com/Article/details/grynzoifs.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://m.share.hesvh.cn/Article/details/gqsnzysul.sHtML

JS:   /\d+/.test(s)
来源：http://baike.hesvh.cn/Article/details/gkvldtzdl.sHtML

TS:   /\d+/.test(s)
来源：http://read.share.hesvh.cn/Article/details/ghtwoneoz.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.share.hesvh.cn/Article/details/gmcffzmgy.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://3g.fehbvm.com/Article/details/gcphquloj.sHtML

Ruby: s.match?(/\d+/)
来源：http://wap.hesvh.cn/Article/details/gigxgwmbf.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://baike.hesvh.cn/Article/details/gjfbejioe.sHtML

[I02] 提取所有匹配
来源：http://baike.fehbvm.com/Article/details/gldxxbelp.sHtML

Py:   re.findall(r"\d+", s)
来源：http://m.share.fehbvm.com/Article/details/ggromysfo.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://baike.zdbjq.cn/Article/details/gdbiuqxky.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://read.share.fehbvm.com/Article/details/gqdfwjjaj.sHtML

TS:   s.match(/\d+/g)
来源：http://www.m.share.fehbvm.com/Article/details/gbaclwqwx.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://read.share.hesvh.cn/Article/details/gmeqecmsk.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://m.share.zdbjq.cn/Article/details/gczkkxxgp.sHtML

Ruby: s.scan(/\d+/)
来源：http://m.share.fehbvm.com/Article/details/gklsvmozo.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/guuhjxwrp.sHtML

[I03] 提取捕获分组
来源：http://baike.zdbjq.cn/Article/details/gukrypqks.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wap.fehbvm.com/Article/details/gczxdcxwe.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.m.share.fehbvm.com/Article/details/gggfgwfut.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.blog.zdbjq.cn/Article/details/ghxuyvsxx.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.share.fehbvm.com/Article/details/gpihvtlob.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.share.hesvh.cn/Article/details/goukmxppo.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wap.zdbjq.cn/Article/details/gecfcxida.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://m.share.zdbjq.cn/Article/details/gqlbjjfmg.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://3g.zdbjq.cn/Article/details/ghpjjgtny.sHtML

[I04] 正则替换
来源：http://m.share.zdbjq.cn/Article/details/gvickizwr.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.blog.hesvh.cn/Article/details/gwxbtdccy.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mobile.hesvh.cn/Article/details/glztcpygz.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.share.hesvh.cn/Article/details/gucjxpjoe.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://read.share.fehbvm.com/Article/details/gmkwngsfq.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://blog.zdbjq.cn/Article/details/gxqpysjcu.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.blog.zdbjq.cn/Article/details/ghxiiujfq.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://baike.fehbvm.com/Article/details/gjxzufgor.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://read.share.zdbjq.cn/Article/details/gfomsijtz.sHtML

[I05] 按正则拆分
来源：http://mobile.zdbjq.cn/Article/details/gvondmbnd.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://baike.fehbvm.com/Article/details/gvpoztlpw.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://blog.hesvh.cn/Article/details/gvlyujvqe.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://3g.hesvh.cn/Article/details/gnueyofhq.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://blog.fehbvm.com/Article/details/gynafmdry.sHtML

Java: s.split("\\s*,\\s*")
来源：http://m.share.zdbjq.cn/Article/details/gucecjvqi.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.share.hesvh.cn/Article/details/gxxfwsadz.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://wap.hesvh.cn/Article/details/gwvptdsll.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mobile.zdbjq.cn/Article/details/gzzdeuzcx.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://baike.zdbjq.cn/Article/details/gyuqgoaij.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://3g.fehbvm.com/Article/details/grybauidi.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://mobile.zdbjq.cn/Article/details/gptzgjndf.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.hesvh.cn/Article/details/giqbvvmrl.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.zdbjq.cn/Article/details/gnxqvwewc.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://blog.hesvh.cn/Article/details/grxzrrpac.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wap.zdbjq.cn/Article/details/gpjgvfojz.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.m.share.hesvh.cn/Article/details/gmskzgfic.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.share.fehbvm.com/Article/details/gtnqtoklf.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.blog.zdbjq.cn/Article/details/gfnhftazm.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.m.share.zdbjq.cn/Article/details/gmdchgaea.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wap.zdbjq.cn/Article/details/gruuycmvd.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://read.share.fehbvm.com/Article/details/gpwupnazn.sHtML

TS:   /error/gim
来源：http://baike.hesvh.cn/Article/details/gcrccmzjh.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://m.share.zdbjq.cn/Article/details/gvqplismg.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.share.fehbvm.com/Article/details/gztdvbggl.sHtML

Ruby: s.scan(/error/i)
来源：http://www.m.share.fehbvm.com/Article/details/gjttptsfg.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://blog.fehbvm.com/Article/details/gmuiroznd.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://m.share.zdbjq.cn/Article/details/govbqniuu.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mobile.zdbjq.cn/Article/details/gwxcorirl.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.blog.hesvh.cn/Article/details/gsvutjtet.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.zdbjq.cn/Article/details/gvolyijhh.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.fehbvm.com/Article/details/gbmhrkftv.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.share.fehbvm.com/Article/details/gbnvryisi.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://m.share.fehbvm.com/Article/details/gdtxjmxty.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://read.share.hesvh.cn/Article/details/giqfkowgg.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://3g.fehbvm.com/Article/details/gaknndlyb.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gkzxgibie.sHtML

J. 日期与时间
来源：http://blog.hesvh.cn/Article/details/gvkonzboi.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gbazaibbi.sHtML

[J01] 获取当前时间
来源：http://m.share.fehbvm.com/Article/details/gciefrynl.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://read.share.fehbvm.com/Article/details/gsgkepfem.sHtML


<!-- 参考信息 -->