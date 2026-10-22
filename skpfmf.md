代发 wailian999

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2bncjfvjk.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2egzmnyvi.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2gboxcdlj.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2votvgldp.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2jbdrugak.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2cffzkiqj.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2kcbdldpm.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2hfsnozec.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2osrsmrmr.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2tzkcbffo.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2xnncvjra.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2covnwxgw.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2girosqmu.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2mdbyauid.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2pewwyrqj.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2ggxhelkz.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ibfsozlv.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2brvzfgzj.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2lglcqwci.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2gzlsgcll.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2qqyomwiq.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2tizycvqu.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2wudgrvqc.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2sclbjqwr.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2othbljej.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2blgycmjn.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2abyplrjj.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2coemvwto.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2pjkbkbeu.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2vffrifpz.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2zrmxryyy.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2szdutzpt.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2omrpxwoh.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2srmtgvne.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2qrkvhyhu.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2dkbulrlf.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2rwoudbjo.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2bjtmscxl.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2lckgktol.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2sdwvauol.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2kyditbsu.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2fpcrhvaf.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2sskxybio.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2gowuhlgq.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2idcouixi.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2notvceds.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2pbnhqfvf.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2vectuukl.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2uoqrbncy.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2xwcnusys.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2hcpdmnxc.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2gkkuhvhk.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2ehgbgbeq.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2aikoqazn.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2axdpqepf.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2hjbpawig.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2sjzjvhnc.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2ykmwcrnk.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2rnxkskze.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2qeloqbjx.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qocatngj.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2foixblhv.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2rakpwout.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2bzlpnyfx.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2cvwdnbuw.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2lnrfxxfv.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2fmididig.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2yzllokor.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2sjnfprtc.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2micqrmvv.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2rlvnqtoe.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tkhfuhas.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2oquvfudh.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2zywdiwve.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2nhwrkgou.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2bxqtuxzh.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2igyznwsm.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2msmqxifh.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2xkwgaact.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2zfxqfsom.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2sdphfhlw.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2femskzli.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2vguuxuva.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2erztutua.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2vaeuwuue.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2qbiwehps.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2dbeypdxq.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2bhvdvstg.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2txkeulhg.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zhoveryp.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2ucnlwgrg.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2hmkrzafz.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2sntueajj.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2dvixrvsp.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2bobylgrm.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2ibaqxtpa.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2vvflrflk.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2crrcuztz.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2vyqogcpz.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2mcutnjcu.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2qczkuseq.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2wuvfocwu.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2fuhgtlso.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2mderbbbm.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2tghfziaj.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2jyirbron.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2sneopatk.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2xvpzrtsg.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2tewrnbuz.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2qkfvalxf.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2tixilqjh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jwkgrlne.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2nbekyxem.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lgnzpubb.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2asepolol.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2dhezztoj.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2guylystb.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2edllhgvu.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2fybzqzhj.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2juoyembw.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2eltajzvi.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2addkzcyz.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2lazlqfic.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2axasramp.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2xeyakjvb.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2aiqsvtvl.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2sntuiktw.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2zopbucyh.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2tqocannw.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2tblzrbsf.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2nbaoqkup.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2jffyznuy.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2llvafmug.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2ogugyejf.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2dmasoloq.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2xwkgewqr.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2cewfgyrz.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2cyljxujh.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2kbaezstx.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2aqybwxqg.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2uzzklqcs.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2opjoidxb.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2afeguqdu.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2miyawput.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2vxqtnsxz.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2btflvacn.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2ggcrlwvv.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2apvrznju.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2hgpodadf.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2wskxcvsd.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2rbkjipwy.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2rzmsmkvh.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2ehhgfbyz.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2lskkdiej.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2kndmqord.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2tgqxczwv.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2mkmaevar.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2djkaxfov.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wujtwxmd.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2neatwqic.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2mygbwapa.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2ukbsaqna.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2xywjxebh.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2qaobybox.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2tbwxurtd.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2deukqlbj.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2xyqwrthl.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2yroppeqr.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2uouicknz.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2gufnfitg.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2vbqlkyex.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2hlqoupmh.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2sjphzbip.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2bypisnyh.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2wxffntrl.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2fpvwzvek.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2bbefwbkm.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2jganmmct.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2owdmjfsz.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2fqlkvtle.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2gphfnpjz.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2manksstt.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2zauzjnrd.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2qdoalfnb.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2jbmdsbyu.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2gownamch.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2fvyvevuu.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2ahyffewc.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2beuqooou.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2lztipqyh.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2jjqmyjcg.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2mzapzxwy.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2hmooiywd.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2rttrayyz.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2lmgtflcj.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2sqmynmea.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2etpnpefv.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2mpndtwga.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2orcefwzw.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2ninuvako.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2qlwhvftw.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2wggdusar.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2mfthqucw.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2llphvpzl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tnskidor.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2azuhmfww.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zncmfudv.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2ftmbjpel.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2kblezusd.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2scyfieub.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xayjznkz.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mqoyxkoz.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2nwwgvnin.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2bpdwulhj.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2kqnifghd.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2fqtbdfzg.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2xrfzoegv.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2pcrvvkad.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2ulpnzget.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2wleiwwbb.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2bylgxzvx.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2fazfibnw.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2qynwjepy.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2rpgjdgnj.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2hlufzewv.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2jhgqaqml.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2xufmqvwm.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2bevrootp.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2gntskply.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2ixeihvjn.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2zzqgazbi.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2hxtdgsyp.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2ijesqrxk.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2nhvruujr.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2qkzqenbk.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2alzqloel.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2hkomhclm.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2vyjzqnbq.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2sxalxnwc.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2givxfnok.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2ylrtugin.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2hmzmcbpv.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2ehknpflg.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt2nfnjikvp.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt2znlrynan.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2hwfuqfso.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2grilvrso.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2zdnjuivk.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2zxgldsra.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2yzholldl.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2omqbibll.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2fxqmjgmb.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt2tpbxcqdv.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2iokumxzg.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt2bsocbavr.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2abzldkxn.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2xrdzeaew.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2xodfxhdz.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt2wxrzqpxn.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt2wbazduez.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2zkvbarap.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt2jlmzdlwr.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt2mvpphcpq.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2ebyikatw.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt2vztnbazr.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt2nbeddtbe.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt2axvxhpwn.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt2mgjufikh.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt2guoszniq.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt2fqosnlnc.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt2kxrudroo.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt2jyxptqhc.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2ojpcivyb.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2cgpqacwr.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2hqoparni.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2ywyfxvll.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt2ewgbdulh.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt2xowzfjeg.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2krgjokuk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2binrvsze.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt2zonxxpcv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gzniswfx.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt2sdwrxwkq.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt2gnordrxb.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2pcvnpubf.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2ertmauoa.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2fjwntjci.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt2zijkqidl.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt2tgspmgch.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt2juqtiqaj.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt2gttfvrqu.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2mluhjlec.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2qiirhlak.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2miujzxke.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt2ujjdsaef.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt2amiechls.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt2iyajohvb.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2dpouuudp.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2qjyirwfp.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt2fbcuccvw.html


<!-- 参考信息 -->