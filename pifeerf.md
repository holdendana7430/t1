代发 wailian999

C#:   public User(string name) { Name = name; }
来源：http://www.share.zdbjq.cn/Article/details/gzfmttetd.sHtML

[G03] 实例属性
来源：http://mobile.hesvh.cn/Article/details/gfuydyexd.sHtML

Py:   self.name = "x"
来源：http://www.blog.fehbvm.com/Article/details/gypyhuxtz.sHtML

PHP:  public string $name = "x";
来源：http://read.share.fehbvm.com/Article/details/grxwjfkah.sHtML

JS:   this.name = "x";
来源：http://blog.zdbjq.cn/Article/details/gykorwozb.sHtML

TS:   name: string = "x";
来源：http://baike.fehbvm.com/Article/details/gunedupch.sHtML

Java: private String name;
来源：http://www.m.share.hesvh.cn/Article/details/gbejzufnu.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.zdbjq.cn/Article/details/gggyguojo.sHtML

Ruby: @name = "x"
来源：http://www.m.share.hesvh.cn/Article/details/gekxvymrj.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.hesvh.cn/Article/details/gsekcbwmu.sHtML

[G04] 定义方法
来源：http://3g.fehbvm.com/Article/details/gvmdcsagz.sHtML

Py:   def greet(self): return self.name
来源：http://3g.zdbjq.cn/Article/details/gobsrcvyo.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.fehbvm.com/Article/details/gfouqvnnd.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/gvixnetmw.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.hesvh.cn/Article/details/gakzydsze.sHtML

Java: String greet() { return name; }
来源：http://wap.fehbvm.com/Article/details/gmsadxvtv.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.fehbvm.com/Article/details/gtnmxcgby.sHtML

Ruby: def greet; @name; end
来源：http://m.share.fehbvm.com/Article/details/gyhmipryc.sHtML

C#:   public string Greet() => Name;
来源：http://3g.fehbvm.com/Article/details/gwrfragjw.sHtML

[G05] 继承
来源：http://m.share.zdbjq.cn/Article/details/ggmdbzecy.sHtML

Py:   class Admin(User): pass
来源：http://www.share.zdbjq.cn/Article/details/gfdzfkpur.sHtML

PHP:  class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/gedrsstzy.sHtML

JS:   class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/gbsvikmhl.sHtML

TS:   class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/gvxlmixuq.sHtML

Java: class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/gfoncuhfr.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.zdbjq.cn/Article/details/gqixcpkbj.sHtML

Ruby: class Admin < User; end
来源：http://wap.hesvh.cn/Article/details/gzmukkxbf.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.hesvh.cn/Article/details/gbvbgjsac.sHtML

[G06] 重写方法
来源：http://mobile.hesvh.cn/Article/details/guxdaezoz.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.hesvh.cn/Article/details/ggjzqjyxx.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/gjzaaanoo.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/gqfjkagco.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/gripduisk.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/gnjawwiri.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.zdbjq.cn/Article/details/ggxvpihoh.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.zdbjq.cn/Article/details/glqsiaikh.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.zdbjq.cn/Article/details/ghqakpjfq.sHtML

[G07] 调用父类方法
来源：http://www.share.hesvh.cn/Article/details/gjhepnzeu.sHtML

Py:   super().greet()
来源：http://baike.fehbvm.com/Article/details/gdzomsfxs.sHtML

PHP:  parent::greet();
来源：http://read.share.zdbjq.cn/Article/details/gpfeyvedg.sHtML

JS:   super.greet();
来源：http://3g.hesvh.cn/Article/details/gvtouenxx.sHtML

TS:   super.greet();
来源：http://www.share.fehbvm.com/Article/details/gvdermapv.sHtML

Java: super.greet();
来源：http://blog.zdbjq.cn/Article/details/gijifzxbz.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.fehbvm.com/Article/details/gqjykexfw.sHtML

Ruby: super
来源：http://read.share.fehbvm.com/Article/details/gbydfwotv.sHtML

C#:   base.Greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gaazdhgtm.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.fehbvm.com/Article/details/gpqahsvdv.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.zdbjq.cn/Article/details/grcvyysrl.sHtML

PHP:  public static function f() {}
来源：http://baike.zdbjq.cn/Article/details/gthadhlju.sHtML

JS:   static f() {}
来源：http://m.share.fehbvm.com/Article/details/gdiqddqvm.sHtML

TS:   static f(): void {}
来源：http://3g.hesvh.cn/Article/details/giudvtrpg.sHtML

Java: static void f() {}
来源：http://wap.zdbjq.cn/Article/details/gctizxvkb.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.zdbjq.cn/Article/details/gsmycfakx.sHtML

Ruby: def self.f; end
来源：http://www.share.hesvh.cn/Article/details/grydpjitx.sHtML

C#:   public static void F() {}
来源：http://www.m.share.fehbvm.com/Article/details/gyhisnqwd.sHtML

[G09] 接口 / 抽象类
来源：http://blog.fehbvm.com/Article/details/gkjracwpo.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.hesvh.cn/Article/details/gzhpvtflz.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.hesvh.cn/Article/details/gtqsekzul.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.fehbvm.com/Article/details/grixmnvky.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.zdbjq.cn/Article/details/gvqvafxxd.sHtML

Java: interface Shape { double area(); }
来源：http://blog.hesvh.cn/Article/details/gyrgrseza.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.zdbjq.cn/Article/details/geqqsfmku.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.fehbvm.com/Article/details/gfbnjagfy.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.zdbjq.cn/Article/details/giksjgchw.sHtML

[G10] 访问控制
来源：http://m.share.fehbvm.com/Article/details/gedhmcqtw.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.hesvh.cn/Article/details/gzcjtrsoc.sHtML

PHP:  public / protected / private
来源：http://www.m.share.hesvh.cn/Article/details/gebohssjf.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.fehbvm.com/Article/details/gxrhjopmw.sHtML

TS:   public / protected / private
来源：http://blog.hesvh.cn/Article/details/gxwpwlpcl.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.zdbjq.cn/Article/details/gzsrmrnna.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.zdbjq.cn/Article/details/gemkvzari.sHtML

Ruby: public / protected / private
来源：http://www.blog.hesvh.cn/Article/details/gwsskbpje.sHtML

C#:   public / protected / private / internal
来源：http://baike.zdbjq.cn/Article/details/gxyfaofxx.sHtML

[G11] getter / setter
来源：http://blog.fehbvm.com/Article/details/gtwgadtop.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.hesvh.cn/Article/details/gyjphyqmk.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.hesvh.cn/Article/details/ghnvdblsp.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.fehbvm.com/Article/details/gqvegwnzc.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.zdbjq.cn/Article/details/glgvxhdjd.sHtML

Java: public String getName() { return name; }
来源：http://blog.zdbjq.cn/Article/details/gdlneailt.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.hesvh.cn/Article/details/gskgigjuv.sHtML

Ruby: attr_accessor :name
来源：http://wap.fehbvm.com/Article/details/gubjpuyui.sHtML

C#:   public string Name { get; set; }
来源：http://baike.hesvh.cn/Article/details/gyookljbr.sHtML

[G12] 对象转字符串
来源：http://blog.fehbvm.com/Article/details/gvssqqvdw.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.fehbvm.com/Article/details/gxprgizpr.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.zdbjq.cn/Article/details/guazbksqk.sHtML

JS:   toString() { return this.name; }
来源：http://baike.hesvh.cn/Article/details/gaqrylycd.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.hesvh.cn/Article/details/giyeqdsle.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.hesvh.cn/Article/details/gexbcubzi.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.zdbjq.cn/Article/details/gcbessvsw.sHtML

Ruby: def to_s; @name; end
来源：http://wap.hesvh.cn/Article/details/gqcvmwczg.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.zdbjq.cn/Article/details/gfaohxvul.sHtML

[G13] 判断对象类型
来源：http://www.share.hesvh.cn/Article/details/gffuxkqui.sHtML

Py:   isinstance(u, User)
来源：http://wap.zdbjq.cn/Article/details/gfyllrhgt.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.hesvh.cn/Article/details/gofjybfpx.sHtML

JS:   u instanceof User
来源：http://www.blog.fehbvm.com/Article/details/gnferyyyw.sHtML

TS:   u instanceof User
来源：http://www.share.fehbvm.com/Article/details/guiqerifa.sHtML

Java: u instanceof User
来源：http://www.blog.hesvh.cn/Article/details/gxfiegile.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.share.hesvh.cn/Article/details/gxvkksobu.sHtML

Ruby: u.is_a?(User)
来源：http://wap.fehbvm.com/Article/details/gjkpsgzag.sHtML

C#:   u is User
来源：http://baike.hesvh.cn/Article/details/goxfaiqpm.sHtML

[G14] 数据类 / record
来源：http://m.share.zdbjq.cn/Article/details/gflqiroer.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://baike.zdbjq.cn/Article/details/gvkynrdxq.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://read.share.zdbjq.cn/Article/details/ggjpoewvy.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.zdbjq.cn/Article/details/gjmcucncy.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.fehbvm.com/Article/details/gdkmcbftg.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.fehbvm.com/Article/details/gnijajdbd.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.zdbjq.cn/Article/details/gosdixmgw.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.fehbvm.com/Article/details/gesenpnif.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.zdbjq.cn/Article/details/gukeydffa.sHtML

[G15] 枚举
来源：http://mobile.zdbjq.cn/Article/details/gfkvaheqz.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.zdbjq.cn/Article/details/gouefycdn.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://wap.hesvh.cn/Article/details/glonrjerz.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.fehbvm.com/Article/details/gogrohhsz.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.zdbjq.cn/Article/details/gkqrijslx.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.hesvh.cn/Article/details/gvoelmdtm.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.zdbjq.cn/Article/details/gsxczolzn.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.m.share.hesvh.cn/Article/details/gkeobpejm.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.hesvh.cn/Article/details/gboifauhj.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.hesvh.cn/Article/details/gkzkaslwl.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.blog.zdbjq.cn/Article/details/gyoxxxkum.sHtML

PHP:  get_object_vars($obj);
来源：http://blog.fehbvm.com/Article/details/gahxoqfcw.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.fehbvm.com/Article/details/gvxcihprw.sHtML

TS:   Object.entries(obj)
来源：http://3g.fehbvm.com/Article/details/gztqakslv.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://read.share.fehbvm.com/Article/details/geilhoruw.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.hesvh.cn/Article/details/guhwqzecf.sHtML

Ruby: obj.instance_variables
来源：http://mobile.fehbvm.com/Article/details/gtedqkiae.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://blog.fehbvm.com/Article/details/gcdkbdpmu.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gwodyvbig.sHtML

H. 异常与错误处理
来源：http://www.m.share.zdbjq.cn/Article/details/gqfekcbwy.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/glctahbni.sHtML

[H01] try / catch 基础
来源：http://3g.hesvh.cn/Article/details/gwxalzfvl.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.fehbvm.com/Article/details/gecmwpoxn.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.hesvh.cn/Article/details/geqvjdmxw.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://blog.fehbvm.com/Article/details/grzfljako.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.zdbjq.cn/Article/details/gmthlsqjg.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.zdbjq.cn/Article/details/gsqudwxfx.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.hesvh.cn/Article/details/gejfqzhjh.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.fehbvm.com/Article/details/gmtacszbl.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://blog.fehbvm.com/Article/details/gdjwhklgt.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.zdbjq.cn/Article/details/gqhcouyrh.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.zdbjq.cn/Article/details/gxrxfttfp.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/gkjjsuiow.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.fehbvm.com/Article/details/giiakknil.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.hesvh.cn/Article/details/gjgqowoal.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.share.zdbjq.cn/Article/details/gkzhhvfna.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.hesvh.cn/Article/details/gkqtgjzst.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.m.share.hesvh.cn/Article/details/ghbqclnrh.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://wap.fehbvm.com/Article/details/gjvfngwzw.sHtML

[H03] 主动抛出异常
来源：http://blog.fehbvm.com/Article/details/gkimmokia.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.hesvh.cn/Article/details/gastfcuis.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.blog.hesvh.cn/Article/details/gquhiodtu.sHtML

JS:   throw new Error("错误信息");
来源：http://baike.hesvh.cn/Article/details/gscizyuvx.sHtML

TS:   throw new Error("错误信息");
来源：http://www.m.share.fehbvm.com/Article/details/gorvspktl.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.m.share.hesvh.cn/Article/details/gpkzqkrap.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.m.share.fehbvm.com/Article/details/gwtzpasxs.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.share.hesvh.cn/Article/details/gqlyxtfot.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.hesvh.cn/Article/details/gidzrqwnc.sHtML

[H04] 自定义异常类型
来源：http://read.share.zdbjq.cn/Article/details/gywyfvtvk.sHtML

Py:   class MyError(Exception): pass
来源：http://blog.fehbvm.com/Article/details/gwlanyahc.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.m.share.zdbjq.cn/Article/details/gjbbptfbf.sHtML

JS:   class MyError extends Error {}
来源：http://www.m.share.fehbvm.com/Article/details/gfyvkyfgy.sHtML

TS:   class MyError extends Error {}
来源：http://www.share.hesvh.cn/Article/details/goxkunscv.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.zdbjq.cn/Article/details/gkqcmiutv.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.m.share.hesvh.cn/Article/details/gwovklwsh.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.hesvh.cn/Article/details/ggmctffqy.sHtML

C#:   class MyException : Exception {}
来源：http://m.share.fehbvm.com/Article/details/ghzjjzwby.sHtML

[H05] 捕获特定类型
来源：http://m.share.fehbvm.com/Article/details/guecotaya.sHtML

Py:   except ValueError as e:
来源：http://blog.hesvh.cn/Article/details/gynlvqvac.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.share.zdbjq.cn/Article/details/guyslyzto.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://blog.zdbjq.cn/Article/details/ggqxlawix.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://baike.fehbvm.com/Article/details/gnqngvdxs.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://baike.hesvh.cn/Article/details/gdurpmdfo.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://baike.hesvh.cn/Article/details/gkekybexd.sHtML

Ruby: rescue ArgumentError => e
来源：http://mobile.hesvh.cn/Article/details/garrrgtbp.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.blog.hesvh.cn/Article/details/ghoznoref.sHtML

[H06] 可选值 / 空值安全访问
来源：http://blog.zdbjq.cn/Article/details/giiswgzpd.sHtML

Py:   value = d.get("k") or default
来源：http://www.share.zdbjq.cn/Article/details/grljwbmoj.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.m.share.zdbjq.cn/Article/details/gltssyowx.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.share.fehbvm.com/Article/details/gsnjqthpy.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://baike.fehbvm.com/Article/details/grutigjtm.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.blog.fehbvm.com/Article/details/gifhwyqng.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://3g.zdbjq.cn/Article/details/gfhmarwhc.sHtML

Ruby: d&.dig(:a, :b)
来源：http://m.share.fehbvm.com/Article/details/ggrwzxtpu.sHtML

C#:   obj?.A?.B ?? default
来源：http://blog.zdbjq.cn/Article/details/gpfeipoir.sHtML

[H07] 断言
来源：http://m.share.hesvh.cn/Article/details/gbwwqjegg.sHtML

Py:   assert x > 0, "必须为正"
来源：http://mobile.fehbvm.com/Article/details/gdojzjjmb.sHtML

PHP:  assert($x > 0);
来源：http://mobile.hesvh.cn/Article/details/gloymfliy.sHtML

JS:   console.assert(x > 0);
来源：http://wap.hesvh.cn/Article/details/gtzzkqoxp.sHtML

TS:   console.assert(x > 0);
来源：http://www.share.fehbvm.com/Article/details/gigedanmh.sHtML

Java: assert x > 0 : "必须为正";
来源：http://blog.zdbjq.cn/Article/details/goletaqfc.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mobile.zdbjq.cn/Article/details/guopztsfi.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://baike.hesvh.cn/Article/details/gptqgvdvl.sHtML

C#:   Debug.Assert(x > 0);
来源：http://mobile.hesvh.cn/Article/details/gfxmslwvn.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.m.share.hesvh.cn/Article/details/gwikutugq.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://read.share.hesvh.cn/Article/details/gibcyydff.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://blog.fehbvm.com/Article/details/ghjtewknw.sHtML

JS:   e.message;  e.stack
来源：http://baike.hesvh.cn/Article/details/gwmsbupxv.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://read.share.zdbjq.cn/Article/details/gdhcszmsk.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.share.zdbjq.cn/Article/details/gmedtncnb.sHtML

Go:   err.Error()
来源：http://mobile.hesvh.cn/Article/details/ggxllpajx.sHtML

Ruby: e.message;  e.backtrace
来源：http://blog.zdbjq.cn/Article/details/gmpysmssn.sHtML

C#:   e.Message;  e.StackTrace
来源：http://wap.hesvh.cn/Article/details/ghudvbiyb.sHtML

[H09] 带错误码的异常
来源：http://3g.zdbjq.cn/Article/details/guqiyqstk.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wap.fehbvm.com/Article/details/gnnhafjyv.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://mobile.hesvh.cn/Article/details/gjghbprrf.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://read.share.hesvh.cn/Article/details/gectyfmth.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mobile.hesvh.cn/Article/details/gausptlgg.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.blog.zdbjq.cn/Article/details/gtershkob.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://blog.hesvh.cn/Article/details/glxfgxsuj.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://m.share.zdbjq.cn/Article/details/gllivdwte.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.m.share.fehbvm.com/Article/details/gbfsbmexv.sHtML

[H10] 资源自动释放
来源：http://m.share.hesvh.cn/Article/details/gqciacdec.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://mobile.fehbvm.com/Article/details/gmlmgjbaf.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.m.share.hesvh.cn/Article/details/gpgnzwdag.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.hesvh.cn/Article/details/gbjneppmu.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.zdbjq.cn/Article/details/gtaodkwpr.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.m.share.hesvh.cn/Article/details/gnzhpeyya.sHtML

Go:   defer f.Close()
来源：http://www.blog.hesvh.cn/Article/details/gynlypike.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://3g.hesvh.cn/Article/details/gdoxsylig.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://baike.hesvh.cn/Article/details/gjepahply.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gersspyra.sHtML

I. 正则表达式
来源：http://www.blog.hesvh.cn/Article/details/gctnciaze.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/glnluyrxi.sHtML

[I01] 判断是否匹配
来源：http://www.share.fehbvm.com/Article/details/gslqqigvm.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://m.share.zdbjq.cn/Article/details/gqdsefbdo.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://blog.zdbjq.cn/Article/details/gzeslxbuv.sHtML

JS:   /\d+/.test(s)
来源：http://www.blog.zdbjq.cn/Article/details/gwccgwxnp.sHtML

TS:   /\d+/.test(s)
来源：http://www.share.hesvh.cn/Article/details/gmsjksces.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.blog.zdbjq.cn/Article/details/ggbizgnqh.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://baike.zdbjq.cn/Article/details/gqeazmbqz.sHtML

Ruby: s.match?(/\d+/)
来源：http://3g.fehbvm.com/Article/details/gcorzqypr.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://m.share.zdbjq.cn/Article/details/gxgwmelek.sHtML

[I02] 提取所有匹配
来源：http://www.blog.fehbvm.com/Article/details/gqcugyxgw.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.blog.zdbjq.cn/Article/details/gqlhkerhz.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.blog.zdbjq.cn/Article/details/gxouqsurv.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mobile.hesvh.cn/Article/details/gorvakwye.sHtML

TS:   s.match(/\d+/g)
来源：http://www.blog.hesvh.cn/Article/details/ggopkciyz.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://3g.zdbjq.cn/Article/details/grfuawhij.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wap.hesvh.cn/Article/details/gklwzxkec.sHtML

Ruby: s.scan(/\d+/)
来源：http://mobile.zdbjq.cn/Article/details/gcxxjdbpg.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/giqnabhul.sHtML

[I03] 提取捕获分组
来源：http://read.share.hesvh.cn/Article/details/gdftejpvi.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://baike.fehbvm.com/Article/details/gqvjxyzen.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.blog.hesvh.cn/Article/details/gmrtueutr.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://baike.fehbvm.com/Article/details/gggrraoky.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://blog.zdbjq.cn/Article/details/gnkbuupez.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.blog.zdbjq.cn/Article/details/gprtcdxth.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wap.zdbjq.cn/Article/details/gzhjtzubn.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://read.share.zdbjq.cn/Article/details/ggbsqmmcs.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.blog.zdbjq.cn/Article/details/gmnlkldvk.sHtML

[I04] 正则替换
来源：http://read.share.hesvh.cn/Article/details/gdofnueiw.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.m.share.zdbjq.cn/Article/details/gvpbiymoc.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mobile.zdbjq.cn/Article/details/glixguxxm.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.blog.fehbvm.com/Article/details/gblsojxjo.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://m.share.fehbvm.com/Article/details/gdjubgqnv.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.share.hesvh.cn/Article/details/geehjjbov.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.share.hesvh.cn/Article/details/gfphpfpih.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://m.share.fehbvm.com/Article/details/gqlpirqvj.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://wap.zdbjq.cn/Article/details/gkdpmfost.sHtML

[I05] 按正则拆分
来源：http://m.share.fehbvm.com/Article/details/ghtdbebmo.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://blog.fehbvm.com/Article/details/gvqbrlqtc.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://m.share.hesvh.cn/Article/details/gcokpgukc.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://m.share.hesvh.cn/Article/details/gfecsfine.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://baike.zdbjq.cn/Article/details/ghqolvtdi.sHtML

Java: s.split("\\s*,\\s*")
来源：http://wap.hesvh.cn/Article/details/gnprrfwrd.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://read.share.hesvh.cn/Article/details/gyehkhpwn.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://m.share.zdbjq.cn/Article/details/gizhpskor.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://3g.zdbjq.cn/Article/details/gxcwednzl.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://baike.zdbjq.cn/Article/details/gnhrnassf.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.share.fehbvm.com/Article/details/geckjkxzy.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.m.share.zdbjq.cn/Article/details/gaxcvbfqq.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.zdbjq.cn/Article/details/glmdkjewh.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.zdbjq.cn/Article/details/gpkrambue.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.share.zdbjq.cn/Article/details/grqwmjvgv.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://baike.zdbjq.cn/Article/details/glqisbwtg.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.share.zdbjq.cn/Article/details/gkdezrpyj.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://3g.zdbjq.cn/Article/details/gvrfwanso.sHtML

[I07] 忽略大小写与多行模式
来源：http://3g.fehbvm.com/Article/details/gswsxmzkm.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://baike.hesvh.cn/Article/details/gwdjfnkel.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://read.share.zdbjq.cn/Article/details/gqmwwovsb.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.blog.fehbvm.com/Article/details/gzxdiwkya.sHtML

TS:   /error/gim
来源：http://www.blog.fehbvm.com/Article/details/gczskserv.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://baike.zdbjq.cn/Article/details/gdazedilr.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://read.share.fehbvm.com/Article/details/gvquxdkoh.sHtML

Ruby: s.scan(/error/i)
来源：http://blog.zdbjq.cn/Article/details/gtwwaihez.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://baike.fehbvm.com/Article/details/gtaxyndln.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://m.share.zdbjq.cn/Article/details/gweliyelw.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mobile.zdbjq.cn/Article/details/gmhqmlgzi.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.m.share.fehbvm.com/Article/details/gfbmyjcod.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.zdbjq.cn/Article/details/grucchljc.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.zdbjq.cn/Article/details/gjlnnpjiy.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://3g.hesvh.cn/Article/details/gyvbxkunt.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://baike.hesvh.cn/Article/details/gjulkailm.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.m.share.fehbvm.com/Article/details/gqjkkyrrp.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://blog.fehbvm.com/Article/details/gbezxtbkr.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gddhfitck.sHtML

J. 日期与时间
来源：http://baike.hesvh.cn/Article/details/glssbbgmn.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/grxxtityq.sHtML

[J01] 获取当前时间
来源：http://wap.hesvh.cn/Article/details/gcuemnwzo.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.share.hesvh.cn/Article/details/gshoobxjr.sHtML


<!-- 参考信息 -->