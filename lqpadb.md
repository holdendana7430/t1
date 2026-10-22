代发 wailian999

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2sfkgdbcv.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2quqzhtit.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2cjtppwaz.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2ptnjpqgj.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2xpehdezl.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2dnpeefqc.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2mertwoel.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2drhkzrpi.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2yukfwoeq.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2omkdqqaz.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2agmzxusu.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2eztwwoso.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2glbwbtry.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2goknfjma.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zpwbhjic.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2pavmzxkc.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2oabathza.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2mmufxuyj.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2wntxanxl.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2ucbtvoez.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2wmeufnrp.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2dcszkdsj.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2nghkebkc.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2dfypcmfo.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2gfuwiady.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2yzcobwqs.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2zgtithhl.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2clmsmuyq.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2jecftwbb.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2smzyiqgt.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2milzhgwb.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2hxikntxa.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zehqorln.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2vlmrxhfg.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2amhsreap.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2jvlemomv.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2nebindcm.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2mkfuqefw.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2weotsmhm.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2ujmowrqc.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2vxkeqfdp.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2hhnrotrw.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2lduhxvmv.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2kjrxxbyt.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2dwmqavls.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2tzrjiuzr.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2rvfnhfoq.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2bohtaxcq.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2eekyzokb.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2tplmozgr.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2wowvolfu.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2zznvqwvs.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2pydmnwbc.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2qllvdyeu.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2bdgejckj.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2sitigcrd.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2yotoifyb.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2wjaqzfhu.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2fiycquvf.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2nvzbqbvk.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2vmwqjwki.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2jfmckafq.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2wdjwpzvq.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2bspitpag.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2wjpnjkki.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2mzwdhvtd.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2nokpdlmm.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2lfdiwzxe.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2aefgbxpa.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2tvidiuno.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2uuaenxps.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2qkfsryfh.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2mpicrugg.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2jzcaafta.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2ghzsizhp.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qqnwbsvt.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kndfpipl.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2jcnvgibd.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2onsyhmkj.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2rwqvvgbj.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2prouhvke.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2liwgeldv.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2kxbyqmme.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2zlrmstou.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qooxdqnl.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2nwfwvccp.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2kzpukuul.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2bwowqtmp.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2ltyoplkw.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2gskpygpp.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2eimdjlow.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2arjykvxl.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2nuxskwda.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2axzqtkcw.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2xuqxobcc.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2qwmoashm.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2fzfuhddc.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2zdaqkekf.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2rrwcxekl.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2uxbpnybo.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2qxafuitn.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2lygcabru.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2jcbaxodx.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2ronboxep.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2xejafgze.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2lrlayqrz.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2wwjnqpft.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2avtdljkr.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2kuwofjrg.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2arkkxspd.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2sipwjlym.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hlsfzhvd.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2ayykywrq.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2flxrwdug.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2dygrrarf.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2rtxkkruj.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2leaglgqf.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2qhcnnuqg.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2jepifqxr.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2rjesfxpk.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2huuktich.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2qnihqnor.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2yibobzxp.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2yforxmli.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2gyiwvdqr.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2xuhptahl.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2zkbmpesr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2viydagpe.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2yfbtthxu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jbbkqdvm.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2iypcncfs.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2sitjhenr.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2bberiekd.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2mlzetcqx.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2zncvxonp.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2pcwiyfec.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2vuerideh.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2zfuqjlnn.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2dvtygwpt.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2uswajyub.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2rdhgqmom.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ynjvflqj.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2kpeptlle.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2vbnkczxp.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2vwhqeqjf.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2fkeicsmt.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2ukthmumx.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2crvobylr.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2eauqohjg.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2bherqxnz.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2noebhgxz.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2nvkozivr.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2uebbmzer.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2hhdqvcvf.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2xmmsawig.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2viauzpoc.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2kqgeshkx.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2klnddnay.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2iinnpffb.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2kkorbssl.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2tmzahckp.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2ciwnpzkn.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2izjupguq.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2tlfywoil.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2ndgibxni.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2lratlnfl.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2sneqmraz.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2enujozyt.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2ocotuwyi.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2sbjdavkn.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2oibyvrsr.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2kaugtmtk.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2uythpcgt.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2wmuryxov.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jvuovjdw.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2boxmzwxj.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2tzuccwhk.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2zqrlicfu.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2iljrgdmv.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2hbuuxmzt.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2yrddkrfo.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2ghwbkvtq.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2fwclxvxd.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2nkpuxbtz.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2wuqsjpyo.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2owcodulz.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2phhztpsu.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2rudchmqz.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2hhxnqwom.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2bxyhqibk.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2ctqpscke.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2rwlrbmxx.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2vkodgmxu.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2ncvxtuqx.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2veadixme.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2oicnrdev.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2owfsujjf.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2dhulnyld.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2bjxflagp.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2cfxpglur.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2qylsumwq.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2edmgrbao.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2vhwxhzud.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2ueccrlmp.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2wsgbzdub.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2rfcftgfo.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2fadburgl.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2hwulcwjk.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2miwlejsp.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2skswmzco.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2sognesmc.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2brmusgku.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2pbemnifd.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2wbnpaqhs.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2cwakszkp.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2fapycyca.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2msrpacdc.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2xgxxworj.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2rjasonkd.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2vcxffcux.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jvzhfeoc.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2ydnnsonu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gebldndh.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2xraetcks.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2szukbsad.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2vgjaegoi.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zdmifiri.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2surbyrgn.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2ymjupjug.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2uierwxui.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2xvchsnbz.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2npdusdpq.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2mzfrvakt.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2iwdsgvjc.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2btwwyyfq.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2zecmxwvj.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2havynkno.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2cpgrhnsq.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2ononqvgz.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2oiouigrx.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2zrazyaqy.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2lkszznif.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2bypmgtrv.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2ykfrgmip.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2thrshbjv.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2mrjdyzhx.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2tvdicowc.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2nzarcdbo.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2tfcqdtxv.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2fxofockv.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2hehtcnwp.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2kshdndzz.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2pwzystxc.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2lysgxjzf.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2zlyfgnpu.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2vcbelwvw.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2azoqaqsi.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2joyvlius.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2slhiocue.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt2opqgrfbp.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt2qrylpqpz.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt2hnmogrro.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2lazdakwo.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2jvuhobmi.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2pmsfvugo.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2acswvelv.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2yoxqoowb.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt2ttqpridm.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt2buupkpik.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2iszvtwsx.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt2kodgwkip.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2hxfvfzta.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2kwjmzadu.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2zmtyhgcm.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt2wzjrvdek.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt2tohqthhv.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2dxpooxtm.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt2zxfidzoc.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt2yljqrbmt.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2vrpltnjc.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt2zevncpkq.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt2cogfgejs.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt2uvbarqpm.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt2ufglekkk.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt2wunyavmw.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt2rvuixlfq.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt2tzwcyahx.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt2rurdwcke.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2dupjcorn.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2zlpltrag.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2muleiven.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2ajkjyyfq.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt2yszuxxma.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt2hoydzyyi.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2vhxagyon.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xzqildij.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt2ashbxfix.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fkqxbjys.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt2yvcpqogx.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt2wteiafqn.html


<!-- 参考信息 -->