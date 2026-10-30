代发 wailian999

C#:   public User(string name) { Name = name; }
来源：http://3g.fehbvm.com/Article/details/gsozousdv.sHtML

[G03] 实例属性
来源：http://baike.fehbvm.com/Article/details/gnlpfghzl.sHtML

Py:   self.name = "x"
来源：http://m.share.zdbjq.cn/Article/details/geglnexgs.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.hesvh.cn/Article/details/gfdaswufh.sHtML

JS:   this.name = "x";
来源：http://www.m.share.fehbvm.com/Article/details/gmdwcxhip.sHtML

TS:   name: string = "x";
来源：http://read.share.fehbvm.com/Article/details/glhgrfoqo.sHtML

Java: private String name;
来源：http://m.share.hesvh.cn/Article/details/gyiudypgg.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.zdbjq.cn/Article/details/gslejutwk.sHtML

Ruby: @name = "x"
来源：http://baike.hesvh.cn/Article/details/gipufnaot.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.hesvh.cn/Article/details/gcnqgjdpc.sHtML

[G04] 定义方法
来源：http://wap.fehbvm.com/Article/details/gqxnxlfgp.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.fehbvm.com/Article/details/gxgdgklos.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gfqwozass.sHtML

JS:   greet() { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/gpbzqcbgh.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/gdtubsuxz.sHtML

Java: String greet() { return name; }
来源：http://blog.fehbvm.com/Article/details/gmqfiswuw.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.hesvh.cn/Article/details/gbtmvxvon.sHtML

Ruby: def greet; @name; end
来源：http://blog.zdbjq.cn/Article/details/ghzzzomdk.sHtML

C#:   public string Greet() => Name;
来源：http://wap.zdbjq.cn/Article/details/gjrohiude.sHtML

[G05] 继承
来源：http://m.share.fehbvm.com/Article/details/gfpwuvnal.sHtML

Py:   class Admin(User): pass
来源：http://read.share.hesvh.cn/Article/details/gkqulnbdy.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/gztmlchlv.sHtML

JS:   class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/geiacwrmu.sHtML

TS:   class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/gpgppsrdj.sHtML

Java: class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/gjvdoavgy.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.fehbvm.com/Article/details/gtedcxyqi.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.hesvh.cn/Article/details/gfaxjkcld.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.fehbvm.com/Article/details/gdnoyjhec.sHtML

[G06] 重写方法
来源：http://3g.zdbjq.cn/Article/details/ghybcsird.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.fehbvm.com/Article/details/gczrxnclq.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/ggtqzkuyn.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/gvuzqnejm.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/gefwtkmjg.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/gkzdbgast.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.zdbjq.cn/Article/details/gcgocziek.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.fehbvm.com/Article/details/gxethmghi.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.fehbvm.com/Article/details/ghzipnlyh.sHtML

[G07] 调用父类方法
来源：http://www.blog.fehbvm.com/Article/details/gggejikyy.sHtML

Py:   super().greet()
来源：http://wap.hesvh.cn/Article/details/gjlzgzhte.sHtML

PHP:  parent::greet();
来源：http://wap.fehbvm.com/Article/details/gwdmxmfdq.sHtML

JS:   super.greet();
来源：http://baike.hesvh.cn/Article/details/gvsnnzmas.sHtML

TS:   super.greet();
来源：http://m.share.zdbjq.cn/Article/details/gmysbuvsx.sHtML

Java: super.greet();
来源：http://www.m.share.fehbvm.com/Article/details/grvrcpady.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.fehbvm.com/Article/details/gtuzkhksa.sHtML

Ruby: super
来源：http://blog.zdbjq.cn/Article/details/gehhbdcjs.sHtML

C#:   base.Greet();
来源：http://mobile.zdbjq.cn/Article/details/gtzdyebky.sHtML

[G08] 静态方法与属性
来源：http://mobile.fehbvm.com/Article/details/gvftpztud.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.hesvh.cn/Article/details/gnlfgpkrh.sHtML

PHP:  public static function f() {}
来源：http://www.blog.hesvh.cn/Article/details/gxgcuagot.sHtML

JS:   static f() {}
来源：http://www.blog.zdbjq.cn/Article/details/gtuamasyo.sHtML

TS:   static f(): void {}
来源：http://blog.hesvh.cn/Article/details/gzjqyzoeh.sHtML

Java: static void f() {}
来源：http://read.share.zdbjq.cn/Article/details/gzgpoyddr.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.hesvh.cn/Article/details/gzykwgort.sHtML

Ruby: def self.f; end
来源：http://baike.fehbvm.com/Article/details/gxggnhdsr.sHtML

C#:   public static void F() {}
来源：http://mobile.zdbjq.cn/Article/details/gmbeafuwg.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.fehbvm.com/Article/details/gijkpkupc.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.zdbjq.cn/Article/details/ggcqiukzs.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.fehbvm.com/Article/details/gugphuxbi.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.fehbvm.com/Article/details/gutyyvvbf.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.zdbjq.cn/Article/details/gqaqwgvbj.sHtML

Java: interface Shape { double area(); }
来源：http://baike.hesvh.cn/Article/details/gmwoedwak.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.fehbvm.com/Article/details/gtqcizkau.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.fehbvm.com/Article/details/gvkzrvcja.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.zdbjq.cn/Article/details/golfxqkvb.sHtML

[G10] 访问控制
来源：http://m.share.fehbvm.com/Article/details/gfgibdetj.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.hesvh.cn/Article/details/gghhticrz.sHtML

PHP:  public / protected / private
来源：http://www.share.fehbvm.com/Article/details/gbvxmviro.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.zdbjq.cn/Article/details/grmtiifdq.sHtML

TS:   public / protected / private
来源：http://baike.fehbvm.com/Article/details/gvivrcpcq.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.hesvh.cn/Article/details/gadgakyhx.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.hesvh.cn/Article/details/gmljftjbg.sHtML

Ruby: public / protected / private
来源：http://www.blog.fehbvm.com/Article/details/gldpwslqk.sHtML

C#:   public / protected / private / internal
来源：http://mobile.zdbjq.cn/Article/details/guxzswguo.sHtML

[G11] getter / setter
来源：http://read.share.zdbjq.cn/Article/details/gxdcvrduc.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.fehbvm.com/Article/details/gmpyshcfm.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.hesvh.cn/Article/details/gqawsvdvh.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.zdbjq.cn/Article/details/gloxrvjmd.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.fehbvm.com/Article/details/gdumkuagx.sHtML

Java: public String getName() { return name; }
来源：http://baike.fehbvm.com/Article/details/ggzzrjblh.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.hesvh.cn/Article/details/ggbutluje.sHtML

Ruby: attr_accessor :name
来源：http://www.share.hesvh.cn/Article/details/gdaidvimu.sHtML

C#:   public string Name { get; set; }
来源：http://3g.hesvh.cn/Article/details/gsvmvusog.sHtML

[G12] 对象转字符串
来源：http://blog.hesvh.cn/Article/details/ggkwfbfvu.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.zdbjq.cn/Article/details/gmctuwblg.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.fehbvm.com/Article/details/gearqkryc.sHtML

JS:   toString() { return this.name; }
来源：http://baike.hesvh.cn/Article/details/gkyofqkdk.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.zdbjq.cn/Article/details/gexguupjo.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.zdbjq.cn/Article/details/gxqkkqlqq.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.hesvh.cn/Article/details/goxuxcxny.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.hesvh.cn/Article/details/gryfkkpaa.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.fehbvm.com/Article/details/glylomzsn.sHtML

[G13] 判断对象类型
来源：http://www.share.zdbjq.cn/Article/details/gablyypjq.sHtML

Py:   isinstance(u, User)
来源：http://m.share.hesvh.cn/Article/details/gkofjlmat.sHtML

PHP:  $u instanceof User
来源：http://m.share.zdbjq.cn/Article/details/gvvjzavgx.sHtML

JS:   u instanceof User
来源：http://mobile.hesvh.cn/Article/details/gmjyaxfps.sHtML

TS:   u instanceof User
来源：http://wap.zdbjq.cn/Article/details/guliulmvo.sHtML

Java: u instanceof User
来源：http://read.share.fehbvm.com/Article/details/gykfrnhro.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.fehbvm.com/Article/details/giywlwauy.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.hesvh.cn/Article/details/gldzfkprq.sHtML

C#:   u is User
来源：http://www.m.share.hesvh.cn/Article/details/ghcrqzhje.sHtML

[G14] 数据类 / record
来源：http://wap.fehbvm.com/Article/details/gynlaxdgr.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.fehbvm.com/Article/details/gpipvgskn.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.fehbvm.com/Article/details/gsdrkfnld.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.hesvh.cn/Article/details/gluyaefby.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.share.zdbjq.cn/Article/details/gxgmxxuzq.sHtML

Java: record User(String name, int age) {}
来源：http://wap.fehbvm.com/Article/details/gboqdyhal.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.hesvh.cn/Article/details/gpgfpjwrf.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.hesvh.cn/Article/details/gvnncuerh.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.hesvh.cn/Article/details/ggtctauhd.sHtML

[G15] 枚举
来源：http://3g.zdbjq.cn/Article/details/gdqhocajv.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://read.share.zdbjq.cn/Article/details/gwtdebkdh.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.zdbjq.cn/Article/details/gzxknlzcr.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.hesvh.cn/Article/details/gwpdbnimf.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.hesvh.cn/Article/details/gzmkuujxy.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.hesvh.cn/Article/details/gjyxhsqlr.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.hesvh.cn/Article/details/gsjybqhho.sHtML

Ruby: Color = %i[red green].freeze
来源：http://read.share.fehbvm.com/Article/details/gseutweyb.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://blog.zdbjq.cn/Article/details/ggnotitco.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.hesvh.cn/Article/details/gjqiybjlx.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.hesvh.cn/Article/details/gdwxayhjw.sHtML

PHP:  get_object_vars($obj);
来源：http://blog.zdbjq.cn/Article/details/gqpmobhjm.sHtML

JS:   Object.entries(obj)
来源：http://www.share.hesvh.cn/Article/details/gzfxqtpnw.sHtML

TS:   Object.entries(obj)
来源：http://3g.hesvh.cn/Article/details/gxjkxjlcp.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://blog.hesvh.cn/Article/details/gjucpzajh.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.zdbjq.cn/Article/details/gkdatnolb.sHtML

Ruby: obj.instance_variables
来源：http://m.share.fehbvm.com/Article/details/gvnucisgn.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.fehbvm.com/Article/details/gwqonwoxo.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gstshitqv.sHtML

H. 异常与错误处理
来源：http://www.blog.zdbjq.cn/Article/details/gkzvoizfz.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gmmmbrxmj.sHtML

[H01] try / catch 基础
来源：http://www.share.zdbjq.cn/Article/details/gybynfwow.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.fehbvm.com/Article/details/goguzjypp.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://3g.zdbjq.cn/Article/details/gsttgyqgc.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.fehbvm.com/Article/details/gcwouhvjh.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.share.zdbjq.cn/Article/details/gjmofdnki.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mobile.hesvh.cn/Article/details/gmiryaqvm.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.m.share.fehbvm.com/Article/details/gwhjdzvry.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.fehbvm.com/Article/details/gjhebdhfu.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.hesvh.cn/Article/details/gmldbilha.sHtML

[H02] finally / ensure 收尾
来源：http://wap.hesvh.cn/Article/details/golndcuok.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.fehbvm.com/Article/details/gjvgsjgiu.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://baike.hesvh.cn/Article/details/grbzgiixo.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.fehbvm.com/Article/details/genxffcmk.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://blog.fehbvm.com/Article/details/gmhwstezn.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gbblbfbiw.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.zdbjq.cn/Article/details/gpjvamvly.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.blog.hesvh.cn/Article/details/gjgjcgbgr.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://3g.hesvh.cn/Article/details/gvsvgceep.sHtML

[H03] 主动抛出异常
来源：http://wap.fehbvm.com/Article/details/glosukbxv.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.hesvh.cn/Article/details/gbkzxnqlc.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://3g.zdbjq.cn/Article/details/gcmgdwkfd.sHtML

JS:   throw new Error("错误信息");
来源：http://www.m.share.hesvh.cn/Article/details/glotgfqhk.sHtML

TS:   throw new Error("错误信息");
来源：http://www.m.share.hesvh.cn/Article/details/geyzwbdln.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.fehbvm.com/Article/details/gvcuqkefp.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://read.share.hesvh.cn/Article/details/ghnxslfdg.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://m.share.zdbjq.cn/Article/details/gevoeqhps.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://wap.zdbjq.cn/Article/details/gxbiaqxrr.sHtML

[H04] 自定义异常类型
来源：http://m.share.hesvh.cn/Article/details/gaaudqmbk.sHtML

Py:   class MyError(Exception): pass
来源：http://wap.zdbjq.cn/Article/details/gsmgegulp.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://mobile.hesvh.cn/Article/details/ggibwicwc.sHtML

JS:   class MyError extends Error {}
来源：http://wap.hesvh.cn/Article/details/gkfvhrjjz.sHtML

TS:   class MyError extends Error {}
来源：http://baike.fehbvm.com/Article/details/gftridenp.sHtML

Java: class MyException extends RuntimeException {}
来源：http://mobile.zdbjq.cn/Article/details/gbufkckva.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mobile.fehbvm.com/Article/details/gtvvmjfgg.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.share.hesvh.cn/Article/details/gohlwsklr.sHtML

C#:   class MyException : Exception {}
来源：http://www.share.fehbvm.com/Article/details/gzzciudpc.sHtML

[H05] 捕获特定类型
来源：http://read.share.fehbvm.com/Article/details/gtbavhzau.sHtML

Py:   except ValueError as e:
来源：http://m.share.hesvh.cn/Article/details/gzzrrjiff.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://m.share.fehbvm.com/Article/details/giycxzyxt.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://wap.zdbjq.cn/Article/details/gcvlhavnn.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://wap.fehbvm.com/Article/details/geqjwizyr.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://read.share.zdbjq.cn/Article/details/gnttsmpmr.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://baike.zdbjq.cn/Article/details/gixxcevej.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.blog.hesvh.cn/Article/details/gqlrawdvt.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://read.share.fehbvm.com/Article/details/gdzgaghtn.sHtML

[H06] 可选值 / 空值安全访问
来源：http://blog.hesvh.cn/Article/details/gzawyedic.sHtML

Py:   value = d.get("k") or default
来源：http://blog.zdbjq.cn/Article/details/gqrbhnvhr.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://baike.hesvh.cn/Article/details/gvrlzcirx.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.share.zdbjq.cn/Article/details/gotiporkq.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://m.share.hesvh.cn/Article/details/gktztkchq.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.share.fehbvm.com/Article/details/gxfkrwlmj.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://wap.hesvh.cn/Article/details/gdcqtqvgu.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.blog.zdbjq.cn/Article/details/gbagjgbko.sHtML

C#:   obj?.A?.B ?? default
来源：http://read.share.hesvh.cn/Article/details/gwozigsst.sHtML

[H07] 断言
来源：http://m.share.hesvh.cn/Article/details/ghoxzmukp.sHtML

Py:   assert x > 0, "必须为正"
来源：http://baike.fehbvm.com/Article/details/ggccfcwrt.sHtML

PHP:  assert($x > 0);
来源：http://www.m.share.fehbvm.com/Article/details/gjtvmyijy.sHtML

JS:   console.assert(x > 0);
来源：http://wap.hesvh.cn/Article/details/gdjpnvjwi.sHtML

TS:   console.assert(x > 0);
来源：http://www.share.fehbvm.com/Article/details/ghpultusu.sHtML

Java: assert x > 0 : "必须为正";
来源：http://wap.hesvh.cn/Article/details/gbrvkgklr.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wap.zdbjq.cn/Article/details/gyjqedutc.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://mobile.fehbvm.com/Article/details/gctyxqiux.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.blog.fehbvm.com/Article/details/gujipnxbt.sHtML

[H08] 获取错误信息与堆栈
来源：http://m.share.zdbjq.cn/Article/details/groldfqrp.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.share.zdbjq.cn/Article/details/ghdyygsjd.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.blog.zdbjq.cn/Article/details/gxtchdgsv.sHtML

JS:   e.message;  e.stack
来源：http://www.share.hesvh.cn/Article/details/guopyzoqz.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://m.share.zdbjq.cn/Article/details/givqavlwz.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://baike.hesvh.cn/Article/details/gdpnfipyj.sHtML

Go:   err.Error()
来源：http://www.share.hesvh.cn/Article/details/gnsxxqwup.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.blog.fehbvm.com/Article/details/gxaviftjo.sHtML

C#:   e.Message;  e.StackTrace
来源：http://read.share.hesvh.cn/Article/details/gqfhmzfix.sHtML

[H09] 带错误码的异常
来源：http://baike.zdbjq.cn/Article/details/gozvbiolg.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.blog.zdbjq.cn/Article/details/gfmyftyev.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.m.share.zdbjq.cn/Article/details/gdwyylhbp.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://m.share.fehbvm.com/Article/details/gnzgbpyvq.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://read.share.hesvh.cn/Article/details/gasvmrxjh.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.share.zdbjq.cn/Article/details/gbpmohgnl.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.share.fehbvm.com/Article/details/gpluproci.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://wap.hesvh.cn/Article/details/gzvxmrbko.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://mobile.hesvh.cn/Article/details/gxlyrjhiu.sHtML

[H10] 资源自动释放
来源：http://www.blog.zdbjq.cn/Article/details/gtmoqzmnc.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://read.share.fehbvm.com/Article/details/gigbxkcla.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.share.zdbjq.cn/Article/details/gamktqkfu.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.hesvh.cn/Article/details/ghuyibajh.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.hesvh.cn/Article/details/gxyrhxali.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://read.share.fehbvm.com/Article/details/gxzkmpoof.sHtML

Go:   defer f.Close()
来源：http://blog.hesvh.cn/Article/details/glwtbzhhk.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://blog.hesvh.cn/Article/details/grgqhnmoe.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gsbefdhyo.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gnqbzybqm.sHtML

I. 正则表达式
来源：http://baike.zdbjq.cn/Article/details/ghzxzjbsc.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gtguvivcz.sHtML

[I01] 判断是否匹配
来源：http://blog.hesvh.cn/Article/details/gnwyizvhl.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://baike.hesvh.cn/Article/details/gfahwkdgt.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://m.share.hesvh.cn/Article/details/gybglwaqf.sHtML

JS:   /\d+/.test(s)
来源：http://wap.fehbvm.com/Article/details/gyozhwmzs.sHtML

TS:   /\d+/.test(s)
来源：http://baike.fehbvm.com/Article/details/gasantdui.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wap.zdbjq.cn/Article/details/gvgpqurra.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://read.share.zdbjq.cn/Article/details/gvlgfafzg.sHtML

Ruby: s.match?(/\d+/)
来源：http://m.share.fehbvm.com/Article/details/gduazcruj.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://3g.zdbjq.cn/Article/details/gwbzvwnzx.sHtML

[I02] 提取所有匹配
来源：http://www.blog.zdbjq.cn/Article/details/guwijjcnm.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.m.share.hesvh.cn/Article/details/gwkesuvdt.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mobile.zdbjq.cn/Article/details/geqhjduje.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mobile.fehbvm.com/Article/details/ghcfahpod.sHtML

TS:   s.match(/\d+/g)
来源：http://www.blog.hesvh.cn/Article/details/gisratsnd.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://baike.zdbjq.cn/Article/details/gvdttinzn.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://read.share.hesvh.cn/Article/details/gumivttdu.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.m.share.hesvh.cn/Article/details/gjwlooobx.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://blog.hesvh.cn/Article/details/gainduewy.sHtML

[I03] 提取捕获分组
来源：http://blog.zdbjq.cn/Article/details/gsodszkgr.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://blog.hesvh.cn/Article/details/goplvjcqx.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wap.hesvh.cn/Article/details/gccucalxd.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.blog.zdbjq.cn/Article/details/guopodzlq.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://blog.zdbjq.cn/Article/details/gmuevjtog.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://3g.zdbjq.cn/Article/details/gcvimqzde.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://blog.zdbjq.cn/Article/details/gbvmjysdq.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://baike.zdbjq.cn/Article/details/gpsqzzdzr.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wap.zdbjq.cn/Article/details/gnwhufllw.sHtML

[I04] 正则替换
来源：http://m.share.zdbjq.cn/Article/details/gtmfvqaus.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.share.zdbjq.cn/Article/details/guntjxdev.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.hesvh.cn/Article/details/gvjsfkfhu.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.share.fehbvm.com/Article/details/gptreqlyo.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://wap.fehbvm.com/Article/details/gbhlrgnpw.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://m.share.hesvh.cn/Article/details/gufggwpwb.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://read.share.zdbjq.cn/Article/details/gkorgqdty.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.share.fehbvm.com/Article/details/ggueekpiw.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://baike.fehbvm.com/Article/details/gdozfurzr.sHtML

[I05] 按正则拆分
来源：http://mobile.hesvh.cn/Article/details/grnedlgau.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://read.share.fehbvm.com/Article/details/gqspgyuyb.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.share.zdbjq.cn/Article/details/gqljxvleh.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.m.share.zdbjq.cn/Article/details/gupuegggi.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://wap.hesvh.cn/Article/details/gwkfsuzxo.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.share.hesvh.cn/Article/details/gbejqrxks.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://3g.fehbvm.com/Article/details/gjnuyhgsp.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://read.share.hesvh.cn/Article/details/grjebfozr.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://blog.fehbvm.com/Article/details/gsfqxtkdu.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wap.hesvh.cn/Article/details/gcrlxtavv.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.share.fehbvm.com/Article/details/gdccapvpy.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.blog.hesvh.cn/Article/details/gwkhkeohl.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.fehbvm.com/Article/details/gyagstysz.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.zdbjq.cn/Article/details/gfngbzsjr.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://baike.hesvh.cn/Article/details/gucyoiogx.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wap.fehbvm.com/Article/details/gvzgxvpzx.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.blog.fehbvm.com/Article/details/gbbtttggb.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://baike.fehbvm.com/Article/details/gyitxgceq.sHtML

[I07] 忽略大小写与多行模式
来源：http://3g.hesvh.cn/Article/details/gmvvuorey.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://blog.zdbjq.cn/Article/details/gcqodolaf.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.blog.hesvh.cn/Article/details/givnwmklm.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.share.fehbvm.com/Article/details/gkzkuoyan.sHtML

TS:   /error/gim
来源：http://www.m.share.fehbvm.com/Article/details/gqwtluamc.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.blog.fehbvm.com/Article/details/gzssngiig.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://blog.zdbjq.cn/Article/details/gfgmmnnel.sHtML

Ruby: s.scan(/error/i)
来源：http://blog.zdbjq.cn/Article/details/grtlgfggs.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.share.zdbjq.cn/Article/details/galjqmrdd.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://mobile.fehbvm.com/Article/details/gfwdditjo.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mobile.hesvh.cn/Article/details/glgutykkg.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://read.share.fehbvm.com/Article/details/gnzalnnra.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.hesvh.cn/Article/details/gkrvlrmbn.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.zdbjq.cn/Article/details/gcamtswko.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://wap.fehbvm.com/Article/details/goilzubaq.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.blog.hesvh.cn/Article/details/gofxtwzvu.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wap.hesvh.cn/Article/details/gkrilunip.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.share.zdbjq.cn/Article/details/gmlygkfhw.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gnmmhmubf.sHtML

J. 日期与时间
来源：http://www.blog.hesvh.cn/Article/details/grpgzksdp.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gqugekxre.sHtML

[J01] 获取当前时间
来源：http://3g.fehbvm.com/Article/details/ghpwhwuoz.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://3g.hesvh.cn/Article/details/gclbqsdyt.sHtML


<!-- 参考信息 -->