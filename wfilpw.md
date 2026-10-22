代发 wailian999

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2evzoekpw.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2xzvsgjle.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2mxevtvcv.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2ktkccefu.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2efccnlnq.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2dbatawsd.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2advqlnjo.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2ozibtjqj.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2nommvrby.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2qzhryzig.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2wwlenxui.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2ytaoqqtd.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zxqbktbx.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2chzsjfmv.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2rkxjirsq.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2incnownj.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2fkbavyog.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2yuooipqn.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2oxeolkfe.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2qjhblzkp.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2qkbilmbh.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2kffyatqh.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2uqojhxnt.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2hovghlsm.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2iihvocfk.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2zqloulns.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2wjxyzgye.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2aymuukkk.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2odqoqnfy.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2vwhdjxnm.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2ahqhjajd.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2upgpzaab.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2fitpzrit.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2fegjwupj.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2ynyzsuwu.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2ahfsswhk.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2qfinrfor.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2orxiaggs.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2vchpzmsz.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2epzxhwmh.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2xohgdtni.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2pgimzopw.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2yxfmvoot.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2caakwohm.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2scdqtzub.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2ekazuytm.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2zztubkzf.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2fmgxqpct.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2nvbsatxg.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2fzlgyvje.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2manaxnli.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2zrjccpud.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2cfoqtvls.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2qewiywxw.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2lmyjznxe.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2glkxxxku.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2nkxaafhw.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hamtkidt.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2eorgxtsl.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2bznpongm.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2zbpklaev.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2jrbsxvjj.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2djgexqkd.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2bqzvgwda.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2btmdrzgk.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ohcwgoqd.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lfuhhsrm.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qyazlejf.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2xfrcwxjo.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2aeglbixq.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2zcfrusqj.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2mvgtpuyb.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2iluvseay.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2gntandph.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2divzfded.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2ixddiwtc.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2gunbeubu.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2kkfqtngg.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2sazyiphs.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2pflyiihz.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2wqwtwdok.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2tdkfvkoh.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2vxnipohe.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2jzihybfg.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2nkcciadi.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2bhhihlsk.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2wzltchrp.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2fndwgqwt.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2eugmcnpy.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2wzvjfapq.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2cnafqmaw.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zksjtryc.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2cqihgmky.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2jwzmxujl.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2cctebvtn.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2pyfaihaw.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2rtezoojc.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2qxgixaly.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2hqbvfnhg.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2prpsklzj.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2bpuvwujh.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2vogdspyc.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2brhyytfp.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2iqzzfyhm.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2idpvlaki.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2rqjwwldh.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2jeflxqyb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bqkcwfra.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2yvjyzndh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nguxsdzv.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2nthxjvfs.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2zcwfcnei.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2vbnnzzeb.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2tpboclba.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2zzjkbudz.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2bklhgdrb.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2dtwpurce.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2nzhkqflx.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2ljjkjteg.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2ulouaiea.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2rfualmif.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2emshmjto.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2taohvsqu.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2nwseutmx.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2uahzgfit.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2qjtiqfqh.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2hhkiaklv.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2fbnkgpum.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2xereohhh.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2swnbwzea.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2oebujpoe.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2junyfwri.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2nmjjormb.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2ilqencba.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2qgjpznsf.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2mlmmqhco.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2lahmhime.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2epcodyns.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2axuckvus.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2lutilkhn.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2dlzwwtjt.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2jewerlbc.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2btlathqg.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2ueeyxode.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2bjxonewq.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2ioqutmpb.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2awywlmnd.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2wqeaxbkh.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2qfbcmtof.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2sszlwrru.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2doutqhzn.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2uccwkvao.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2dmvkyovp.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2rgolhkiw.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bapwxnbc.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2fbjuawdp.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2sumxjlfv.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2ehddeyed.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2kfhglinm.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2atkpkxwm.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2rlhvtgyx.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2qpckvpgs.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2eydmazbs.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2trtxbggj.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2flvcagpm.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2njogzlvn.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2tiammlot.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2aoxhneor.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2mxeouubz.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2mwwsafwc.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2fmmmmlcd.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2qngiqjrl.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2zmzyzipc.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2dpisxujt.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2czjmisad.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2rznzekpv.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2qsjdossn.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2fxdybecu.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2eymravqa.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2elxsyqrb.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2zjmkgjww.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2yiqfrxto.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2ckaqpyyb.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2lnwjksjo.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2ryzktrgu.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2sjibndcw.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2udvglree.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2clxksfwo.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2onlznbnp.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2whnzkfid.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2hbmmfhai.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2juvkmfsf.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2aiygtxar.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2sntnkovy.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2lmmbyxyg.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2frzfvzza.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2weofbyqw.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2mchsdnwg.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2ihcowazd.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2bmxzyopt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qjuxgkpj.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2oaeacbcg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fuwwiucc.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2dgfwngwn.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2nohjfzqx.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2gnsqqfym.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vgmugjdi.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2unjoivnl.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2hxnvwlgl.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2sfcpuhei.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2uqiqgpjm.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2qgmndiju.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2aitpinxn.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2mbtpkjnr.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2cjshceyn.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2dowdtmaj.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2tysxjmdg.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2xqchhwvk.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2ckjyaorg.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2qyuhrxmh.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2lcnbilvx.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2vzagoxcj.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2glrcaimd.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2ifyhrgvg.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2fkkznkwk.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2buobpgnp.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2dwdfjuff.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2qtizdcmd.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2ovrdwrup.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2bbgccauk.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2rykctmen.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2uizofbfc.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2rwnycydn.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2zhuthhyk.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2wdhqvzrq.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2kgaehgbj.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2tkdjrflt.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2sedspzor.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2cbbvmlua.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt2efsibmth.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt2ajrwefds.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2nvoftbns.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2pwwtqrzy.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2bcabrdmb.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2wodbecie.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2ruqxxzyq.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2mmzglfml.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt2cdkiqqzo.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt2irpfvsif.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2mlnsklfu.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt2zkfajhly.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2dkszjcrv.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2ffrngmtz.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2bjeowkem.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt2hafeyuqi.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt2dbekbntq.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2xfyzdhie.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt2vgylhdvx.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt2wuxvtqvq.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2sdaloery.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt2xzuqomqe.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt2gttpyipf.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt2gzqwecaw.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt2vqvtsmlz.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt2igstunps.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt2bufzxvuk.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt2tccnqsna.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt2lgxzifof.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2bkteowbu.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2syidcaie.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2hkvafqbw.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2txyrxlnt.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt2jkossklk.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt2uluhwzby.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2ulfczgtx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2burmaqqx.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt2gxnlhjvk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jshboatn.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt2cbhvudgb.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt2nmbpfjsj.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2ybaturce.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2viiwoize.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2xwoobyux.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt2iebnxzbk.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt2ygbblnex.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt2lxkzqglh.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt2klkrdltw.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2lgdhbjte.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2uekoslmw.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2oyathfwq.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt2spncbtlw.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt2wjxrmhbk.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt2uqpmuokb.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt2gsgrabor.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2zrnyxdsb.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt2sjatppuk.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt2zddsoajg.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt2winmygbq.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt2yzlhouhm.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2urefdhjk.html


<!-- 参考信息 -->