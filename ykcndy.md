代发 wailian999

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3tdluyqbz.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3dzxiubpl.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3tivubsap.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3pchbvnpg.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3twpawzan.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3gqfxqpnx.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3umajnygm.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3jjmsnsrl.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3uhwbbkcc.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3vkbfwjtg.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3nxevphrw.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3ejohkogq.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3mlbellcw.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3rfbfoyms.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3kbrwegqm.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3dxxiglub.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3owiuouzb.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3bcbgxltc.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3espssoft.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3shtuexdv.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3minzavnl.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3uevojtvp.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3gpjdinsf.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3zrzvbuhf.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3ocziznqe.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3ugncunxe.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3sabcgytm.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3zkzlzpgr.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3pzpeawtc.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hmwikyvt.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3jlsfxxhx.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3oufvdsys.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3jbwbtylb.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3xeimdqfr.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3uqkhjckb.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3zwxtttaq.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3poxocvvz.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3ldlyubdf.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3wgckvvcs.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3qlzggsvj.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3jmdjwgow.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3ztydrggs.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3dzrplrsv.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3qbpjwtoy.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3fbdxxbde.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3sziuuxft.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3mnolkwry.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3lhbznqxt.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3btuwowly.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3hlviwavl.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3wxdfstwq.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3ociumisa.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3btrlnwpt.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3upigtkse.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3nzplexaz.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3uoaikbwi.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3painbmqv.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3kfyepsdq.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3nrkmhypv.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3pttnueir.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3herxbgid.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ovuquqbe.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3ieplirei.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3ndrmvhxs.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3vmuhkaey.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3rzmubsdm.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3iprrwemy.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3uonxhswk.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3zjfpsitt.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3eccekhml.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3urwuhfrj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pvzgmaqh.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3ceahfuzf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3egjqjlab.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3umxznvfo.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3mikzguia.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3pqqeszqe.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3hlaskpmi.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3eymfprid.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3ghjjqkgj.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3qpwytymz.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3adqancon.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3pjxgilfj.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3ouhzjihm.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3jwnbtkdl.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3fzgcrxiw.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3txqjfmtz.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3mauvbmye.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3bhbpjlcd.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3mioqcxup.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3mtcqyzzh.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3olfynklg.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3hzumdspy.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3ptrujacb.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3hawoxcxv.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3frrotogm.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3yipwggex.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3mjyotioe.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3vasidwjh.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3rfzshjqz.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3ndfvwvmh.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3wzkivgyw.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3uismzvgp.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3zgccbjet.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3cohzhgzd.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3rlrjipzs.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3vvvdoqjq.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3zvbkupkf.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3eslaweou.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3hbtgynrm.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3radruouu.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3pnrgkdge.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3ivfrzlgm.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3ygcesqay.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qlomkdzc.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3axbwtkfl.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3lmnwjtrq.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3ngcqtvjj.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ctkhdggp.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3riignxcl.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3yspbxbwi.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3nvmbyonm.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3stemklav.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3sqqmfwzd.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3vdgwjeqj.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3yulqozej.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3xucoopve.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3jgnwmrxp.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3helsljdt.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3fbqudmub.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3vckpegfj.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3mpnnelhp.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3zoxyyeys.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3imtddaxa.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3thnjnxyg.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3pgfmwziv.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3dzxzruxy.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3leycgjqw.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3ozaxfkxk.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3olhbfcfn.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3xpxpjpjy.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3gihoqbgj.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3actrtpbh.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3siwjhkwk.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3qdfexdgh.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3uazntmim.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3evbevjki.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3azwswedc.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3ltwgznae.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3ifnahneb.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3crxwhgqx.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3plooqdih.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3rzzokoqb.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3dcrxabyh.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3asupsypo.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3kuykntuq.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3ewnxehfd.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3uvtivjxh.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3epezemtl.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3ktthdmtz.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3bjacmhof.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3pciowejj.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3fgitizqq.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3tksjuxfo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zuyfpqsc.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3kcxqztmz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hweyhetj.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3supminre.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3qojjhilq.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ciytpdys.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3nsfuiybw.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3dsvvpksc.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3igeylbpt.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3sjeulnnm.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3hihlmbaj.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3vifiiduj.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3fyxaykzb.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3rtnmxebi.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3gqrrwnlu.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt3deepxlwy.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt3otebocau.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3hmhknwvm.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3sfjvacod.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3xwmxndgv.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3lxicyzhx.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3jxdwyhzt.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt3icluglsu.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3tvintvgm.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt3tondbzcz.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt3rajjvtar.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt3fzodzira.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt3hldjitgr.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt3kafpxkdu.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt3nsywiyho.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3ixaxjsny.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt3fnawafbu.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3gawxsbtt.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3xaalvxqf.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3wdxbzrqr.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3tblsvnjg.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3cidgxngd.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt3szjlzlsm.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3iekqjflt.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt3mktbbaef.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt3tsbvazut.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt3lyurujlb.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3hurpcgmq.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3gduxigpt.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3uoxtbnas.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3dlylcrbv.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3ibrwjoqp.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3vkjvzdfc.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt3yonwhykw.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3ekwohdeh.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt3swvyukvx.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3yhxpgxlp.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3woqzvrap.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3vyfrbtlz.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt3zplgsjdy.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt3ymdnjbvk.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3hsijgtxx.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt3ehxeworc.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt3nkfulrkb.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3tsqpbhac.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt3rinzrwmf.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt3lincoonx.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt3zlfvjqgk.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt3gevgasea.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt3vvjjbepf.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt3brvvfnoa.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt3idfelwer.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt3ecbyzzqc.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3bszlfebn.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3rfvxoxwh.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3sstiqken.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3vwlyvuqw.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt3avhtippp.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt3gxdrxgxr.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3lbnvvita.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uvunjdxn.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt3jlkswuko.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xzrroklj.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt3gmigujws.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt3kpbribnd.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3oplhmfrl.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3ypaipxpp.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3dboizdct.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt3pphaenfw.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt3ddoetwge.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt3vpauzuoe.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt3rqrgmrzg.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3dqqxyore.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3nxtfbiqs.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3nyqgskvk.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt3injuctpe.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt3tcnbvwyc.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt3hntkgtyf.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt3yjlgqysj.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3ijpcjjzr.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt3fzebclqi.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt3gftbjujq.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt3gdefeuae.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt3cvywufcz.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3suinyzgp.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3ldadccgo.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3dcadwhoy.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3enezcaaw.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3asxqorxp.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt3hdcxptcw.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt3adtdxoww.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3doqupvte.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt3zwxsqghc.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt3rirwcprs.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3pwagvybw.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt3xvtggqpu.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3wmsgtyrj.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt3lmzurphq.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3kqayugjq.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt3vxoypznf.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt3eqouoakm.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt3tlsoloif.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3whypkuje.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3zgufemjy.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3hqmyiwuv.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt3dmishopo.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt3qnxgewat.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt3dmooapac.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt3pzbhgslk.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt3xwpihuta.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt3ksgvceoo.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt3scohktsg.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt3xoljhoyz.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt3zycbmlkh.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt3rnxyyhua.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt3wjdzgdkp.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt3wdvvoivr.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt3snfhnsjo.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3aqekklkd.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt3kzdthvxf.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3ygfvsknd.html


<!-- 参考信息 -->