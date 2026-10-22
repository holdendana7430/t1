代发 wailian999

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2wopqwann.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2cmodamhk.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2vxzqbpuf.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2erxxwrbe.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2ukimjzuk.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2ngptbcxx.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2xidtggwh.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2mgkbrxoh.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2dywdjpvf.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2mevmnxjz.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2enpanszi.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2agfyuoxe.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2ykwxmlfk.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2lvgqxeqr.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2zsckseap.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2kcelqgtz.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2aiuhwzst.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2khqzyjga.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2yodaxbhi.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2wefpwjtg.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2dmdowube.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2atupdxwt.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2linidtxh.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2glfqogir.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2iuyvmzir.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2uyilkfza.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2hxgjtkhx.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2sqrjqkkr.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2qqlsueso.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2abrjllmj.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2hpftanci.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2emuvbkup.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2ctdroxjf.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2fpypvljr.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2mjzscwts.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jszupubi.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wrioorhl.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2wgnperqs.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jmqddkib.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2uenchxkc.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2mdktohbl.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2jmckyrjp.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2xpseoric.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2idjxlzwc.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2tclnxavm.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bmdjrfex.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2nmimlvhg.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2eszxgrxa.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2mdjcpvxt.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2epdhlkmh.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2qlldgibi.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2sjkgidbr.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2njahtmxd.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2rbrvpezx.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2ywogpybm.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2ppuqcoal.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2zrurdfot.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2dctgvxwo.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2xgoajnjm.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2jnytheoz.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2zynnsuxz.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2stfrregi.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2yhugleio.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2izjstatg.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2puhfawgl.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2rnzgwfvi.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2qzltkmkj.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2yxhvllbf.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2xvijjvof.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2uxbdaueq.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2gimezhaq.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2vhzeyiqe.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2nbgsnrda.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2gcnbmajj.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2qrobvmir.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2bacfvqbr.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2rgrtschg.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2tjkvrbzd.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2umeudnwy.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2ddeejjru.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2eemlbhxj.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2woqkcrql.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2dxjbcdnw.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2aggnxqgq.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2wttdafhj.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2racfprnq.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2rvfqqcir.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2crnmvxut.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2ujwtossh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pqribggf.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2lbwowtpz.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2yomcdlcp.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2dxnhhqsg.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2rhncailg.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2dekocefa.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2zbggczvn.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2wnqykfcn.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2ywnqzsdf.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2katfxlpq.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2qyctcunc.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2rxoaeitb.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2kfxwyrmq.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2yhmayczl.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2bpogsnqd.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2sqgyumrk.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2axbhphgx.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2ufrxvnuu.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2apdqephg.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2xjimxadl.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2utivmwmk.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2evggbmfb.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2rdpbzgme.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2vgfjgvvo.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2kifxedsg.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2nbeuvbdy.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2nisiggvr.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2sbbirmla.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2qsvfmhmc.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2uklayxnv.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2wqkowvdg.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2lwrvsyon.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2ivcjmcxx.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2bdstmafz.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2lzwziliu.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2ydhxqplj.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2cdomkebv.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2shnksroq.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2dqwhxqhw.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2skrhwtlp.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yzxfobil.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ovmwnsna.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2ckozvkho.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2vfbsimki.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2qgnpupza.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nxowiwdh.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2vncxfgob.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2cjhofkmg.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2ricqkqzg.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2onuihema.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2diicemkd.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2mgqtfcwz.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2nacudodd.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2ngvuolcl.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2katskeqe.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2snfwkhzq.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2ghfujxvv.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2zflescyn.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2naguizur.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ijhopydr.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2ifpnvcwb.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2quwtqhgd.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2ksppukjm.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2uhzpeysi.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2hozxjmrs.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2sqsetdhe.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2vojmjsre.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2hdlpapjd.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2agvcxvuo.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2pqitbnjl.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2ierxdubd.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2kzhswqco.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2wslogqym.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2tkowxzms.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2fpajowmy.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2nypsygid.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2evwwbved.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2skdlbupx.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2vaiwfkzh.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2dnbvogwa.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2kbybdwyu.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2oslcmhdp.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2aacqelpd.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2lwlsubrb.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2ugjleexh.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2rqwmneol.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2nbuelbld.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2loiksdea.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2rjyjnits.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2ecadbyrv.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2nmgolfye.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jmbnnbfz.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2jfaojxjd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xxmsuyct.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2bhmuphdx.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2cooadzmf.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2exhtcdnd.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2npvgfcmp.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ktnhqqxa.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2veabtkrd.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2klnejdgm.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2ovtgawvs.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2cgcyboon.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2qelzivlt.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2jaekoleo.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2obuzcugw.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2qgkjtrao.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2wjhdquqx.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2jmwxutem.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2wprlsjte.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2ahiimnvu.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2bkhhcyql.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2ebznvfqp.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2mfsfqdam.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2ncrrouma.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2wsfzfmpm.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2dnayldyg.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2ctkbltom.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2ibvsegde.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2fkbhardc.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2tgnaagxr.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2uywyeikb.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2crmmocxc.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ilhihkxp.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2spenxdbo.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2mxnjfzay.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2aatdsqre.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2jlelevhf.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2dhodndci.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2tjsbffpg.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt2zlgorrcy.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt2ebkhmfoo.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2yqxpzvib.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2hzjwlbgn.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2twgrknxu.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2izigydmt.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2lqxxbyel.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2ezhzqoay.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2lcfyigsf.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt2plriefdw.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2zzvyysxl.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt2ckzkuglv.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2udimjopr.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2usuideae.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2vwnkdthi.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt2rddcccwu.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt2ewxwfslf.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2ardyruhq.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt2abqyglzd.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt2weftwbry.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2adggstis.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt2cpekdqhf.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt2axpzedmg.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt2qnoeapon.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt2qpjeuinn.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt2opaqszut.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt2iqvuguow.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt2yrabmuxh.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt2fampfcea.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2nxflevmb.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2kjuqqmni.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2vekstzdx.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2csjaheqi.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt2enancbgm.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt2crnhsxtk.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2mmutqmry.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nexvdyun.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt2pnpvkcay.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nrdgganv.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt2ktpqhnmv.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt2wnysxune.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2czryrqss.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2nxzxvcws.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2tmtooxdr.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt2fxctjcgp.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt2dohzgprp.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt2zaavxmcx.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt2yimwherr.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt2sczisbbv.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2imhnoxjw.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2qpojkzra.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt2jozsyath.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt2mlluvcdg.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt2rawgsoho.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt2dwpnvtvk.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2opmzwmet.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt2rixlkdqg.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt2maveqght.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt2llpuahtt.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt2wdgtufrr.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2vxppzcbw.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2eftdqmqy.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2oxfuymah.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2fsvozmku.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2kqfyzxjx.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt2hpxjogns.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt2npftuenj.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt2vdqeeuda.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt2catmmngg.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2pjrilucj.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2ykmoolfp.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt2dcvhczqk.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2yhsexejw.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt2kuyretaw.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2yiezhngl.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt2upfmjvos.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt2pgqnmmwn.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt2momcqvmr.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2zlhzsekl.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2mejtgdss.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2ovplgjod.html


<!-- 参考信息 -->