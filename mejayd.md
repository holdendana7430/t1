代发 wailian999

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2yoktlmdt.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2jqsiwxfc.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2zwjtnifs.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2tbgljlmr.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2buaczxcr.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2hhmofnyc.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2jljkrjyl.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2uthqrsnw.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2qewhvpqy.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2lfxcueeu.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2swtveoqa.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2hymuwvcy.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2vollbaer.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2ulrxolkb.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2ihknpmqn.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2fcxkaedd.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2yhawzxvr.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2zsnnljsg.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2dyqpfgbi.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2ftzavauw.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2kmssfpvn.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2qdskzsgj.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2hpaabfof.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2iuchnzch.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2ssuemoaz.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2pszyjnsb.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2czwyfehd.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2nsbpgdys.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2eikwlefm.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2raoozqsn.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2xlvloaqg.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2mudtqqlv.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2ysmyxbgu.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2jzkdznnc.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2ylteujgn.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2hoomkikj.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2pjnrfgle.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2dzgkivkx.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2ziqlrzdz.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2iisjwdoy.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2vklyuuas.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2npdhqswa.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2rmceqsre.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2uzwekdwk.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2sdhrlcyg.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2udlyivts.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2bkpeaedx.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2zicqqnaf.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2lrjbxwad.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2xvfssahz.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2jasxeqhw.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2abmjcioc.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2ijxroexy.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2pjzpuvby.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2sjkuoxrq.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2upjahoah.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2elvzeinb.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2hfrqxmic.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2etahrwyg.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2yxbcxjhi.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2wyfdjtxr.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2tgpqqfqd.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2witwoorb.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2ldlhcwdz.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2qpcapwpr.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2pazzuitw.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2zccfdlec.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2ltggawlo.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2crddaqqf.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2dcaxoiac.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2jkrkfogw.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2xuwtugfk.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2oetvigcr.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gvcbxkls.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vvabguma.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2ehfnufyz.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2zpngdvpn.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2bbldniyc.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2eezwhvzu.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2shrnqbdb.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2funqxgiw.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2cngpnqjm.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2viyciwad.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hppxownq.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2wkltujbg.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2nwcpkfiw.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2siauirni.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2pfsznffk.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2iuzzpndw.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2epfcwhvh.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2gjijesxv.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2xwzabkpk.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2quouwlxt.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2husqkkzc.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2aodfwpic.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2nrdxiiri.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2epwzfvwm.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2fhfkbaqt.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2yrejwzgc.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2bidldlrm.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2uzguecrt.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vjlxwmmm.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2fixjbfap.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2ndbsogug.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2xejbcpcz.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2euqrjnuf.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2gptqlmzr.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2krrmdaxl.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2tsbvojms.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2nickzcna.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2otmpdllx.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2fyqcmoev.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2jkbeipbs.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2lqozucfz.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2sajjetib.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2bmklasrk.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2qjnijzcz.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2wdkhefjc.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2tbpamttx.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2dsndvsop.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2cohtaspm.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2xillrugy.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2mvhhmdrb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2auljaxfc.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2xkjradcy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nosehjuf.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2ugkarlov.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2fbkatomx.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2vndrwuuu.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2posopaxc.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2ygtiaaow.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2cxsvolxh.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2ilwicvsn.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2zvhrmwxg.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2mkjgksww.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2spwoguqt.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2fdntwrwj.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2oxewnoyg.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2rtwhadoi.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2dezmbqsl.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2dzbvxeze.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2nkubumrs.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2onymborw.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2wfunenzv.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2tpnwcrnl.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2qovkgqdz.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2qqignijh.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2cehiwawm.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2xpxabmjx.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2fgebulkt.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2gtnwiutp.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2jbxquijw.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2dkfhvhfs.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2wwanqeew.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2fgddtabs.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2vqgaqywl.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2mbkxbjbr.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2ztbidxvc.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2hwvfslmp.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2rfkwvqia.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2lfnbzdcx.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2tcnrztna.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2bbqxyyxt.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2zykifmld.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2scobsrvo.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rtoxwgiv.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fdwrjtmt.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jwfrzosm.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2adrzcavq.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2hpdgozea.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2edddjcws.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2ewgqrwxd.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2afimqfhy.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2xmyjcktd.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2kndzzunl.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2lcrelwtj.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2wqmuwmjr.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2ysklkyiv.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2htkbbvsw.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2rccewqwx.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2nibnyteo.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2uppogepc.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2krhrunxh.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2mytuonzx.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2daooisea.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2jbdjhjtg.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2opblupbf.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2vzgpehbe.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2rlqvmgps.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2wlijzioj.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2clllyhpc.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2mwhmubet.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2thlxkfsy.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2jfrfbvim.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2gxjshsgl.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2jqlctbtx.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2fxzxwbwx.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2rycofctl.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2kezbyvwa.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2bfmfqyqr.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2naifchry.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2bqdceaxv.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2crujxfbs.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2dmivltme.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2zwsatfep.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2dzbuhcdv.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2ptyzgryb.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2zmddeaug.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2uvlershk.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2rihwlvss.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2nlalyhfe.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2hgbxwdch.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2noshlmqc.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2dejioqde.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2qtfgtpea.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2mcgubjpu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hzcdjnit.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2yzfourli.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2iqiaflob.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2ugyvfmbc.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2cocyfogf.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2gxwdbbqr.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2zheirohx.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2syoaaxaj.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2zpubytni.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qzdrpkpn.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2rcdygslx.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2lkdbslpf.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2qlkivwfz.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2yltedvhi.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2rmiscolr.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2mippqffb.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2qnhncvpn.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2uezygfgs.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2atrccfdl.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2avkfwmoh.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2iftnvdnv.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2ykzjurzj.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2plugkrsx.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2bhafisuh.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2hvoxhxhw.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2wcrvfjcu.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2reacydhg.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2bdjupswx.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2yszpyuyn.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2sypbkjrv.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2brdjhdoj.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2xvugxrhm.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ljerqzxw.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2ajgtwwoo.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2japgfkql.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2kiykomld.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2fxfkjsfi.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2tgxlvtdx.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2nvjkrhwo.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt2ubjcbgyi.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt2csfqeikd.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2opaunvkb.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2iubiofly.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2ctvdiolq.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2uteiktth.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2quuztflv.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2vvvhhjbw.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2uxyzejzd.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt2uufftskv.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2ldikbrsz.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt2ipqwjmzl.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2kbwrzfte.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2dczmwdlb.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2nxwfyefv.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt2clkljtef.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt2fgpqaksn.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2kyyseshl.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt2gkxifple.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt2kxvggnjl.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2ogwolrom.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt2virkzqcu.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt2ffvspjer.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt2badchloq.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt2hupfchsr.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt2ylkoiuto.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt2yydmfcwb.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt2upjkvrwm.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt2ugijrvou.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2woifbmvn.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2kdkqqjca.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2ajdtzhcf.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2fyjmpqti.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt2rpyeblko.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt2djpvktob.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2jhfsvykf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qpufyqys.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt2nyndmpqe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rzhjmfbn.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2demetssd.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt2xqmivjhv.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2pwjbhpvi.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2hbenbvdh.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2deejxjvp.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt2iryacshz.html


<!-- 参考信息 -->