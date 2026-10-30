代发 wailian999

C#:   public User(string name) { Name = name; }
来源：http://baike.fehbvm.com/Article/details/gfqnavnge.sHtML

[G03] 实例属性
来源：http://read.share.fehbvm.com/Article/details/gujeeyhhi.sHtML

Py:   self.name = "x"
来源：http://www.blog.hesvh.cn/Article/details/glkeztfxz.sHtML

PHP:  public string $name = "x";
来源：http://baike.hesvh.cn/Article/details/gikmeoano.sHtML

JS:   this.name = "x";
来源：http://mobile.fehbvm.com/Article/details/gjvrjnpdv.sHtML

TS:   name: string = "x";
来源：http://baike.hesvh.cn/Article/details/gncnqthni.sHtML

Java: private String name;
来源：http://m.share.fehbvm.com/Article/details/gkrwgewnv.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.fehbvm.com/Article/details/gqyudgcjf.sHtML

Ruby: @name = "x"
来源：http://mobile.hesvh.cn/Article/details/ggvhrqzuq.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.hesvh.cn/Article/details/gyfklafbp.sHtML

[G04] 定义方法
来源：http://3g.zdbjq.cn/Article/details/gmybzainz.sHtML

Py:   def greet(self): return self.name
来源：http://blog.hesvh.cn/Article/details/gcgxedsti.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.hesvh.cn/Article/details/gdetjqgxf.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/ghlvkkstf.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/gsnqibaza.sHtML

Java: String greet() { return name; }
来源：http://m.share.zdbjq.cn/Article/details/gtfhqbfen.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.hesvh.cn/Article/details/gibteptij.sHtML

Ruby: def greet; @name; end
来源：http://3g.hesvh.cn/Article/details/gbbbbadui.sHtML

C#:   public string Greet() => Name;
来源：http://baike.fehbvm.com/Article/details/gntsyvjhw.sHtML

[G05] 继承
来源：http://wap.fehbvm.com/Article/details/gbmabwxgz.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.fehbvm.com/Article/details/gyvrkhssy.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/gyerfrpvm.sHtML

JS:   class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/gefjmqvdt.sHtML

TS:   class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/gwyighezj.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gxswunghz.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.hesvh.cn/Article/details/gslfomzpq.sHtML

Ruby: class Admin < User; end
来源：http://www.share.hesvh.cn/Article/details/gtagyfpvf.sHtML

C#:   class Admin : User {}
来源：http://blog.hesvh.cn/Article/details/ganmpjllh.sHtML

[G06] 重写方法
来源：http://blog.fehbvm.com/Article/details/gjkwwsxdg.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.zdbjq.cn/Article/details/gijdvvdvt.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.zdbjq.cn/Article/details/ggshwwznf.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/gbrerkvxa.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/gulldlcod.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/gqwlbwhag.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.hesvh.cn/Article/details/gnrtmcqli.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.hesvh.cn/Article/details/gmorighmv.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.fehbvm.com/Article/details/gxqtqajei.sHtML

[G07] 调用父类方法
来源：http://baike.hesvh.cn/Article/details/gkwvkxfib.sHtML

Py:   super().greet()
来源：http://baike.zdbjq.cn/Article/details/gvxqjnwrj.sHtML

PHP:  parent::greet();
来源：http://blog.hesvh.cn/Article/details/gluegtdev.sHtML

JS:   super.greet();
来源：http://www.m.share.hesvh.cn/Article/details/gufrbpsib.sHtML

TS:   super.greet();
来源：http://blog.fehbvm.com/Article/details/gngsjjnmz.sHtML

Java: super.greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gtngidhsw.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.zdbjq.cn/Article/details/gfzhvsgqv.sHtML

Ruby: super
来源：http://m.share.fehbvm.com/Article/details/ghvxiplhl.sHtML

C#:   base.Greet();
来源：http://m.share.hesvh.cn/Article/details/gheyouwdf.sHtML

[G08] 静态方法与属性
来源：http://mobile.hesvh.cn/Article/details/goulxpnmz.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.hesvh.cn/Article/details/gfdhqavst.sHtML

PHP:  public static function f() {}
来源：http://blog.hesvh.cn/Article/details/gnuxxmmrv.sHtML

JS:   static f() {}
来源：http://mobile.fehbvm.com/Article/details/gvkkashxh.sHtML

TS:   static f(): void {}
来源：http://www.blog.hesvh.cn/Article/details/ghhyyctav.sHtML

Java: static void f() {}
来源：http://mobile.hesvh.cn/Article/details/gqprggdbj.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.hesvh.cn/Article/details/ggutotoiq.sHtML

Ruby: def self.f; end
来源：http://blog.zdbjq.cn/Article/details/garanbddg.sHtML

C#:   public static void F() {}
来源：http://www.m.share.zdbjq.cn/Article/details/gkcimhfha.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.zdbjq.cn/Article/details/gkxmpoahg.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.zdbjq.cn/Article/details/gqmuzytfp.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.fehbvm.com/Article/details/gqdkxjnsj.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.zdbjq.cn/Article/details/gjwhkmedr.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.hesvh.cn/Article/details/gujgdtydw.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.hesvh.cn/Article/details/gxelpiilv.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.zdbjq.cn/Article/details/giioxzbsq.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.hesvh.cn/Article/details/gnhbumwev.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.hesvh.cn/Article/details/gcffieqkt.sHtML

[G10] 访问控制
来源：http://m.share.hesvh.cn/Article/details/ggxkshzti.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.hesvh.cn/Article/details/gzcskfeia.sHtML

PHP:  public / protected / private
来源：http://m.share.zdbjq.cn/Article/details/gsgkinxyp.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.fehbvm.com/Article/details/gadzlvtzd.sHtML

TS:   public / protected / private
来源：http://m.share.zdbjq.cn/Article/details/gcdvnazwg.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.hesvh.cn/Article/details/gqqcjeuep.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.hesvh.cn/Article/details/geicioyfd.sHtML

Ruby: public / protected / private
来源：http://www.blog.zdbjq.cn/Article/details/gyxosubme.sHtML

C#:   public / protected / private / internal
来源：http://blog.zdbjq.cn/Article/details/ggciyfepo.sHtML

[G11] getter / setter
来源：http://www.blog.hesvh.cn/Article/details/gamoexcoa.sHtML

Py:   @property 与 @x.setter
来源：http://blog.zdbjq.cn/Article/details/gumrqmlzp.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.hesvh.cn/Article/details/gvvrsakcg.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.zdbjq.cn/Article/details/guryjliuu.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.zdbjq.cn/Article/details/gtwqyqvxw.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/gssuzzrrn.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.fehbvm.com/Article/details/gbpxsdsiu.sHtML

Ruby: attr_accessor :name
来源：http://m.share.fehbvm.com/Article/details/gbdpceihq.sHtML

C#:   public string Name { get; set; }
来源：http://3g.zdbjq.cn/Article/details/ghuuchwel.sHtML

[G12] 对象转字符串
来源：http://wap.fehbvm.com/Article/details/gauszokln.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.zdbjq.cn/Article/details/gpxnfnzak.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.zdbjq.cn/Article/details/guicfjcqv.sHtML

JS:   toString() { return this.name; }
来源：http://blog.hesvh.cn/Article/details/ggzxkswmz.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/gcedcebvo.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/gwxiwwtle.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.hesvh.cn/Article/details/gzoklhypo.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.fehbvm.com/Article/details/gonqjzlqi.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.hesvh.cn/Article/details/ghvmkvffv.sHtML

[G13] 判断对象类型
来源：http://mobile.fehbvm.com/Article/details/gotebjvgg.sHtML

Py:   isinstance(u, User)
来源：http://read.share.hesvh.cn/Article/details/gvmlzynvf.sHtML

PHP:  $u instanceof User
来源：http://mobile.fehbvm.com/Article/details/gvtqdtlzr.sHtML

JS:   u instanceof User
来源：http://read.share.fehbvm.com/Article/details/gnzvcbxgh.sHtML

TS:   u instanceof User
来源：http://baike.fehbvm.com/Article/details/gspobyypz.sHtML

Java: u instanceof User
来源：http://wap.zdbjq.cn/Article/details/guftwlbeh.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.hesvh.cn/Article/details/gufnfqwhl.sHtML

Ruby: u.is_a?(User)
来源：http://3g.zdbjq.cn/Article/details/gwqrtkitn.sHtML

C#:   u is User
来源：http://wap.fehbvm.com/Article/details/gkwxndltq.sHtML

[G14] 数据类 / record
来源：http://blog.hesvh.cn/Article/details/gsnzccqng.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.fehbvm.com/Article/details/gxnfkqymi.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.fehbvm.com/Article/details/gmwpfzhrp.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.fehbvm.com/Article/details/gdfsvnhfz.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.hesvh.cn/Article/details/gfdrosgvo.sHtML

Java: record User(String name, int age) {}
来源：http://3g.fehbvm.com/Article/details/gtoyvjque.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.hesvh.cn/Article/details/gzfdsrhdl.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.zdbjq.cn/Article/details/gyvtecrwl.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.fehbvm.com/Article/details/gfscrxgmp.sHtML

[G15] 枚举
来源：http://blog.zdbjq.cn/Article/details/guvcuzxmq.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.hesvh.cn/Article/details/gynbrodpf.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.zdbjq.cn/Article/details/gnnpgeerd.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.fehbvm.com/Article/details/gfsuymyoq.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://3g.hesvh.cn/Article/details/gnhhhocns.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.zdbjq.cn/Article/details/gebzcvpxs.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.hesvh.cn/Article/details/ggtkbkkqb.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.m.share.zdbjq.cn/Article/details/gbovxgmlc.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.zdbjq.cn/Article/details/gobasfffr.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.fehbvm.com/Article/details/gidxvrkvz.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.hesvh.cn/Article/details/gkjrxkjys.sHtML

PHP:  get_object_vars($obj);
来源：http://blog.fehbvm.com/Article/details/gzzuuvvrd.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gihtjrcyq.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gtygzhmif.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://blog.hesvh.cn/Article/details/ggazrmehi.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.fehbvm.com/Article/details/ghmhpdbmq.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.fehbvm.com/Article/details/gmigvxjjp.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.fehbvm.com/Article/details/gjvqrqqhk.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gasgkimyr.sHtML

H. 异常与错误处理
来源：http://mobile.zdbjq.cn/Article/details/gpjimplik.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gxknsuvpz.sHtML

[H01] try / catch 基础
来源：http://blog.hesvh.cn/Article/details/gwgkoyoaj.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.hesvh.cn/Article/details/gqhecjzck.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.blog.zdbjq.cn/Article/details/glswgxcqu.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://blog.hesvh.cn/Article/details/gscptornf.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.m.share.zdbjq.cn/Article/details/grvhxjakc.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.zdbjq.cn/Article/details/gvcratlbk.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.fehbvm.com/Article/details/gmpbjntif.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://blog.hesvh.cn/Article/details/gmzxmnnut.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.fehbvm.com/Article/details/gtbxtabem.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.zdbjq.cn/Article/details/guumaqlge.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.share.zdbjq.cn/Article/details/gzomroiui.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/gmuvxyyjv.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.hesvh.cn/Article/details/gfjpqtvvp.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/gzhzfpxiw.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.share.fehbvm.com/Article/details/gnpkugmbh.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.zdbjq.cn/Article/details/givoktjxo.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.hesvh.cn/Article/details/ghjskujwf.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://blog.hesvh.cn/Article/details/gkeiltajv.sHtML

[H03] 主动抛出异常
来源：http://www.blog.zdbjq.cn/Article/details/gzhaodtqh.sHtML

Py:   raise ValueError("错误信息")
来源：http://blog.zdbjq.cn/Article/details/gdgdksdhx.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.m.share.zdbjq.cn/Article/details/gfdfzkvym.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.zdbjq.cn/Article/details/gmbbdquxx.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.fehbvm.com/Article/details/gkxepvjrd.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://m.share.fehbvm.com/Article/details/gtqncfmzs.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://baike.hesvh.cn/Article/details/gyhtvznzn.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.blog.zdbjq.cn/Article/details/gnsjfyfnw.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://blog.zdbjq.cn/Article/details/gadikkmba.sHtML

[H04] 自定义异常类型
来源：http://mobile.fehbvm.com/Article/details/gpusrvisv.sHtML

Py:   class MyError(Exception): pass
来源：http://3g.fehbvm.com/Article/details/gnouvipaw.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://blog.hesvh.cn/Article/details/gpisjdbai.sHtML

JS:   class MyError extends Error {}
来源：http://www.blog.fehbvm.com/Article/details/gnhcmizrn.sHtML

TS:   class MyError extends Error {}
来源：http://baike.hesvh.cn/Article/details/gthqbtpkl.sHtML

Java: class MyException extends RuntimeException {}
来源：http://3g.fehbvm.com/Article/details/gfwugnwks.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.blog.zdbjq.cn/Article/details/gvsulwctj.sHtML

Ruby: class MyError < StandardError; end
来源：http://mobile.hesvh.cn/Article/details/gejjetrto.sHtML

C#:   class MyException : Exception {}
来源：http://m.share.zdbjq.cn/Article/details/gmwnssmsm.sHtML

[H05] 捕获特定类型
来源：http://blog.zdbjq.cn/Article/details/guyktpkjw.sHtML

Py:   except ValueError as e:
来源：http://read.share.fehbvm.com/Article/details/goqqzjhnl.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://baike.zdbjq.cn/Article/details/ggtyfoygd.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gqsiqqujw.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://wap.zdbjq.cn/Article/details/gccyptjoe.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://m.share.zdbjq.cn/Article/details/gbsmhcegb.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.blog.zdbjq.cn/Article/details/goemeztbu.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.fehbvm.com/Article/details/ghoagkuvj.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.blog.hesvh.cn/Article/details/gzpvmzpqp.sHtML

[H06] 可选值 / 空值安全访问
来源：http://wap.zdbjq.cn/Article/details/gjcbkorkx.sHtML

Py:   value = d.get("k") or default
来源：http://m.share.fehbvm.com/Article/details/gxgzpygxm.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.blog.fehbvm.com/Article/details/gqtqdrvgf.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://3g.fehbvm.com/Article/details/glleegxwr.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://read.share.fehbvm.com/Article/details/gmxxmeaim.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://baike.fehbvm.com/Article/details/gnjpqukpo.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://baike.zdbjq.cn/Article/details/gpwcwjzap.sHtML

Ruby: d&.dig(:a, :b)
来源：http://blog.zdbjq.cn/Article/details/gyfiebubg.sHtML

C#:   obj?.A?.B ?? default
来源：http://blog.hesvh.cn/Article/details/gvvtlfcuj.sHtML

[H07] 断言
来源：http://m.share.fehbvm.com/Article/details/gxxpvgrsr.sHtML

Py:   assert x > 0, "必须为正"
来源：http://mobile.fehbvm.com/Article/details/gzzmmvqxy.sHtML

PHP:  assert($x > 0);
来源：http://mobile.hesvh.cn/Article/details/gihpnlvbi.sHtML

JS:   console.assert(x > 0);
来源：http://baike.fehbvm.com/Article/details/gurcnuljc.sHtML

TS:   console.assert(x > 0);
来源：http://read.share.fehbvm.com/Article/details/gvnihnmgy.sHtML

Java: assert x > 0 : "必须为正";
来源：http://read.share.fehbvm.com/Article/details/ghltygsgn.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.share.zdbjq.cn/Article/details/gsfpzjles.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://baike.hesvh.cn/Article/details/gdqczydgm.sHtML

C#:   Debug.Assert(x > 0);
来源：http://m.share.hesvh.cn/Article/details/ggnxtuzpc.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.m.share.zdbjq.cn/Article/details/guqqidkiv.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://m.share.zdbjq.cn/Article/details/ggcctblek.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.blog.zdbjq.cn/Article/details/gvrgqhevt.sHtML

JS:   e.message;  e.stack
来源：http://wap.fehbvm.com/Article/details/ggesbdyvp.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://baike.hesvh.cn/Article/details/gdcuiwhix.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://3g.fehbvm.com/Article/details/gzdqsdlfk.sHtML

Go:   err.Error()
来源：http://www.m.share.hesvh.cn/Article/details/gshoofkpz.sHtML

Ruby: e.message;  e.backtrace
来源：http://mobile.zdbjq.cn/Article/details/ggpifvgen.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.m.share.hesvh.cn/Article/details/gvyjzbeev.sHtML

[H09] 带错误码的异常
来源：http://blog.hesvh.cn/Article/details/gaxgcxfwa.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://read.share.fehbvm.com/Article/details/gliuyquwk.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://m.share.hesvh.cn/Article/details/gcktniwfd.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.blog.hesvh.cn/Article/details/gptfbromx.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.blog.fehbvm.com/Article/details/ggorodibg.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wap.zdbjq.cn/Article/details/gfpioufbt.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.share.hesvh.cn/Article/details/gylmqmgmq.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://baike.hesvh.cn/Article/details/gpyiedbea.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://wap.zdbjq.cn/Article/details/govubtqbf.sHtML

[H10] 资源自动释放
来源：http://read.share.fehbvm.com/Article/details/gukobczpb.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://blog.hesvh.cn/Article/details/gtawiiezo.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://read.share.hesvh.cn/Article/details/gztgmhaph.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.hesvh.cn/Article/details/gzsveylib.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.fehbvm.com/Article/details/gkjkciusk.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.m.share.hesvh.cn/Article/details/ghvcyatjh.sHtML

Go:   defer f.Close()
来源：http://baike.zdbjq.cn/Article/details/ggjnknbfv.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wap.hesvh.cn/Article/details/gdgcnwigb.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gaserjije.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/geaapvoyl.sHtML

I. 正则表达式
来源：http://3g.hesvh.cn/Article/details/gbzgtauzj.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/guutajdoh.sHtML

[I01] 判断是否匹配
来源：http://www.m.share.zdbjq.cn/Article/details/grvmdjubh.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.blog.fehbvm.com/Article/details/gwgnqlxhl.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://blog.zdbjq.cn/Article/details/gvnxxbsby.sHtML

JS:   /\d+/.test(s)
来源：http://www.blog.zdbjq.cn/Article/details/gpfhqkfav.sHtML

TS:   /\d+/.test(s)
来源：http://www.share.fehbvm.com/Article/details/gutrdzacd.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://m.share.hesvh.cn/Article/details/gvltzpuwi.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://read.share.zdbjq.cn/Article/details/gixawluiy.sHtML

Ruby: s.match?(/\d+/)
来源：http://baike.zdbjq.cn/Article/details/gsighjikc.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.blog.zdbjq.cn/Article/details/gfrgjbesy.sHtML

[I02] 提取所有匹配
来源：http://baike.zdbjq.cn/Article/details/gyjwobrxh.sHtML

Py:   re.findall(r"\d+", s)
来源：http://blog.fehbvm.com/Article/details/gwflpmcrf.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://baike.hesvh.cn/Article/details/gviilpgcl.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.share.fehbvm.com/Article/details/gejqrjjpe.sHtML

TS:   s.match(/\d+/g)
来源：http://blog.hesvh.cn/Article/details/geiwetsat.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.blog.hesvh.cn/Article/details/gwaffqhrd.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mobile.hesvh.cn/Article/details/gpsgqjyui.sHtML

Ruby: s.scan(/\d+/)
来源：http://baike.fehbvm.com/Article/details/gcsjsituf.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.share.hesvh.cn/Article/details/goaqtltmp.sHtML

[I03] 提取捕获分组
来源：http://www.blog.hesvh.cn/Article/details/grksewifl.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.blog.fehbvm.com/Article/details/goymptbnk.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mobile.zdbjq.cn/Article/details/guhexxuss.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wap.hesvh.cn/Article/details/gdztvetrg.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://baike.hesvh.cn/Article/details/gnmoegdcb.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://mobile.zdbjq.cn/Article/details/gcldqgter.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://m.share.hesvh.cn/Article/details/gijlgbvzp.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://blog.fehbvm.com/Article/details/gbxsiufzq.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://baike.hesvh.cn/Article/details/giknlwptu.sHtML

[I04] 正则替换
来源：http://m.share.zdbjq.cn/Article/details/gzunupclu.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.m.share.hesvh.cn/Article/details/gykvwfjtj.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gcdgalgcx.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://m.share.fehbvm.com/Article/details/gmkhycdst.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://3g.zdbjq.cn/Article/details/gunroqqiv.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://3g.fehbvm.com/Article/details/gvuvcdzyk.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://blog.zdbjq.cn/Article/details/grqaizmcw.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://3g.hesvh.cn/Article/details/gnwkrdesl.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.blog.hesvh.cn/Article/details/groplhqoi.sHtML

[I05] 按正则拆分
来源：http://www.blog.hesvh.cn/Article/details/gafhsceno.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.m.share.hesvh.cn/Article/details/gdvkqcuhd.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://baike.zdbjq.cn/Article/details/gzlatpslh.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://baike.zdbjq.cn/Article/details/guejmhwrw.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://3g.fehbvm.com/Article/details/gkvllmbmq.sHtML

Java: s.split("\\s*,\\s*")
来源：http://blog.hesvh.cn/Article/details/gztkpymsn.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://baike.fehbvm.com/Article/details/gjxpjubir.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://mobile.zdbjq.cn/Article/details/gmhakfqyd.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://blog.zdbjq.cn/Article/details/gkbtsxppl.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wap.fehbvm.com/Article/details/gaxnsyjoc.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://read.share.zdbjq.cn/Article/details/gacjzutbc.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.blog.zdbjq.cn/Article/details/gfieegpvm.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.fehbvm.com/Article/details/gnbpodhuv.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.fehbvm.com/Article/details/gweziutev.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://blog.fehbvm.com/Article/details/gkzwlqacr.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wap.fehbvm.com/Article/details/gdkrkatxx.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://m.share.fehbvm.com/Article/details/gyroubtmi.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://3g.fehbvm.com/Article/details/glzehngog.sHtML

[I07] 忽略大小写与多行模式
来源：http://3g.hesvh.cn/Article/details/gfpywnxbg.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mobile.zdbjq.cn/Article/details/gelozlowm.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.share.zdbjq.cn/Article/details/gpzmwbdqq.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mobile.fehbvm.com/Article/details/ghnvnluwg.sHtML

TS:   /error/gim
来源：http://wap.hesvh.cn/Article/details/gsfindbqd.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://3g.hesvh.cn/Article/details/guazmbzio.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.share.fehbvm.com/Article/details/grottltwk.sHtML

Ruby: s.scan(/error/i)
来源：http://www.share.fehbvm.com/Article/details/gmnxpodur.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.blog.hesvh.cn/Article/details/genicpuxi.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.m.share.fehbvm.com/Article/details/gvofcohog.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.share.hesvh.cn/Article/details/gzqcexcxs.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://blog.fehbvm.com/Article/details/gpcozarjt.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.hesvh.cn/Article/details/gnvmfxzbt.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.hesvh.cn/Article/details/gpdbsftsn.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://m.share.hesvh.cn/Article/details/gwexkovdm.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://blog.zdbjq.cn/Article/details/gsabnvvid.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://m.share.hesvh.cn/Article/details/geegmxzjc.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://baike.hesvh.cn/Article/details/giodevjri.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gmunndhmp.sHtML

J. 日期与时间
来源：http://www.share.fehbvm.com/Article/details/gcodqgulk.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gpdtbiwge.sHtML

[J01] 获取当前时间
来源：http://blog.fehbvm.com/Article/details/gnkejztba.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://read.share.zdbjq.cn/Article/details/garfqugzx.sHtML


<!-- 参考信息 -->