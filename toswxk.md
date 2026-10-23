代发 wailian999

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3gymclciz.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3oxwloyqd.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3dqunyvvd.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3xgintdlp.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3fstloora.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3vdgptcux.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3vnrjwmpb.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3vjmmfagk.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3brthwxkm.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xdmwwtvp.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rfpmzrqi.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ivchhabj.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3tvmahdpm.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3iufrfkbg.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3kayepxah.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3lskauncf.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3gvapepbf.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3rhiapyyh.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3xnovnhvh.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3gprodosx.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3cuxcofnk.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3jeoihyez.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3kdpvmhzp.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3uzxodlux.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3zcnncocm.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3adoxgywl.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3ljfdzhsg.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xqntlgzh.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3cclpokxh.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3wzzthelf.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3xtsqwlzf.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3sjndchtl.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3bzpsdggs.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3axolfsgn.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3ghwxqrkw.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3lkvzrsea.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3dyktiboy.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3whmipiax.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3fcbtwwyd.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3zezddifm.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3ofhenaxk.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3ibjunbbj.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3mseqzilb.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3boipqcyd.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3kzeakwap.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3imgvcjgu.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3vivqoual.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3jnrxhdil.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3keqriyyo.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3vpnalwle.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3heewbvth.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3fsjfumuw.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3cgzfpzus.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3yfegmovp.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3wbpccuxt.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3afpfzayz.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3qqyafksz.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3wpkmufew.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3vpzmjadg.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3jcsjyksx.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3rexsufah.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3nonsfomp.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3uzhsmlwt.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3ieoebkhj.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3mdizfsqk.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3kzvywwdl.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3uinizjvj.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3zhmwfamq.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3kldlfllj.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3jtdpsyft.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3oqasfoiw.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3utlrohel.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3frcthqac.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hkdomlpj.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3welboiqm.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3arupcwai.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3oowvgckb.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3lgjpalim.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3zewsoxry.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3bplrawgy.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3utblprqn.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3wccdhkcs.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3btkmksqo.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zgioxhxy.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3yzkncekw.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3glahkjhg.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3oqeruoxr.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3vqtwatyv.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3juhdbrai.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3pnmiktev.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3jrzbvggc.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3heeaolqj.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3pnwfmcqu.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3dusswtlc.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3fyxhfjug.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3jkdpqrjl.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3cadjbauv.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3tanbhyfy.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3uucrxnnc.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3haooxlwb.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3rkrvxkan.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3zjgsmjne.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3flkxkjue.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3zvrkdzbt.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3ovgomthc.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3tysgxock.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3pbacifsu.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3znhihtep.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3pyukqpit.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3dbkwkpkk.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3gwcdylnx.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3wgbxnedl.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3hzhzwouy.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3zylvijcc.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3rjeflqvy.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3eqswgxjj.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3imebscwr.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3bskdripj.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3xmmlsjqg.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3jvxjehiu.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3bgalsgad.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3ubppnwdi.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3egjyhckc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hqeeeukr.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3fvksmzbw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ydwjgici.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3jvlohfte.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3eodoyxrf.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3voqlzphd.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3lrafpglw.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3vspgwlfl.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3jaytxrsh.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3rrjuljuq.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3qxdlenbj.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3cxedyhnx.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3yikjnqco.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3qewxwmwf.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3hdmriysp.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3ndtwywaf.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3lqmvsuhl.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3vhimytqt.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3eeukuvsj.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3aowvvszd.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3hieqlblo.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3qkcxtjvf.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3wcbzyzxh.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3nxffqcws.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3xekxryxs.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3shbrzbgy.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3jafvlnjb.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3jgvtmljn.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3zzaoiaeo.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3bcrvkzub.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3lzhpbthm.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3slkgrdok.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3xjuvhjnx.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3snphwlrv.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3jqwemuny.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3jlmgopqw.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3wwfvhrav.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3twggifxa.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3jaztvalk.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3xldgyazo.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3hsoalpyk.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3hfpqdmgj.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3hvcywcjh.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ghfpiuvd.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3aayfshkt.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3vmipmwyv.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3qfhiygtg.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3llrfsoia.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3umfjntyx.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3uqckfoap.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3jumdpasm.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3amkfbcxn.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3zvvfxdym.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3pnjercsu.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3gvnpqtze.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3gghxjanm.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3xmlbixis.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3nbwrzpoe.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3wkjvemoc.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3lwpbqhrn.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3migckzne.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3dlpvupyc.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3rvdevhqu.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3leqbneub.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3uzbtgplu.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3hmhbfazb.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3gibegarw.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3caxdxtku.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3qmciofzo.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3koebmlsl.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3evbueymk.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3mgxhttzg.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3vwuoqtry.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3wuosksef.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3abqnphaz.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3ecfgdoeg.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3niiizcsw.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3aewkzkjh.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3lyoztrxp.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3gimjjpft.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3tdlfzbnu.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3nsesyyej.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3suuwnnov.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3vtgewjhl.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3pypekqdn.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3fzdqzhqj.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3isjixtti.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3vcipmgnl.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3cassatzi.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3zjprrhmh.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3fsirqton.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3mpzviyoy.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3pfajzlqc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ozlgtdbo.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3pnicktaw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cdfhinqr.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3rkmzwrfr.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3wkzjolfo.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3ddcylrbi.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rgrffixn.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3gijnnvas.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3xbeaxifz.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xyqkyrnh.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3ipewaplj.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3ztovtfyi.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt3qzhbpaav.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3hkqyilgw.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt3njymulcv.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3mmnolgtx.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3riqsalki.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt3cezjqiko.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3mkbdusvo.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3pxcosvkx.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3apkiqlkb.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3wyhjhaez.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt3qadtylpz.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3tmuotymp.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3uudvctia.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt3qntmlhsn.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3jxzuzfag.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt3yaumgovq.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt3rtuqsbrk.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt3rgcuwjnc.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3bpwejdhx.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3qynsudyp.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3esyweiea.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3ujliobmx.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3pmoxgdbx.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3kdrqwblv.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt3ircahtsn.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt3ireqzygx.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3ghvywmdw.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt3fcfdllma.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt3auzeyira.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3gfaoyzrl.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3hcussdtz.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3kotgpzfd.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3ciuqxtpw.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3ejctunaq.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3wwaeqqic.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt3dlkyuwre.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt3swulouyv.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3jlktfzzx.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt3enqdqgyc.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3vfeykvlq.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3stbmnaiy.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3oqcryhav.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt3ruwzktxj.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt3tqsqgkux.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3emoalwrq.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt3gghqerpt.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt3qglsjnqf.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3lboqhunw.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt3lknuwqxk.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt3lquqkqlz.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt3ofywhrsg.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt3mjfoewqd.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt3xbutptuo.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt3trhmhtot.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ttzxkygr.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt3yazfyaxr.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3ujfwiuqw.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3jpxbphuk.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3vwbygwih.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3uobyluho.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt3llupsfqp.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt3swoagrlo.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3pxisgyyc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ymhusria.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt3rmbsvcef.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ieibwdfh.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3fxszucid.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt3yldvxxab.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3powxpdev.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3qniepnvc.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3bavkskfy.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt3pixbhgci.html


<!-- 参考信息 -->