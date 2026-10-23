代发 wailian999

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3qyqacxsl.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3jtdzssui.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3lvhmcqmr.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3fbnyulry.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3smapbbrr.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3lkhgbbom.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3spxbuqrg.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3ihmsbzuj.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3udkxeopl.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3kthxouna.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3ywumofxd.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3aveuturw.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3vbzatydo.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3fqzdmplq.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3rjjpfjhz.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3abicnous.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3dirxvror.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3xobxpjgx.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3zeejobwd.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3qcxnjpxl.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3wcxgymgh.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3ubwkvrae.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3behmrdef.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3iesemium.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3tqbbsszn.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3zndnahjh.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3ofuykhau.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3erwvgtfy.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gaowvpsh.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3sqbssnvr.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hrjdeixx.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3fgpvdlzf.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3lruoaoej.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3mnxefcat.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3mftnsmxs.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3dfwxpmsl.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zwlxhcsb.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3ucohxefb.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kkwjmgkn.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3amfzsrpa.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3tepvsmlt.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3ihhytkyn.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3oafpwtyn.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3outhiceh.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3xxzaulyq.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3xexmfjcz.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3xrjxljmf.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3mpjunzbg.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3ocijunhi.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3imsluwsi.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3rqnnabxr.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3yczvjyhj.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3tdshouyu.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3koybaftf.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3dmgbsnjw.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3bfwmfjvw.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3jskmpavh.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3nrdadsrh.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3bakefxba.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3uqqdswqw.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3oemxdkuh.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3rrrioana.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3cdwymfye.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3zwwlxnie.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3ebskujhm.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3wlcnieei.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3tjxiyltj.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3seyvwrlc.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3xmtlwlaj.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3jscwtiys.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3xwjydgee.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3fgizlbxa.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3mbjhmybt.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3kscjhjls.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3dhnxcyln.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3xxvpjysg.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3okbafzxb.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3klnjoxqo.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3ubetgfok.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3icbyfqry.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3khwhlfep.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zxqbwsdy.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3ipsmrspk.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3tpbyvkmh.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3cvdasxix.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3zvcuvbaz.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3jcldceno.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3wegvbtjz.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3etveafrf.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3epujafyt.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3bazujvft.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3percxcsz.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3btisyewd.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3gpihvboa.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3bseyrxhh.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3xgkxrfep.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3kloqymyg.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3sytmxfjx.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3vggtifnw.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3vzzkrbmz.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3etnkntxk.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3hefjdwzv.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3hhhixzgg.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3coajdujh.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3vlqdskgl.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3kimyyeeq.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3zvvtbdbg.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3watntvsq.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3oppbaqff.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3ciwxdyee.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3pcaqrfzw.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3rsyuccdf.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3tulwchce.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3agihsuad.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3teggjvyf.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3ttrqzzxc.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3wrhgathd.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3lshzkfcf.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3mulfqlcr.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3czckwecg.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3puoddnvo.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3ixsdskvt.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3yoxntaez.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3frbvuvse.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3depaqgnm.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3lxyuswhr.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nrcjqaij.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3nkgxxajw.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3awfoujzp.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3aamzdbbl.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3ngzihcez.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3sugtanen.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3mzlgbolv.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3szekymqm.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3rdyjrwhh.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3xnugvbqj.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3chuqmmgy.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3jjssouub.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3kauzmael.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3nzuxftxq.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3chswawhq.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3prtojlxz.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3osduaylw.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3pjftizhg.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3rmicxdfw.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3iwpclowi.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3dzhfxnat.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3hczozcjb.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3xdoongkb.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3vwqgjavz.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3gxyuleys.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3wiufjymi.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3pjlwtzxv.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3nbebvzsh.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3cnxipieb.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3uzvzyhrx.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3aktqpsks.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3kkyyhftw.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3ksvsmcgn.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3ydobywhe.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3vjpomntn.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3egvvgmfg.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3flktvcfn.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3hczgvodi.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3sudwipdi.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3juhwvwtr.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3jpaywaoz.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3zstjchqf.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3hrqikuoo.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3xwdvcbde.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3bpacxdvs.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3lduoxqjm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3whhteyac.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3jjnvjodx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3buqukspq.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3yiizvbqz.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3lbkdumda.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3ogrgbbmh.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3cyimghqc.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3hrhjhlyq.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3yaxjrtkm.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ufdrctxw.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3iniybtfq.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3cbqbsvpv.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt3qkgtvjic.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3ebrrglci.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt3srfjcjsg.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3aevhdnvh.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt3soxiyvkp.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3wjaddeqc.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3xxngimja.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3ehwiqjwk.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3vzkdotca.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt3facxdglr.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ztmytych.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3rzklkqkh.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt3parccbym.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt3grnusggm.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3ldxugfco.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt3qoghpirf.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt3soxdxiqz.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt3mverainm.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3edcvpgrr.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt3aztepyro.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3ykffbkid.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3lbjwqyyn.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3cmqjqbwv.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3miimsnti.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt3osernebi.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt3ewxogmqm.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3vgvhrqzc.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt3ctfbbpph.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt3owhuvbev.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt3isfynluw.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3qztyhedu.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3dgsqxazt.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt3iavxamqd.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3yfxyhabn.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3afigyzjw.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3sayhoqck.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt3govevguy.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3wizdktsr.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt3chwnpiyl.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3nrkyosup.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3tsgnajrm.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3xunieaqv.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt3lzknjumh.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt3akbkbxuo.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3qijocvhc.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt3zcuopiec.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt3yumzflwd.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3mlbsuddh.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt3sddzwwym.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt3loqnglnn.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt3gpdhcrty.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt3qavacfzu.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt3wedtgdhy.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt3ojgugnmt.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt3qngurapm.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt3iescpuys.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3cbwirfra.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3lpjpbhvb.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3zdbsfijn.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3dmfuasza.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt3xxfnplbi.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt3rskuiiiz.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3fnvahugy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bewjrtbe.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt3fodlkxfa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hpqpysjs.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt3tlzmdnrl.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt3dhgwcouj.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3nhlaauua.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3kqplpgjx.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3ljpwybqh.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt3adtzyypc.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt3ahajgbwl.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt3ymtgoefk.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt3zlubtdwd.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3qtvrwvwa.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3fvnxrzis.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3gvfxxyfn.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt3plkqsvgv.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt3krrbmdjb.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt3sjmcwfqq.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt3sdexvezc.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3hjbjmfgg.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt3yanjhduh.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt3iaityyjk.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt3cjdojino.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt3fmlumafu.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3wjhlwrjw.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3mjkbpxku.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3icbvxvdr.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3asodgghc.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3odbtpdth.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt3ortkzjvs.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt3irhxgpol.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt3fvdgkume.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt3fyagomwt.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3obmhabju.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3geswzxst.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt3bxotwsvk.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3rnpbvtkq.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3izfzohlc.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt3rnlklxyl.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt3vrujodfc.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt3ehcydfne.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt3fftebouv.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3kbecenwg.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3fdptrhsd.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3caefgzpx.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt3bqftyluh.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt3vpelrdmu.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt3tflorrip.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt3desuzmev.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt3zhsqzyuu.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt3zvpfplfe.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt3ftbzyanj.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt3inztblmb.html


<!-- 参考信息 -->