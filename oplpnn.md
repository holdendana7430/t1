代发 wailian999

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3khxmgzta.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3mpgdlmya.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3kxtptdpt.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3jkbfxvzj.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3odwlxbit.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pulgezhg.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xmraheyi.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3rswbhsku.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3udywbhhe.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3bmxhiocd.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3inmjpcgs.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3agnchyng.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3xuixomvm.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3myzzdogv.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3hhlqwqpp.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3trnuwmqv.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3zzvcejqc.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3pwbwdfsf.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3jmiruisa.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3cnzrxlom.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3btnkbzwi.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3enloqhlk.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zhboazed.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ogczybrn.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3penoipqj.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3eweethzy.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3ozmwiyss.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3kqhceaco.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3jivrclbl.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3ztjbgiib.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3snnhgivi.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3yegtvukp.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3oywtfuim.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3blopzgrz.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3qjnhbtom.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3hedrznlz.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3kxbxsuyu.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3hgsbmepr.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3fupbalvw.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3ksbezydj.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3mrzhetud.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3ztpgyuzg.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3kxfrihmn.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3iglnumoe.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3joiejbqo.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3oxlhsebd.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3maalicjf.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3dhsjlghj.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3oghggdbl.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3fzabfbjv.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3bsbjobjt.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3tqmgeapi.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3uozjnzmm.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3nmxrezjz.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3kvkaalxk.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3hrrnvvnd.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3yypabrhn.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3odizokpb.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3adbghnps.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3lluihmie.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3oxvpppdi.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3tvckiguw.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3pbctjkvo.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3tblrhbim.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3aaauyknx.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3dqlicgvu.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3hrczrtox.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3nenlvpwj.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3ypkjcyhp.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3vmojkaqk.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3hrcjdexb.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3vmgigslp.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3vlbipsxy.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3rctnztfb.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3alhwdzna.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3meqyygww.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3syoeiyus.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xsqajhws.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pxveynjd.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3idtcalyo.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3knxezckg.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3zxhwahzz.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3avbcplwk.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3gfsjhhcs.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3mdqutjia.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3vwgmvmci.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3zyjlqqgi.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3xrhclokp.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3mulfutik.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3qcnohojc.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3dcsthsnk.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3lwxynoci.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3jajjuezt.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3hqrlqpct.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3kvwviuya.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3pwatmayr.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3wdzlbrsx.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3iabohowm.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3vtxxmdyj.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3kjcpzvif.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3jaaudgif.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3zvemivkt.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3hhiucjum.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ipwftphi.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3ezdjguyo.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3bbgaztvw.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3ugaouiwt.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3jxhyqdrh.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3qzbpfuzp.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3lvmquiwa.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3vyuwhphz.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3doscgzlg.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3yyyxpjdu.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3qeuaiajl.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3reqdkaqe.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3lppbequl.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3yrjenepm.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3syqhhrbu.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3hrpweawk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jvchcwhi.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3pvkzzurd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hgpcwwtc.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3jfpbkvue.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3cgdmtbha.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3lutnxojs.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3nfdsaarm.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3ykbwwzrz.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3neyytrxo.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3higaazww.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3dqrvkewk.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3kjjvwwxu.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3vpmxjtrr.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3kppqgkji.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3vdfuanbi.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3doarmybk.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3meopkgtd.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3nhdpjrjw.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3xrfgecgm.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3oybgqkxb.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3spaejqhj.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3exbotyvp.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3mdkpqwhs.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3kfbhazfl.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3tgtbqien.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3aaefujzu.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3jnovxftd.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3ngaglyxd.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3huoehwre.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3nbyyifuw.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3kgxarkym.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3vheiuyzu.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3qbxafdgk.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3tatqtcqh.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3cusbaquc.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3qmbclnmw.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3hsjzrvbm.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3jtuwscyu.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3pbbhezzm.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3zjvlfxfe.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3teujrhez.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3claaugxc.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fiqypzho.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3gsomhrfj.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3besoqdpw.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3knwmtudj.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3msbdatvh.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hmmewfae.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3hqjukyhh.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3kdkbgmex.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3brbrznpy.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3gwddymin.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3mjbskkhq.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3adwauczt.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3jgexswvb.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3dvrsvzmf.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3wkgfegxq.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3dttygmop.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3xokmesvp.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3hflxoedm.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3yoxhskdx.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3kagdhybj.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3hraynval.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3yopqpfvl.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3esbushpz.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3nlohcqhp.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3fofaesnh.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3uwmunohb.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3crthlajc.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3xxipmzac.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3hkregjzi.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3gmtzgggj.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3uryvmgyx.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3oqpukhhy.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3fxhtqvoq.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3jrbbrsva.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3sgukscxj.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3vjjkinww.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3hkaxpzeb.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3zbnpmfnt.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3qzonggey.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3mvbegxcz.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3wpuyiras.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3pelxhvsa.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3zaatexdl.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3uplpncwd.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3uvkzhfvc.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3enmmqfut.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3oiusnzkn.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3slnzicxy.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3yiohnzkt.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3vqbymxfr.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3idfsdjkh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3svssmxre.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3qtllqhbw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3guvwzunb.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3hnzvvsar.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3logfqapt.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3ixcjxcwt.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zslqgmqu.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ykqrlptw.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3iireunpb.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3gqlnlmmz.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3iklnlmsp.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3phcaoxdb.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt3mtrdcsgr.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3sxwbmqnt.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3grwicobf.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3tejiteyl.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt3uromoyzs.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt3zahefhym.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3nuqsfuza.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3oucirkhe.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3usvjqroz.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt3tmsuutlp.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt3jvaevcdh.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3orefsfyk.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3jsaqheba.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt3ybkjkcyp.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt3rftzsyhy.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt3ephtlnvy.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt3valkqwwh.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt3wgihflyo.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt3zdlyjdti.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3hcziudto.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3iudlkqxb.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3iptkurqo.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3ucvuukcb.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3iclwmsnh.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt3qtetchuc.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt3mktvcqru.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3mocewlkj.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt3fhxlsflb.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt3tsthxeiy.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3sgnhjjut.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3fdmyakrc.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3itbgfdxu.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3bpuyzkgu.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3kzmygjpj.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3xjkgizph.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt3ntbkhmiy.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt3igkuvrzl.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3rqmexrul.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt3mnxvfuqj.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3hogqlfqk.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3sgpwgouu.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3xemhkkns.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt3ummqphqx.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt3vnlybihb.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3hsrsubcz.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt3emahcoht.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt3qcagmopy.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3xtphbxqk.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt3wponwmft.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt3xumkswil.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt3ipgayble.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt3lgotrqdm.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt3qujhmlia.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt3dfczvsmr.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt3kfnvqnkt.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt3ujefcvln.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3fcpiqqfv.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3vzsvsnnu.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3vvkixsub.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3syyiuung.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt3kzpldkwi.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt3jughlqia.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3ppgevzfm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pjaaunmi.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt3nikxmeov.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hzwvwqge.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt3fvqpyyuh.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt3xvatodbp.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3dfqfsoju.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3iqibedih.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3seotujdh.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt3qtadvjcb.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt3bdocgckh.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt3taqhdqbh.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt3cjocsutl.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3iiretiqc.html


<!-- 参考信息 -->