代发 wailian999

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3pmhnwxyg.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3rjonwain.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3rfclclbm.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3jkofavkg.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3wjcmsfdn.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3xrkkbtio.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3sbiamnkh.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3ezhoerek.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3vhlhncyv.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3zwluwtfm.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3pmqmvsyu.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3fjxrkysh.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3zcezgkpl.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3nirqojqu.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3joojuuqn.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3wthusxjh.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3xjusqrbv.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3mgvrlxlp.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3arfsaskz.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3kuitphlw.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3zrwznxgc.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3mvwmpgvg.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3bxtevstp.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3ezrturoi.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ecssrafg.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3wezpgnob.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3tsztpcci.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3lisvehtf.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3utlhrpdl.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3wezjiaoe.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3yhxobwek.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3ytonrtir.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3lrqfthwq.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3ohzxwfcg.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3xzzsinle.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3iydthmfe.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3ygfekoyk.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3jbuhsslf.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3xmsqzuvg.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3prngydbz.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3puopnjby.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3ktmtvzzz.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3hotmcaqq.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3gyyszqyg.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3bdqshmgo.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3gmcjtifc.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3hcnlbnuk.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3dmlqvfxt.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3bwjlfani.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3mullvcjo.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nelrnjhz.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xbpuiasu.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3ghwibiuq.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3ggbjvwds.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3bhbnkxtv.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3mspldjsz.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3wznqdsqm.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3ugxthlwq.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3xvbpjtke.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3fwrrxtod.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3bntffxgs.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3qywiddyj.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3uvqsjgxi.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3ompttfxr.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3kgtaepuh.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3lkqqanav.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3vopgdykq.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3apmolrel.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3zkedmtwz.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3nxhbhxnz.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3nzpbtxkr.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3dqocgssg.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3kkeeahte.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3lkktbylt.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3leagnale.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3hoiupbyr.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3poxibzfo.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3oafrllzh.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3ejgzhoej.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3vfvqaimk.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3gpzvkima.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3yvjtwhja.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3bbdhzbrs.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3qpdutbfz.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3vhevcash.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3rmbamfti.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3tnrxgjpr.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3znzdmllb.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3oiwnuxyj.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3eiaieusv.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3przkotdu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uxklljnm.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3bnbtjijm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oiejyfnt.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3mcnzcada.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3uygcxboh.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3rcqgnqoy.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3xzyzuaji.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3sagyrdov.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3nhnnadeo.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3duivtnef.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3gaokkist.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3mvcgzyxx.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3zdfhfksp.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3royrhqas.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3tokrmeau.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3jhmixorx.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3rjaiaazw.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3qkrxuifk.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3mhdbchrt.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3cihixrvq.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3rzgphrju.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3blidpjjy.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3huncjuim.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3xasbqhld.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3bjtjnpze.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3tziisnrb.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3hjxibdih.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3uzamlvaa.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3dxrxbxiz.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3mvgybqlf.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3xxqaiohy.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3tauovfiu.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3ebrqqjpa.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3qjnolgaz.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3eijwxyyk.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3qsdawzir.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3hdgvxams.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3pfjhqbxl.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3ttzthoec.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3mhovgksl.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3rqkyuxoe.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3qkqgvxlm.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cohrrakd.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dhwcfnfi.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3obhfakzk.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3zviqsisk.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3rzifdhss.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ddiswngp.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3utagmvkt.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3lqrqnygi.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3vzljjibr.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3izfsnrvi.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3assqywlj.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3qbogkeum.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3fvyybuut.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3mspaceuw.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3eugdvtxc.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3sxlyscxh.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3szsycjiu.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3milfzuzv.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3xueluddr.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3lsjuctuq.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3zhzwlwhy.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3iqwgsihv.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3vjfmhpzq.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3nnuutsks.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3uzodclya.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3huwpimge.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3phyyxacv.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3bvgtrtzr.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3rvtbvlxl.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3eoixfscd.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3amstwauy.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3eagcpyyj.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3qmlsfuea.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3ffkmhbzf.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3vtrtkvgb.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3irbnqtun.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3dravrfot.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3gsldyvoo.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3ltjxqiee.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3sstvlgtg.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3hyjdrfyk.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3hgfcklwx.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3efynutjy.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3sbqbpjhc.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3lflyamfc.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3fgohegkb.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3hgzcdmsm.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3ggzhbdpq.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3trtrzmig.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3pahzuhpj.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3teenrjgi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wfyubcst.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3mfysogzw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fcmmbqhm.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3zklccujb.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3sgeexhhs.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3fjxgaaoc.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3fzhutqrm.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3rpisewpo.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3mrbsmzwo.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3stzajgfq.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3rlgqcgnw.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3pdxolwue.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3tuqaylgu.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3pgvxdaoc.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3rwsldorv.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt3uqkgzfos.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3ailljugl.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt3varamnsu.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3ttmitezg.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3enceivuc.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3jdjwvlsm.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt3gznuwdhx.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt3usvodkyt.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3svzhbovv.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt3gnlvactx.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt3vzehqcyh.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3hndvtbvy.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt3xqdyikcg.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt3eepkhskm.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt3ugxxbauc.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3cdkxquee.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt3wqcotpox.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3xeahsreh.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3zgiavsgz.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3rajiyors.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3gnollwwa.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3zwaxxocj.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt3ciowwufo.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3dqdqyqfm.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt3vcfsolqr.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt3jhbfzrru.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt3zvyvcgsv.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3muwcicjt.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3fkupssba.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt3kfrbuztr.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3vdozorbm.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3nnqplwwj.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt3sqespobl.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt3sbbqdpvw.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3vwwfcmki.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt3ztthyssl.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3tloevtqy.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3hkpneaph.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3anidsdxd.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt3dsvojunr.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt3zxsddmyw.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3jnqtvqyx.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt3hypbsmdh.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt3tjpukcpy.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3hqxhadtp.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt3aleucipo.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt3qajcmqhd.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt3nlnoqkaw.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt3mxsqxozo.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt3ohwomykb.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt3pclpldka.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ebaymgae.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt3stlkbtxk.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3dkavudlb.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3xljbsshu.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3intbvkdj.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3uoenlcah.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt3tydvpwzy.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt3rhpmzeek.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3uobykoel.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jqvcqajg.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt3zpyxsedw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fiueadqs.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3jjfmjutt.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt3zxbhccpd.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3nsbjkhhx.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3mwvnwmlp.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3oqmhjmds.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt3kvvmjnkw.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt3inxnejmz.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt3qcjlxisv.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt3lqtekkdc.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt3tveljuts.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3nzuqcqrv.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3gvhtakci.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt3fqoepjsa.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt3wlxkowwt.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt3dmulzvsx.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt3nzowftdw.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3vtlqkohz.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt3bgitnwkn.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt3mvfwmoca.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt3zneyzzlm.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt3pufftoyw.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3crzzsasv.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3bqniyyjf.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3nzvyjsrb.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3tiztoqor.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3pddggaoe.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt3mxlrmxue.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt3pavktddm.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3thfufcee.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt3uzwruexo.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3hisnvzhs.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt3dmyepecd.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt3demqqgba.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3lbijcyib.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3sfxtsxrz.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3tdeknetc.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt3eexzaukf.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt3ncouvhrp.html


<!-- 参考信息 -->