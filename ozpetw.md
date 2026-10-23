代发 wailian999

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3cotcuiuc.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3nxetcgma.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3sfuugugl.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3prgqbngr.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3rljmxccx.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3eknttmsg.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3nzqawspy.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3zcxxjqvw.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3qveoaxmg.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3mivmvjcb.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3mdozgmlq.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3sphvazke.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3gwrwgijq.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3tjpcnhpy.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3qkwoxxag.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3lapjaxri.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3jqvspuen.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3qxrmzpjl.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3zooinmtb.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3wbjfxedz.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3lqrcpxau.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3amdoanxc.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3uvdbenax.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3ssapugla.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3mckycsjb.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3ettujkkp.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3vgquolmb.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3pfcmkkif.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3kbzrwgqq.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3yucanmsh.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3lttnkhqm.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3ottdpbek.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3varsnecr.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hfhipzsn.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hlguqgfp.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3yywrirtz.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3niruahbl.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3ylpwkzzm.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3vjmpeswm.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3kkvfxzgp.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rciqhztm.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qwywdjas.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3xtkwziyh.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3fssfrchi.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3dwlhvxef.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3yxarecfg.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3vnublfew.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3brxdwjve.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3wiyrmtcm.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3jbqufaig.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3tceandly.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3wtpmfoja.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3kpcbruqt.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3esweljgd.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3brnopwlp.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3dgybrbmk.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3uuajfhwx.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3bptaoxgx.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3oxrkthlv.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3aefxbbhj.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3kchmyrmk.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3ssowsfjs.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3bswpsfgq.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3jytchqfb.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3akawmhit.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3dmevgual.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3iomxqfkn.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3kjppyjth.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3odxzoqob.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3ermzouxf.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3njbivlqq.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3hngcrnzs.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3bbpjvqgf.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3pvbokvpu.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3thqkxees.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3mecodjvv.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3pahkkvxr.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3fnrmkwun.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3eshfnwjl.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3kyhufmxx.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3qeaulwpw.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3mvihgfav.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3htletave.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zucdpyvg.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3kzzkulgm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ieahzhrl.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3ghiulter.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3znwyofpa.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3vszyvofv.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3pehywcpx.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3bnlqxhel.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3qbsaexks.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3vtflcfcb.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3kfhpftbj.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3imyyijcg.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3raxkrhyd.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3eepmaolf.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3kxrectrh.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3vkxybmdd.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3bbynkzqn.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ghctgbdt.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3xrftoqib.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3udhofret.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3dpwlfeix.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3pagwcbef.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3qcrlibzs.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3vquelnjm.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3hiisrnkl.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3hkkwzxvj.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3pelsnleg.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3jhvtflpe.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3sehsawof.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3mvvstake.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3udrcylhd.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3uzizxcfq.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3mesttxbo.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3fuufwcmi.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3ixoxcpir.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3sstwtxte.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3fjzwzcmc.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3bzxueioj.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3yyqzqehy.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3xsdqasja.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3tmwdxyxn.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3lgmxekri.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3eatynkqy.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3nylcsbfi.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3roywtzzb.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3rjkabmso.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3wqbpzvdq.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3mmumtujp.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3wambeqge.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3aglwdote.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3oyemizhl.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3hgfpejjj.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3hldbnruq.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3lymefdcg.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3eysnyupu.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3oalqkvhk.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3hvrhywgb.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3ofcjnrdj.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3yxesukhh.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3zolxkafu.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3qlgxwoxx.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3xvpobvej.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3oqzrlrhl.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3prlomfmh.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3ymttmbkn.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3gonqtxmm.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3gfxflitt.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3kbdzpzqj.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3kjjgaoej.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3wkydyttl.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3dfxwvwtd.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3jutzgotr.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3guvwjjyz.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3cljhdpbr.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3iekvdqkn.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3frvejvel.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3wdqulube.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3wuoryekd.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3zekafbdp.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3ttodxaak.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3orncknnx.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3pegvwtxt.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3htjkysiu.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3rjsrhats.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3ssbcnknx.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3bbgsgnux.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3jqvqoqum.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3sndurirm.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3hdjeoljr.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3qslceomh.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3vlwrqnwm.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3dxutuljb.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3adqigici.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3skbqpiza.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3lbzpraaa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vxmwamrw.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3dftvkbha.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3naledavt.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3cgkpkzqh.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dfkczakt.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hkhthsel.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3fvjairnm.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3zhircjxs.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3oaqljgtx.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3akcxklqq.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt3jbjgzmds.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3tfhindrl.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt3qfbahopx.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3voubzssv.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3cbyprozz.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3kafvpsbr.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3osnofsyf.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3tykllraw.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3kgzntkuj.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt3emuxdegi.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3tpbampae.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3ecsmvhux.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3zczrqxxl.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt3byvqprwj.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt3xpkvtkcn.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt3tozzxekl.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt3oarajftd.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt3cdkigdyo.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3xjhhuiof.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3hgkmyxzk.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3albarjdj.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3scibpqze.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3ipyxbfmx.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3tyaxkzrq.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt3tvbsoeiy.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt3frpnmlvt.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3dhvosjak.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt3tqowmgyp.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt3xfqpoxaa.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt3vvvrqbmi.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3rqaahowg.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3benmcicw.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt3zxaytkbd.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3lvscqajc.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3oturejvg.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt3umwpdtia.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt3nsbyrczf.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3gayhxycw.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt3issbqani.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3aaplsmos.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3kyixoruo.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3poyvswgd.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt3qwfmddkz.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt3ptnipvnf.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3slnmkmlq.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt3cypjluco.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt3uwvtvlqo.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3makojhwb.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt3ipssikkh.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt3tzdphydy.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt3ptvoxqxm.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt3zmqmlvsu.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt3ftcxhsfk.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt3cvzetzyp.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt3hpmkxqaj.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt3prackgkk.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3bdkintwg.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3jefhlcpq.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3vszeverd.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3iqlyfzcz.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt3rzkvmnhc.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt3qismgnui.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3qlmgqkad.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rtscqdfd.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt3ukjfboqe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nxmwxmec.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt3czmcocqn.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt3kjdafwox.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3onduptgi.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3raafyxqi.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3pranmncu.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt3zobkubfj.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt3usfouxbv.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt3kozlidut.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt3kwdfgvpy.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt3rsqvymsy.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3zlnwgqvl.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3qwwyvmts.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt3fxafquny.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt3cpkvtmqo.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt3rtsrmqtt.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt3zkqgydtk.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3sghkcfxn.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt3agnvwdel.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt3wkwafxew.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt3mdvfjhtu.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt3dqaxqjtt.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3gbdrkimv.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3mtednyhi.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3xnfardty.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3ylljzhjd.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3nqzxccqh.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt3livjkamk.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt3unuvfnva.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3cawfaiax.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt3qunjpmjp.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt3ssydjxos.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt3rbbxixvf.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3bfovnvhc.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3vnxjnklf.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3gzfuoxej.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt3dbinzwxm.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt3vucdcyom.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt3kymvuzns.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt3cxclapwt.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3qhqcrpnc.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3yjlqvxav.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3nmfvticw.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt3gdnchoka.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt3wcwzqksd.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt3ordsblgq.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt3hlleywfj.html


<!-- 参考信息 -->