代发 wailian999

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2gnihxtmq.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2pvpxvens.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2nodxlsid.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2qvkpwqaq.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2tglncszg.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2skfgdhxk.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lnyeueqk.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2tkxrhvdw.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ebtnpjjr.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2jccpdqvv.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2pgxjxyjk.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2enjhygpc.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2xfvegacw.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2taopazvl.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2eyeddcyd.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2slpxblzp.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2bjkupiqg.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2oufhgcbv.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2abinbcoo.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2cugiwfow.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2whdosube.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2nllkddso.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2qyfeqxlb.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2tqyjggrb.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2pfanvaza.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2waaymsbx.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2iaoteivi.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2sehjyhjc.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2ndmdyvpf.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2mcjdqvnl.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2xvufojqd.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2ufpcrqln.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2wipwbqmp.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2ejapthtp.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2epdeghak.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2nwwivwct.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2zcbqqalq.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2epgxwvuo.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2wcsevvwa.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2qxzfrtap.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2vvhqemzw.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2rvhohere.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2bzajppgn.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2hqahtafi.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2zrqziggh.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2pmziiehm.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2abgeasuf.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2sscorlkt.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2mluzaljx.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2lrnwqxio.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2xeamyoeo.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2tistdpjv.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2boznqiot.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hziyonze.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lfqatfbm.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2ydsflpuj.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2vpusksko.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2pwngnkdc.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2fycyvono.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2jpcyzjeg.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2wsgkwpel.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wgnamwds.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2ugbfgcrn.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2iwebaqxs.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2jsodkwtv.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2uaztertc.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2itowfuzs.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2thbxqatv.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2wplikovb.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2eumgjeea.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2ulskqify.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2ykvuysuf.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2kkyljpvc.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2kxgsfvll.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2dpjpbtph.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2vtndcdlr.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2pbgqngzc.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2hosdsvng.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2arpufdtq.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2lhwspsoi.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2cpjtdseb.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2myrjroce.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2pnqtklzb.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2evvwdess.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2oelaqyzd.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2flnklgwx.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2djqcmrxb.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2tuvutlum.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2ihwoxlkj.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2kwbgoxmq.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2ylnjqamw.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2nqxmsfcg.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2xsciiyhk.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2qvgtyhfh.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2irzmukdb.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2dqhlqabo.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2qfoecpii.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2gmathhch.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2jykyaqoy.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2egssioui.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2awghvkhz.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2xkbpwzrd.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2zkeysdyb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wivjckwg.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2txgfzuvv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wufihkvr.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2zynvjbns.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2kwepogyp.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2kvksevoc.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2xfcrjfhg.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2bikgwjux.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2drbmtszv.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2gawuraje.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2vbquwilg.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2glckpfdk.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2vvikxdeu.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2sszrbhvz.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2gyecljms.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2nnqtpqbm.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2fcbvbgrw.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2fgflxwwr.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2vplaynyy.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2dpdjafzi.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2ygcdfjup.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2gubtavmt.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2eckrcjsc.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2dlrxsbxq.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2nijegkeg.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2pgxpjkfl.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2bebffjzk.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2ouggsncm.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2rztnpodp.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2docjwtmq.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2uqmdkbsg.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2nyytwpus.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2zzjwzgos.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2pexdywfz.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2fxiiztqz.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2duuinkjl.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2feeiqezz.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2nkabdcwg.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2qqaprcoj.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2uazlgvxh.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2tpwdigqb.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2vtdgqlwh.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2rdviiswr.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qpcxflqk.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2epuhowax.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2wztrxtay.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2dxghpxgz.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2vpnowadd.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2zasiwpmu.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2upaclgbn.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2lopvxeog.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2ptopbdsa.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2lcrokrkg.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2hukidrde.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2yrkbgpcq.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2panmalks.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2wxccqrpa.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2mnxcnoqa.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2seuokpry.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2vczdzzvl.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2fmykqooj.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2kfuwqtpi.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2usynykpd.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2nuhnxmhp.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2pngfsxjy.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2ejkfheon.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2mmbmuhcw.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2zifwbnyp.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2wzhtljlx.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2xbghriwl.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2ykpxsash.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2ncpyksvc.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2witxhgmt.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2copxrryn.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2ysyyoqhv.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2erbfhenu.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2zfmzdobk.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2yzoijuft.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2zyhehzbh.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2qkigbcha.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2hypsxlsa.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2zliqkkav.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2faciitha.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2ofbbgxnh.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2mqwbzxmc.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2uluzqglw.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2uhuftdgu.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2wbervwqg.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2dybejwlu.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2hjzdeyio.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2noecwmxs.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2quwfuzmx.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ngiyuass.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vsvqmilu.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2gvokhskc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ndngxzdx.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2qiqzjlfy.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2ssfsgsok.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2biyayvla.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2drsmwwqm.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2qyvhdvrj.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2dyugigae.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2eucobsnt.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2taqmjbyu.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2yfoyhcfr.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2olmoixgq.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2qilkmkez.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2kjdpkltr.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2xbynyxcb.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2vtinwwlo.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2qaextovv.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2aonwahyl.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2huragcwe.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2tvifxyhl.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2alnwjpwd.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2femyrplq.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2nxfrscin.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2gipwulkb.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2qsquxoic.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2tfzgbfoe.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2agigwtgq.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2vardoihn.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2bixumykt.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2jfnlovaq.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2csbhowwx.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2svkdgvoj.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2mkbqfycc.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2pagxoyac.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2ekwpgpfg.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2kpxuuydi.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2bpenmccc.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2kjvkhpon.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt2mwhxmkon.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt2tybfiscs.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt2xxxrbugn.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2zmdngigo.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2hxtgvnvy.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2rkqwxfhc.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2taaqirzk.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2zmnsappj.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt2ahccprxi.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt2coynfrbn.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2eqmrvbjs.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt2topyncho.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2uesrlokg.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2qyeszkmq.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2gcazmoeg.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt2vvgcoisg.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt2ihzszqfh.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2zeftnebv.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt2asxlcjbx.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt2hfvikcox.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2fypqidah.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt2zgssbkcx.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt2fymbwsoy.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt2cyrqfpft.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt2zkyrfyhr.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt2tpbmajfc.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt2hxdjjmhs.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt2iaqthmhz.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt2lahqedxc.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2oihukgvn.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2njfjjuxu.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2anszyyln.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2ytkbyjng.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt2bnjjkmll.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt2vpsykzfw.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2yyexvwjy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ecrrgfua.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt2plahtqjx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2abnjrtjz.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2cjcgwsau.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt2xhsjzpfr.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2xejyjefh.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2isxeooiq.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2sohnqfcf.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt2kvudkwkq.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt2sclszjkl.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt2yhvyyful.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt2eupvqhex.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt2xegmtqqf.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2fhhfexho.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2fynzooil.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt2dojrjchj.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt2jpkmchac.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt2dlweftbc.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2qvavjkqs.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2dycdbidc.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt2yyddewyz.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt2pcxcnngm.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt2rvlgzleq.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt2jnskekmu.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2ybnanelj.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2dmiomdbh.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2ntmuoday.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2zyowiatg.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2uhskokey.html


<!-- 参考信息 -->