代发 wailian999

Ruby: @name = "x"
来源：http://blog.fehbvm.com/Article/details/giswucjcp.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.zdbjq.cn/Article/details/gwjqpqaud.sHtML

[G04] 定义方法
来源：http://3g.hesvh.cn/Article/details/gaeolyyke.sHtML

Py:   def greet(self): return self.name
来源：http://baike.hesvh.cn/Article/details/gidjgllaa.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.zdbjq.cn/Article/details/gkgnxvtza.sHtML

JS:   greet() { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/glsinsred.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.hesvh.cn/Article/details/giaazdukq.sHtML

Java: String greet() { return name; }
来源：http://blog.fehbvm.com/Article/details/ggrcphonq.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.fehbvm.com/Article/details/giijcbolr.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.hesvh.cn/Article/details/ggxyezjme.sHtML

C#:   public string Greet() => Name;
来源：http://blog.fehbvm.com/Article/details/gyqekgtyy.sHtML

[G05] 继承
来源：http://baike.fehbvm.com/Article/details/gnfgpxjje.sHtML

Py:   class Admin(User): pass
来源：http://mobile.hesvh.cn/Article/details/gsgawntoi.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/gxpoledxe.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/gajsbhnup.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/gbdqydsvf.sHtML

Java: class Admin extends User {}
来源：http://read.share.hesvh.cn/Article/details/gdnpevmly.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.zdbjq.cn/Article/details/gbuggmbla.sHtML

Ruby: class Admin < User; end
来源：http://www.share.fehbvm.com/Article/details/gjndzhgcz.sHtML

C#:   class Admin : User {}
来源：http://mobile.zdbjq.cn/Article/details/gjbxbeujh.sHtML

[G06] 重写方法
来源：http://baike.fehbvm.com/Article/details/gnmnzokhw.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.zdbjq.cn/Article/details/gqtbpaaea.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/gtsqiuknd.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/gpdqfbwrw.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/glvndrjmq.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/gtldtvzkg.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.hesvh.cn/Article/details/gfqnwmshe.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.zdbjq.cn/Article/details/gghqalvvk.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.fehbvm.com/Article/details/gcrueuhol.sHtML

[G07] 调用父类方法
来源：http://blog.fehbvm.com/Article/details/gqeockoze.sHtML

Py:   super().greet()
来源：http://www.blog.hesvh.cn/Article/details/gryfyxkbh.sHtML

PHP:  parent::greet();
来源：http://www.blog.hesvh.cn/Article/details/gjooucgyd.sHtML

JS:   super.greet();
来源：http://read.share.zdbjq.cn/Article/details/gzdrqmfuj.sHtML

TS:   super.greet();
来源：http://mobile.zdbjq.cn/Article/details/gngmxbeem.sHtML

Java: super.greet();
来源：http://3g.zdbjq.cn/Article/details/geddhlrhw.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.zdbjq.cn/Article/details/ghpluqwjq.sHtML

Ruby: super
来源：http://3g.zdbjq.cn/Article/details/gxbwkmojk.sHtML

C#:   base.Greet();
来源：http://www.blog.hesvh.cn/Article/details/gghiwevdt.sHtML

[G08] 静态方法与属性
来源：http://wap.fehbvm.com/Article/details/gkeehxquy.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.hesvh.cn/Article/details/gqspgbtpj.sHtML

PHP:  public static function f() {}
来源：http://mobile.fehbvm.com/Article/details/gocmeckyz.sHtML

JS:   static f() {}
来源：http://3g.hesvh.cn/Article/details/gnnychyhc.sHtML

TS:   static f(): void {}
来源：http://3g.hesvh.cn/Article/details/gnlpouqty.sHtML

Java: static void f() {}
来源：http://m.share.hesvh.cn/Article/details/guerixbff.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.hesvh.cn/Article/details/grqjqtxtl.sHtML

Ruby: def self.f; end
来源：http://www.share.fehbvm.com/Article/details/gzriokncm.sHtML

C#:   public static void F() {}
来源：http://www.blog.hesvh.cn/Article/details/gbyvzwyij.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.zdbjq.cn/Article/details/gapqevwom.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.fehbvm.com/Article/details/gzbbhigak.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.zdbjq.cn/Article/details/gcszzzhzp.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.zdbjq.cn/Article/details/grlbzqbka.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.zdbjq.cn/Article/details/gdwohgohp.sHtML

Java: interface Shape { double area(); }
来源：http://3g.zdbjq.cn/Article/details/gnmekwasg.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.fehbvm.com/Article/details/gepgnwgqx.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.zdbjq.cn/Article/details/grrkkbbdp.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.fehbvm.com/Article/details/gyqziuhbx.sHtML

[G10] 访问控制
来源：http://www.m.share.zdbjq.cn/Article/details/gfmfkfyme.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.hesvh.cn/Article/details/gxzwdigfp.sHtML

PHP:  public / protected / private
来源：http://baike.zdbjq.cn/Article/details/glyqafrtq.sHtML

JS:   #private 字段；其余公开
来源：http://blog.zdbjq.cn/Article/details/gzivjimel.sHtML

TS:   public / protected / private
来源：http://3g.hesvh.cn/Article/details/ggkoipper.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.hesvh.cn/Article/details/gxzhlgoeb.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.zdbjq.cn/Article/details/gvnsvizei.sHtML

Ruby: public / protected / private
来源：http://www.m.share.fehbvm.com/Article/details/ggucxxiaz.sHtML

C#:   public / protected / private / internal
来源：http://blog.fehbvm.com/Article/details/gzwepqogf.sHtML

[G11] getter / setter
来源：http://m.share.fehbvm.com/Article/details/gtemputbo.sHtML

Py:   @property 与 @x.setter
来源：http://3g.zdbjq.cn/Article/details/gxnkdmewu.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.fehbvm.com/Article/details/gwvecncxb.sHtML

JS:   get name() { return this._name; }
来源：http://wap.fehbvm.com/Article/details/gmbljmqjh.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.hesvh.cn/Article/details/gmuntdurp.sHtML

Java: public String getName() { return name; }
来源：http://baike.hesvh.cn/Article/details/gvrukjrfw.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.hesvh.cn/Article/details/gclwbrgxa.sHtML

Ruby: attr_accessor :name
来源：http://read.share.hesvh.cn/Article/details/gflzgkczb.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.fehbvm.com/Article/details/gjoekpcok.sHtML

[G12] 对象转字符串
来源：http://3g.fehbvm.com/Article/details/ggbubqcuq.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.zdbjq.cn/Article/details/grorxdfxd.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.zdbjq.cn/Article/details/gjdvnhyne.sHtML

JS:   toString() { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/gynsuzmnw.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.fehbvm.com/Article/details/gqsofazbj.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.zdbjq.cn/Article/details/grlwoxytr.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.fehbvm.com/Article/details/guebeekiq.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.hesvh.cn/Article/details/gdbgntyak.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.fehbvm.com/Article/details/gxpqwzipw.sHtML

[G13] 判断对象类型
来源：http://m.share.fehbvm.com/Article/details/gvxylobhb.sHtML

Py:   isinstance(u, User)
来源：http://baike.zdbjq.cn/Article/details/ghwgvmuew.sHtML

PHP:  $u instanceof User
来源：http://read.share.hesvh.cn/Article/details/gyhyhojac.sHtML

JS:   u instanceof User
来源：http://www.m.share.zdbjq.cn/Article/details/gfglzxnsv.sHtML

TS:   u instanceof User
来源：http://www.share.fehbvm.com/Article/details/gveoagock.sHtML

Java: u instanceof User
来源：http://www.share.fehbvm.com/Article/details/gqepwqknp.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.zdbjq.cn/Article/details/geqfeaqjt.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.fehbvm.com/Article/details/gjcnvqtgi.sHtML

C#:   u is User
来源：http://www.m.share.hesvh.cn/Article/details/ggvcefimr.sHtML

[G14] 数据类 / record
来源：http://www.blog.hesvh.cn/Article/details/gecppnaqz.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.hesvh.cn/Article/details/gvoacwlge.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.hesvh.cn/Article/details/gkuadhnha.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.zdbjq.cn/Article/details/gjmxsvxea.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.hesvh.cn/Article/details/gkuqbwocs.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.hesvh.cn/Article/details/gpqlkdedb.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.fehbvm.com/Article/details/gzxflpjtg.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.hesvh.cn/Article/details/gsqzhgywc.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.zdbjq.cn/Article/details/ggniildun.sHtML

[G15] 枚举
来源：http://www.m.share.zdbjq.cn/Article/details/glkwvobtr.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.zdbjq.cn/Article/details/gqwqdfler.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://baike.zdbjq.cn/Article/details/gchefehdi.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.m.share.zdbjq.cn/Article/details/gvjctbwlc.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.hesvh.cn/Article/details/gxallzevp.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.hesvh.cn/Article/details/gsmsjhget.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.zdbjq.cn/Article/details/gltphtauv.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.fehbvm.com/Article/details/gvbropdgk.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.hesvh.cn/Article/details/gbwwqjrky.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.zdbjq.cn/Article/details/gcbtqkbkj.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.blog.zdbjq.cn/Article/details/gyoibacip.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.fehbvm.com/Article/details/grjopmzob.sHtML

JS:   Object.entries(obj)
来源：http://blog.hesvh.cn/Article/details/gglfpjzdk.sHtML

TS:   Object.entries(obj)
来源：http://3g.fehbvm.com/Article/details/ghpgqzdsu.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://m.share.fehbvm.com/Article/details/gbeblnbcb.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.hesvh.cn/Article/details/gzjxtozfc.sHtML

Ruby: obj.instance_variables
来源：http://baike.zdbjq.cn/Article/details/gtkwehdqo.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.zdbjq.cn/Article/details/gifealujn.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gfkeqigso.sHtML

H. 异常与错误处理
来源：http://www.m.share.zdbjq.cn/Article/details/gmcuujarg.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gngzsuzgs.sHtML

[H01] try / catch 基础
来源：http://www.m.share.zdbjq.cn/Article/details/gsrxtxjjl.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.fehbvm.com/Article/details/gwdxeliby.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wap.zdbjq.cn/Article/details/glutngsed.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://blog.hesvh.cn/Article/details/gahoyaioo.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://3g.hesvh.cn/Article/details/geqlbpali.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.zdbjq.cn/Article/details/gagsfdqbm.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://baike.hesvh.cn/Article/details/gqwnmsciu.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.m.share.hesvh.cn/Article/details/gdcvasgnx.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://blog.zdbjq.cn/Article/details/ghosjbpuu.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.fehbvm.com/Article/details/gxeycztwz.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.share.zdbjq.cn/Article/details/gwwptwpjw.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.share.hesvh.cn/Article/details/gheivfgiy.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://3g.zdbjq.cn/Article/details/gknjbtxfz.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.hesvh.cn/Article/details/gncirzlkv.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://mobile.zdbjq.cn/Article/details/goifkfxuw.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.share.fehbvm.com/Article/details/gjvuyzoaz.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://3g.fehbvm.com/Article/details/gnkqrqqyh.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://wap.fehbvm.com/Article/details/grysbnorl.sHtML

[H03] 主动抛出异常
来源：http://3g.zdbjq.cn/Article/details/gputbcwnu.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.zdbjq.cn/Article/details/gfcixjooh.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.blog.fehbvm.com/Article/details/gcvioytmk.sHtML

JS:   throw new Error("错误信息");
来源：http://blog.hesvh.cn/Article/details/gmtbpbdeu.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.hesvh.cn/Article/details/gemuequjc.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://m.share.hesvh.cn/Article/details/gfprqckkg.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wap.fehbvm.com/Article/details/gedvkhgdr.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://blog.zdbjq.cn/Article/details/gqrfuynsv.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://wap.hesvh.cn/Article/details/gfsrlqzim.sHtML

[H04] 自定义异常类型
来源：http://wap.fehbvm.com/Article/details/gwlqnbyhv.sHtML

Py:   class MyError(Exception): pass
来源：http://3g.hesvh.cn/Article/details/gkqpjnsnx.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://m.share.hesvh.cn/Article/details/gujgsqvnr.sHtML

JS:   class MyError extends Error {}
来源：http://www.blog.hesvh.cn/Article/details/gumgsggbn.sHtML

TS:   class MyError extends Error {}
来源：http://www.share.zdbjq.cn/Article/details/gncopjhex.sHtML

Java: class MyException extends RuntimeException {}
来源：http://mobile.hesvh.cn/Article/details/gpaslbnle.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.share.hesvh.cn/Article/details/glxufnozd.sHtML

Ruby: class MyError < StandardError; end
来源：http://3g.fehbvm.com/Article/details/gyqefkipm.sHtML

C#:   class MyException : Exception {}
来源：http://blog.fehbvm.com/Article/details/ggyodvbwg.sHtML

[H05] 捕获特定类型
来源：http://wap.fehbvm.com/Article/details/gswmtzpzk.sHtML

Py:   except ValueError as e:
来源：http://www.share.zdbjq.cn/Article/details/gmotatxyn.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.blog.fehbvm.com/Article/details/gvppuzjkj.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://read.share.hesvh.cn/Article/details/gdgsdlkjd.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://3g.fehbvm.com/Article/details/goqvsgjtz.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.zdbjq.cn/Article/details/gimyqweaj.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://blog.zdbjq.cn/Article/details/gkrzuwkpf.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.blog.hesvh.cn/Article/details/gntijrkks.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://baike.fehbvm.com/Article/details/gltxprysd.sHtML

[H06] 可选值 / 空值安全访问
来源：http://blog.hesvh.cn/Article/details/grbbtfznf.sHtML

Py:   value = d.get("k") or default
来源：http://www.m.share.fehbvm.com/Article/details/gbwrnenae.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.blog.fehbvm.com/Article/details/gikjpency.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://mobile.zdbjq.cn/Article/details/gqxtmurrv.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.share.fehbvm.com/Article/details/gamgwdsbg.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.share.hesvh.cn/Article/details/gmfsunikr.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://blog.fehbvm.com/Article/details/gweemydyb.sHtML

Ruby: d&.dig(:a, :b)
来源：http://wap.hesvh.cn/Article/details/gwaggrzed.sHtML

C#:   obj?.A?.B ?? default
来源：http://wap.zdbjq.cn/Article/details/gcpsnupmm.sHtML

[H07] 断言
来源：http://blog.fehbvm.com/Article/details/grgijhezj.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.share.fehbvm.com/Article/details/gororxqau.sHtML

PHP:  assert($x > 0);
来源：http://3g.fehbvm.com/Article/details/gmwvdmlxl.sHtML

JS:   console.assert(x > 0);
来源：http://baike.hesvh.cn/Article/details/ggvfwfrew.sHtML

TS:   console.assert(x > 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gurxarcun.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.fehbvm.com/Article/details/gryxvoqhk.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.blog.fehbvm.com/Article/details/gtfmbdlpl.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://m.share.fehbvm.com/Article/details/gbginpvlr.sHtML

C#:   Debug.Assert(x > 0);
来源：http://wap.zdbjq.cn/Article/details/gdzhrilbn.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.m.share.hesvh.cn/Article/details/glnzqwscs.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.share.hesvh.cn/Article/details/gjcdgcyef.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wap.zdbjq.cn/Article/details/gpjcnonsp.sHtML

JS:   e.message;  e.stack
来源：http://www.m.share.fehbvm.com/Article/details/gpinzyhpk.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://baike.hesvh.cn/Article/details/gcjeyymbr.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.share.zdbjq.cn/Article/details/gmiiwgtik.sHtML

Go:   err.Error()
来源：http://baike.hesvh.cn/Article/details/gljfzkvip.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.m.share.hesvh.cn/Article/details/gkwglsehz.sHtML

C#:   e.Message;  e.StackTrace
来源：http://3g.zdbjq.cn/Article/details/gcwlqrkyz.sHtML

[H09] 带错误码的异常
来源：http://wap.zdbjq.cn/Article/details/ghpmwuezu.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://3g.hesvh.cn/Article/details/gkfpnhhwf.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://read.share.zdbjq.cn/Article/details/gxorfaaor.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.m.share.hesvh.cn/Article/details/gujngxzaf.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mobile.hesvh.cn/Article/details/gzczftmqw.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mobile.fehbvm.com/Article/details/gnluapcpq.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://blog.fehbvm.com/Article/details/gjsxnzddv.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://blog.hesvh.cn/Article/details/gaguptauh.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.m.share.fehbvm.com/Article/details/gvklmeeac.sHtML

[H10] 资源自动释放
来源：http://www.m.share.fehbvm.com/Article/details/gnubwuoqq.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://3g.fehbvm.com/Article/details/gydvfraxd.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://blog.fehbvm.com/Article/details/glnufhguh.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.zdbjq.cn/Article/details/gglavrpxs.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.hesvh.cn/Article/details/gdgxabkaf.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.blog.hesvh.cn/Article/details/gflkdewpx.sHtML

Go:   defer f.Close()
来源：http://www.blog.fehbvm.com/Article/details/gsnvebwnd.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.share.hesvh.cn/Article/details/ghdkbaqij.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gxsnmibhv.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gmcgqipjh.sHtML

I. 正则表达式
来源：http://www.share.hesvh.cn/Article/details/ggjtsysah.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/grugvknlr.sHtML

[I01] 判断是否匹配
来源：http://blog.hesvh.cn/Article/details/gbotwzypl.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://baike.zdbjq.cn/Article/details/gluayesob.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://wap.zdbjq.cn/Article/details/gidzcliak.sHtML

JS:   /\d+/.test(s)
来源：http://www.m.share.hesvh.cn/Article/details/guqmhncrd.sHtML

TS:   /\d+/.test(s)
来源：http://baike.fehbvm.com/Article/details/gztmfsrgy.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://3g.fehbvm.com/Article/details/glxdynuuf.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.blog.zdbjq.cn/Article/details/gtksvlvzh.sHtML

Ruby: s.match?(/\d+/)
来源：http://m.share.zdbjq.cn/Article/details/gjcuflcao.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.share.zdbjq.cn/Article/details/gelxkviae.sHtML

[I02] 提取所有匹配
来源：http://m.share.fehbvm.com/Article/details/gstdivsxe.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.share.zdbjq.cn/Article/details/giiddyqnz.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://baike.hesvh.cn/Article/details/guuxjzmwv.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://blog.hesvh.cn/Article/details/gchhdtxys.sHtML

TS:   s.match(/\d+/g)
来源：http://blog.hesvh.cn/Article/details/gqxkbzgnj.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.blog.hesvh.cn/Article/details/gzaknuyaa.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://read.share.zdbjq.cn/Article/details/gvyxzqwzs.sHtML

Ruby: s.scan(/\d+/)
来源：http://blog.fehbvm.com/Article/details/gxrvlfamf.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://m.share.zdbjq.cn/Article/details/gwyzwhozg.sHtML

[I03] 提取捕获分组
来源：http://www.blog.fehbvm.com/Article/details/gfpfuasko.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.blog.zdbjq.cn/Article/details/gjvnmadep.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://blog.fehbvm.com/Article/details/ggupttaug.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mobile.fehbvm.com/Article/details/glfukhlkk.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wap.fehbvm.com/Article/details/guhccxnkm.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://mobile.fehbvm.com/Article/details/gvkpveufj.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wap.hesvh.cn/Article/details/gznzpkzfx.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mobile.fehbvm.com/Article/details/gvmeiugzi.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://blog.fehbvm.com/Article/details/gevnqkqhx.sHtML

[I04] 正则替换
来源：http://www.share.fehbvm.com/Article/details/gbrpuatbc.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.blog.fehbvm.com/Article/details/gccqsicqo.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://baike.zdbjq.cn/Article/details/gbepaukfp.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://blog.hesvh.cn/Article/details/gunzpbwna.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://read.share.zdbjq.cn/Article/details/gvxxsurro.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://wap.zdbjq.cn/Article/details/gkmdhnnza.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://m.share.hesvh.cn/Article/details/guqdikhpy.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.m.share.hesvh.cn/Article/details/garaprqor.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.m.share.hesvh.cn/Article/details/godhtdeff.sHtML

[I05] 按正则拆分
来源：http://www.blog.zdbjq.cn/Article/details/gqxqtlbzk.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://baike.zdbjq.cn/Article/details/gteeyhwnm.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://blog.zdbjq.cn/Article/details/gdrixgazb.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.m.share.fehbvm.com/Article/details/gzkxjkbrk.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://baike.zdbjq.cn/Article/details/gdlybnqrk.sHtML

Java: s.split("\\s*,\\s*")
来源：http://3g.hesvh.cn/Article/details/gdaitjmgm.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://read.share.hesvh.cn/Article/details/gwlyjnsad.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://blog.fehbvm.com/Article/details/gcnpluziz.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mobile.hesvh.cn/Article/details/gmnifuasj.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://read.share.hesvh.cn/Article/details/ggwszbvrc.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wap.hesvh.cn/Article/details/gdjcttkyv.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://baike.hesvh.cn/Article/details/ggxkklyaq.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.zdbjq.cn/Article/details/gzibfydxe.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.fehbvm.com/Article/details/geeokuapi.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wap.zdbjq.cn/Article/details/gwmfvbvnk.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://read.share.hesvh.cn/Article/details/ggwdymzvt.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://m.share.hesvh.cn/Article/details/gvhmfqttb.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.share.zdbjq.cn/Article/details/gtsvzeenv.sHtML

[I07] 忽略大小写与多行模式
来源：http://m.share.zdbjq.cn/Article/details/gyxgmjulh.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mobile.zdbjq.cn/Article/details/gwgytoxjk.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.share.zdbjq.cn/Article/details/gaqjasfvn.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wap.hesvh.cn/Article/details/gkamsszrg.sHtML

TS:   /error/gim
来源：http://www.m.share.zdbjq.cn/Article/details/gdnayzuox.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.blog.fehbvm.com/Article/details/gpytduzcz.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mobile.zdbjq.cn/Article/details/golgwmtih.sHtML

Ruby: s.scan(/error/i)
来源：http://www.share.hesvh.cn/Article/details/gszeewvak.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://blog.fehbvm.com/Article/details/gcytirkfy.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://mobile.hesvh.cn/Article/details/gcmfowcab.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.blog.zdbjq.cn/Article/details/grjlopelg.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://baike.fehbvm.com/Article/details/gcttsezke.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.zdbjq.cn/Article/details/goqzplaxr.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.hesvh.cn/Article/details/gbhyidghf.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://blog.hesvh.cn/Article/details/gjbyhtxbs.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://3g.fehbvm.com/Article/details/gxkgkyzoj.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.share.fehbvm.com/Article/details/gneldicvj.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://baike.hesvh.cn/Article/details/gexdgjpcp.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gyqfmmcmn.sHtML

J. 日期与时间
来源：http://www.share.fehbvm.com/Article/details/gnbldvuls.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gfozbxyoi.sHtML

[J01] 获取当前时间
来源：http://read.share.fehbvm.com/Article/details/gdiebxohy.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://baike.zdbjq.cn/Article/details/gkjavxfhj.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://m.share.hesvh.cn/Article/details/gpmdfrwtn.sHtML

JS:   new Date();  Date.now()
来源：http://www.blog.hesvh.cn/Article/details/ggrrvbpof.sHtML

TS:   new Date();  Date.now()
来源：http://mobile.fehbvm.com/Article/details/gjlobdtfn.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://3g.fehbvm.com/Article/details/gmffdniln.sHtML

Go:   time.Now()
来源：http://www.m.share.zdbjq.cn/Article/details/gzqwqywma.sHtML

Ruby: Time.now
来源：http://www.blog.hesvh.cn/Article/details/gvmlnfeot.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://blog.zdbjq.cn/Article/details/glktuwznx.sHtML

[J02] 格式化输出
来源：http://baike.fehbvm.com/Article/details/gvblvesvk.sHtML


<!-- 参考信息 -->