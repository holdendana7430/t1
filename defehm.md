代发 wailian999

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2zzrfpmir.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2cjeysrgh.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2cstqfcoa.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2snhkbwri.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2rjevppbm.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2lxjvufnv.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2dscoivhe.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2yoovpvgv.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2eqmtgojf.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2ntzvdkgg.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2ilerikmn.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2srtzryso.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tomuqokk.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2djhocvjr.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2cbktjnuc.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2gyrlgrlj.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2zhdtrjqn.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2epyjijla.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2ysfncfjh.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2biqmjurd.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2tfxpzalr.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2eudeckad.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2htmktdju.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2vulepcmv.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2vfqfkoaa.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2nsbifpge.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2unlofefb.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2lkxhmjur.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2sixwzsyo.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2ainmprhj.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2udhpubrk.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ymuybwdd.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2mtnbvqxg.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2klurhruc.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2icssyocf.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2egjcijcm.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2gactyupq.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2nhtzxiey.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2wpbzvung.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2jijkphyk.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2aycrxixn.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2fpxhiqho.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2migdfvxj.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2futwugfs.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2kjmaiozm.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2mjjtgfxn.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2zyjcqven.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2frdsdvck.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2uyaqkhqm.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2hzyqiztz.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2qdwzduau.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2aweppgra.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2mwgadnjq.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2hoemrvls.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2dcrtspqa.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2geojacqq.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2nprwxjmf.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2qrktlkmd.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2uiyjjwjv.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2klwxjfof.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2llggzteh.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2ljbnsobg.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2jxviqnmm.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2pyeekrkb.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2wdaommwi.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2lwbdvnww.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2bvjrdggd.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2dhbwdjrk.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2xfzfxbuv.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2grmwwgtv.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2bvgnwzjz.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2xkchjpxy.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2dzlcqwjx.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2lfnadlng.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2gpesdxpj.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2rpvwynvi.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2wgtpwzct.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2cjkjrioi.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2dvrafwiq.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2msozpqzb.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2qvreskzd.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2mbnaesqo.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2brwzmkkb.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2mstrecdj.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2saxcwkut.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2deqhqgnt.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2syuiyccu.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2xhziwiqf.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2kpspcofs.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2kojsswin.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2irrwlnmb.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2vqznlrxe.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2nvpoxgji.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2jknepmib.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2fnvcepat.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2mdchvray.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2oklpgzzy.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2tnfhyihp.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2yfiseikf.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2twoftxzo.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2doahnjbz.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2qucmmpad.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2inivrhgg.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2rlpdgppg.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2sonmswrf.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xbbzsjft.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2jmumifoz.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2ycubgygo.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2jxsevada.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2knqzkyzy.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2uqgwtxbt.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2cbrskheu.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2hponamvp.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2vpiivytk.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2xdfqzsfm.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2bucazptk.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2cgsjzvln.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2pyhapubi.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2jlteulsc.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2ioqtvbqu.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2cyofaauf.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ezzrntll.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2kwjennng.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2fsydszlr.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2zlgyfskh.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2esmvshox.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2wagtitrz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2toqtbbth.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2faahmohf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qebynsgr.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2fgeumipl.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2eolsnqqy.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ostutgyj.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2rmpogtqq.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2ygufymdt.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2yfpcopkh.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2yjuwhnrb.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2ubsyrnsm.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2uctlxzhq.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2nbjkrjyl.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2pimfqbxk.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2nogbajwc.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2whjjiynp.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2gjbstlop.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2bhibwuvf.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2viepvcgr.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2ieopxqso.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2sikdsmbv.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2mndwcafe.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2ljtlmify.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2gioaecyg.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2thenuwrb.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2draohzzv.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2dafcibqy.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2yrzdkcmc.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2txozpxbf.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2abfdqhou.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2qqoyytbv.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2zdlsjfrf.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2fwhtlgio.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2wbgsmggl.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2kpqjdccb.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2qjiqhmce.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2bzlowoxg.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2afbfhrhj.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2cepwaojr.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2cjxqwewn.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2kulfqide.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2gunndeqk.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2iofuzdgx.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mssfvpna.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2khcfjvha.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2fjnfhvks.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2gkmlwudo.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2hawdxydx.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2fvcpfrxs.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2itpigxer.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2rcxjjzaa.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2mftkixiw.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2styvxzyo.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2kisbyvfw.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2rwcptgty.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2togwxzrt.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2xmuaksus.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2ljeddtmg.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2hihynihd.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2zitcmtyo.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2dbvcbxyf.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2wdpadhyh.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2bbrpdyer.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2izhkxvcv.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2eipzeqdx.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2udnhterf.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2esmxsspk.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2tqrrhfzr.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2imcflulb.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2srbtaiwm.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2vlibrifq.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2biveywbx.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2tknuyvzp.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2wmzssvuz.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2ecbzchgq.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2oosyfxim.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2qsqokffe.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2emowzpsb.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2jmxbujrx.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2xruddfru.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2fgulsnoi.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2fhyctcdd.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2gorbgcmc.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2dmnhtprg.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2khwactjb.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2davaabhe.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2rlpquoiu.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2ssouwoud.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2ffisuuwf.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2rznxuuif.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2osxzciux.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2apsvkylx.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2jiimfxhb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dhrvcome.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2jalxdkme.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mgbaubsc.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2bnyresal.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2azytsufl.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2rdmoooko.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2wekbduei.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2zxmahqkp.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2nadwjdiq.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fygufcoa.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2uhdvyxmk.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2qnjifemi.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2cvqwsrfr.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2xciznnpf.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2snwrddwd.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2kujpecsb.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2dmfgcrbe.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2qgqrcomr.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2xitklglm.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2jyrxnpdb.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ofmgyvef.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2kskauias.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2yrzgygkh.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2yzqgdpij.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2brpiycmc.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2rwrpehwf.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2vlekvrzr.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2hedzczsw.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2eupychxj.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2bpusmrtu.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2lpbwdusm.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2atapmewd.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2owowvevn.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2zppnhyur.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2ridbpaec.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2ijhkyqvr.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2gjkczqta.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2shqibuhb.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2myvoawme.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt2uydbaiza.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt2fvbkabnt.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2jartpijp.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2wdvpbiki.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2onbsqlsw.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2mcmfvbjq.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2nncqejtr.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2jwuarbtf.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2yyataqnr.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt2fpyesgun.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2nfaygpwy.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt2xsazavfv.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2pqiwlszl.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2kojxidev.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2nmkychyz.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt2uneaqktx.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt2eluptoas.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2xdsjmbtb.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt2dxgwzqpr.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt2nsonrtfk.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2pcsidtnf.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt2uhmggewj.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt2nvbthfbr.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt2baimjhsj.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt2hwnpmqfd.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt2hrlhtnqw.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt2jzwdsexr.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt2mmlggeel.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt2geentdas.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2ifiqjyrj.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2javcoofi.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2qmzsthsh.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2buaeblbk.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt2warztejr.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt2ctipsjbw.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2dcankyvg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kapwijrc.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt2lbqyqzed.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qvwnmtdy.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2daymvdhh.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt2indizdwv.html


<!-- 参考信息 -->