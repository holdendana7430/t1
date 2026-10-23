代发 wailian999

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3tyxymwaf.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ycoissvm.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3tvxlesgo.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3lfzmrqhu.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3krbcpqqv.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3ffhgjbyp.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3khpwhjuc.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3lwnjpipa.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3imkgvrcu.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3owflnlhu.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3xvlozbez.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3omxlujhj.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3byvfvoiz.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3uoiicgud.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3gcxlgija.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3qbovqdfw.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3lmaemyib.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3ntcqhtzn.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3pvewjzhc.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mfxjcipb.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3wkcmvwsa.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wcdoyqtz.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3exowedyf.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3tmhrqpdt.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3arrrbuhk.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3dmltnnna.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3pbnzsjfs.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3xfkdatzq.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3coycwjct.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3vhnfnpaw.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3exxmxupl.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3xtzautof.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3cibdvshv.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3uwnyqvqk.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3izrtgufb.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3mxunytlb.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3vdlnvwov.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3jodifobz.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3gwszbwcj.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3dzkezvkx.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3pbpkefqr.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3walhnfsc.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3yiemrvls.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3vgicosws.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3pbrovfvx.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3plnfcrpv.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3hlhcvbcr.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3daolgvsp.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3hyfbmfbf.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3dvzrguzt.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3cobakoqp.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ehmfdbos.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3bmwqrmxb.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3fbzjembo.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3yphydszk.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3bsspgmqx.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3kkaejpxa.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3junmoanh.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3wjrszmmy.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3vgzrnlap.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3bjribate.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3ktcpildp.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3ygdzoqpd.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jmbrtglz.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3segymfrq.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3eszxpiji.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zergcxzr.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3hwdrflga.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3kplevuui.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3bxvuxatr.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3sipfejfx.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3mrwyyney.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3xicnnwkx.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fnawlmys.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3rlqkdgtt.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3uffupydh.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3obmakirb.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3dhrmzkgr.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3azlpdgkz.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3ukcqqdxl.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3xmhasrvz.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3gjjzzsax.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3cbrvroih.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3ymdkntqd.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3ykroeoqy.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3vytvafgi.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3tdethcae.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3ozczjvdo.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3ycldubma.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3xjzlihbr.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3dfyasrnv.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3csfkteki.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3eexxmguj.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3xyaromag.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3hivwzgan.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3bdakqtmg.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3oucrssja.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3iudujroy.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3hbludbur.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3kfekdlzp.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3wyldnycv.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3xfllvnrs.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3sfadjgsy.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3hsbeltbf.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3aagpbvbd.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3ywfxnkbv.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3ohyyquhz.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3rnfysfjb.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3mmglklie.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3dqqgdwms.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3bnsgjtrf.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3oeavgxym.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3amnoxgmg.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3xolyfmna.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3xjktyyiv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fjqvcogc.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3hbgvamsh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pizevjrn.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3jgfoekxc.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3vgdoxssj.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3uavdasqr.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3oywswxvu.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3banzeeeh.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3dpowracb.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3epgqrfbq.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3qzkvtowi.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3ilflmbst.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3ecjpzqjc.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3gpjckdsp.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3dfqjqrnq.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3mbzklogo.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3sqlnldpw.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3nutdvapg.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3bmbevgri.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3xdyliadm.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3irbpfibe.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3deizbbrb.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3mndurnyv.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3sdgjxich.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3rerfwxpt.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3jiiilcmd.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3bvcozrcb.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3rhesmpgy.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3xgdppqvv.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3jzcgsubs.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3zdtkbauw.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3mvmyijoj.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3qruynaye.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3yykssdra.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3ewlepaek.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3nvkfdezq.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3yxxrnlyu.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3ugxfpfzo.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3ilkxiyvs.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3snahuzyq.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3qqwpzozb.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3inxugtgk.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dovghyee.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dumdjdxf.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3omvocxcj.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3inhwjrvg.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3sdpkionw.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3orkofnqa.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3bcdqnzad.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3asezlzwr.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3rcfthrkb.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3gdndficf.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3rgbujpyu.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3rlmisxmr.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3vavjeudo.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3sunzjvfs.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3rbbmgsud.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3hzhaiqsm.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3bfvywukn.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3kichgtvd.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3lohocrmg.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3rbrvblyx.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3mbbbhdar.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3gaavkwas.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3benmxsdc.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3yisfrrrr.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3lbsulago.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3veydenun.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3qshkbobh.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3hsyhybez.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3blngsbva.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3wcvgelpn.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3sgnszrjd.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3jplhbami.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3ohtsvzbw.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3llbgdemk.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3mfztjnsy.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3nyzekano.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3rhuynlwd.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3uildsuxy.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3gtoowhsf.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3sdjuctcq.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3rmxnqust.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3fauxalpw.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3qxjlcfew.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3czvmcgoe.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3stmyzjzi.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3pighyvkk.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3kiyiwjln.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3fvknpsht.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3msrauash.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3qvfgmrek.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3sntrajsk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iuigumkw.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3ttknydzp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ubkcvnut.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3balmfchv.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3nyzspwyy.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3iqaxbfao.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3lknligxt.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xwqqtltx.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3ilwdiktm.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3golscyxj.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3cxdrybht.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3mihnaclk.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt3ectlmjpt.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3zvzivcwe.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt3idxktilo.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt3ahdbwmxw.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3hkwroqpl.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt3ltcgjxku.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3pvluilsb.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3mmzvgpex.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3ybzjfjww.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3xtcjztcx.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3uozxiuft.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3jckjyvqv.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3revsnfnf.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt3jrujefgp.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt3qgsgjnia.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt3lcowpmzd.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt3gfbnmswh.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt3cofmfakc.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3gdwkqtwh.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3woqbcndn.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3yneljphf.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3cazctztt.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3tmtmlhmi.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3clnyryfm.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3fevywwgr.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3twwerlxx.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3zdcefmrg.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt3bcgjqcad.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt3ufzarrwe.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt3nszklwbn.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3dljhvwrf.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3gkraudyw.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt3cfopajos.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3pgkqnwag.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3olksocjg.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3yfdsguuh.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt3nakjfbhv.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3tyajtoai.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt3cfhfoqqj.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3vdkglnic.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3yixqnqdn.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3aqmzeqpu.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt3dfqwfwbi.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt3quelvqsr.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3eaxrirhl.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt3rysvktxq.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt3fmsmkdoq.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3zlpbvfph.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt3wxvlamyl.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt3jdiwtcbc.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt3wwygbmrv.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt3dxdnjfub.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt3bdwunmxi.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt3uargbwqt.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt3mvaubgfi.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt3qaniaiow.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3fgjidssi.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3alzksqwm.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3pncaohsm.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3dodokhzf.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt3waujxikh.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt3pglvgcwg.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3ycqcyvpp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ehfrnadr.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt3rbsfwley.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zdywqmaj.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3inotiiod.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt3dpnhlqjm.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3xcvrlfvx.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3dzoeavvd.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3uxeibnhl.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt3fubudrpn.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt3vwhxethu.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt3eltplzqd.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt3tqksrjry.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3xyuhnpdo.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3yvtxbtsf.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3khsvgdqx.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt3phlgnbtu.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt3dwxdavka.html


<!-- 参考信息 -->