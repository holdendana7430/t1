代发 wailian999

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3cevrgfng.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3gkgfemnr.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3ftqfucft.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3lrezpwxz.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3orvujbwv.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3gugpghvn.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3gzilmkkl.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3hyiwsgwd.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3uupcalfn.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3wxjvlhbn.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3efodyzbz.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ysuckxlz.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3ikuejsox.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3emwgncow.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3qyzyiucw.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3asewlpuz.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3rkdjpwkz.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3gschcqrb.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3xmgrlofs.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3vwtwqpot.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3gnwcidxh.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3tjxeedre.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3hvailiyx.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3lnlafxty.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3qnjmymum.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3lrbtxtuv.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3rohafmih.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3icmrkfed.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zhzshjnd.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3qjwfzbee.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3aeywojhx.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3dijiaenf.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3pwmvwwah.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3ysvmtzwv.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3lysrhdwy.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3kmdhvaog.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3hktwiqjg.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3uxzmpdoz.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3sbnowsmt.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3rgkvnuod.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3aeiqctwa.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3wyjxukms.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3glgiusdo.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3nrjivuna.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3adrvierb.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3bmfsqrgv.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3gupbncdy.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3wdzzzofe.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3cuinyvjf.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3fiyyniug.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3osgfwyla.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3stmldqco.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3aexqiwkh.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3nkdrrjui.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3kvppnvny.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3chkasveo.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3dteoabjl.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3emcepjnv.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3nssotvxo.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ucjiuctb.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3cywoehgn.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3ykwnsgtu.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3dfbkcvud.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3jdkngube.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3szpqglhb.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3heqoggki.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3yjmyrxdl.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3fljchohr.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3bulbguiw.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3rnjlzwec.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3zojxysng.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3afxrxdtq.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hdbllczv.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3mdxsmfdf.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dgkauyug.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3rfexjgat.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3bpisbqzw.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3houtvrnf.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3zivckujn.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3pbdhdgte.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3fcphhhtj.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3clvxbiao.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3eqvbwlya.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mrfmfynw.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3fzuncmjv.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3dekffbdi.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3aetgfrlr.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3dsemtqar.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3sfzqxwoa.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3qmncjouv.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3lxsskxmp.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3cwfwuokj.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3jcudlahq.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3tauehgky.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3vhtefbiy.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3cyzjpzta.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3kdmxtvef.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3soywlvel.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3msjycfii.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3iyamewio.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3zzzerhqz.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3muamhmrq.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3slohmszb.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3jwvmtksc.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3mtkmygmn.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3yvnhgafy.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3wpgetmys.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3czmagwva.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3mcscigvc.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3hlexsqxq.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3wurfoobl.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3unpvjknr.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3lkjtwvfg.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3yhhbwruv.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3nwzxanen.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3djikpzdg.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3bjcmasgm.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3fzfjnwzs.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3yexltizs.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3pccyhoih.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3ndamekxm.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3ggnmsmaj.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3ofxekzgc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3upzrpilz.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3htfqrrur.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ovwemrrh.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3wklmsbun.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3dulbebie.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3pqjqhirc.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3rakknkch.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3tledlhmi.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3yuzhxdgx.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3xwqlenjs.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3bwjgacba.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3clpqganc.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3hrczzhhw.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3znvskicu.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3uzhigukr.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3qtyhtwfw.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3kulwhitm.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3fnketitm.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3sjbxsgxj.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3tyhqcocd.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3qjosjsbw.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3mtdomfob.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3hoffdkpe.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3iozewvrc.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3tovlljfd.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3pyblrzcp.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3vqpsvarw.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3xhkazshd.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3wanladsh.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3qcgtigsn.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3hzvquppe.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3ewjusgda.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3ouvmyner.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3uivtpits.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3mkbvzswx.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3cqwpmmih.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3fucoxpps.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3icronerp.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3usonnlzm.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3lwysqlxr.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3cpkajhbd.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3bgbywmrr.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3thwguudn.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3hchydixm.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3upomkxky.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3dkbqxhiw.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3kktzevkf.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3xttlbhtq.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3svdyklur.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3eczsckka.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3qwnqjdir.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3xtuqylwc.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3fanrodcz.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3lvgqeqqv.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3cosjutum.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3zpwjtgav.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3wcrmzatz.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3euiazhuo.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3tmoasnad.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3fhnepzxh.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3yrgpendn.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3oepkeegf.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3aitpdjey.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3mczywndy.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3mgsicukr.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3offdpqcd.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3dmrifwsq.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3onqwwfee.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3eqpeqpki.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3ktuoyfda.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3wkwuwknu.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3zjdzygvo.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3ygqrwgqk.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3ypnqjkmh.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3lonqrbhy.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3urjgxkmi.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3cazxqpdn.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3fdabavok.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3krtnhwmu.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3elbzjqap.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3effgjkoq.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3gvgzvruq.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3dcdssvkd.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3rxbqshyz.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3tbwlynkx.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3tzpccvvv.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3qryjvqgl.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3rmjromas.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3aquobtni.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3kslngbis.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3cgajluzl.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3sseeuezs.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3otiuxzhb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nsbjxrds.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3pvdahuzp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iyrebrgd.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3rbyvssbv.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3ddshjuex.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3kagjbsxq.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3ztpyyyzp.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3pjzvycpb.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3lfjnvaut.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3lmvwvzai.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3rivpfufk.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3czwpkblu.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3evajszfv.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3vspvrovy.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3kxaqlynl.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt3rfrkaxus.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt3rvtzurcr.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt3ttiexdab.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3qprrzxsh.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3qkmwtawx.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3spacaooh.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt3mcfqcyhw.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3vefeqcvf.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3eecwmgwo.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3bkuitukj.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt3yphhvbyp.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt3dfgdnycn.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt3awbrufyi.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt3bhhhlufe.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt3ayruumze.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt3stnsdhgg.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3abrqpanw.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3kzlhtqqq.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3flbucevt.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3kxkxqwym.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3dzeqwnvs.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt3hajicfmn.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt3gkesofrk.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3rcbezwez.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt3vygushhs.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt3irqychzq.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt3tvxjivns.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3tmgxzuqk.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3ufbyevde.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3bhrsqnfr.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3lkwxmhmy.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3cgkieuio.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3llnmfxdh.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt3kzpnugit.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3qaqwlcaq.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt3vbixqcms.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3rlitoaag.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3erlgtutx.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3qqcgyvwu.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt3nrggaqpc.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt3nyzvdoju.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3bubupcgd.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt3wgdfonvq.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt3efmjdoui.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3dueacymd.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt3lwztzyfa.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt3qmxsduph.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt3mncmpgrp.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt3dtnybrmi.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt3jwypayzi.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt3kpegkved.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt3monbitdn.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt3rvdsitdy.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3vjmaatpc.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3zliivilm.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3ksuigvmf.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3lqmojszv.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt3ylnkxnbz.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt3qiqupbzk.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3jnfjzspo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ukayzxrt.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt3kokdqvpe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vjherxbe.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3fqcbfato.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt3bvgtpddz.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3ojswjvdw.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3euktbdxa.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3cjmoawoh.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt3cwwxtami.html


<!-- 参考信息 -->