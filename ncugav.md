代发 wailian999

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3uzmffsvu.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ftjhjhfw.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3jyaueyuu.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3zvssrrqg.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3buynqtfe.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3tyqccmzi.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3gyyxjpyy.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3pwjlwhxh.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3rhppbxks.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3ayexxkhe.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3rihdfnjw.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3uzlaiuoq.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3pwhwuido.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3heholjfq.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3fgrxphbg.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3cfabqvlo.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3jrlympmo.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3dzhuxfhv.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3vejqnecd.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3ebwkcjcb.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3ipqxfdlx.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3zqactpwu.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3lmyaqrjn.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3amspxyvw.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3fzygswoi.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3blldwfcc.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3mtbhcxgm.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3tvfxocpd.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3kgouexkd.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3wkphhwdg.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3udxkslzg.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qbzlvxqj.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qzdnldtc.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kvecucqw.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ktzdobpe.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3vymgtqhk.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3wehxytte.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3mbxvlgyw.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3gbgkcpkl.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3hdksrgix.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xexlnbqm.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3udzubvht.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3usbpgbjk.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3igohhsfi.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3vraohmpr.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3mqtegbop.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3ttqznoak.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3wkjottne.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3swvkodzu.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3ofdnfkuf.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3oxgbxtmg.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3arwjjfiu.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3wihxthii.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3bxlzewzf.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3qszagmks.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3ovvdgohg.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3xuoaeyaj.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3jsovtams.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3eaguxqil.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3pvwebyqh.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3kevmznhl.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3sqeyaybk.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3merzjqte.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3zlsrcmdl.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3aqvcyjfi.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3xkfsxehk.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3borgfvst.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zpampcht.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3hzbpczhu.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3nrroutor.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3bslxqyqa.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3qstiqahl.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3dcrhwjmd.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3pbyyfwqz.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3izywrwnl.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3icsnttqg.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3aeasxlaj.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3wdyjnjls.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3csdmtlxc.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3soapshzp.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3vwutmita.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3hfcyhqzv.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3sgnsotwm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xasnjcfb.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3kjftlzxt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ofnqeaym.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3fhngppuo.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3pqwoukks.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3jjswublp.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3efhecjgl.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3blmiaoqd.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3rysesfaf.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3rihcshie.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3kzhuqxre.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3ieukebhn.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3opicppzq.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3wxelmvge.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3mvohgwdi.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3mnypkhxy.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3xlqirypn.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3okgwcfny.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3gobyztoq.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3cbiojacn.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3efnxneqb.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3wstsrhsr.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3cplxnfgr.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3dzxesbpy.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3rmolqjct.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3yuedezoa.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3wwcfdnpe.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3winknswz.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3uyktstmv.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3uratfvfa.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3noskcwch.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3gxrdkpzd.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3yofzuhlb.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3hbrmkubi.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3ftviwkqn.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3qwkodhxi.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3lgyisjuo.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3pgljoiie.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3miuulbpp.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3mafzfkgb.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3vtgycajl.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3huvnexqu.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wuynbpii.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3zetfllny.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3igdbmrsn.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3waaaaavw.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3bnflrqpk.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3dshsdfoj.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3spbzkvbr.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3kmlzlsrd.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3aejaaznt.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3zlhrmdpc.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3bjnfnvyc.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3fribllxs.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3vqdrlxts.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3uximcoxd.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3ggimrlwn.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3liwkwhyy.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3cqxqgrgf.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3vnqievfz.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3rnqcxmki.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3rrcrwpca.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3jcpjerfx.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3msesloyn.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3xoivzsoo.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3srurjpkr.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3algryoqa.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3ublfmdkz.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3rvnnbcip.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3qtaxofdc.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3jvrkuccu.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3hxsugldd.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3xawzpsac.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3uvtldrtk.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3iwmcqscj.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3bthdxlgx.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3zzpzmkxz.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3wyogisgm.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3lnygnhbx.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3wdsffxuo.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3jkrrvzdm.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3uqpeoyof.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3zryfydbr.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3rcgurltf.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3rmbqnfoo.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3opoxfweg.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3ijvpgjlr.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3pexpbnqx.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3bumpoazm.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3sujrucln.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3daubkcpg.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3wbkatnck.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3bfulfvab.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3udqwjrbf.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3wmbhsxzs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hzxrcxlk.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3esqqtmqv.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3nndhwvub.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3eaqnimco.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3zkcckvaj.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3vfbbiofg.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3xclhqrfc.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3cxmszfak.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3grevswco.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3abtwdonx.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt3yzwyjlok.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3rqcgcckk.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3fcfkqkhn.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt3vedfpete.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3vhblhmbm.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt3bcjrcsux.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3alzmnjco.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3wjixmttc.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3neurkpis.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3qsueixpi.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3tzdifcao.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3nihqkojw.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt3liucgqns.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt3vrewntcw.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt3glgnwsme.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt3fhlqlnai.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt3dzkynokd.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt3sxwsnjcm.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt3daoajqta.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt3cikimgeb.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3xnrdoxlc.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3qdohjhpm.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3jxriblsj.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3mabjkckz.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt3ohpvjkxh.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt3voxaeyik.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3kkftbcqj.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt3aljmwhtu.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt3ahmmvhzn.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3yjwjocou.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3ewvvuygz.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3nmwsxhmy.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt3duderzzv.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3itlkheon.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3dxpzzmbb.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3iwgwypqm.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt3fgfflqud.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3zymbzgpm.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt3oddqcohf.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3fszznygu.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3gnvqcikn.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3jklokmfh.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt3fqvqdiru.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt3jdcmjiyl.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3gvomgtti.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt3hyqnblxe.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt3wphrtlrr.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3gcgomhsx.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt3icsurkdl.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt3ryycqtfe.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt3fpkorxbz.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt3sxtrufhn.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt3hbjeunau.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt3zvjvtavu.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt3obaxmado.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt3ggbvmzou.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3gvftncvz.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3ccufettw.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3gcgjvcuu.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3zwztiuql.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt3nzweiois.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt3anzsufoi.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3uwfmiwil.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cfemahyn.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt3gdwecawz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vnnecwxq.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt3tdneeefk.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt3njwywvye.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3afwhhlyp.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3tyojemsh.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3deqfbfqj.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt3eglrduxg.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt3ctzextbb.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt3vxsitffd.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt3wqsbxbkf.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt3ndpaplmi.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3yqdkxjyp.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3uknfxnfu.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt3tltphelj.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt3txlpflrd.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt3zrmmeqrj.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt3ojrivjik.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3mrsnlvrs.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt3ugtdddto.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt3dhgsurdg.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt3jpfgcwuf.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt3ahfadpdw.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3btpyrdaj.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3shqipmae.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3wvugzrux.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3onhbihwe.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3tppmhebx.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt3annyewiy.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt3hrmeqajc.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt3wiewvpzx.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt3ygserjfz.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt3bvhvpecw.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt3wapuppxb.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt3brxfmfsc.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt3yfjcgivv.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt3gkuosmnj.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt3yoczwlla.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt3wxttspxe.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt3ariouhef.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt3vfprcdbf.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3uawqvbub.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3cxspotcv.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3lvidfwei.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt3eiegdyqv.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt3uxpyfpds.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt3xwxnncss.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt3xkkyvzov.html


<!-- 参考信息 -->