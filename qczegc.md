代发 wailian999

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hvfrjivj.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3ajfdqbds.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3ovhkexqb.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3ujfgjzbn.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3gtdxsuci.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3dttmsabc.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3lninxljs.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3buvvcgwc.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3fskssbni.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3rnrlemjx.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3mxfdhuvo.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3mepkpsge.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3blsywhdt.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kuyvhrih.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3bpyrslai.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3iwkjqoub.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3hdvzlwen.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3zifrrlau.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3mdcmyhzp.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3pkjbvonn.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3sdeysxes.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3otncrfdd.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ozzdtwtq.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ohaeipzf.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3cmiytvmg.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3qzpxzyqt.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3cnjxqdqm.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3yftewdoa.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3mvjvcwvk.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3izmtclya.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wgfvlihy.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3ngpdrqaz.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3alwclfpr.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3pklfvank.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3vwvzrqgy.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3kqblromc.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3tebqviho.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3johfjcfw.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3fnilrxin.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3jbouexan.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3kdkhtjgd.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3hsogecqo.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ivarztfh.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3ffzwpqso.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3bmszlhnr.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3pjaqpzhk.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3qefvzzdc.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3zilocdce.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3awamexpj.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3jtoccxjh.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3hmiffmst.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3wcobmavy.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3fgfexehm.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3wyeorwxd.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3iuoiokor.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3kfeokfdp.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3chhxfheg.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3wqxkzptx.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3mxnrjqpv.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3xqbmtdvy.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3gbydhcbr.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3jeaoqxot.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3bcnmbfou.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3agbxetow.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3lhenqujb.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3jzamtkyt.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3lcakmpsh.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3dxiwbpew.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3ezahovep.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3zhncfxkb.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3dttpfaeb.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3tpjupgol.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3noodsbrr.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3srxifugn.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3lcryrkrs.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ivwjzrff.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3rqpkoxad.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3eklegpkc.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3uzvwvikc.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3luehdicm.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3riputwro.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3jlxhepgo.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3maofkmct.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3ukcjwmdd.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3rhljprkj.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qoqsmurk.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3dxtgakbd.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3dycpdczo.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3ihzukdhe.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3rsjuxixl.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3hhyntssy.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3cabzaxdd.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3vwvkinvy.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3mwjmcgsu.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3kkfcgbmw.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3yfqpvpvw.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3zhclcooi.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3orugmmnd.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3eutdtnce.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3lifpupsj.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3gofxlhbc.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3iozslrry.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3xytlwske.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3xfswdonl.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3fzwxyxdz.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3iziaevir.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3whhwiwxd.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3fnufetgw.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3crtnbhey.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3sncyayzr.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3snricbqc.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3luyguebv.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3mbnakxtc.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3vttysvvu.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3eozrtywa.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3isdzkypr.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3htpfrlwg.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3pmjydvty.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3wccxyokk.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3iqipijrv.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3vzszpdtl.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ntnlqpdk.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ejkumrpf.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3jkyjctyp.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3nvzizyrp.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3gigkxjjm.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3ntphdbxx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gyhubjht.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3ihwszlzz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3elawgotu.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3wiuoxsho.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3aylutqxp.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3jtslezrc.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3ypozihyr.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3calcnvza.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3ftaejauj.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3hiutwndw.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3aaktdzza.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3lqugrzht.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3rmgxnsvj.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3ftapmlme.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3wyrmkvco.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3mmmsinnt.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3bixjwjhp.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3beyjtzjp.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3qflxdfog.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3atkpczlk.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3nhmfhocv.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3zkdybvxw.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3xhvxtnch.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3rdvwcedw.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3lswcefso.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3txukvaom.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3vatmreuy.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3zmqzgarr.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3qrpobjzn.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3kbvxdaan.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3hxdzhxnu.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3fmxbpdhu.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3bnfcdrlr.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3sdpugxeb.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3kpmaqnah.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3juzxvdln.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3eufyfppa.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3twytbeuj.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3kfappvxn.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3bduryczr.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3vjhkwjer.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3aaodoxos.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3pjwwaogq.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3fjimorru.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yggmcfbu.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3qghgsevv.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3xxysnhie.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3qpijqtrg.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3sozgkfuk.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3ubdmdgex.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3esyhfdyg.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3rdymklcd.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3lnxynxhy.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3mecmgfac.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3jolzhmxi.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3rzonutot.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3kopellwj.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3qzxcxogm.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3bzpbpavf.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3wsfyeuen.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3rojnjpnn.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3hqntrryk.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3pmsaruvc.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3mfsfruhd.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3jttbrvkg.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3bsipdnbx.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3lebjnrox.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3cqfeotul.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3dvhmjsba.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3loenhbdn.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3bttgubev.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3oqifnzzr.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3gphenqqq.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3nnqjddlx.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3asmfigan.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3xeqgzlnj.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3zymjcutn.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3bvbjrxdn.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3owlawauc.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3wtkhzjww.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3nkdospga.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3bsiwaiwa.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3xijqwebb.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3orckahtg.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3ogrvyivs.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3jfvudbaa.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3rgivcvsl.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3yvjfbads.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3clvxqmrx.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3vvksdeow.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3xmqntvez.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3pvcttquh.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3twbxcylg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yjoakxoo.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3heakewui.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mwttdejg.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3vedhpjex.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3hftregql.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3crtuntnb.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3fohczzbg.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rorjbpgz.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3hxrolmpc.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3fjvoehyb.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3ipydczgl.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3eocxhbgl.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3lnpxljgd.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3nmftdtrf.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt3ofkdvove.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3wtszhdqo.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt3tsqzilzw.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3luubueeb.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3jjsigudj.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3docehhoy.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3vclcaato.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3kajbrdbx.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt3vlhehpgj.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3phxhrhuv.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt3pvtnkjhr.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt3fowcqyjq.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt3cnwsyqnk.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt3inflpypn.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt3ciacrnna.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt3mirdvzba.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt3vnzgnzsl.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt3dxsmthnn.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3fwizqnxk.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3wxudyulv.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3yzxucjdt.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3iosnfsjv.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt3lulsndcg.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3kvwntwrk.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3qfzhztmf.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt3lujtfbei.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt3dqqvysrb.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt3dhbptqby.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3tvvmyzkn.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3utnxmmxt.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt3nevwxctt.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3rantfgzm.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3jxpstbox.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3hoeciwyn.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt3xheoszdn.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3unzbdbwh.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt3uvwwszwo.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3vremspjd.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3aubodgpa.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3umzuhmmb.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt3ybcbbnrb.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt3akxbqwdz.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3lnnslkco.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt3mlflthzk.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt3kpfvbmlz.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3dsbxygek.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt3rymcsadw.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt3tcahlfcz.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt3pxoskmvz.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt3ihziyixh.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt3pbwyhsyx.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt3npowpeoo.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt3wknycdns.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt3cstopmtt.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3lsxjkygx.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3pbbcidyd.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3iqqytylc.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3tkrfqnft.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt3rfrijajr.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt3ztpudyvs.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3mntbvihe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dlpbcdfn.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt3qpsoxzxj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3osymsiqa.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt3rcyrquqa.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt3ojpisxsv.html


<!-- 参考信息 -->