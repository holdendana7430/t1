代发 wailian999

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2hyyubkpg.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2ciyurglk.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2obihvilx.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2qnpnupat.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2qkxjbwzb.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2dqmdqxku.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2znayafcq.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2hmxnyawz.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2kwabprin.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2lelyhsws.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2wauqxpdt.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2zfphflsv.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2svtkkgdn.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2qgbjuslk.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2vkxfljgq.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2bazdqwpc.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2invdqcfz.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2ufwbvxsa.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2ydturgqp.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2vxgukmpo.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2fbdlnsps.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2upysaoij.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2aomjrwmd.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bznowkhh.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rftxmbjs.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2chpqwkbb.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2qayrbjvu.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2zebepiqf.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2uvsewidv.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2lyantzzr.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2xiwvkzzc.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2asriaijp.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kmyvttfz.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2nxmgexrv.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2egyhlube.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zwmsmngb.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2wkstpcey.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2fpbowlnn.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2dsmzeoap.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2fmguwlku.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2lceqwpap.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2hjhkgwyc.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2rbhmtuio.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2ebohzhec.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2ghcealci.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2omvhisqi.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2xmawoyeb.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2kalrebtb.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2pimnkfkn.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2brnddvop.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2swnefgao.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2gmsygbvh.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2bzwlctym.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2ybzkdzre.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2ueegfwev.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2vsvydhlw.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2ikrsmwzj.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2fqvksoau.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2wzbowgir.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ryunlpma.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2exdimbyr.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2oefazovw.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2ukoqpzhi.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2cqylnork.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2vpzgmkzn.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2fbycphak.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2yegbgglj.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2gqyalunz.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2ubyqlvdb.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2rzrcecpo.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2kiwyabkb.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2jskeheix.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2uusiscvd.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2nkawzywl.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2zazwqmth.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lapydgli.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2jryzumkg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2luzhascl.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2cutiofwx.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2qlkglzsv.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2ynhnwpwk.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2vbdaducu.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2mgzlmsft.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2stmbxqaa.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2ipfdpnmj.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2gwzcohoi.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2othtptmy.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2jmduuvun.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2sriudnek.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2bhqslvnv.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2goestaxt.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2ogsegwfb.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2vhdkuylt.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2tabnwuuf.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2wlxcfyuc.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2xazlzojy.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2heuvpvvz.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2stxslnnd.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2zhgpjptm.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2cmzbqooq.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2iqfmbpmg.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2wbsxxxdo.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2xwoutbez.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2brzohbky.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2ilkvicru.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2tfbcbobd.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2iwzrfvvg.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2vilcdjsl.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2flyscgpo.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2rumuvcxl.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2hbugxzzc.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2cybszjws.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2huqedjwf.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2okxctcfx.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2xdavevgr.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2pbfnuftb.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2savuujrm.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2zyjjijdl.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2ykalfwzb.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2ijcrfdsr.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2lwyiawhl.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2zjlfapbr.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gussdkcs.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2srcuideu.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2ejwwbzkd.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2cnydhqby.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2esfrajsn.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2tfasrzei.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2qacyirbz.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2xkoagcqs.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2mnoyytik.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2idyxruaf.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2zjthzmmf.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2hosnuxhj.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2tksxmoqh.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2tuqrglpy.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ccnlualt.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2onrfvmkw.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2iadrilai.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2yaxhosqk.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2rwuhispa.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2nhaxadzi.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2yjwdfgzw.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2avncyocb.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2nbhmmvyq.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2wcrqsvaf.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2wfhkgfhl.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2muhdirlz.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2syuvvzyr.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2gjwzlbjv.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2ddiksyjm.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2gpaijzpc.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2hdgyfuae.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2auslrxvx.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2oypmhdjv.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2vunxupok.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2ewsftjqz.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2mzwckyka.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2sptlebnp.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2uajyfcsj.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2gnxlceie.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2zguxlyos.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2wxkliatz.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2coruormi.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2pnctnwpp.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2kowbgmxs.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2uewmzsyz.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2mvimwaov.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zzgzjqou.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2yvjnkfoz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fhuqwiuz.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2bimzfszw.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2djmdavqz.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2taifnvlu.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2umztvahp.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2qvdrgumz.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2ysqstyxs.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2gnsbizbj.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2bdaqwacn.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2sibeeajx.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2gkyctcrb.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2lsfczjfz.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2vizjtirg.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2cxearkbr.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2hsoprehs.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2hmxvlmwj.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2znoqpohb.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2ucimsfkl.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2mgpuztoy.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2uqmxrhul.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2hlcvtxwv.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2vdzbhpmu.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2tysnjypf.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2crdgyqvc.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2mhpmxzob.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2whodpsxs.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2lnciipmt.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2optasszx.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2jfmqvsqg.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2cbbawkzu.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2aifkpqpy.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2jgmvgvck.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2etoyovoi.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2lhmgvdzc.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2iopudqfs.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2ktmyjynw.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2ekjalnxs.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt2utuqsziq.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt2gozdizms.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2xzniyrul.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2ltitbyoz.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2orctjiei.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2xfrqlnlb.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2jxkwibgz.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2zvwcdhhs.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2ofkdvoih.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt2yrnklndg.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2lvicigkf.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt2qckvlmmh.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2mmnnaaeq.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2jjbcpnaf.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2tfofxptq.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt2qdvhclzo.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt2oyjsouyq.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2rszwmxto.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt2ealqeyad.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt2zcvbhnpu.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2odfmlydo.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt2vehvdhdg.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt2agjrmmij.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt2srdfnapn.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt2jbolozni.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt2yonrgkrq.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt2bhernfux.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt2uyqobpcc.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt2lqyvkscq.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2jbovlapc.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2nfvclqki.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2pdnynakv.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2jjogyvrg.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt2qmcqbenw.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt2qnzanyxm.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2okbhypjd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ilgepyty.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt2yqphuhsx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2heoezdrk.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt2yffhwuvz.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt2dbzqojex.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2hcpmpoxx.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2okqlcraw.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2orsplzfi.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt2wravjfoy.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt2ubteagts.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt2qzbgcydj.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt2qhxaficf.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2mridnvel.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2qalukbvs.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2dichmfym.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt2ayraevqc.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt2mnilgwth.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt2xutapvon.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2hhrvajhi.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2lqypyslf.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt2hnnafufk.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt2uqswcjbt.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt2nanfxpgt.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt2skxuiezl.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2ojessvvi.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2vzhmblsq.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2hrniljlk.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2omenmrsa.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2fgmckrjx.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt2yoeqspsa.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt2doegsyyy.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2okezdmxg.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt2vtwgfgwy.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2ijospvzx.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2iatmsxmb.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt2gduuwoee.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2qazkybpk.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2ydrkwdrl.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2rnvmjwlk.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt2cpxvbofs.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt2edynenwd.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt2xhubnjle.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2fchcqpol.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2jnbvtxeg.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2ovxnhkez.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt2ozfqjfvj.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt2rqcqnqdc.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2excxsvds.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt2hssqqqxz.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt2csaviibc.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt2tmvgitsx.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt2ysxrsrsh.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt2evqswpam.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt2bcdujjtl.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt2flmbrhxp.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt2ralwwfdt.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt2qwaasowc.html


<!-- 参考信息 -->