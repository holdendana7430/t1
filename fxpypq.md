代发 wailian999

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2zvwsxsmz.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2cvnexlpn.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2kgtzgomj.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2pgqfxakf.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2yzboayke.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2wevojbme.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2zphlconj.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2jkpfepxp.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2ebluzdwc.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2yvhlazhx.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2ffwcqzcc.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2symoffrw.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2ryrcqznm.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2ztdxpqrk.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vaemlzrw.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2djuifhyl.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2zrqqkbyq.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2pbenbxrr.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2ktjhbsxu.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2fnryzeib.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2fxndymjs.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2ngnqnswu.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2eqhnihzg.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2jrbipjpq.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2ppqhmptj.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2brafulwi.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2wrvcccou.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2csaaetky.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2cetnqevj.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2hdljapgr.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2ynlxlxnf.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2kyfupoiw.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jdcvkrsc.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2fevpikgg.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2rxfqdrpp.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2mejjunhx.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2hhnhcbut.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2kmewxbzt.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2edeqgjmr.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2dlestgam.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2luxrzcla.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2eujqlrca.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2rekxesdw.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2trpwilxi.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2txdcmqfr.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2boamoneu.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2zvepmsrr.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2lwrnmezh.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2wdxhweit.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2srjdxvje.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2skjnypjc.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2axgewjzb.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2zlicpcsp.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2peqziprm.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2lempzvdq.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2rflzilsq.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2xmouvpod.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2fcyclbls.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2owybkgru.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2whbcuvgq.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2iradyrqx.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2xuesnden.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2pcmzcnrc.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2aiwdpjqq.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2bixnbsuh.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2fhqbagvm.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2zttzsohh.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2gzgkjpdv.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2ygwqidgh.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2zfsiycpf.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2jrsooicn.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2lobppevh.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2pmyjweuh.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2tqtwludf.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2aignfgmh.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2xdjwpimm.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2sbdiabwu.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qvtyiysi.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2apjwfejv.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2zkmiareh.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2xpwwrcjw.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2zppxtnjo.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xmbbqbhu.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2tuqyfspz.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2ibbbbuho.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2ymeixjjl.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2fdkkkyfr.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2onjnlxyt.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2syykoepe.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2uwufvxjj.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2bfrtcrxh.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2xdpwxtms.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2ghxgkitn.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2drwqdnms.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2dpvyvdud.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2vmeanczl.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2taqaxujp.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2orjokzxs.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2gpdajbzi.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2ecfmhgpt.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2jluzpgjh.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2oeowhmxq.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2ljphstsy.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2hzwtuxdn.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2yprpcndi.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vzxgguto.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2kxcajcet.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2jghbfixr.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2uhuvabcj.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2pdgsgvwy.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2kefdvdcj.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bylgocby.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2adamsoao.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2ibwsieoh.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2xcmvcxow.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2epjrqutt.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2etnipzqd.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2pesfheeh.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2liuoecwz.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2gmhpbtya.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2dhunroyn.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2rmryfooc.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2bsszoppr.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2mfqknfdd.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2vccpgsdd.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2yzylwcue.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2imwvudqt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2apfbfbpa.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2rrcyqetf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zbhhgqrr.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2mtwwheyo.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2bbxkpoqk.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2izryasjy.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2lzmihndv.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2kianodjk.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2lfaimcqt.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2cabmrtiw.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2xbkqpgej.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2ixzfqpdj.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2magexgme.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2khddkrzs.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2vfxraeev.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2eocqassm.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2zvgqcypy.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2ctbodtkr.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2ftprufny.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2uzexcqrm.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2eicaplqr.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2lyjbngob.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2looxxglz.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2dwehsqkx.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2qvldesym.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2dztfayjk.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2yrgytrzn.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2vcpkagrd.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2xkepkdlv.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2iqhmcqmp.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2rdcidvju.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2cjsyiezh.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2lrtvvokf.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2clhybpfj.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2vfotcbbi.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2hlurdpax.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2khjtrzda.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2hbxtqlor.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2kpmicxvm.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2xgroiqla.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2zekajabe.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2yysttwjt.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2psmqdpna.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2hrqhicci.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2slbkgqdv.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2efjnicjn.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2scrrsgqa.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hjagmlup.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2uwssmpvu.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2hylvelan.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2ghebzspq.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2ahhoolzl.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2smpllajg.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2nnfymjnf.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2uxsmxpnl.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2volddftk.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2roglwhwc.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2sanzdukd.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2pdsmwelf.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2piajovpt.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2yutfgzcx.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ynjaatvd.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2lfiwsozu.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2jwxlgrvk.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2ujtstiae.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2lsklwlag.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2ucxhpsiw.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2ewsjimhb.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2vqdqxxsb.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2ftqspmtr.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2kilkgjpb.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2gulxtzxi.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2pyrmdtes.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2bzpqqjnm.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2yevgzooq.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2ozysznle.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2oztakgfa.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2wzgcqjqe.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2gspwtmpv.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2bqwiwazq.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2fasdivhn.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2yasmozmm.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2kuggdfzz.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2ccpsjlkk.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2zmizaymv.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2cyvbmgoz.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2yqzrzqyd.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2hldearwj.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2ejyqifre.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2nzqiefdu.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2zoxydjul.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2fuoqjbqp.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2avyywzgf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kyoztgza.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2boexbzwl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wcxlujxx.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ngqtpush.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2wqrauvog.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2rdeucpft.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2sozlsjpv.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2siusvsmo.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2scwriezc.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2ukeldzlx.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2qbfvafow.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2mvcbbpea.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2cotbdudy.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2lxcnuipp.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2hyfgabzz.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2fnrbsess.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2jmxgjhzw.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ksrozorl.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2spgitdzn.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2ppbflllj.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2gcakqlqm.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2mxprsxxc.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2avhvuiso.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2fqgwkpme.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2ltoiirlh.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2bonzgsxe.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2rsyalndr.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2oqivnuxy.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2dojxmknl.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2inmtjuqv.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2hzragcyn.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2ehvbrccf.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ulsxlfhg.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2upqtnrrn.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2egpwkybh.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2ncbcfxyp.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2dgliwnuh.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2txktesfk.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2fzcheiot.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt2uopbzhlq.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt2cpaharxg.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt2wleduopu.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2ykepbmge.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2iftolkmi.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2fdehhbtl.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2wnqhwlho.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2uuetbqum.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt2pssmemmu.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt2melkaadj.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2ljmlbstl.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt2cjshhxjw.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2yxyvlwrs.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2pmmmarxg.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2gdrkqulc.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt2rojpbgjo.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt2qzsosodu.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2vmjnkuet.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt2sqkblwzf.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt2zvbfapyk.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2izefmvtx.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt2ikenjbqp.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt2fskyklcz.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt2tdacaiqz.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt2iueahjuy.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt2dwmtnkiz.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt2xqduulww.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt2xkojpclo.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt2vazotpln.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2zckreyhq.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2zqszwtsj.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2lictsbzn.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2ewuwgzin.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt2dbunojfd.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt2hkdggntk.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2nwkmqpaj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ukbmocao.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt2vxcdrztf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2stgxuorh.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt2tqidaubr.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt2oodrglrt.html


<!-- 参考信息 -->