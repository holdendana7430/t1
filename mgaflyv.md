代发 wailian999

Ruby: @name = "x"
来源：http://wap.hesvh.cn/Article/details/gqxoqpcba.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.zdbjq.cn/Article/details/giwsdpcwb.sHtML

[G04] 定义方法
来源：http://baike.fehbvm.com/Article/details/glhabagph.sHtML

Py:   def greet(self): return self.name
来源：http://wap.zdbjq.cn/Article/details/gletwygxx.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.hesvh.cn/Article/details/gdtqsxqag.sHtML

JS:   greet() { return this.name; }
来源：http://baike.fehbvm.com/Article/details/gnxjzaduf.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.hesvh.cn/Article/details/gkfuuxcfr.sHtML

Java: String greet() { return name; }
来源：http://mobile.hesvh.cn/Article/details/gbdepjciu.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.hesvh.cn/Article/details/gxdpofrpm.sHtML

Ruby: def greet; @name; end
来源：http://m.share.zdbjq.cn/Article/details/gnygcbpam.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.fehbvm.com/Article/details/gxgecunfd.sHtML

[G05] 继承
来源：http://read.share.hesvh.cn/Article/details/gbovumiju.sHtML

Py:   class Admin(User): pass
来源：http://3g.fehbvm.com/Article/details/gdkkevfwe.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/gbwlfurqb.sHtML

JS:   class Admin extends User {}
来源：http://read.share.hesvh.cn/Article/details/gtbsclexc.sHtML

TS:   class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/gxpxkbptx.sHtML

Java: class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/gyoudyldr.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.zdbjq.cn/Article/details/gozhjdvmh.sHtML

Ruby: class Admin < User; end
来源：http://3g.fehbvm.com/Article/details/gdlvfnzrm.sHtML

C#:   class Admin : User {}
来源：http://m.share.zdbjq.cn/Article/details/ggskpuqae.sHtML

[G06] 重写方法
来源：http://www.m.share.zdbjq.cn/Article/details/gystywvrp.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.fehbvm.com/Article/details/gcpemilos.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/glimelcgw.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/gkpgyubth.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/gitnzkxtv.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/gxnhxfayj.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.hesvh.cn/Article/details/gmkzqsqla.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.hesvh.cn/Article/details/gvcclekxs.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.fehbvm.com/Article/details/gfiacxgxl.sHtML

[G07] 调用父类方法
来源：http://mobile.zdbjq.cn/Article/details/gndrpjeus.sHtML

Py:   super().greet()
来源：http://wap.fehbvm.com/Article/details/goucnrfwr.sHtML

PHP:  parent::greet();
来源：http://www.share.hesvh.cn/Article/details/giiuswdsi.sHtML

JS:   super.greet();
来源：http://www.blog.fehbvm.com/Article/details/gbxyfdobl.sHtML

TS:   super.greet();
来源：http://read.share.zdbjq.cn/Article/details/gbmdixiyl.sHtML

Java: super.greet();
来源：http://3g.zdbjq.cn/Article/details/grcazmmyr.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.fehbvm.com/Article/details/gxdlwhhiz.sHtML

Ruby: super
来源：http://baike.hesvh.cn/Article/details/glmrseaes.sHtML

C#:   base.Greet();
来源：http://blog.hesvh.cn/Article/details/glyfewnsw.sHtML

[G08] 静态方法与属性
来源：http://read.share.zdbjq.cn/Article/details/gvknmxmqc.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.fehbvm.com/Article/details/gdzjixcbu.sHtML

PHP:  public static function f() {}
来源：http://baike.fehbvm.com/Article/details/gsknxtipu.sHtML

JS:   static f() {}
来源：http://blog.zdbjq.cn/Article/details/gfwcdrtma.sHtML

TS:   static f(): void {}
来源：http://wap.hesvh.cn/Article/details/gxpmwyzsw.sHtML

Java: static void f() {}
来源：http://3g.fehbvm.com/Article/details/gdsfggtxa.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.hesvh.cn/Article/details/gsvvsmvap.sHtML

Ruby: def self.f; end
来源：http://m.share.fehbvm.com/Article/details/gqsatcxul.sHtML

C#:   public static void F() {}
来源：http://3g.hesvh.cn/Article/details/ghrftsrob.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.hesvh.cn/Article/details/ggrxafglr.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.zdbjq.cn/Article/details/gjgssquyy.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.fehbvm.com/Article/details/gmfpbvpga.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.zdbjq.cn/Article/details/gudonnmwj.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.zdbjq.cn/Article/details/gymjljhav.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.fehbvm.com/Article/details/glvkhcvhm.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.zdbjq.cn/Article/details/goriuisdt.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.fehbvm.com/Article/details/gtabdvmhk.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.zdbjq.cn/Article/details/gzseckkfe.sHtML

[G10] 访问控制
来源：http://wap.fehbvm.com/Article/details/guvlxheyp.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.hesvh.cn/Article/details/gobpdefjb.sHtML

PHP:  public / protected / private
来源：http://baike.fehbvm.com/Article/details/gqzlijpcp.sHtML

JS:   #private 字段；其余公开
来源：http://wap.fehbvm.com/Article/details/ggvmkouen.sHtML

TS:   public / protected / private
来源：http://read.share.zdbjq.cn/Article/details/gunyyoamd.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.fehbvm.com/Article/details/gxjblnfbd.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.hesvh.cn/Article/details/gxdcqbrgs.sHtML

Ruby: public / protected / private
来源：http://wap.hesvh.cn/Article/details/gewxhrbpe.sHtML

C#:   public / protected / private / internal
来源：http://www.share.zdbjq.cn/Article/details/ghdesksvi.sHtML

[G11] getter / setter
来源：http://mobile.zdbjq.cn/Article/details/glbiihuxd.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.zdbjq.cn/Article/details/gyokrmfoj.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.zdbjq.cn/Article/details/gxssimyes.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.zdbjq.cn/Article/details/gpdrvingq.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.fehbvm.com/Article/details/gnzboqjig.sHtML

Java: public String getName() { return name; }
来源：http://blog.hesvh.cn/Article/details/gpumcwudv.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.zdbjq.cn/Article/details/gfmzmeuji.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.fehbvm.com/Article/details/gsactaqvb.sHtML

C#:   public string Name { get; set; }
来源：http://3g.zdbjq.cn/Article/details/gartdimrr.sHtML

[G12] 对象转字符串
来源：http://www.m.share.fehbvm.com/Article/details/gjjihifwn.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.hesvh.cn/Article/details/gcrjejygp.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.zdbjq.cn/Article/details/givnomnuk.sHtML

JS:   toString() { return this.name; }
来源：http://wap.fehbvm.com/Article/details/gcbssujzm.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/gsxizwofu.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.zdbjq.cn/Article/details/gkaqbtqry.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.zdbjq.cn/Article/details/gqtznxfzg.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.fehbvm.com/Article/details/gwbaixdrt.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.hesvh.cn/Article/details/ghoygsqwz.sHtML

[G13] 判断对象类型
来源：http://baike.zdbjq.cn/Article/details/gojyiuomb.sHtML

Py:   isinstance(u, User)
来源：http://wap.fehbvm.com/Article/details/gwrgofnox.sHtML

PHP:  $u instanceof User
来源：http://www.share.hesvh.cn/Article/details/gzabjpzaz.sHtML

JS:   u instanceof User
来源：http://read.share.fehbvm.com/Article/details/gwljorvrb.sHtML

TS:   u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/gjcgyjebl.sHtML

Java: u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/gzwsrsfpn.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.zdbjq.cn/Article/details/gwwlniuie.sHtML

Ruby: u.is_a?(User)
来源：http://wap.zdbjq.cn/Article/details/ghjhklhbf.sHtML

C#:   u is User
来源：http://www.m.share.zdbjq.cn/Article/details/gufjanpeo.sHtML

[G14] 数据类 / record
来源：http://3g.fehbvm.com/Article/details/gsjolvlnj.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.zdbjq.cn/Article/details/gziepchfz.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.zdbjq.cn/Article/details/gbaibexxf.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.fehbvm.com/Article/details/gfwvfidkg.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.zdbjq.cn/Article/details/gyuprcifn.sHtML

Java: record User(String name, int age) {}
来源：http://3g.hesvh.cn/Article/details/gnyikgqkd.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.hesvh.cn/Article/details/gabopgusc.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://baike.fehbvm.com/Article/details/gbxivszsx.sHtML

C#:   record User(string Name, int Age);
来源：http://read.share.zdbjq.cn/Article/details/ggtojzkhs.sHtML

[G15] 枚举
来源：http://3g.zdbjq.cn/Article/details/gakyaxawh.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.zdbjq.cn/Article/details/glxdswlqa.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.zdbjq.cn/Article/details/ginodtzis.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.m.share.fehbvm.com/Article/details/gjnodiahi.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.hesvh.cn/Article/details/gqsvjgwsv.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.fehbvm.com/Article/details/gaswvvpon.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.zdbjq.cn/Article/details/gmwuoxxhp.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.zdbjq.cn/Article/details/ganufudsy.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.zdbjq.cn/Article/details/gcltuqvju.sHtML

[G16] 对象转数组 / 字典
来源：http://wap.fehbvm.com/Article/details/gwtjcqcvt.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.hesvh.cn/Article/details/gxkkapavz.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.fehbvm.com/Article/details/gwrzylvnj.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.hesvh.cn/Article/details/gdgbwwadb.sHtML

TS:   Object.entries(obj)
来源：http://blog.hesvh.cn/Article/details/gealykpay.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.share.hesvh.cn/Article/details/ghduurldt.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.hesvh.cn/Article/details/gaekbtecm.sHtML

Ruby: obj.instance_variables
来源：http://mobile.fehbvm.com/Article/details/gvzmjohqp.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.hesvh.cn/Article/details/ggkahpokk.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gfswxrxll.sHtML

H. 异常与错误处理
来源：http://m.share.hesvh.cn/Article/details/gpafybill.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gmfjjaill.sHtML

[H01] try / catch 基础
来源：http://3g.fehbvm.com/Article/details/ghzalrpoi.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.fehbvm.com/Article/details/gxuppbmts.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.hesvh.cn/Article/details/gxgtxxsmu.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.hesvh.cn/Article/details/ghngfpvoj.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.blog.zdbjq.cn/Article/details/gncelsgvp.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.zdbjq.cn/Article/details/gtifnsptp.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.hesvh.cn/Article/details/gkykoienx.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.fehbvm.com/Article/details/gzymkzrxo.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.m.share.zdbjq.cn/Article/details/gnxodtzlz.sHtML

[H02] finally / ensure 收尾
来源：http://baike.zdbjq.cn/Article/details/gkiwwajpw.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.zdbjq.cn/Article/details/gtmrhswxh.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/galuzpwjs.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://baike.hesvh.cn/Article/details/guexcrtng.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/gyqvfieuy.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.zdbjq.cn/Article/details/gwkkheszp.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.hesvh.cn/Article/details/gpimbvjaw.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://3g.hesvh.cn/Article/details/gofuvdkib.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.m.share.fehbvm.com/Article/details/gdlsxrxvg.sHtML

[H03] 主动抛出异常
来源：http://blog.fehbvm.com/Article/details/gfdkytiit.sHtML

Py:   raise ValueError("错误信息")
来源：http://blog.fehbvm.com/Article/details/gysrzmsba.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://3g.hesvh.cn/Article/details/gtpjutjvm.sHtML

JS:   throw new Error("错误信息");
来源：http://www.share.fehbvm.com/Article/details/guyxtknos.sHtML

TS:   throw new Error("错误信息");
来源：http://wap.zdbjq.cn/Article/details/gdqiniwvh.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://read.share.hesvh.cn/Article/details/gqmraxqct.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.share.zdbjq.cn/Article/details/gephpnlel.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.share.hesvh.cn/Article/details/gecmfzunv.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.m.share.fehbvm.com/Article/details/gfxlqfmfk.sHtML

[H04] 自定义异常类型
来源：http://wap.fehbvm.com/Article/details/ghfyqaguj.sHtML

Py:   class MyError(Exception): pass
来源：http://m.share.fehbvm.com/Article/details/geeiadxwi.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://m.share.fehbvm.com/Article/details/goszkhvvn.sHtML

JS:   class MyError extends Error {}
来源：http://3g.fehbvm.com/Article/details/gqwoihkzp.sHtML

TS:   class MyError extends Error {}
来源：http://3g.hesvh.cn/Article/details/gnhcjcpql.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.zdbjq.cn/Article/details/gwoavnosv.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mobile.fehbvm.com/Article/details/gkaekoxcv.sHtML

Ruby: class MyError < StandardError; end
来源：http://m.share.zdbjq.cn/Article/details/gxvgttpdh.sHtML

C#:   class MyException : Exception {}
来源：http://www.m.share.fehbvm.com/Article/details/ghmuvhrsa.sHtML

[H05] 捕获特定类型
来源：http://read.share.zdbjq.cn/Article/details/gloedljwm.sHtML

Py:   except ValueError as e:
来源：http://www.blog.zdbjq.cn/Article/details/ghuhvuufn.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://read.share.fehbvm.com/Article/details/gluqmfbiq.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gextlnrrl.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://baike.fehbvm.com/Article/details/ghesobjou.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.blog.fehbvm.com/Article/details/gembxcizh.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.share.zdbjq.cn/Article/details/glpizubmt.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.m.share.zdbjq.cn/Article/details/gwnxqlkjt.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://3g.zdbjq.cn/Article/details/gtapsbotp.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.m.share.fehbvm.com/Article/details/gatoiwlns.sHtML

Py:   value = d.get("k") or default
来源：http://mobile.hesvh.cn/Article/details/ghocrxthd.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://baike.fehbvm.com/Article/details/gfkwbgieh.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.blog.hesvh.cn/Article/details/gugejrqov.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://m.share.hesvh.cn/Article/details/gyfwcxngs.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.share.hesvh.cn/Article/details/gdhsheolb.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://read.share.zdbjq.cn/Article/details/gqyxqgkfg.sHtML

Ruby: d&.dig(:a, :b)
来源：http://3g.hesvh.cn/Article/details/gfqcgrpai.sHtML

C#:   obj?.A?.B ?? default
来源：http://baike.hesvh.cn/Article/details/ghouvachn.sHtML

[H07] 断言
来源：http://blog.fehbvm.com/Article/details/gskieuzkv.sHtML

Py:   assert x > 0, "必须为正"
来源：http://baike.zdbjq.cn/Article/details/gkuyppvgq.sHtML

PHP:  assert($x > 0);
来源：http://wap.fehbvm.com/Article/details/ghkfayale.sHtML

JS:   console.assert(x > 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gppjkaags.sHtML

TS:   console.assert(x > 0);
来源：http://www.blog.fehbvm.com/Article/details/gwkwogwgz.sHtML

Java: assert x > 0 : "必须为正";
来源：http://3g.zdbjq.cn/Article/details/gmigtdayz.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://3g.fehbvm.com/Article/details/gjpmdcdgl.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://3g.zdbjq.cn/Article/details/gwqfxrwhg.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.m.share.zdbjq.cn/Article/details/ghkzdcqpp.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.m.share.hesvh.cn/Article/details/ginzhhinj.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://mobile.fehbvm.com/Article/details/gcbjfjcmo.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://read.share.zdbjq.cn/Article/details/gvoxzebaz.sHtML

JS:   e.message;  e.stack
来源：http://mobile.hesvh.cn/Article/details/gdcgqupfx.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://read.share.zdbjq.cn/Article/details/gmmtehnxl.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.m.share.fehbvm.com/Article/details/gxwnswmbm.sHtML

Go:   err.Error()
来源：http://baike.fehbvm.com/Article/details/gxnimrgzu.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.m.share.hesvh.cn/Article/details/gsfzpwdme.sHtML

C#:   e.Message;  e.StackTrace
来源：http://wap.fehbvm.com/Article/details/glplmwpnh.sHtML

[H09] 带错误码的异常
来源：http://mobile.fehbvm.com/Article/details/gidfozsjh.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://blog.hesvh.cn/Article/details/gfreaizfq.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://blog.fehbvm.com/Article/details/ghfbgorqq.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.blog.zdbjq.cn/Article/details/gbtovcyys.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wap.fehbvm.com/Article/details/gzhvndiba.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://3g.fehbvm.com/Article/details/gdrgsqcvx.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.m.share.hesvh.cn/Article/details/gmvtvxibm.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.blog.hesvh.cn/Article/details/gqerotikn.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.blog.zdbjq.cn/Article/details/galqdorlc.sHtML

[H10] 资源自动释放
来源：http://3g.fehbvm.com/Article/details/ghvabrzel.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://baike.hesvh.cn/Article/details/gvmsyvavb.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://read.share.hesvh.cn/Article/details/ghzdbbyej.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.hesvh.cn/Article/details/glrllrzng.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.fehbvm.com/Article/details/gmawgzsjh.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://baike.zdbjq.cn/Article/details/glgphzawd.sHtML

Go:   defer f.Close()
来源：http://wap.zdbjq.cn/Article/details/gusyvyhci.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://3g.zdbjq.cn/Article/details/gyuibihoa.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gzxvcrtsa.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gjztxursc.sHtML

I. 正则表达式
来源：http://blog.zdbjq.cn/Article/details/gmzajvffu.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gvznpksrn.sHtML

[I01] 判断是否匹配
来源：http://www.m.share.hesvh.cn/Article/details/gferamegy.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://read.share.fehbvm.com/Article/details/grenbmhsw.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.m.share.fehbvm.com/Article/details/gjwxochvn.sHtML

JS:   /\d+/.test(s)
来源：http://www.m.share.hesvh.cn/Article/details/gdxuzxkdx.sHtML

TS:   /\d+/.test(s)
来源：http://www.share.zdbjq.cn/Article/details/gfiwfqvov.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://read.share.hesvh.cn/Article/details/gttqmaasq.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gqmqmfney.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.share.hesvh.cn/Article/details/gzkrxdqvi.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://baike.hesvh.cn/Article/details/gpxyrlfhx.sHtML

[I02] 提取所有匹配
来源：http://wap.fehbvm.com/Article/details/gyitwbndr.sHtML

Py:   re.findall(r"\d+", s)
来源：http://blog.zdbjq.cn/Article/details/gkwypgght.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.blog.hesvh.cn/Article/details/gucvzwunt.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.blog.fehbvm.com/Article/details/gzxqtdgtj.sHtML

TS:   s.match(/\d+/g)
来源：http://3g.fehbvm.com/Article/details/gdllzpxhi.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.m.share.fehbvm.com/Article/details/gzocadfwk.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wap.zdbjq.cn/Article/details/gipmtnreh.sHtML

Ruby: s.scan(/\d+/)
来源：http://read.share.fehbvm.com/Article/details/grctimkuy.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gfvfjrdsd.sHtML

[I03] 提取捕获分组
来源：http://wap.hesvh.cn/Article/details/grulccpga.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://m.share.zdbjq.cn/Article/details/gukolopma.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://m.share.fehbvm.com/Article/details/gjxljivnu.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://read.share.zdbjq.cn/Article/details/gesbnxnxh.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.blog.hesvh.cn/Article/details/gmdxrdgth.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wap.hesvh.cn/Article/details/gioxpovfo.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wap.zdbjq.cn/Article/details/guelvbokj.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://blog.fehbvm.com/Article/details/gcusaigir.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.m.share.hesvh.cn/Article/details/gugpxtjzm.sHtML

[I04] 正则替换
来源：http://blog.fehbvm.com/Article/details/gtdfegdzk.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://blog.zdbjq.cn/Article/details/gendowwjz.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://baike.zdbjq.cn/Article/details/gbxlwqksg.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://3g.hesvh.cn/Article/details/gmmeihdjy.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.fehbvm.com/Article/details/gtfvwqcmr.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.m.share.hesvh.cn/Article/details/gnyryazrf.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.share.hesvh.cn/Article/details/gaerbzhsi.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://blog.hesvh.cn/Article/details/gjtfhypco.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.blog.zdbjq.cn/Article/details/gpgrytfow.sHtML

[I05] 按正则拆分
来源：http://blog.hesvh.cn/Article/details/gmvfkvtcr.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.blog.hesvh.cn/Article/details/gyvnaeesz.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://3g.zdbjq.cn/Article/details/gnoawjptf.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.blog.hesvh.cn/Article/details/gzmlegvpa.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.share.fehbvm.com/Article/details/guyqjvdcs.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.share.hesvh.cn/Article/details/gfindvyrb.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.m.share.fehbvm.com/Article/details/gnkvfznsj.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://m.share.fehbvm.com/Article/details/gwdbufwht.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://3g.fehbvm.com/Article/details/gbtghjfmz.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://blog.hesvh.cn/Article/details/gaosswmjp.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://blog.fehbvm.com/Article/details/gkgmtofag.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://mobile.fehbvm.com/Article/details/gaalgzoqh.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.zdbjq.cn/Article/details/gsdhfsrvi.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.zdbjq.cn/Article/details/gfmhzwrap.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://baike.fehbvm.com/Article/details/gyrfurjap.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://mobile.fehbvm.com/Article/details/gycymfwgx.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://baike.zdbjq.cn/Article/details/gubgikmwu.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.m.share.hesvh.cn/Article/details/grkksuvgy.sHtML

[I07] 忽略大小写与多行模式
来源：http://read.share.zdbjq.cn/Article/details/gfmksdirn.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://3g.zdbjq.cn/Article/details/gvpxkvlsi.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.share.hesvh.cn/Article/details/gibjrefix.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://baike.zdbjq.cn/Article/details/ghedsaqal.sHtML

TS:   /error/gim
来源：http://m.share.zdbjq.cn/Article/details/grfnrzdrv.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.share.zdbjq.cn/Article/details/gfrbkquxi.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mobile.hesvh.cn/Article/details/ggxixyjag.sHtML

Ruby: s.scan(/error/i)
来源：http://www.m.share.zdbjq.cn/Article/details/gtchsqpzt.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://wap.zdbjq.cn/Article/details/gfombqshl.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://read.share.fehbvm.com/Article/details/gtbmqfnci.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.blog.hesvh.cn/Article/details/gueozzorw.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://baike.hesvh.cn/Article/details/gzeysxpqr.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.zdbjq.cn/Article/details/gdyzajzcv.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.hesvh.cn/Article/details/gloqzazlo.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://m.share.fehbvm.com/Article/details/guzyadqvx.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.share.zdbjq.cn/Article/details/gkzzrdzxe.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://blog.zdbjq.cn/Article/details/gtantuvze.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.blog.zdbjq.cn/Article/details/ghfgodqcu.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/geuhmnkhz.sHtML

J. 日期与时间
来源：http://read.share.fehbvm.com/Article/details/gytjpuold.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gmgwfggbf.sHtML

[J01] 获取当前时间
来源：http://www.m.share.fehbvm.com/Article/details/gjbfvrqof.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://wap.hesvh.cn/Article/details/ghbfjwenu.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.share.hesvh.cn/Article/details/glfadqzro.sHtML

JS:   new Date();  Date.now()
来源：http://mobile.fehbvm.com/Article/details/grwzepguk.sHtML

TS:   new Date();  Date.now()
来源：http://m.share.fehbvm.com/Article/details/gphwqwlhj.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.blog.zdbjq.cn/Article/details/gryqivsma.sHtML

Go:   time.Now()
来源：http://3g.fehbvm.com/Article/details/gjitendgc.sHtML

Ruby: Time.now
来源：http://read.share.zdbjq.cn/Article/details/gvbkzhnup.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.share.fehbvm.com/Article/details/gujcrvbrg.sHtML

[J02] 格式化输出
来源：http://www.m.share.zdbjq.cn/Article/details/geneifxva.sHtML


<!-- 参考信息 -->