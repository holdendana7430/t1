代发 wailian999

Ruby: @name = "x"
来源：http://read.share.zdbjq.cn/Article/details/ggwtqebsa.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.zdbjq.cn/Article/details/gjtlrkezv.sHtML

[G04] 定义方法
来源：http://www.share.fehbvm.com/Article/details/gflhzreut.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.hesvh.cn/Article/details/gxndqndmx.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.fehbvm.com/Article/details/gditceqhn.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/gqtnzhlel.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.hesvh.cn/Article/details/gthylaykc.sHtML

Java: String greet() { return name; }
来源：http://m.share.hesvh.cn/Article/details/guhgjwmxv.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.hesvh.cn/Article/details/gxlfxuefj.sHtML

Ruby: def greet; @name; end
来源：http://wap.fehbvm.com/Article/details/gnjpddzew.sHtML

C#:   public string Greet() => Name;
来源：http://baike.hesvh.cn/Article/details/gavstrwmo.sHtML

[G05] 继承
来源：http://baike.hesvh.cn/Article/details/gurdwioas.sHtML

Py:   class Admin(User): pass
来源：http://mobile.hesvh.cn/Article/details/gtrlnebsi.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/gedwdeump.sHtML

JS:   class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/gfxuagawy.sHtML

TS:   class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/gdfrndpoa.sHtML

Java: class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/gdpgztruj.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.hesvh.cn/Article/details/gcgcfpfmt.sHtML

Ruby: class Admin < User; end
来源：http://m.share.zdbjq.cn/Article/details/gvgivvlpk.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.fehbvm.com/Article/details/gdeqwwqnr.sHtML

[G06] 重写方法
来源：http://wap.zdbjq.cn/Article/details/gyjcyidlm.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.zdbjq.cn/Article/details/gdqsiqviy.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/ghpjknxhy.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/gixlgwhxh.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/gknguhord.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.zdbjq.cn/Article/details/gbwzzlsms.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.fehbvm.com/Article/details/gqntafxdh.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.fehbvm.com/Article/details/gspohpjnl.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.fehbvm.com/Article/details/gebmeyhfy.sHtML

[G07] 调用父类方法
来源：http://www.blog.zdbjq.cn/Article/details/gumxtknhh.sHtML

Py:   super().greet()
来源：http://read.share.zdbjq.cn/Article/details/gtuenkdau.sHtML

PHP:  parent::greet();
来源：http://3g.zdbjq.cn/Article/details/gyqfzifmx.sHtML

JS:   super.greet();
来源：http://www.blog.zdbjq.cn/Article/details/gxsdpxqog.sHtML

TS:   super.greet();
来源：http://wap.hesvh.cn/Article/details/gdlsonqtc.sHtML

Java: super.greet();
来源：http://www.blog.hesvh.cn/Article/details/guordgksw.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.hesvh.cn/Article/details/glbuhgrxt.sHtML

Ruby: super
来源：http://www.m.share.zdbjq.cn/Article/details/gpdsqwzhl.sHtML

C#:   base.Greet();
来源：http://www.share.zdbjq.cn/Article/details/gxjriofsl.sHtML

[G08] 静态方法与属性
来源：http://www.blog.fehbvm.com/Article/details/gkdfomqto.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.fehbvm.com/Article/details/ggqroygvs.sHtML

PHP:  public static function f() {}
来源：http://read.share.zdbjq.cn/Article/details/gzravlibx.sHtML

JS:   static f() {}
来源：http://baike.hesvh.cn/Article/details/gfyvsjgrm.sHtML

TS:   static f(): void {}
来源：http://www.share.zdbjq.cn/Article/details/gwvfdtbmg.sHtML

Java: static void f() {}
来源：http://3g.zdbjq.cn/Article/details/gexvondme.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.fehbvm.com/Article/details/gkvxctuze.sHtML

Ruby: def self.f; end
来源：http://wap.hesvh.cn/Article/details/gqhrwfgtw.sHtML

C#:   public static void F() {}
来源：http://www.m.share.hesvh.cn/Article/details/gejrcgkcg.sHtML

[G09] 接口 / 抽象类
来源：http://baike.zdbjq.cn/Article/details/gjgumtqad.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.zdbjq.cn/Article/details/gqllcssxf.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.hesvh.cn/Article/details/gxyubkpzv.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.fehbvm.com/Article/details/gwlgsxfqn.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.fehbvm.com/Article/details/guvhxrmrr.sHtML

Java: interface Shape { double area(); }
来源：http://wap.zdbjq.cn/Article/details/ghvqeisne.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.hesvh.cn/Article/details/gzimqdgrl.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.hesvh.cn/Article/details/gzqvvajej.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.hesvh.cn/Article/details/gaxvugurj.sHtML

[G10] 访问控制
来源：http://blog.fehbvm.com/Article/details/gbmdmhrws.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.hesvh.cn/Article/details/gmqahxjvc.sHtML

PHP:  public / protected / private
来源：http://www.blog.hesvh.cn/Article/details/gjctfyqxw.sHtML

JS:   #private 字段；其余公开
来源：http://baike.hesvh.cn/Article/details/gctqrjgmx.sHtML

TS:   public / protected / private
来源：http://www.share.fehbvm.com/Article/details/gygrmzuwm.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.fehbvm.com/Article/details/gvrmznfip.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.hesvh.cn/Article/details/gsgydrjjw.sHtML

Ruby: public / protected / private
来源：http://wap.hesvh.cn/Article/details/gbqiyiuxp.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.zdbjq.cn/Article/details/glatzahlq.sHtML

[G11] getter / setter
来源：http://mobile.zdbjq.cn/Article/details/gatjovccd.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.hesvh.cn/Article/details/gxhamjrxu.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.fehbvm.com/Article/details/gttkxktio.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.zdbjq.cn/Article/details/gosecsvfm.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.zdbjq.cn/Article/details/gjzptqxwz.sHtML

Java: public String getName() { return name; }
来源：http://3g.fehbvm.com/Article/details/ggasnwmll.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.hesvh.cn/Article/details/gzspcdfed.sHtML

Ruby: attr_accessor :name
来源：http://www.share.fehbvm.com/Article/details/grwtlbevf.sHtML

C#:   public string Name { get; set; }
来源：http://wap.fehbvm.com/Article/details/gajcsiwew.sHtML

[G12] 对象转字符串
来源：http://3g.fehbvm.com/Article/details/gznwlfnio.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.fehbvm.com/Article/details/gxybgvkew.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.fehbvm.com/Article/details/gqvjrkeoz.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/gerzoffhl.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.hesvh.cn/Article/details/gkvoadxul.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.hesvh.cn/Article/details/gdxxswgpb.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.zdbjq.cn/Article/details/gqxppvram.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.hesvh.cn/Article/details/gplvznlzg.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.fehbvm.com/Article/details/gxhjooret.sHtML

[G13] 判断对象类型
来源：http://wap.hesvh.cn/Article/details/gpxnsloeg.sHtML

Py:   isinstance(u, User)
来源：http://www.share.fehbvm.com/Article/details/gjqjzhixc.sHtML

PHP:  $u instanceof User
来源：http://www.blog.zdbjq.cn/Article/details/gwokmyrel.sHtML

JS:   u instanceof User
来源：http://baike.fehbvm.com/Article/details/gaommjdtf.sHtML

TS:   u instanceof User
来源：http://baike.hesvh.cn/Article/details/gxjeuzzlo.sHtML

Java: u instanceof User
来源：http://wap.fehbvm.com/Article/details/griswitge.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.zdbjq.cn/Article/details/gwovcbrld.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.hesvh.cn/Article/details/gdgzqqlms.sHtML

C#:   u is User
来源：http://m.share.hesvh.cn/Article/details/gdzvwnsqp.sHtML

[G14] 数据类 / record
来源：http://read.share.hesvh.cn/Article/details/gfnkbolfa.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.zdbjq.cn/Article/details/ggvaizfmq.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.zdbjq.cn/Article/details/geyiniyjk.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.hesvh.cn/Article/details/gnlfmfisy.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.zdbjq.cn/Article/details/gbbotbmdz.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.fehbvm.com/Article/details/gxmmleauh.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.fehbvm.com/Article/details/gyejcdfwu.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.fehbvm.com/Article/details/gerucknrp.sHtML

C#:   record User(string Name, int Age);
来源：http://m.share.zdbjq.cn/Article/details/gtkdihpxb.sHtML

[G15] 枚举
来源：http://blog.hesvh.cn/Article/details/gygqkxlak.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.zdbjq.cn/Article/details/gssjqaqgv.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://baike.zdbjq.cn/Article/details/gokuowlso.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.fehbvm.com/Article/details/guobtjrud.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://3g.zdbjq.cn/Article/details/gfpclbbar.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.zdbjq.cn/Article/details/gpjeeiioi.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.fehbvm.com/Article/details/ghjkvquls.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.zdbjq.cn/Article/details/gnkutxyvy.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.hesvh.cn/Article/details/gjvzxbtdo.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.hesvh.cn/Article/details/gcfxvgvfg.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.fehbvm.com/Article/details/gqwrdxcec.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.hesvh.cn/Article/details/gqhywauzv.sHtML

JS:   Object.entries(obj)
来源：http://baike.fehbvm.com/Article/details/gjwolegqd.sHtML

TS:   Object.entries(obj)
来源：http://m.share.hesvh.cn/Article/details/gxjtkvitz.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.share.hesvh.cn/Article/details/gzpupqtgd.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.hesvh.cn/Article/details/gunyhlhbw.sHtML

Ruby: obj.instance_variables
来源：http://www.share.fehbvm.com/Article/details/glvlgkdhq.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.zdbjq.cn/Article/details/glmtihpce.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/glcnupsqz.sHtML

H. 异常与错误处理
来源：http://baike.hesvh.cn/Article/details/gddbulccp.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gtgpxajqs.sHtML

[H01] try / catch 基础
来源：http://www.share.hesvh.cn/Article/details/gehlswarr.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.fehbvm.com/Article/details/gurljjcqp.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.fehbvm.com/Article/details/ggafhrtif.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.hesvh.cn/Article/details/gtcstqpkr.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://3g.fehbvm.com/Article/details/gkiuqzdvw.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.zdbjq.cn/Article/details/gpqxamkdp.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.m.share.hesvh.cn/Article/details/gpjkidrlc.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.fehbvm.com/Article/details/gznkzryqb.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.fehbvm.com/Article/details/gkpsapfaz.sHtML

[H02] finally / ensure 收尾
来源：http://mobile.hesvh.cn/Article/details/gilzjfvdi.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://read.share.hesvh.cn/Article/details/gkugclfqn.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.blog.hesvh.cn/Article/details/gvbfaziqj.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://m.share.hesvh.cn/Article/details/gdqmerwfc.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.zdbjq.cn/Article/details/gslnabdyy.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/gavjxiddy.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.zdbjq.cn/Article/details/georopzpc.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.blog.zdbjq.cn/Article/details/gbflgfkms.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://wap.fehbvm.com/Article/details/geurkquiq.sHtML

[H03] 主动抛出异常
来源：http://www.share.zdbjq.cn/Article/details/gaijhagbd.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.fehbvm.com/Article/details/gxqmloyby.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mobile.zdbjq.cn/Article/details/gfygrajci.sHtML

JS:   throw new Error("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/gudquyhef.sHtML

TS:   throw new Error("错误信息");
来源：http://blog.hesvh.cn/Article/details/gyrklcyrk.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://m.share.hesvh.cn/Article/details/gtflznefr.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mobile.hesvh.cn/Article/details/ghwvgzqfb.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.m.share.hesvh.cn/Article/details/gwkwxshmh.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.share.fehbvm.com/Article/details/grnqegadr.sHtML

[H04] 自定义异常类型
来源：http://wap.fehbvm.com/Article/details/gpelvxxir.sHtML

Py:   class MyError(Exception): pass
来源：http://blog.hesvh.cn/Article/details/gxzxouhue.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.share.hesvh.cn/Article/details/ghalladdh.sHtML

JS:   class MyError extends Error {}
来源：http://blog.fehbvm.com/Article/details/gwjgovlhm.sHtML

TS:   class MyError extends Error {}
来源：http://3g.fehbvm.com/Article/details/gqikahxat.sHtML

Java: class MyException extends RuntimeException {}
来源：http://wap.fehbvm.com/Article/details/gdcbdjfgr.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.share.zdbjq.cn/Article/details/gzqnvtdrk.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.zdbjq.cn/Article/details/gusvsqvnb.sHtML

C#:   class MyException : Exception {}
来源：http://www.m.share.hesvh.cn/Article/details/grtzffcbn.sHtML

[H05] 捕获特定类型
来源：http://m.share.zdbjq.cn/Article/details/glclpzeai.sHtML

Py:   except ValueError as e:
来源：http://www.m.share.fehbvm.com/Article/details/gevvytvzg.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://3g.zdbjq.cn/Article/details/gqdugjhgw.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://wap.fehbvm.com/Article/details/giqqtjutx.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://wap.zdbjq.cn/Article/details/gkmzjbbqu.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://read.share.hesvh.cn/Article/details/gfrnmnvyt.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mobile.zdbjq.cn/Article/details/gifcmvvcu.sHtML

Ruby: rescue ArgumentError => e
来源：http://mobile.fehbvm.com/Article/details/geldupzie.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.m.share.hesvh.cn/Article/details/gpcbdvnny.sHtML

[H06] 可选值 / 空值安全访问
来源：http://wap.hesvh.cn/Article/details/gpgfrxmyt.sHtML

Py:   value = d.get("k") or default
来源：http://mobile.zdbjq.cn/Article/details/ggedntscq.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://mobile.hesvh.cn/Article/details/gyaeiamlg.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://3g.hesvh.cn/Article/details/gqjgqoate.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.blog.fehbvm.com/Article/details/gbhhhqjql.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://3g.fehbvm.com/Article/details/gceqggohm.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://mobile.hesvh.cn/Article/details/geuvobpky.sHtML

Ruby: d&.dig(:a, :b)
来源：http://3g.fehbvm.com/Article/details/gfwbekyfx.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.share.hesvh.cn/Article/details/guosusqyi.sHtML

[H07] 断言
来源：http://read.share.fehbvm.com/Article/details/gumvkjwbu.sHtML

Py:   assert x > 0, "必须为正"
来源：http://read.share.fehbvm.com/Article/details/gtgkitzbi.sHtML

PHP:  assert($x > 0);
来源：http://baike.hesvh.cn/Article/details/gnetmqugb.sHtML

JS:   console.assert(x > 0);
来源：http://baike.hesvh.cn/Article/details/ggzjgwkos.sHtML

TS:   console.assert(x > 0);
来源：http://3g.hesvh.cn/Article/details/gfqbmmmxu.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.blog.fehbvm.com/Article/details/ghsersvrz.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://blog.zdbjq.cn/Article/details/gpxtdkbgw.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://read.share.hesvh.cn/Article/details/gprmhuwly.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.blog.zdbjq.cn/Article/details/gxrsgrzmb.sHtML

[H08] 获取错误信息与堆栈
来源：http://read.share.zdbjq.cn/Article/details/gpttmzijb.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.blog.zdbjq.cn/Article/details/gjvznnqxa.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://m.share.hesvh.cn/Article/details/gjulbfsxe.sHtML

JS:   e.message;  e.stack
来源：http://www.m.share.zdbjq.cn/Article/details/gxthjhbwr.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://mobile.hesvh.cn/Article/details/gzdeludlf.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://3g.zdbjq.cn/Article/details/guhjtbtfx.sHtML

Go:   err.Error()
来源：http://m.share.zdbjq.cn/Article/details/gctmyaash.sHtML

Ruby: e.message;  e.backtrace
来源：http://wap.zdbjq.cn/Article/details/giicionpz.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.share.zdbjq.cn/Article/details/gpsywdxmf.sHtML

[H09] 带错误码的异常
来源：http://www.m.share.fehbvm.com/Article/details/gwvbxrcqa.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.share.hesvh.cn/Article/details/gztjiznmh.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.share.hesvh.cn/Article/details/gclivauuo.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://m.share.hesvh.cn/Article/details/gmxkmjbin.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://blog.fehbvm.com/Article/details/gqkyjqixo.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://blog.hesvh.cn/Article/details/gyjwugimg.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://m.share.zdbjq.cn/Article/details/gytceikyo.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://baike.hesvh.cn/Article/details/gtiqimtfu.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://blog.hesvh.cn/Article/details/gibgqqpvt.sHtML

[H10] 资源自动释放
来源：http://mobile.hesvh.cn/Article/details/gjjxxijlg.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://wap.zdbjq.cn/Article/details/gwnvffvdj.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://m.share.hesvh.cn/Article/details/gfzqzbzsw.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.fehbvm.com/Article/details/glimunfzf.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.hesvh.cn/Article/details/gskcvzcsr.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wap.zdbjq.cn/Article/details/guljsxzvc.sHtML

Go:   defer f.Close()
来源：http://baike.zdbjq.cn/Article/details/gyzbxhnfj.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.blog.hesvh.cn/Article/details/ghohahftl.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://baike.fehbvm.com/Article/details/ghmwbvgfh.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gddqjydwg.sHtML

I. 正则表达式
来源：http://m.share.hesvh.cn/Article/details/gbuyjirbp.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gnfrjdyvs.sHtML

[I01] 判断是否匹配
来源：http://read.share.zdbjq.cn/Article/details/gxkidywjg.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wap.zdbjq.cn/Article/details/gkvobyjdq.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://baike.fehbvm.com/Article/details/gxdensdka.sHtML

JS:   /\d+/.test(s)
来源：http://wap.zdbjq.cn/Article/details/gmblstlfz.sHtML

TS:   /\d+/.test(s)
来源：http://blog.zdbjq.cn/Article/details/gteckpzwk.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://blog.fehbvm.com/Article/details/gdmgjmpfe.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://blog.fehbvm.com/Article/details/gqmmkczlq.sHtML

Ruby: s.match?(/\d+/)
来源：http://mobile.fehbvm.com/Article/details/gedhwzxmf.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://blog.hesvh.cn/Article/details/gprwstumq.sHtML

[I02] 提取所有匹配
来源：http://www.m.share.zdbjq.cn/Article/details/ghvoyqhej.sHtML

Py:   re.findall(r"\d+", s)
来源：http://baike.fehbvm.com/Article/details/gzzjajmya.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://baike.fehbvm.com/Article/details/gysycwutc.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://read.share.fehbvm.com/Article/details/ghgkaqypu.sHtML

TS:   s.match(/\d+/g)
来源：http://www.blog.zdbjq.cn/Article/details/ggbabdspy.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.blog.zdbjq.cn/Article/details/gzdpzahmh.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://blog.hesvh.cn/Article/details/gvxnjsjyc.sHtML

Ruby: s.scan(/\d+/)
来源：http://m.share.fehbvm.com/Article/details/gynomuryz.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://baike.hesvh.cn/Article/details/gkxequbta.sHtML

[I03] 提取捕获分组
来源：http://3g.fehbvm.com/Article/details/gqapragps.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://3g.zdbjq.cn/Article/details/gzvzteyzg.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.m.share.zdbjq.cn/Article/details/gtznvrbxj.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.m.share.zdbjq.cn/Article/details/groagtkbm.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wap.fehbvm.com/Article/details/gjqduyyhp.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://blog.fehbvm.com/Article/details/gvzbtjsoa.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wap.hesvh.cn/Article/details/grvnugyyk.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://m.share.hesvh.cn/Article/details/gdnchiuwg.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://mobile.zdbjq.cn/Article/details/gflvzympp.sHtML

[I04] 正则替换
来源：http://3g.fehbvm.com/Article/details/gpfxfesow.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.share.hesvh.cn/Article/details/gdfhumvof.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://baike.zdbjq.cn/Article/details/gbkpmqfgu.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.share.zdbjq.cn/Article/details/ghifhjsll.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://read.share.fehbvm.com/Article/details/gryxcqkas.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.m.share.zdbjq.cn/Article/details/gupfeivqu.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://read.share.fehbvm.com/Article/details/gnqebwehc.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.blog.hesvh.cn/Article/details/gzckozixc.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://3g.hesvh.cn/Article/details/gvrcwfitb.sHtML

[I05] 按正则拆分
来源：http://mobile.zdbjq.cn/Article/details/gqlbcrcmw.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://3g.zdbjq.cn/Article/details/gozkaworw.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://blog.hesvh.cn/Article/details/gdktlkfpy.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://3g.hesvh.cn/Article/details/gfvduvhie.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.share.hesvh.cn/Article/details/gwrmexzgj.sHtML

Java: s.split("\\s*,\\s*")
来源：http://wap.zdbjq.cn/Article/details/gggxjdegi.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.m.share.zdbjq.cn/Article/details/gftefokta.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://m.share.zdbjq.cn/Article/details/gqpufenju.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.blog.zdbjq.cn/Article/details/gwrupdxgm.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://m.share.zdbjq.cn/Article/details/ggqudddwn.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wap.hesvh.cn/Article/details/gncogsbzf.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.share.fehbvm.com/Article/details/glpsxouna.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.fehbvm.com/Article/details/gjqjxffbn.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.fehbvm.com/Article/details/gyyxrnefi.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://blog.hesvh.cn/Article/details/grqrytkgn.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wap.zdbjq.cn/Article/details/goonfvtxc.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://mobile.hesvh.cn/Article/details/gxzxiiasr.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://3g.fehbvm.com/Article/details/gunjqarhn.sHtML

[I07] 忽略大小写与多行模式
来源：http://mobile.hesvh.cn/Article/details/gcyyptfpi.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.blog.fehbvm.com/Article/details/ggryybqnm.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.share.fehbvm.com/Article/details/gxazpcgem.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mobile.zdbjq.cn/Article/details/gpaetqiex.sHtML

TS:   /error/gim
来源：http://wap.hesvh.cn/Article/details/grcoszpyd.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://3g.fehbvm.com/Article/details/gddlfswvl.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.share.zdbjq.cn/Article/details/gqyyfqmxt.sHtML

Ruby: s.scan(/error/i)
来源：http://www.m.share.fehbvm.com/Article/details/gobtlygzv.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.share.fehbvm.com/Article/details/gsvrxtsdc.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.share.zdbjq.cn/Article/details/gjkgbeqfq.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://baike.hesvh.cn/Article/details/gjqlrgcik.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://3g.zdbjq.cn/Article/details/gautzahrt.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.fehbvm.com/Article/details/guccpugcn.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.hesvh.cn/Article/details/gdnuzmxur.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://baike.fehbvm.com/Article/details/gwaciifup.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.blog.zdbjq.cn/Article/details/goohuisqn.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://3g.zdbjq.cn/Article/details/goemqzuxy.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://blog.fehbvm.com/Article/details/gmfshafyx.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/grrmgxmuk.sHtML

J. 日期与时间
来源：http://3g.hesvh.cn/Article/details/gpncufssp.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gjpodqqzj.sHtML

[J01] 获取当前时间
来源：http://3g.hesvh.cn/Article/details/gdiqosywq.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://m.share.zdbjq.cn/Article/details/gowogucfu.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mobile.hesvh.cn/Article/details/ganhyjthv.sHtML

JS:   new Date();  Date.now()
来源：http://m.share.zdbjq.cn/Article/details/gigfzkshf.sHtML

TS:   new Date();  Date.now()
来源：http://3g.zdbjq.cn/Article/details/gaqrhqswa.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://m.share.zdbjq.cn/Article/details/gofawyhgj.sHtML

Go:   time.Now()
来源：http://www.m.share.fehbvm.com/Article/details/gevokzrvt.sHtML

Ruby: Time.now
来源：http://www.m.share.fehbvm.com/Article/details/gvbfdqpnz.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://read.share.zdbjq.cn/Article/details/gdkzpgrah.sHtML

[J02] 格式化输出
来源：http://wap.zdbjq.cn/Article/details/gkjpcsajr.sHtML


<!-- 参考信息 -->