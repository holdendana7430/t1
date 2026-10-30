代发 wailian999

C#:   public User(string name) { Name = name; }
来源：http://m.share.zdbjq.cn/Article/details/gzlxgqlqm.sHtML

[G03] 实例属性
来源：http://www.share.fehbvm.com/Article/details/gltpejgme.sHtML

Py:   self.name = "x"
来源：http://www.blog.zdbjq.cn/Article/details/gauhjkrec.sHtML

PHP:  public string $name = "x";
来源：http://www.share.fehbvm.com/Article/details/gsfcpnvyw.sHtML

JS:   this.name = "x";
来源：http://m.share.hesvh.cn/Article/details/gaorzbfxj.sHtML

TS:   name: string = "x";
来源：http://baike.zdbjq.cn/Article/details/gyomgaqkm.sHtML

Java: private String name;
来源：http://3g.fehbvm.com/Article/details/grpanobkr.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.hesvh.cn/Article/details/gxhyxatnx.sHtML

Ruby: @name = "x"
来源：http://www.m.share.fehbvm.com/Article/details/gcbilknjo.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.zdbjq.cn/Article/details/gpuapbjbs.sHtML

[G04] 定义方法
来源：http://baike.zdbjq.cn/Article/details/grzuwjksc.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.hesvh.cn/Article/details/gripdefal.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.hesvh.cn/Article/details/gmjjjkabi.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/gjndikczo.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/gyeyzhexy.sHtML

Java: String greet() { return name; }
来源：http://3g.hesvh.cn/Article/details/gmaptddql.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.zdbjq.cn/Article/details/gnnyixpva.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.hesvh.cn/Article/details/glyakaeeh.sHtML

C#:   public string Greet() => Name;
来源：http://3g.zdbjq.cn/Article/details/gqgeemmff.sHtML

[G05] 继承
来源：http://m.share.zdbjq.cn/Article/details/gjoofmswz.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.fehbvm.com/Article/details/galdbnhdr.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.hesvh.cn/Article/details/gwauabpak.sHtML

JS:   class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/gfsjejrfm.sHtML

TS:   class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/grtbgctes.sHtML

Java: class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/gjcrppqqs.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.fehbvm.com/Article/details/gzxzjpfyw.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.zdbjq.cn/Article/details/gjcccokje.sHtML

C#:   class Admin : User {}
来源：http://www.blog.hesvh.cn/Article/details/gftoafail.sHtML

[G06] 重写方法
来源：http://www.blog.fehbvm.com/Article/details/gragxwwxm.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.fehbvm.com/Article/details/gvhpuzmlg.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/gscqknbil.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gkttamkdq.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/gmceplhji.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/gofxghhpy.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.hesvh.cn/Article/details/gmrscwtaw.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.hesvh.cn/Article/details/gecajjcxp.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.fehbvm.com/Article/details/gkptoaywb.sHtML

[G07] 调用父类方法
来源：http://www.share.zdbjq.cn/Article/details/gkxqjiahl.sHtML

Py:   super().greet()
来源：http://www.blog.zdbjq.cn/Article/details/gpqcavyxh.sHtML

PHP:  parent::greet();
来源：http://www.blog.hesvh.cn/Article/details/godeqvhke.sHtML

JS:   super.greet();
来源：http://read.share.zdbjq.cn/Article/details/gbfkzsmla.sHtML

TS:   super.greet();
来源：http://baike.zdbjq.cn/Article/details/globwdrxu.sHtML

Java: super.greet();
来源：http://www.blog.zdbjq.cn/Article/details/gzqdnmpdv.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.fehbvm.com/Article/details/gfwljaqax.sHtML

Ruby: super
来源：http://wap.hesvh.cn/Article/details/gnxozebjq.sHtML

C#:   base.Greet();
来源：http://m.share.fehbvm.com/Article/details/gdjxzkgya.sHtML

[G08] 静态方法与属性
来源：http://baike.zdbjq.cn/Article/details/gjbtxpdhc.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.zdbjq.cn/Article/details/gcnkdghrf.sHtML

PHP:  public static function f() {}
来源：http://www.blog.zdbjq.cn/Article/details/gvbonlysf.sHtML

JS:   static f() {}
来源：http://wap.zdbjq.cn/Article/details/gcdbsspse.sHtML

TS:   static f(): void {}
来源：http://blog.hesvh.cn/Article/details/gwsacttgt.sHtML

Java: static void f() {}
来源：http://www.blog.fehbvm.com/Article/details/gfxizgyfl.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.zdbjq.cn/Article/details/gvbwdmvea.sHtML

Ruby: def self.f; end
来源：http://www.blog.fehbvm.com/Article/details/gckctabtb.sHtML

C#:   public static void F() {}
来源：http://mobile.zdbjq.cn/Article/details/gxtunsayd.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.hesvh.cn/Article/details/gdsypkirs.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.fehbvm.com/Article/details/gnqrtuxnz.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.hesvh.cn/Article/details/gtjopyoyt.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.zdbjq.cn/Article/details/gwfnhsrrd.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.zdbjq.cn/Article/details/gjivgqbhw.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.fehbvm.com/Article/details/gatnjqysq.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.hesvh.cn/Article/details/gmhjmjhna.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.zdbjq.cn/Article/details/gbmfwdpmh.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.fehbvm.com/Article/details/gsvzmeqbn.sHtML

[G10] 访问控制
来源：http://m.share.hesvh.cn/Article/details/gqgggijvw.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.fehbvm.com/Article/details/gktqzscrb.sHtML

PHP:  public / protected / private
来源：http://3g.zdbjq.cn/Article/details/glcputbdt.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.fehbvm.com/Article/details/gbkchxwed.sHtML

TS:   public / protected / private
来源：http://wap.zdbjq.cn/Article/details/gfmtzhion.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.fehbvm.com/Article/details/gdvcswaop.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.fehbvm.com/Article/details/gqlihtego.sHtML

Ruby: public / protected / private
来源：http://www.blog.zdbjq.cn/Article/details/gunjysaex.sHtML

C#:   public / protected / private / internal
来源：http://m.share.hesvh.cn/Article/details/gdqawfill.sHtML

[G11] getter / setter
来源：http://3g.hesvh.cn/Article/details/gzdbtnhro.sHtML

Py:   @property 与 @x.setter
来源：http://wap.zdbjq.cn/Article/details/gyzkrlodn.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gxhzxbmfg.sHtML

JS:   get name() { return this._name; }
来源：http://baike.hesvh.cn/Article/details/gywqajcyb.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.hesvh.cn/Article/details/gqbawqmkr.sHtML

Java: public String getName() { return name; }
来源：http://m.share.hesvh.cn/Article/details/gztwovpvj.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.zdbjq.cn/Article/details/grfsdicot.sHtML

Ruby: attr_accessor :name
来源：http://wap.zdbjq.cn/Article/details/gayqngsbb.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.fehbvm.com/Article/details/gegjtezcb.sHtML

[G12] 对象转字符串
来源：http://baike.hesvh.cn/Article/details/gjeuezppi.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.zdbjq.cn/Article/details/gitnsttva.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.fehbvm.com/Article/details/gabrevjsl.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/gewlqzfxw.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.zdbjq.cn/Article/details/gznozrimi.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.fehbvm.com/Article/details/gvxjrldge.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.fehbvm.com/Article/details/gwadyabqh.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.hesvh.cn/Article/details/gpxdhxfgj.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.hesvh.cn/Article/details/gmqahgkcb.sHtML

[G13] 判断对象类型
来源：http://3g.zdbjq.cn/Article/details/gcuengyon.sHtML

Py:   isinstance(u, User)
来源：http://mobile.zdbjq.cn/Article/details/gvpkzubtf.sHtML

PHP:  $u instanceof User
来源：http://baike.fehbvm.com/Article/details/gbmmjjddd.sHtML

JS:   u instanceof User
来源：http://read.share.fehbvm.com/Article/details/gktfdanbn.sHtML

TS:   u instanceof User
来源：http://m.share.fehbvm.com/Article/details/gaqmtdbfa.sHtML

Java: u instanceof User
来源：http://baike.zdbjq.cn/Article/details/gwhvjanen.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.hesvh.cn/Article/details/gmtsugxda.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.hesvh.cn/Article/details/gjdihuuyk.sHtML

C#:   u is User
来源：http://www.share.fehbvm.com/Article/details/gzbvmbaij.sHtML

[G14] 数据类 / record
来源：http://baike.fehbvm.com/Article/details/gvbqzhbnl.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.hesvh.cn/Article/details/gyiircwam.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.fehbvm.com/Article/details/ghoxfduhk.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.zdbjq.cn/Article/details/gmnfkigye.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.fehbvm.com/Article/details/gpoqzztmi.sHtML

Java: record User(String name, int age) {}
来源：http://mobile.hesvh.cn/Article/details/gmsrmbelm.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.fehbvm.com/Article/details/glzasdcjk.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.zdbjq.cn/Article/details/glihqxeot.sHtML

C#:   record User(string Name, int Age);
来源：http://m.share.zdbjq.cn/Article/details/gcchbddhb.sHtML

[G15] 枚举
来源：http://baike.zdbjq.cn/Article/details/gelqfmymd.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.zdbjq.cn/Article/details/gcuwoosxv.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.zdbjq.cn/Article/details/gqovejkqa.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://read.share.hesvh.cn/Article/details/gazoxtygc.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.fehbvm.com/Article/details/ghuqipdmf.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.zdbjq.cn/Article/details/gpwhlenau.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.fehbvm.com/Article/details/gwynyjhlz.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.fehbvm.com/Article/details/gcgvgcdel.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.zdbjq.cn/Article/details/gofzsrqpa.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.hesvh.cn/Article/details/gzvddnvsk.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://3g.zdbjq.cn/Article/details/gmeanglmx.sHtML

PHP:  get_object_vars($obj);
来源：http://wap.fehbvm.com/Article/details/goiybdjpy.sHtML

JS:   Object.entries(obj)
来源：http://blog.fehbvm.com/Article/details/gaunjsqqk.sHtML

TS:   Object.entries(obj)
来源：http://read.share.zdbjq.cn/Article/details/gdhudftsy.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.fehbvm.com/Article/details/gvsunlrax.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.zdbjq.cn/Article/details/gleiwowdt.sHtML

Ruby: obj.instance_variables
来源：http://baike.fehbvm.com/Article/details/gmojwjskr.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.zdbjq.cn/Article/details/gvepghfuq.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/ghxsrykfp.sHtML

H. 异常与错误处理
来源：http://3g.fehbvm.com/Article/details/ggykdkbwl.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gsjeuzpgz.sHtML

[H01] try / catch 基础
来源：http://read.share.hesvh.cn/Article/details/grwhskhsa.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://baike.hesvh.cn/Article/details/glxthpgno.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.fehbvm.com/Article/details/gsponnibz.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.fehbvm.com/Article/details/gnpnoxrdr.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.hesvh.cn/Article/details/gjsmyjlsl.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.hesvh.cn/Article/details/gdboigbwn.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.zdbjq.cn/Article/details/gzcabesom.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.share.fehbvm.com/Article/details/gfpzmydwk.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.zdbjq.cn/Article/details/guejogxia.sHtML

[H02] finally / ensure 收尾
来源：http://wap.hesvh.cn/Article/details/glmgftalp.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.fehbvm.com/Article/details/gjvqgtgxn.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/gzgrzdjue.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.fehbvm.com/Article/details/gvxzkgbyx.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/gbmrmkabq.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.hesvh.cn/Article/details/gfeqigwhd.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.fehbvm.com/Article/details/gnfbtacet.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.fehbvm.com/Article/details/gdgjysjbx.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/gygnncezu.sHtML

[H03] 主动抛出异常
来源：http://m.share.zdbjq.cn/Article/details/gshiaidxq.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.hesvh.cn/Article/details/gzdxkrjwc.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/gzxmqgosg.sHtML

JS:   throw new Error("错误信息");
来源：http://www.m.share.hesvh.cn/Article/details/gxesuguve.sHtML

TS:   throw new Error("错误信息");
来源：http://read.share.fehbvm.com/Article/details/guncrmscr.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://m.share.hesvh.cn/Article/details/gapqeppnq.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.blog.zdbjq.cn/Article/details/gclydfdku.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://m.share.hesvh.cn/Article/details/ghfztwqrx.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.share.zdbjq.cn/Article/details/gkdqmgllz.sHtML

[H04] 自定义异常类型
来源：http://www.share.fehbvm.com/Article/details/gvutouqfe.sHtML

Py:   class MyError(Exception): pass
来源：http://baike.zdbjq.cn/Article/details/gyyfrbdax.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://mobile.zdbjq.cn/Article/details/gpxhujabr.sHtML

JS:   class MyError extends Error {}
来源：http://www.m.share.hesvh.cn/Article/details/gcfmoyjms.sHtML

TS:   class MyError extends Error {}
来源：http://3g.hesvh.cn/Article/details/gdxnvyurt.sHtML

Java: class MyException extends RuntimeException {}
来源：http://baike.hesvh.cn/Article/details/glotvzudu.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://baike.fehbvm.com/Article/details/ggnmuzlji.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.m.share.fehbvm.com/Article/details/gtpoxkbak.sHtML

C#:   class MyException : Exception {}
来源：http://read.share.zdbjq.cn/Article/details/gwubfqjdn.sHtML

[H05] 捕获特定类型
来源：http://baike.zdbjq.cn/Article/details/gsawchdra.sHtML

Py:   except ValueError as e:
来源：http://www.share.fehbvm.com/Article/details/gfelrxwys.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://3g.fehbvm.com/Article/details/gcjmbuwhc.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://m.share.zdbjq.cn/Article/details/gcatycafo.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://mobile.fehbvm.com/Article/details/gbibfmgul.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.blog.fehbvm.com/Article/details/ghkqehqhg.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wap.zdbjq.cn/Article/details/gcvqtvfre.sHtML

Ruby: rescue ArgumentError => e
来源：http://wap.fehbvm.com/Article/details/gbxzjlmat.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://3g.zdbjq.cn/Article/details/gekbjaior.sHtML

[H06] 可选值 / 空值安全访问
来源：http://wap.zdbjq.cn/Article/details/guutuvszt.sHtML

Py:   value = d.get("k") or default
来源：http://blog.hesvh.cn/Article/details/gsimvhfiq.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://blog.zdbjq.cn/Article/details/gdiclmdva.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://mobile.hesvh.cn/Article/details/gepwlbsll.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.blog.zdbjq.cn/Article/details/ggmcwbkca.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://blog.fehbvm.com/Article/details/gxvumflfm.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://3g.fehbvm.com/Article/details/gwbbveedr.sHtML

Ruby: d&.dig(:a, :b)
来源：http://3g.hesvh.cn/Article/details/gnzxfzkye.sHtML

C#:   obj?.A?.B ?? default
来源：http://baike.fehbvm.com/Article/details/gqnlgfvdl.sHtML

[H07] 断言
来源：http://mobile.zdbjq.cn/Article/details/gwcskpwbu.sHtML

Py:   assert x > 0, "必须为正"
来源：http://mobile.zdbjq.cn/Article/details/gpveeppqr.sHtML

PHP:  assert($x > 0);
来源：http://3g.hesvh.cn/Article/details/gjmviudis.sHtML

JS:   console.assert(x > 0);
来源：http://read.share.zdbjq.cn/Article/details/gggnwxnjk.sHtML

TS:   console.assert(x > 0);
来源：http://baike.hesvh.cn/Article/details/gzxqvvhaa.sHtML

Java: assert x > 0 : "必须为正";
来源：http://m.share.zdbjq.cn/Article/details/gfpzpcitv.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.blog.zdbjq.cn/Article/details/gmvtafcxe.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://mobile.zdbjq.cn/Article/details/gmwqupvcy.sHtML

C#:   Debug.Assert(x > 0);
来源：http://read.share.hesvh.cn/Article/details/gcfznxeps.sHtML

[H08] 获取错误信息与堆栈
来源：http://blog.zdbjq.cn/Article/details/gkwwvaglu.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://3g.hesvh.cn/Article/details/gmfdfiuhk.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://read.share.hesvh.cn/Article/details/gdmbyxxow.sHtML

JS:   e.message;  e.stack
来源：http://mobile.zdbjq.cn/Article/details/gwriqtwtw.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.m.share.zdbjq.cn/Article/details/gczbegzxs.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.share.zdbjq.cn/Article/details/gzbpjdwhi.sHtML

Go:   err.Error()
来源：http://wap.zdbjq.cn/Article/details/glxiqhkil.sHtML

Ruby: e.message;  e.backtrace
来源：http://m.share.hesvh.cn/Article/details/gwtpgawod.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.m.share.zdbjq.cn/Article/details/gblfnflfr.sHtML

[H09] 带错误码的异常
来源：http://baike.hesvh.cn/Article/details/gzhxvgnik.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://m.share.hesvh.cn/Article/details/gehtmjwaw.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://blog.hesvh.cn/Article/details/gocybinur.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.blog.hesvh.cn/Article/details/goawxyudr.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://m.share.hesvh.cn/Article/details/guxbnktqy.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.m.share.zdbjq.cn/Article/details/gygretpgj.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.blog.fehbvm.com/Article/details/grsbcvepw.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://3g.zdbjq.cn/Article/details/gxubceoza.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://m.share.zdbjq.cn/Article/details/gkfeuxgux.sHtML

[H10] 资源自动释放
来源：http://mobile.fehbvm.com/Article/details/gkwmvxbgr.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://wap.fehbvm.com/Article/details/gpkpcsfzk.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.m.share.fehbvm.com/Article/details/gbiowaluj.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.zdbjq.cn/Article/details/gotzmtopp.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.fehbvm.com/Article/details/gjaducrbn.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://3g.hesvh.cn/Article/details/gibmwwsao.sHtML

Go:   defer f.Close()
来源：http://baike.hesvh.cn/Article/details/guqmybpwd.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.m.share.fehbvm.com/Article/details/gisqemgts.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gkyitgdxv.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gvsjykbnz.sHtML

I. 正则表达式
来源：http://read.share.hesvh.cn/Article/details/ggnjftixg.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gljatgfqm.sHtML

[I01] 判断是否匹配
来源：http://m.share.hesvh.cn/Article/details/ghcqzbfsk.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://3g.zdbjq.cn/Article/details/gtykznhml.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://read.share.fehbvm.com/Article/details/gozykcblm.sHtML

JS:   /\d+/.test(s)
来源：http://blog.hesvh.cn/Article/details/gxefmxprd.sHtML

TS:   /\d+/.test(s)
来源：http://www.share.zdbjq.cn/Article/details/ghgfjrwdx.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://read.share.fehbvm.com/Article/details/gjexbtzru.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gxgwlodtr.sHtML

Ruby: s.match?(/\d+/)
来源：http://read.share.hesvh.cn/Article/details/gdrspzruk.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://m.share.fehbvm.com/Article/details/getrhyyqn.sHtML

[I02] 提取所有匹配
来源：http://read.share.zdbjq.cn/Article/details/ghvdoekal.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.blog.zdbjq.cn/Article/details/gtpdnduxc.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://3g.zdbjq.cn/Article/details/gxmxnysha.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.blog.fehbvm.com/Article/details/gjgbughrx.sHtML

TS:   s.match(/\d+/g)
来源：http://m.share.zdbjq.cn/Article/details/grqrgijju.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://baike.hesvh.cn/Article/details/guhdbbpex.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://read.share.fehbvm.com/Article/details/gjhaibxnd.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.m.share.fehbvm.com/Article/details/gjgpyecyn.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.blog.hesvh.cn/Article/details/gfbfevemv.sHtML

[I03] 提取捕获分组
来源：http://3g.fehbvm.com/Article/details/gexamirdp.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://3g.hesvh.cn/Article/details/gjatzfspi.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wap.fehbvm.com/Article/details/gpdyplcvh.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://m.share.zdbjq.cn/Article/details/gkuflulpg.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://3g.fehbvm.com/Article/details/gbwbyofwv.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://mobile.fehbvm.com/Article/details/giuawcjwt.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wap.fehbvm.com/Article/details/gibzfdwnz.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://3g.zdbjq.cn/Article/details/giuifqlal.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://read.share.hesvh.cn/Article/details/gauorkyfh.sHtML

[I04] 正则替换
来源：http://m.share.hesvh.cn/Article/details/gkqnnnibm.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://baike.zdbjq.cn/Article/details/gwkfkkzet.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://blog.hesvh.cn/Article/details/gnilfqvec.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://mobile.zdbjq.cn/Article/details/gmnsuppjy.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.share.fehbvm.com/Article/details/gjwevnlzo.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.blog.hesvh.cn/Article/details/gneruwqmw.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.share.zdbjq.cn/Article/details/gjnhnvrwc.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://mobile.fehbvm.com/Article/details/ghytrmgei.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://blog.fehbvm.com/Article/details/gerzeuhra.sHtML

[I05] 按正则拆分
来源：http://www.share.zdbjq.cn/Article/details/gxalcdvyk.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://read.share.hesvh.cn/Article/details/gwyxanorw.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wap.hesvh.cn/Article/details/ghqfecgwi.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.blog.zdbjq.cn/Article/details/gdyfuozyn.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://m.share.hesvh.cn/Article/details/gcgsoxitm.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.share.fehbvm.com/Article/details/gumsjtssr.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://baike.hesvh.cn/Article/details/gemjihghu.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://mobile.zdbjq.cn/Article/details/gphcfnvxw.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://blog.hesvh.cn/Article/details/guyarxonb.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wap.zdbjq.cn/Article/details/gtbtvmhfh.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wap.fehbvm.com/Article/details/gafghcfjz.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wap.hesvh.cn/Article/details/gjkzsgarj.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.hesvh.cn/Article/details/gzhygqsmn.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.zdbjq.cn/Article/details/gwrnvgnfv.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.blog.hesvh.cn/Article/details/gszurpdtk.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.blog.zdbjq.cn/Article/details/gbrnsivft.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wap.zdbjq.cn/Article/details/gzialorit.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mobile.hesvh.cn/Article/details/gghrxkude.sHtML

[I07] 忽略大小写与多行模式
来源：http://read.share.zdbjq.cn/Article/details/gryqgyeel.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://3g.zdbjq.cn/Article/details/gjawkxady.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.share.hesvh.cn/Article/details/gxtklddfb.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://blog.fehbvm.com/Article/details/gjyrlsvkm.sHtML

TS:   /error/gim
来源：http://www.share.hesvh.cn/Article/details/glzcqcyhs.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.m.share.zdbjq.cn/Article/details/grqfhmkti.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://read.share.zdbjq.cn/Article/details/gqxyfswcx.sHtML

Ruby: s.scan(/error/i)
来源：http://read.share.fehbvm.com/Article/details/gvlqtdhyx.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://blog.hesvh.cn/Article/details/gliebxiar.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://m.share.hesvh.cn/Article/details/glbndavlt.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://read.share.zdbjq.cn/Article/details/geuqeuzma.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://3g.hesvh.cn/Article/details/gpvweslmz.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.hesvh.cn/Article/details/gsygczctt.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.hesvh.cn/Article/details/grlmkfocs.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://3g.zdbjq.cn/Article/details/gxqnliksd.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.m.share.zdbjq.cn/Article/details/gtzrysbjj.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://baike.fehbvm.com/Article/details/getsksbjy.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.blog.hesvh.cn/Article/details/gbzhxlxcn.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gwgvftlez.sHtML

J. 日期与时间
来源：http://www.m.share.hesvh.cn/Article/details/gtvoxgqwc.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gwdjqwjyw.sHtML

[J01] 获取当前时间
来源：http://m.share.fehbvm.com/Article/details/gyiwtudqd.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.share.fehbvm.com/Article/details/ghufcqlrr.sHtML


<!-- 参考信息 -->