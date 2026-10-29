代发 wailian999

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.zdbjq.cn/Article/details/ggipgnmaq.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.fehbvm.com/Article/details/ggosuzwkh.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.fehbvm.com/Article/details/goetpbbuz.sHtML

Java: String greet() { return name; }
来源：http://wap.fehbvm.com/Article/details/gitvrtkzv.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.zdbjq.cn/Article/details/goifdaeeq.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.fehbvm.com/Article/details/gzzheatny.sHtML

C#:   public string Greet() => Name;
来源：http://blog.hesvh.cn/Article/details/gjznubwsi.sHtML

[G05] 继承
来源：http://mobile.fehbvm.com/Article/details/gbvcvietb.sHtML

Py:   class Admin(User): pass
来源：http://3g.fehbvm.com/Article/details/gvstmlnup.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.hesvh.cn/Article/details/guupznkst.sHtML

JS:   class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/gqkplpnqd.sHtML

TS:   class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/gjweywsbg.sHtML

Java: class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/gxfulrfsw.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.fehbvm.com/Article/details/gzynzdutl.sHtML

Ruby: class Admin < User; end
来源：http://mobile.fehbvm.com/Article/details/gzvwoqrew.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.hesvh.cn/Article/details/gkuhlbyox.sHtML

[G06] 重写方法
来源：http://www.m.share.fehbvm.com/Article/details/gxfehadot.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.zdbjq.cn/Article/details/gtbqngkqo.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/gjkxhrwrs.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gtkjwvrhy.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/ghwetosdt.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/gnxttijwy.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.fehbvm.com/Article/details/ghmoijdkv.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.zdbjq.cn/Article/details/gsdvnurkg.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.fehbvm.com/Article/details/ghxejxnmv.sHtML

[G07] 调用父类方法
来源：http://mobile.fehbvm.com/Article/details/gubnkhlwe.sHtML

Py:   super().greet()
来源：http://www.blog.hesvh.cn/Article/details/gsuycagsk.sHtML

PHP:  parent::greet();
来源：http://www.blog.fehbvm.com/Article/details/gciedxnpn.sHtML

JS:   super.greet();
来源：http://baike.hesvh.cn/Article/details/gowahplpk.sHtML

TS:   super.greet();
来源：http://www.blog.fehbvm.com/Article/details/gugizpwnx.sHtML

Java: super.greet();
来源：http://m.share.zdbjq.cn/Article/details/gfwaafirk.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.zdbjq.cn/Article/details/gefbrguwh.sHtML

Ruby: super
来源：http://3g.zdbjq.cn/Article/details/ghvjtxvwq.sHtML

C#:   base.Greet();
来源：http://wap.fehbvm.com/Article/details/gncnxpptw.sHtML

[G08] 静态方法与属性
来源：http://m.share.fehbvm.com/Article/details/gkxfhqxvv.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.hesvh.cn/Article/details/giuxpsynj.sHtML

PHP:  public static function f() {}
来源：http://3g.hesvh.cn/Article/details/gzmtvozqg.sHtML

JS:   static f() {}
来源：http://www.blog.fehbvm.com/Article/details/grpqnwdnz.sHtML

TS:   static f(): void {}
来源：http://www.m.share.fehbvm.com/Article/details/ggfdvdsfd.sHtML

Java: static void f() {}
来源：http://read.share.zdbjq.cn/Article/details/grzvmmsdu.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.zdbjq.cn/Article/details/gkcgenekz.sHtML

Ruby: def self.f; end
来源：http://www.share.fehbvm.com/Article/details/gtfhofjgc.sHtML

C#:   public static void F() {}
来源：http://www.share.fehbvm.com/Article/details/gejuykeey.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.hesvh.cn/Article/details/gjkvugekm.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.zdbjq.cn/Article/details/gnqjhfywu.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.fehbvm.com/Article/details/gcbxaenky.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.zdbjq.cn/Article/details/gvlgnnuuh.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.zdbjq.cn/Article/details/gevcfgnmx.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.fehbvm.com/Article/details/gygfarsim.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.hesvh.cn/Article/details/geuseagfi.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.zdbjq.cn/Article/details/gelplezxq.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.zdbjq.cn/Article/details/gbtiliotv.sHtML

[G10] 访问控制
来源：http://mobile.zdbjq.cn/Article/details/gqonvoaoc.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.fehbvm.com/Article/details/ghhehoroe.sHtML

PHP:  public / protected / private
来源：http://wap.fehbvm.com/Article/details/gibowkytg.sHtML

JS:   #private 字段；其余公开
来源：http://3g.hesvh.cn/Article/details/gtxxwoknr.sHtML

TS:   public / protected / private
来源：http://www.share.zdbjq.cn/Article/details/gzyiicjeq.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.fehbvm.com/Article/details/gufsoxrba.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.fehbvm.com/Article/details/gscyrtaob.sHtML

Ruby: public / protected / private
来源：http://wap.zdbjq.cn/Article/details/gdrsiodzx.sHtML

C#:   public / protected / private / internal
来源：http://www.share.zdbjq.cn/Article/details/ggpkjchvj.sHtML

[G11] getter / setter
来源：http://www.blog.hesvh.cn/Article/details/gqurmmapt.sHtML

Py:   @property 与 @x.setter
来源：http://blog.fehbvm.com/Article/details/grfhptjfh.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.hesvh.cn/Article/details/gqionvzqj.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.hesvh.cn/Article/details/gobnxllkz.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.fehbvm.com/Article/details/gzwhkbmpi.sHtML

Java: public String getName() { return name; }
来源：http://mobile.hesvh.cn/Article/details/gweslbwxr.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.hesvh.cn/Article/details/glxogplqs.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.zdbjq.cn/Article/details/ghiyzqhok.sHtML

C#:   public string Name { get; set; }
来源：http://3g.fehbvm.com/Article/details/gqpbdqevh.sHtML

[G12] 对象转字符串
来源：http://baike.zdbjq.cn/Article/details/gyhxzjjam.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.hesvh.cn/Article/details/gaemijsiv.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.fehbvm.com/Article/details/geqoukjnk.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/grfhktrik.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.zdbjq.cn/Article/details/gnmsovkkr.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.fehbvm.com/Article/details/gjcpklypo.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.zdbjq.cn/Article/details/gititvrgs.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.hesvh.cn/Article/details/gkvdufaxh.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.fehbvm.com/Article/details/gbeabmmsn.sHtML

[G13] 判断对象类型
来源：http://wap.fehbvm.com/Article/details/gmlweofgo.sHtML

Py:   isinstance(u, User)
来源：http://www.share.zdbjq.cn/Article/details/gbwgomgzu.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.fehbvm.com/Article/details/gomzxwckp.sHtML

JS:   u instanceof User
来源：http://mobile.hesvh.cn/Article/details/gacjydrgb.sHtML

TS:   u instanceof User
来源：http://www.share.zdbjq.cn/Article/details/gkcncbpvm.sHtML

Java: u instanceof User
来源：http://www.m.share.hesvh.cn/Article/details/gyuecjyyg.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.zdbjq.cn/Article/details/gyqrpywlz.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.hesvh.cn/Article/details/giuihusez.sHtML

C#:   u is User
来源：http://mobile.zdbjq.cn/Article/details/gtbvvdxmy.sHtML

[G14] 数据类 / record
来源：http://wap.zdbjq.cn/Article/details/gcsqrjvkt.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.hesvh.cn/Article/details/gdoqkuplt.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.hesvh.cn/Article/details/gcxhxvpuz.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.hesvh.cn/Article/details/gpwkooodm.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.hesvh.cn/Article/details/gvkwxwdzc.sHtML

Java: record User(String name, int age) {}
来源：http://read.share.hesvh.cn/Article/details/gtlwljxpg.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.fehbvm.com/Article/details/gswkppgyo.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.zdbjq.cn/Article/details/gbzffqvdg.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.hesvh.cn/Article/details/gxemvzobn.sHtML

[G15] 枚举
来源：http://3g.zdbjq.cn/Article/details/gqfgqcmyl.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.zdbjq.cn/Article/details/gsqordizg.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.zdbjq.cn/Article/details/gyvkjzwcd.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.zdbjq.cn/Article/details/gvjizxkcp.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://3g.zdbjq.cn/Article/details/gzqscthle.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.hesvh.cn/Article/details/gqumkieoq.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.zdbjq.cn/Article/details/gbekacgrh.sHtML

Ruby: Color = %i[red green].freeze
来源：http://m.share.fehbvm.com/Article/details/gglynyzvp.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.zdbjq.cn/Article/details/gonxfpcnm.sHtML

[G16] 对象转数组 / 字典
来源：http://www.m.share.zdbjq.cn/Article/details/gkjgfuwdg.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.zdbjq.cn/Article/details/gwuepxbya.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.fehbvm.com/Article/details/gkbmkyrnz.sHtML

JS:   Object.entries(obj)
来源：http://read.share.fehbvm.com/Article/details/gliakghsm.sHtML

TS:   Object.entries(obj)
来源：http://wap.zdbjq.cn/Article/details/ghwbglhau.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.share.hesvh.cn/Article/details/glyvvkhxm.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.zdbjq.cn/Article/details/gdpoupthg.sHtML

Ruby: obj.instance_variables
来源：http://read.share.zdbjq.cn/Article/details/gvztdxyly.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.hesvh.cn/Article/details/ghtpsuvde.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gcbbgdjly.sHtML

H. 异常与错误处理
来源：http://blog.zdbjq.cn/Article/details/gssbwlhzu.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/ghmynbhhq.sHtML

[H01] try / catch 基础
来源：http://baike.fehbvm.com/Article/details/ghrctzvcw.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.zdbjq.cn/Article/details/gdsxjlewx.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.zdbjq.cn/Article/details/gclvrovat.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://m.share.hesvh.cn/Article/details/gmjvlvhny.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.zdbjq.cn/Article/details/gmekrhhve.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.blog.hesvh.cn/Article/details/ggssyblbo.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://read.share.fehbvm.com/Article/details/gviyfewkz.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.hesvh.cn/Article/details/gtugszwbo.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.m.share.zdbjq.cn/Article/details/gdlnwubib.sHtML

[H02] finally / ensure 收尾
来源：http://baike.zdbjq.cn/Article/details/gixldfrty.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://baike.fehbvm.com/Article/details/gktzltzey.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.zdbjq.cn/Article/details/gdydqxsxk.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://wap.fehbvm.com/Article/details/gfgtejaik.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.zdbjq.cn/Article/details/ghaislqdb.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://wap.fehbvm.com/Article/details/gpqyimdmt.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.fehbvm.com/Article/details/gsywuxwaw.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.m.share.zdbjq.cn/Article/details/gwhbsdgjh.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/gldesosvt.sHtML

[H03] 主动抛出异常
来源：http://www.blog.fehbvm.com/Article/details/gcelgeszu.sHtML

Py:   raise ValueError("错误信息")
来源：http://3g.hesvh.cn/Article/details/ggkwgywqv.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mobile.zdbjq.cn/Article/details/gecvhjpgb.sHtML

JS:   throw new Error("错误信息");
来源：http://www.share.zdbjq.cn/Article/details/ghzlxqpfv.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.fehbvm.com/Article/details/gafurfmnw.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://mobile.zdbjq.cn/Article/details/greagdisl.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://m.share.fehbvm.com/Article/details/gcfebvuvb.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.m.share.fehbvm.com/Article/details/graievkjp.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://m.share.hesvh.cn/Article/details/gxwyvsnwv.sHtML

[H04] 自定义异常类型
来源：http://m.share.hesvh.cn/Article/details/gmbahpngg.sHtML

Py:   class MyError(Exception): pass
来源：http://baike.fehbvm.com/Article/details/ggxzfgmyk.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.zdbjq.cn/Article/details/ghavcpnno.sHtML

JS:   class MyError extends Error {}
来源：http://www.m.share.fehbvm.com/Article/details/gpcefxksz.sHtML

TS:   class MyError extends Error {}
来源：http://blog.fehbvm.com/Article/details/gtsjbfgwx.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.share.hesvh.cn/Article/details/gzuqpnfth.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.blog.hesvh.cn/Article/details/gfybvotfq.sHtML

Ruby: class MyError < StandardError; end
来源：http://read.share.hesvh.cn/Article/details/gnizhkrzy.sHtML

C#:   class MyException : Exception {}
来源：http://m.share.hesvh.cn/Article/details/geovenlsg.sHtML

[H05] 捕获特定类型
来源：http://www.blog.hesvh.cn/Article/details/gyywlwszn.sHtML

Py:   except ValueError as e:
来源：http://www.m.share.zdbjq.cn/Article/details/gmgkyglxm.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.m.share.fehbvm.com/Article/details/gczncdssk.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://blog.fehbvm.com/Article/details/gpzudjvhd.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://read.share.fehbvm.com/Article/details/gwplpolkr.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://blog.zdbjq.cn/Article/details/gdzimkjvj.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.share.fehbvm.com/Article/details/gmthbettk.sHtML

Ruby: rescue ArgumentError => e
来源：http://blog.zdbjq.cn/Article/details/gyjxhleow.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://3g.fehbvm.com/Article/details/gakgqiymn.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.share.hesvh.cn/Article/details/gfhmllizu.sHtML

Py:   value = d.get("k") or default
来源：http://mobile.zdbjq.cn/Article/details/griejpgjv.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.hesvh.cn/Article/details/gepnglhdr.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.zdbjq.cn/Article/details/gyudsmuij.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://mobile.fehbvm.com/Article/details/gyeqejzgj.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.m.share.zdbjq.cn/Article/details/gbiyhibpb.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://blog.zdbjq.cn/Article/details/gzhivjhrf.sHtML

Ruby: d&.dig(:a, :b)
来源：http://read.share.zdbjq.cn/Article/details/gtdakoivp.sHtML

C#:   obj?.A?.B ?? default
来源：http://wap.hesvh.cn/Article/details/ghdbvsbja.sHtML

[H07] 断言
来源：http://m.share.fehbvm.com/Article/details/gznxuocfb.sHtML

Py:   assert x > 0, "必须为正"
来源：http://blog.fehbvm.com/Article/details/gcmicvaia.sHtML

PHP:  assert($x > 0);
来源：http://3g.zdbjq.cn/Article/details/gtljhteoo.sHtML

JS:   console.assert(x > 0);
来源：http://m.share.hesvh.cn/Article/details/gfwepkhyu.sHtML

TS:   console.assert(x > 0);
来源：http://mobile.zdbjq.cn/Article/details/gxktcmrwl.sHtML

Java: assert x > 0 : "必须为正";
来源：http://blog.zdbjq.cn/Article/details/gnmebyvtq.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wap.zdbjq.cn/Article/details/gmgtzzgkg.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.share.zdbjq.cn/Article/details/gvzwyrjaf.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.share.fehbvm.com/Article/details/gqnvxezga.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.blog.zdbjq.cn/Article/details/gqfalezli.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://baike.hesvh.cn/Article/details/gvmjthrsk.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://baike.fehbvm.com/Article/details/gxdtdmaba.sHtML

JS:   e.message;  e.stack
来源：http://3g.fehbvm.com/Article/details/gswamlaym.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://m.share.hesvh.cn/Article/details/gdjxuufoe.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://m.share.hesvh.cn/Article/details/gwvqodtjj.sHtML

Go:   err.Error()
来源：http://www.blog.fehbvm.com/Article/details/gfebtogyc.sHtML

Ruby: e.message;  e.backtrace
来源：http://m.share.hesvh.cn/Article/details/gblnylhem.sHtML

C#:   e.Message;  e.StackTrace
来源：http://3g.zdbjq.cn/Article/details/gnljfjkzg.sHtML

[H09] 带错误码的异常
来源：http://www.m.share.fehbvm.com/Article/details/gztzteqpq.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://3g.hesvh.cn/Article/details/gfwsitbqy.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://3g.hesvh.cn/Article/details/gsobvuiim.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wap.hesvh.cn/Article/details/ghhggzeuk.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mobile.hesvh.cn/Article/details/ggrlzkgvh.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.m.share.fehbvm.com/Article/details/gcqvltgvk.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wap.zdbjq.cn/Article/details/gsyoyrcfy.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://m.share.zdbjq.cn/Article/details/gdkifuunu.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://baike.hesvh.cn/Article/details/gvbdwegmu.sHtML

[H10] 资源自动释放
来源：http://m.share.hesvh.cn/Article/details/ggbjmkbey.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://baike.hesvh.cn/Article/details/gheumhndp.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.blog.fehbvm.com/Article/details/gjajojfla.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.hesvh.cn/Article/details/gouxwcpne.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.zdbjq.cn/Article/details/gnnhzoejg.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://m.share.fehbvm.com/Article/details/gdtlotdcz.sHtML

Go:   defer f.Close()
来源：http://read.share.hesvh.cn/Article/details/gpjjrejls.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://baike.zdbjq.cn/Article/details/gqgxbhktx.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/ggioaxsxh.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gzqusjxrt.sHtML

I. 正则表达式
来源：http://www.share.zdbjq.cn/Article/details/gpcndonpz.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gvjmeqbru.sHtML

[I01] 判断是否匹配
来源：http://mobile.fehbvm.com/Article/details/gpxtbcfgr.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://blog.hesvh.cn/Article/details/ghihsnxgb.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://blog.zdbjq.cn/Article/details/geujtznwc.sHtML

JS:   /\d+/.test(s)
来源：http://blog.fehbvm.com/Article/details/gkfbbtihi.sHtML

TS:   /\d+/.test(s)
来源：http://3g.hesvh.cn/Article/details/gmudohiol.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.share.hesvh.cn/Article/details/gtmrjaucj.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.m.share.fehbvm.com/Article/details/gioogumem.sHtML

Ruby: s.match?(/\d+/)
来源：http://wap.zdbjq.cn/Article/details/gczhtejpx.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://3g.hesvh.cn/Article/details/gffxiysje.sHtML

[I02] 提取所有匹配
来源：http://baike.zdbjq.cn/Article/details/gsagrfmlr.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.blog.fehbvm.com/Article/details/gjsafvvia.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://3g.zdbjq.cn/Article/details/gonkdcanx.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.m.share.fehbvm.com/Article/details/gomhevoke.sHtML

TS:   s.match(/\d+/g)
来源：http://www.share.zdbjq.cn/Article/details/gtfdcyhzm.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://read.share.hesvh.cn/Article/details/gdnyplbav.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.share.hesvh.cn/Article/details/glrgkvyns.sHtML

Ruby: s.scan(/\d+/)
来源：http://read.share.fehbvm.com/Article/details/gljbahror.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.blog.hesvh.cn/Article/details/ggcbwjvhx.sHtML

[I03] 提取捕获分组
来源：http://read.share.hesvh.cn/Article/details/gcyfkmhja.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gtgztcxah.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.blog.zdbjq.cn/Article/details/gooddgghh.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wap.fehbvm.com/Article/details/gctslwrms.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://read.share.fehbvm.com/Article/details/gvzsduhrn.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://blog.zdbjq.cn/Article/details/gmiklphzw.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://m.share.fehbvm.com/Article/details/gkkvldabo.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.blog.zdbjq.cn/Article/details/gvjojhicu.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://blog.fehbvm.com/Article/details/gnvdykjss.sHtML

[I04] 正则替换
来源：http://m.share.zdbjq.cn/Article/details/grigcqqqo.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://wap.fehbvm.com/Article/details/gesfmjtkm.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.share.zdbjq.cn/Article/details/gsrrnrxoo.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.fehbvm.com/Article/details/giuyhjwwq.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://3g.hesvh.cn/Article/details/gnmnfzwtp.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://m.share.fehbvm.com/Article/details/gmkwgxxej.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://m.share.fehbvm.com/Article/details/gxzturfqt.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.m.share.zdbjq.cn/Article/details/gflqvmzst.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.blog.hesvh.cn/Article/details/gxkdeterk.sHtML

[I05] 按正则拆分
来源：http://blog.fehbvm.com/Article/details/grrnlnrqt.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://wap.hesvh.cn/Article/details/gkdfekavf.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.share.zdbjq.cn/Article/details/ggfxjitgs.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://read.share.zdbjq.cn/Article/details/gvwwkvokd.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://blog.hesvh.cn/Article/details/gsxrsxsio.sHtML

Java: s.split("\\s*,\\s*")
来源：http://m.share.zdbjq.cn/Article/details/gbmtlnbgt.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://3g.fehbvm.com/Article/details/gctncfgdj.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.share.hesvh.cn/Article/details/gunpwrcyb.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.share.hesvh.cn/Article/details/gnmnmvngz.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://blog.zdbjq.cn/Article/details/gfzpwxedq.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.share.fehbvm.com/Article/details/gsisbetpe.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.blog.fehbvm.com/Article/details/ghrhhjiky.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.fehbvm.com/Article/details/gufuiylmb.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.zdbjq.cn/Article/details/gorgotard.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wap.zdbjq.cn/Article/details/gohinnufb.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://mobile.fehbvm.com/Article/details/gxemaodyi.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.blog.fehbvm.com/Article/details/gvxiquoud.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://blog.fehbvm.com/Article/details/gbfubfaur.sHtML

[I07] 忽略大小写与多行模式
来源：http://3g.hesvh.cn/Article/details/gqjlxichf.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://baike.hesvh.cn/Article/details/gnvmzkrvq.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://m.share.zdbjq.cn/Article/details/gmxkmnbol.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://3g.fehbvm.com/Article/details/ghegnopuv.sHtML

TS:   /error/gim
来源：http://baike.fehbvm.com/Article/details/gmpmsoqmc.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://blog.zdbjq.cn/Article/details/gkzdjuvrc.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://read.share.zdbjq.cn/Article/details/gnukhqydc.sHtML

Ruby: s.scan(/error/i)
来源：http://www.m.share.zdbjq.cn/Article/details/gzolyjeyb.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://read.share.hesvh.cn/Article/details/gaksncgtr.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://wap.fehbvm.com/Article/details/gtpqaozcf.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://baike.zdbjq.cn/Article/details/gkenuyafl.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.share.zdbjq.cn/Article/details/glxwirkkk.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.fehbvm.com/Article/details/gxzfdungd.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.fehbvm.com/Article/details/gsmaeczqu.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.blog.zdbjq.cn/Article/details/gdlxruwpo.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://m.share.hesvh.cn/Article/details/gtuuowsxi.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wap.zdbjq.cn/Article/details/gqluvunte.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.share.hesvh.cn/Article/details/geimtxafr.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gadousobe.sHtML

J. 日期与时间
来源：http://www.m.share.fehbvm.com/Article/details/gufoecuyl.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gsunqzasy.sHtML

[J01] 获取当前时间
来源：http://3g.fehbvm.com/Article/details/gnzxovhhl.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://baike.hesvh.cn/Article/details/gvphtxeqt.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://wap.hesvh.cn/Article/details/gzhhxmvjb.sHtML

JS:   new Date();  Date.now()
来源：http://baike.zdbjq.cn/Article/details/gkauygxdg.sHtML

TS:   new Date();  Date.now()
来源：http://www.blog.zdbjq.cn/Article/details/gfoekpdoa.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://mobile.zdbjq.cn/Article/details/goqcidyfm.sHtML

Go:   time.Now()
来源：http://m.share.hesvh.cn/Article/details/gbnqyzkhy.sHtML

Ruby: Time.now
来源：http://read.share.hesvh.cn/Article/details/gkblyrrws.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://read.share.fehbvm.com/Article/details/gmdtctjew.sHtML

[J02] 格式化输出
来源：http://mobile.fehbvm.com/Article/details/gpuecivpd.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.fehbvm.com/Article/details/gfbeldydz.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://m.share.zdbjq.cn/Article/details/graqdqfvl.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://3g.fehbvm.com/Article/details/gdldrzdnv.sHtML

TS:   d.toISOString()
来源：http://blog.fehbvm.com/Article/details/gtutkejsy.sHtML


<!-- 参考信息 -->