代发 wailian999

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2bjxsephv.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2rpifjkjk.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2paputeca.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2kdbrdcpq.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2ylhpplys.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2uqfsopkd.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2vdtmnymq.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2rameaock.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2ntobyjhi.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2pejyixcv.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2hofolmsj.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2eoyybmnb.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2hghpyqpv.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2bugnfrat.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2byouoyhu.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2jljdrduc.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2wcncrcvm.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2bfexsrxj.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2wjotxtjc.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2fnhvkknf.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2fpukvivt.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2bepnpyfk.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2ghhmplzv.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2ollbywin.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2xyadryar.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2nuwteikl.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2abazawcw.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2frepnysf.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2tnnapybi.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2dmafjofy.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2ehauviqv.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kpxovgqs.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2yofihclb.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2fmpbifbo.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wwiscdgf.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2mawmimoc.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2hpjypbhb.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2njhunaau.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2dtgxhevm.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2uppzpsss.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2efgzsbiw.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2esopmote.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2nayszhcf.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2vwxsrmzd.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2amisbavx.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2doskhihd.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2rzythnrx.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2umztzicq.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2damgsmco.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2sjfdyooo.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2tmfunaly.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2velqvquh.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2axoynlwz.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2dxmpdsar.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2wabfajul.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2afqvhhsv.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2hjjibvuq.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2ykerwmsc.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2xwmvoukg.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2tudphlus.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2ktxtdrys.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cmxrrrjt.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2zemrdgkt.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2kocmlcmb.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2kluqgozq.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2eopfujgw.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2blsvziqp.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2iueavbjd.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2ybekehds.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2vmzbmwex.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2gmmbpkkj.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2fdtvwuzl.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2hthjdfyp.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2fuzulrat.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2dkhfyvai.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2alkhdxxd.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2anqzgspm.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2gpdlecal.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2datxagzb.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2hcvivryj.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2wvnmbfpu.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2effhticd.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2fknguvfa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ndqethzh.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2gmrkovdm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mktsnkqi.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2iurqcwmw.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2rdrndnro.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2hkslldcc.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2pvfbafav.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2jzwjpbic.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2niogkhcx.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2pwudqrni.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2wcidzpla.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2pffznxuc.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2ggikznqh.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2zzflpria.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2iamosoaz.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2hrmaieiw.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2dfviqhhy.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2ostbkxtu.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2gdihpupt.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2qdsluvbd.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2jvlcvasy.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2jzigeuvm.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2bqayrxhg.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2mfczivoh.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2eofssyio.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2zxvmqrih.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2gldrhkgr.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2trbvhwax.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2gfshrkak.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2wwtqdrly.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2gfshwbng.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2gfiqmkom.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2gkgrkipu.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2tdgvnbqi.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2hmebsgzp.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2mfnulddr.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2wuypafzj.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2qojwdrim.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2ywjcmyxf.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2vjeekmtb.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2qaauioqg.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2ommijtgx.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gltqxjtb.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2navcyzko.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2jtvfhjrr.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2mezhtezw.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2zltafdfv.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2djcpkwyf.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2xijjvews.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2bcnlmaek.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2zevqjxic.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2lbplrsru.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2aqhtydws.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2opmghptz.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2llemnsip.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2dxtuzijk.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2kvyhskqk.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2spkkjuyo.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2znwqhenl.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2gxyercin.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ckclibgf.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2bdrpozel.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2mqfntucy.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2zgcrewti.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2gbtzjmfi.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2rvckcblh.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2esuhsuep.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2gnrpkwvv.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2yajfwfmu.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2egxojeks.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2zjgrpcfj.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2wlppqjbv.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2hxcorodl.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2nrwletzk.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2tnjvtlbp.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2xtxhqnjq.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2shqungvf.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2freoadlm.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2mrpfxmxt.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2qekunovw.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2bobwkmbg.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2ivgligdq.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2gqmaboaf.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2ixbrzkws.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2jiskqrxa.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2jxjmegpb.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2cbvllqjk.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2cptdaliw.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2wbmoprjc.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2uceweluo.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2hyetanih.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2tpmdvyyq.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ulpmdjql.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mmllbfsr.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2ffcbpixe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tckpbjhb.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2gbhnsljx.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2qolmvsar.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2nqqxpqyz.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2nsmaycuf.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2yirxdfvl.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2terztgbn.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2jvkfbjvd.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2tsqyvtxy.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2jhxctxbx.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2tbuljjct.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2eukwzacn.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2khfffoqc.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2homvcqdp.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2lbbfsjfh.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2sxvwkazc.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2mvcvzdly.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2zgckwxfu.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2uqbjgqlu.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2kyjdnkdu.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2wzptrvjg.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2hxrfenvl.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2rudxsssq.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2hltjwurm.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2wlypcfco.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2kwcwfawt.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2tepxlaop.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2wkuoolmv.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2nyinzdgl.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2saypoqvo.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2slobrurq.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2wvraegor.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2bsegjrbh.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2kkzgotkm.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2nigdpatn.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2rzjtgtfk.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2xvmorgeh.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt2djugqysi.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt2vegezfpz.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt2sxzvqyit.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2fzbkqqxv.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2alkmrcgq.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2erpukkpu.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2hoomhnif.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2mnzhylwa.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt2jmxdjpmf.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt2wrhdoeun.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2hlbmxsfp.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt2mxekiunk.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2pukjqxxt.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2dckpxsmi.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2osuuchfh.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt2ynmtbvzo.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt2tohzpheq.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2hpphclqj.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt2prgmxedp.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt2zwubinik.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2hrbdagke.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt2volkxmdz.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt2cvzgapoa.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt2enfltbml.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt2konqsojr.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt2iaxpyded.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt2ktgxccya.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt2gawoyrjm.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt2kiltqcnd.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2vpqtyeqx.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2qopevlig.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2fxxzwbrv.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2jtsphkai.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt2ramzommm.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt2zfgliebo.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2lfmveagm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ugwwltxi.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt2kzjnxjvv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jlcexgtg.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2jxdvpczt.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt2ditfkend.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2tarcqstn.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2ibvufich.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2ueupbunw.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt2rfsphbuq.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt2vyxuvfbu.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt2geglebhi.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt2grufvkog.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt2zgoxdydl.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2wjlowhdz.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2ogyknyfu.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt2bfwvipqv.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt2wwrtyhud.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt2adivohss.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2eidhizpw.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2ltaxfhvp.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt2rmlnvniv.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt2kdgbvscd.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt2xcqxqmcm.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt2npcxpxgb.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2jxkljtft.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2xsaegsit.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2xxfzxyyn.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2kohhsuve.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2hijsohnk.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt2vtbmzuhr.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt2tolitqfr.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt2westbseb.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt2zixctfxb.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt2xgpywysg.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2molotykm.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2mbsotjpv.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt2boosdvsz.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2oztcmxji.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2cvikrtpk.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt2lhzoxcyl.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt2uurplipk.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt2apalthws.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2ficqlgun.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2qvjgcxbw.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt2wxduqdhl.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt2upriliwj.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt2mukghdaw.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2pigwcalj.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt2sbarwzuw.html


<!-- 参考信息 -->