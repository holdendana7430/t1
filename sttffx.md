代发 wailian999

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3kmgkzzfi.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3ztewyjof.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3diewrhly.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3aguhxnbj.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3pnqomciu.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3bjxpbwey.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3xeisbmhl.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3vwqdsltu.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3vvvxbchv.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3mwrvsqpd.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3hsfvzbkd.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3nvzplfry.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3jmhqscml.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3evemjfzk.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3pzilpxor.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3bvnozmhk.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3xiijidwv.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3fbwnaehm.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3lxmpawnn.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bkwggpyv.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3rgtgboqi.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xoshfqyp.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3ufkipfty.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3zbunxxyu.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3yqxqmtwc.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3shhpqdmc.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3tvlyqwgf.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3cznkvfwg.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3gqjkzcxs.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3dxtbwkgz.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3sfapnlad.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3bphvejid.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3bdtkhefe.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3esyzosbl.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3vauxezdr.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3aqazfpph.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3dqnrxeax.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3ccpxcvwd.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3uvcuchyu.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3cvipnjey.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3nwjbejvg.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3kuxfcqzb.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3qcimjwrv.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3zcdoaapx.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3nxsqduzs.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3wktwhssx.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3doscpznw.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3yzudbsqy.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3udjolgfd.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3ilkuaxjy.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3eruoxjcp.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3sdyshhuh.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3rmdfwdhj.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3ajcjdgqq.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3qzahjdfo.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3ahjmttqx.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3fgcwdzse.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3gwczddqp.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3xpuyjvvh.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3jfvqjnrv.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3dtdknfwv.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3nvfinamf.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3jmafumxk.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ogzyrxyj.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3cpjhwmms.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3hbcgpnzl.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mtihsqdx.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3merltekm.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3zffmlgxr.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3bpikjnez.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3juuyyvuc.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3lapkjxru.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hunmazrs.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ypxzjeed.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3kgqqzyax.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3imnhrmxm.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3yrxfqvhv.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3gruyvczn.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3amsygzcl.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3egycarqm.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3ylpqkgdt.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3jyazgesk.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3nqoczvhw.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3wtsxwzhc.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3nuowakkd.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3ieqadjwf.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3gotldkmq.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3uoqxobns.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3irpkhpcx.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3ajuoujci.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3rltnnafp.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3gubaveno.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3pzxncroq.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3whaezojq.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3fvyeigae.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3ucmqpmtm.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3idfekcgs.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3susturvg.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3dekgpjuc.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3emsmbnkr.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3wqokdvva.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3bozpknkw.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3wnxkuymn.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3zyddjkjx.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3ykbznhaf.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3pvmudsav.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3xbgpbhsj.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3opheweut.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3aojnsrop.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3gttzvchg.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3hxdfhsaz.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3ictxyald.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3odnafcsx.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3dyrugqtl.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3goprwrjn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gsfvbfyz.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3luopueij.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nfagnorj.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3yoynfxfy.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3yaymeotp.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3yjpobjsa.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3zzkjidun.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3qoqvkymu.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3ldvtlfnx.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3tjpjmktm.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3ltmeigpl.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3uksxgfzx.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3zyexbxfl.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3xqqgfngj.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3qbqxhztc.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3xywuinow.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ktmirpry.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3tixyhqdj.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3ieygdktz.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3ydcotlph.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3cgyvcaxf.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3sgjcuaos.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3xmgkzhpa.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3xpnpbvmp.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3dfjgbuif.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3oycgopry.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3jgjfzvrw.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3iptxspwe.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3fhupgvst.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3mqmruhpc.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3imcibhhe.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3xmonqgsg.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3xxsuybui.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3ozsolkhe.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3zrqlnolp.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3qagxjaye.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3pjjuxjxw.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3efwfxohx.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3aqjkubvx.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3bqoknkpa.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3ffsrlkun.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3dmjbpehk.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3zqmdkpvx.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3gkozgkfm.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3atbgmcmt.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3ubmakhru.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3ygombokg.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3laitdaok.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3jpgvyzjh.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3lyydbmwo.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3kdgybxkf.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3tcmhdxrx.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3qgezzcqe.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3kunlthck.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3wtbevoiw.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3sckywkgl.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3yfoowdoy.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3bjlvzval.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3tvflxpzu.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3eggvnbpm.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3umdfwlju.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3yjanfxvs.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3xjhslgzv.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3adrwzkzc.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3fmwyavnr.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3iakrvggy.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3fizlpxys.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3aocpuciv.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3uxaqscch.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3gbujhjru.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3bvrqrrcp.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3dugwumdd.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3kuxagtew.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3huzcwbso.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3vayxvdgv.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3lqwqodmc.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3rekzrohr.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3ztkxfshk.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3vukmqtut.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3vzapxfti.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3ijlhokyk.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3slbuaheb.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3tgalqcwj.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3lqluxrrw.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3mqiyztpu.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3hdhevcyf.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3egbgxpaf.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3sgpixlok.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3wfkqkwcj.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3mjbppyki.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3stowgzbm.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3nowwqfri.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3tkqnqsen.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qbzvaycy.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3zylytfzt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ahttrihd.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3sdosmjnl.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3zcuyuebc.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3kxytzyvi.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3quqirtlg.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zvonzidj.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3smtsvqty.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3bxhcktjm.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3dqatgzum.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3mtbjbpgt.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt3qmahrsue.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3zecnpoix.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt3qcvhomyr.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3cxipwncm.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3ftqyhpyo.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3yhftrvxm.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3hhjvhgaa.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3byedxmsn.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3yjqxablv.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt3nafdnaxg.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3xyylldbl.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3kirwjgtn.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3owmqhtqn.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt3xsugoqar.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3dwvobraf.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt3gykpprsb.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt3fipfgxqa.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt3nfdtzcgt.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3nyiosyvi.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3hboaejlp.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3lulzhmzq.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3urtkkrck.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3voigjdkp.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3fzgbgpzi.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3czsnxqqz.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3ploeisaj.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3wxvuhnqr.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt3lgcvrhek.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt3laqzzuka.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt3hbbempnr.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3tdpfwepy.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3pftsgnex.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt3shrtstyt.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3uoxwjzyx.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3bgolvqoi.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3mwyckyte.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt3mxybfpxr.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3muiapxdz.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt3mlchjjrz.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3dpziafvx.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3svyqpbmx.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3fkhbrwul.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt3imluiyik.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt3sueyxzdj.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3pfzoskyv.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt3qfxmhaun.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt3ltxeezlf.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3qughezwh.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt3dcucktxa.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt3iqfmtkil.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt3dkjnqbja.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt3oyehmasg.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt3mhuwttim.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt3fvgznqvp.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt3qcjuwdps.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt3idswlhgl.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3sfuhxjah.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3qvdaibti.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3lvrmqwhn.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3powgbdnp.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt3zbvsgmti.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt3oribidxb.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3wroivwql.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fqifsykv.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt3ezbknkau.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wkvkpvtq.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt3pcmzqnjj.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt3nwbxfkwt.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3rjcxfzxl.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3lieezjdy.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3ehpendps.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt3jplixolv.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt3myvobmlu.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt3njilprai.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt3rsvzrvvd.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt3viwgvfvv.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3iwuofcvg.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3cdalnpek.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt3lbzdhywh.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt3qeprrvwc.html


<!-- 参考信息 -->