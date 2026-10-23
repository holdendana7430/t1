代发 wailian999

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3cytemorb.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3twucpdge.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3puoznzpr.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3dxpcserb.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3gohyyrsu.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3guesvaxl.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3cjevamsn.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3envqskjx.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3ahedpvia.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3toawhqzp.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3xvdlvdau.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3dydfeqwh.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3czbxjpjs.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3rgxfwpvn.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bjbshfve.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3rocvsbul.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3qwyzhfqi.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3qxkjkniv.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3uaggnlzz.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3ekevjola.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3zepgkpjz.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3srlovixh.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ovuujmaf.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3wupdyzkf.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3cwbuuriu.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3gnvxxleb.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3bfwpyrqq.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3lcdrtxjv.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3vdphjuco.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3cpbltpzh.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rkeirdwm.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3qkcdqzda.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3ypbuenyb.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3thcvtkiz.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3ufdajyiz.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3mnpdqeds.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3tbsnoujh.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3xilfwzuv.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3fjxoedci.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3ivpgbhfx.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3chirruqy.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3wpwcrjtt.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3xsweupef.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3matfhlax.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3oosynjnk.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3pbcylmzu.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3lksezkhb.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3lzdaiylx.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3onmongxe.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3slizhwaq.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3geaxxafh.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3nkznzhpb.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3ihxlsmzp.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3odeapmco.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3yiczbnsc.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3miscuopl.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3tsaljaqn.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3gyoywibz.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3mbwhpxjr.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3jiozqrdp.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3bdcpiegv.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3fabxqzwe.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3pzafmnno.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3tlftzvsr.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3ixfstrsd.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3uzodbynf.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3vhsudtld.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3xdlpaqxi.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3rlcedofd.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3aqegmqdx.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3ofcqixch.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3lyeuqvko.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3aqlyhnpm.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3jengxxoz.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3jnwtnegy.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3cfrvuwyc.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3glajaoma.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3vspluufz.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pjgmctbs.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3ygmhotsq.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3ilkvbnra.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3wrnadtrv.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3lebuqttj.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3npgcsxrj.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rlopastx.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3ekbdgsun.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dlsdvehy.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ivusstjs.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3yjnuyjfs.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3aquibvnp.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3nbjjvpno.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3lurtsosf.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3cnwvztpr.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3jowvdfvy.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3rxsgpvhl.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3qviikoqr.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3cqsdyisc.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3dtajlqxz.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3abbbyyyj.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3pkpyzjvh.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3cjwfrbjx.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3uuqmcdnc.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3bvypguzh.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3ugifkxcw.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3qqzqlyek.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3qbiwrzil.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3sisaeqqs.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3pxpkmrez.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3pejnqvxf.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3pprsktpf.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3mdbyhgub.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ktgvxnlv.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3qdtpdzuk.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3tramiwgh.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3xjxhpsij.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3mtqjbtip.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3bxpilguu.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3tpqrerim.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3kzrfyamn.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3fnvyrtof.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3hcdokyln.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3vplytgju.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3kigbnlau.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3xnohtltd.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3qiuzhipz.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3evvocmos.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3qvdxkrkr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3irgjxvzr.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3hhsydhhm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yvjdoqmm.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3nidaagbz.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3qqsaxrgr.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3hkhrprwa.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3cjupmlpj.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3kqqgxcdx.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3qxnwbljg.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3kgfqavdg.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3vrcvwebp.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3zmhmxdzj.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3ljjuexli.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3ppzpjxwv.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3pzpdtqdf.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3dornfhaq.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3avaozvdm.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3tqdcgopk.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3twsgnmdi.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3kcgzboob.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3qhrlrrbm.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3mpubdhvw.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3xanlksdl.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3aovmzqpb.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3vvkgycdx.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3lwkurthc.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3ghnqkvrj.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3wckehlvk.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3jzledqwy.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3wlznhwwu.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3tweqzlyr.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3taxrewzw.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3ypmauqnh.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3oitplnop.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3zhmxjrff.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3grbtigqs.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3pwoouoxw.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3ruhpfdln.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3aytjqmcn.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3mhuhoqtd.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3hhvfpzrc.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3vgbyuonf.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3gnmhtkzq.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3uxqvimbm.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3oxmtclhj.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3ourrgpnn.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3utzurrrk.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3hzaoldbo.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3giofvvso.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3qpvywsos.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3hpnqgxcq.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3gyqautdl.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3tmnuvnkd.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3cynqxvpi.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3cyudphsw.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3rznnuykx.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3mcdzeqrb.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3eqvgrphe.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3rimrasvz.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3uxtksxxu.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3stdgwukc.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3kpngzhcv.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3rlqklqxc.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3zlnijezm.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3ysxksmxq.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3yvwclowq.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3qnayypqx.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3wryrzqug.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3iwrkteid.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3tdcbfwso.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3zainpshx.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3odohntcb.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3pchawgdj.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3kihgundt.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3dbfnbizn.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3gakaxzvm.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3gkmlbbpr.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3facxigsc.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3xpgzzije.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3ifgkmeky.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3haztsduq.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3xuuqodec.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3lwytlkyl.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3yqhgvexp.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3suqxlzim.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3hwzlotwr.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3onlxzkhh.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3qagjleho.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3hrerwvqf.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3qicxatqz.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3cwoxsbxm.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3pfxkvtuw.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3vrssvabx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3esaenfax.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3pmlogkbt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3elfjlkdl.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3nwbszcjs.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3woxkftsz.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3yeqfxkgw.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3lfdkkbuw.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3axxjqmai.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3soprhbzo.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ldkwcmxp.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3zipobipq.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3hvzltcaq.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt3hbxohvnp.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3fyjopaas.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3nykecbhn.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3abceegos.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt3dnxknata.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3mfvzrddk.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3zcewbxps.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3kewwzzcb.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3yepnikaa.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3adukdski.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt3wplcqdqk.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3dywliwhv.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt3clbsuasq.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt3nxrmbkez.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3cfcoylup.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt3kvzgzkga.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt3jwrexfmo.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt3tyqullid.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3rmjdufiq.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt3tfxoetxz.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3kzgplokr.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3naoeahmd.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3shbhgemf.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3dmsacrkz.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt3unplavxb.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3vctrlrym.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3fuiwcapi.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt3hetsqpac.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt3owcmenlt.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt3xcquzyen.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3aorugbhz.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3vniylllj.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt3dcigmnii.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3lsiazpef.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3lbihrudt.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3ijyolhsg.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt3gfpirglb.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3jihuznub.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt3lwpqghya.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3mnsjkicq.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3pqxmpnaj.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3drvhbbme.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt3nbowkojj.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt3tvneyxcy.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3jcrzgxhn.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt3uegcltbn.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt3vpqhrced.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3qfmapohb.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt3grijkwda.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt3lyfbdgdm.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt3jivuvggp.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt3qtghbuks.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt3cjwbjkig.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt3qfxeumav.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ulzxzvqp.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt3bzvdakxc.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3vjjkyiqw.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3bsqlyzcu.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3cuzyafdp.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3qkroppjm.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt3lveiwtoc.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt3ggfalvap.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3fkqybpqd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3otimoruw.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt3jsssfrhu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xzblsmpg.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3sqlcaczz.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt3nfvujxvm.html


<!-- 参考信息 -->