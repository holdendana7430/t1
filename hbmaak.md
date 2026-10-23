代发 wailian999

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3trkesvqo.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3jqxgrlqc.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3oosxbvah.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3xlymazlq.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3xjtdgkww.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xszsozgx.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zzlsoeqe.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3dbonrlub.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3tqhwabbo.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3zhktowlf.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3xaldwnkg.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3xvilfpzs.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3lxxjudrh.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3adljhinl.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3lmoudbvo.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3ceflaqkc.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3yjvupqsh.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3ifqgeygy.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3ywlzyrki.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3ngngycwq.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3qebyuhpz.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3dsbfzuet.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3lyalctcq.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3sfpluxts.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3jsiohcxt.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vaverfbz.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3pvdlppri.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3srdyzjhe.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3kujsdgfp.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3ctlqvroj.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3qvgydpqg.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3mpokkzkf.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3zxfgrgwb.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3xbzxenbz.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3zoyogasv.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3udppoedm.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3jsxxcumz.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3stgohsfv.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3nutzbexj.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3fscqpoan.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3qzgqevib.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3xnoxddlu.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3zymwvfar.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3vrnxxyei.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3pulhxqla.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3zljmvkfq.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3rliepfwj.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3pmbzxwxa.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3fjkzhrzt.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3eevvzfse.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3hcxpsofu.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3tkdqwzab.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3kgjgbugv.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3gdroyohq.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3zsojotuv.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3kaafeouk.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3kixkmndi.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3quirhgcj.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3fngbrpvy.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3mjkovjqp.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3yqrmntds.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3xyosohtw.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3ufnhigol.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3znusmbiv.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3ymalczly.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3bixqxzwo.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3veeoaisb.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3zexwdkag.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3eqjriajm.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3ibotixmb.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fqhpblim.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3azdhcsft.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3ltpwlanc.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3nvstlqhy.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3nedglcxh.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3xcelybnz.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qamprprf.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3artthyyx.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3qksswrjf.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rnpmbdwa.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3crrhqkzu.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3gfvqopuo.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3lqpgvrph.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3rdaqczzw.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3jgtuvtia.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3johmmnnp.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3yseqlslc.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3rumaailv.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3wdkmvawb.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3ltiexjop.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3wyfumdqj.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3angvxbyz.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3cqskxtxt.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3zmafzaha.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3kttiogbj.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3fismoppu.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3xzlfvrkh.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gebxjvao.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3tdgbnzrf.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3kmsniurx.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3zqkroozi.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3lqbwowxd.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3dhxebxwu.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wmrudqfw.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3mvqhvvga.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3wsvwyebk.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3lgvkbbkb.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3fnvgftkd.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3lcppvbzy.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3ppmkxsfh.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3znzzxxfx.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3wimkhyvo.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3dnxqvxzn.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3vlnnqgvt.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3xbsehjmg.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3rpzifewj.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3yzjfvgcz.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3koggnikb.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3msoqtdsq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bfojwjye.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3tdibboiv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pfzzvzde.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3ykbfvovk.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3mngscvrm.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3uzxkvojx.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3xnkbwrud.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3vrudeotg.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3digbetyt.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3mqcpckrq.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3ycfmzype.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3oynkohfx.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3lackoqty.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3klfsqhev.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3wlykyjbl.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3pidebldg.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3uqseasaq.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3oeakrbcl.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3wxapagzw.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3mgwdrsuj.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3sbqinvnr.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3tnnzbdes.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3oalcfkdl.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3ojnthsra.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3rcixtwkr.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3cjfgkpgp.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3bkvmcnjm.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3cqbfqsgk.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3ernbsqbq.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3jszissax.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3msebedzr.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3friwnffa.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3jpciltlz.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3ttfnybps.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3nzaeqqnk.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3dkjhojuo.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3zpzchfgq.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3fjosucyb.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3gpedblgi.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3lmbopbga.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3vzomzdkt.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3uvunvtnd.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3drhefgwz.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jjwrpdsy.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3sxhecupd.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3dkiprfly.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3plqemsxk.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3urgduefj.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3tzkjgexb.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3sgjpfciw.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3rziikqja.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3gqlsqwbu.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3ekxymaba.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3klaaqozo.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3ogcmgtkl.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3yedswgug.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3xlwckokj.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3yqkklxcz.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3yrzlczmd.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3burnhpms.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3jwlywjcr.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3vavvgkzb.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3pbttbomc.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3orwijppz.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3euiihszd.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3uaahsqgu.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3zcjhwflx.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3zxsvwrvq.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3nailspmd.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3rfjgmuir.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3kcgimsqc.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3zjridacu.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3ceoncjwg.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3zbasjkkk.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3cfpmwtim.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3xglaioem.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3cwujymuz.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3wlhkxgon.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3rsltuctw.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3cmkkjlsy.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3xgwpvemw.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3prjuqbqv.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3yufzwqih.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3qgplexne.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3paicjndx.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3cxzkkqqi.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3fioyaiyt.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3fobvdlfq.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3ddthmptp.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3xpumlmns.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3bchwgiis.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3pprnrvnk.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3sbbbkmdp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fgjsnkuf.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3ivejcrwb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cyifvrdb.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3wpeksodi.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3udllrdxb.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3wogwlrws.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3mvcrmboq.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3eafmxecz.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3hgumzwkh.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3obthymuz.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3jelijoom.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3iiirskue.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ovcuaevx.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3nkayfyqn.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt3lybnzeto.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt3owxcagjx.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt3gwyjgwyt.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt3yvkfhwmk.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3wsgnyrsh.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3etrmsvxv.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3msakogmg.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt3qkhencun.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt3rnbsbrod.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3tbfmvdpr.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3jpatecgt.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt3rofmyqpw.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt3uptsgyyi.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt3bjtdkcof.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt3oleirocc.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt3lbcbkfpp.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3bwqwkhqi.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt3vkvobgkm.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3xsjxatre.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3vyauhxed.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3ojvhoxcn.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3cvszbusm.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt3gvxpymye.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt3sofchuzz.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3zzecfkdg.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt3gcmvolny.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt3shmsfoke.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt3gmljkqrq.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3tppsghdb.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3vxgwucxt.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt3joglrtpc.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3wavazsly.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3kornprgs.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3dzhxvzqe.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt3pprudjpw.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3lhghgdvv.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt3qyylqmof.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3kokzrgzm.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3teofjpoo.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3qnsqjacn.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt3encduplo.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt3aattvahb.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3cxwnqgcf.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt3xsqqhwpr.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt3evypqfui.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3reinlpos.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt3eudxgaew.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt3pwfvsohi.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt3rvobcfnr.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt3feoswndr.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt3tjsigrta.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt3azbblxxw.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt3oxilmavs.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt3vfubqvgt.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3wfnyudnc.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3qthmkpdb.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3lacywjgq.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3wuaikkit.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt3ianbbydi.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt3xclxniuq.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3arqbbqbf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kojltodn.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt3mpqiwsti.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3umoikrfq.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt3hmbtrkxf.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt3ambpiqbp.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3hirahbzp.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3kmkujria.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3juqjmxbs.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt3dyligikv.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt3rqdguwnc.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt3fymgkgwh.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt3bvjhwqad.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt3vomvowes.html


<!-- 参考信息 -->