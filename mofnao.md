代发 wailian999

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2mpvyuslg.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2jiuqyklr.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2mwyrolnb.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2rdfzrakd.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2gsfrjluy.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2atapwkqd.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2lvkkylxy.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2qernctyg.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2xkftffob.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2iwbwocuv.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2nfvqiayo.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2ibhvztvz.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2zbuuzzgr.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2bgdcpbnj.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2qwdothmv.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2pujuqlit.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2xmmmmysz.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2xsfnnzas.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2kofhnuzl.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2jbvegwck.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2xpaiaxum.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2assbebzv.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2acsytuhk.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2gveuitqf.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2rshrvbjr.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2uccrkuge.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2bmmodaim.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2zkkrzjvu.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gkwpawyv.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2lpzpfgly.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rhicsuhj.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2kxaxksgp.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2noiizshl.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2glufighz.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2krlfvvlm.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2akvjvwri.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2iwseildh.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2daneimvb.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2nftgcmar.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qtfriale.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2wooqyguw.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2dzjfrlqz.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2suovpfzc.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2plhdclfd.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2tfpnyzoo.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2aywvjaas.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2orvxuwio.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2xhxrwkby.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2hraoyelu.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2stcmfkru.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2prfmlltx.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2kksdltod.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2iufueuea.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2oaffeest.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2mzixcxmp.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2ebnrtmai.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2mfxqkkdu.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2edplacsh.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2eqkvrzvh.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2ucjqbhrw.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2vnjanwkt.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2jlrqcmvq.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2kwqhgcbg.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2vxjomkho.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2patjwloq.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2uyqjrrmh.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2usopvjae.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2vzxzrqpu.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2oevsgtoo.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2zwfqilcc.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2ffnwonwl.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2vyplshgr.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2cotqjmzv.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2hbmxerbe.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2evxlgweq.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2dfwxbesa.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2tblekpuz.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2rxhqhwtq.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2nvpkuozf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sfkmvxlq.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2sdzjqssb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mdacogvu.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2seymesid.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2afpzhrrg.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2cqxyoubz.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2kjmenxzx.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2gkhsdrkb.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2aiokjzqq.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2auaxelez.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2hnafzeat.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2izgiryie.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2gxcaohzh.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2pofxdabl.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ieuzvdck.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2nvhrckuo.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2pvdfoguh.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2hncabcpr.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2hjgzlnyq.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2jckeejue.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2yxrtklxv.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2qifjfshz.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2fhogrujr.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2gvwtqsgl.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2snrlqigi.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2rhlhripe.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2xfrguvhr.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2zwpwuxkr.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2navcpfhm.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2abqjscjg.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2mmjdelmr.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2ufmqeejb.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2lxxkjgcd.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2xnmwvoak.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2aufvkoaf.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2lsxfukws.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2cadbfosb.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2hskzetrg.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2hyakwugs.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2bkthlyjb.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2prsvkybm.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2lubautxy.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2jlyfwuhh.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cmiftuaa.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2pqdwygwv.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2rjefnfnd.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2vrcgqucx.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2uvkszjam.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2rejnvcsb.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2evlmovww.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2qxrucria.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2egekgrlx.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2ojldogdg.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2tsfyzxrw.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2dpdkzhrs.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2icwtyeih.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2irrzqxqa.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2gwqbblnk.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2vpddflfk.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2rzboahjo.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2pumlxcki.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2nnhxmdyi.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2wyygdwfl.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2yioongua.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2kuuartrl.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2ziljraqb.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2xznlpitp.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2xfjyvjqf.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2tczbaeqw.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2xaxatpnt.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2efnlugaa.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2mpvzgkxo.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2msgbpvzm.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2qhiifojw.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2djbomjos.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2fcexrljs.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2bjuygnak.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2jykxzkey.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2soiqxqgq.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2zkzmcuxs.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2tuqojckz.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2foyqrphh.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2qkxkjcqq.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2msqfcuuh.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2jjxoukis.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2nsgirezq.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2xohdtldf.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2sgiadkac.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2mqezghwk.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2detdymae.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2brucexjv.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2phyfyzeu.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2vikgsrqd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wxrwtoxt.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2xlckzwfo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yocogasc.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2mdgrxvbf.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2mwlkqnyr.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2inmhlwzc.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2mglmxulf.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2nwwbzrho.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2hwebzzyt.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dxybbwpy.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2qdzaefvi.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2ydlaaqua.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2bqatfafa.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2osaklqvy.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2iqhnnnro.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2chnstiqe.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2mvjtdmuu.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2erjvynju.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2zueenlig.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2shbvvvim.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2fsjtwzvq.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2ikoivjbq.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2emjlhzai.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2qgrbqqoe.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2lvvsigih.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2ymaetdzh.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2bfqdwzsx.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2vscbegok.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2aqadjujm.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2pfvvkyrn.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2wccgdmhy.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2fvejedjc.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2swypbyhw.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2amtotvbg.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2zbdqwzcp.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2ttlgktdr.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2qokkqtrl.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2twyhaomu.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2wsfhziss.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt2vvxwxbxw.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt2mpitoboh.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt2ddmnmims.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2cfziepjt.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2spfeivqd.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2lqhbrcty.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2xsxnjdnc.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2vetdbrdn.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt2knroyhgt.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt2amnaofho.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2btpijzrj.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt2zqfuvyua.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2fdasoant.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2dvdwdjee.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2etfuirsk.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt2wlfzmbak.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt2yybdrjsc.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2jeilebgo.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt2vuniibtu.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt2vkuvrumv.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2siwowiii.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt2ushwfwep.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt2uwprrgde.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt2bgibfxuj.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt2tbmaksdv.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt2siynolno.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt2xvgidtpw.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt2gtqmxonp.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt2otnjjwsn.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2vbcbgekn.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2gvlkfwsg.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2hurtavna.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2iyccljwi.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt2ebyygnur.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt2utdoymox.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2ootwbhnr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qyxmecgh.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt2yevkakht.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xshvtoeu.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2kvdlypkg.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt2eyofqent.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2srranzde.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2qwqgaxwv.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2xkfgtxyp.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt2ajlrbjae.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt2gocexwtd.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt2godntgej.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt2oyttaomb.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt2wjomzruw.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2uvnoaunf.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2mgrugmxr.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt2fhwlgnha.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt2aikuviud.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt2wefljnbc.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt2vtspjfaq.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2ukvhhdmk.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt2wyhzgdgt.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt2bsspfutf.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt2gsbvkbls.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt2ticorqfq.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2oqzrtjyf.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2alcukkgm.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2vyhxswgm.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2vhuugmlw.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2qshkevfl.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt2yhvqjfly.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt2krftbydh.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2nephnxyy.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt2orkmngiu.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2ckrzweda.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt2vmoufhzv.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2aqvhnxqi.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt2qzvwtoth.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt2xgpgwkkg.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2lqcqdlxu.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt2xfyntyrl.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt2kgbnucgl.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt2gfrdlwza.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2vfqhbfus.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2qizplcqi.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt2yspotmla.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt2nzpkhkup.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt2ncfosroi.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt2szfybokj.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2tbyfzfyw.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt2jcdrorqb.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt2zlrmjega.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt2yyfcdgnj.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt2jmenqiej.html


<!-- 参考信息 -->