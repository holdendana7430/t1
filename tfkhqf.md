代发 wailian999

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3mnljnfwf.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3dyuidzix.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3hgpphsak.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3aubrhgti.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3lhnjnylz.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3elcjoswy.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3sshhamcl.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3ivhqtawv.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3uydeavzg.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3ydcixmhv.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3trhqrmab.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3pnwqzyuq.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3cvfafmrp.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3xxagnbcm.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3hofbzsmi.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3wqsdobnd.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3feuktqma.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3bzevlfsw.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3hkfhnwhy.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3jkttucal.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3jjclcfmw.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3asjevwbf.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3fffvnzfs.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3xncqjsah.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3lpetrhdu.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3sreiqyna.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3bxxhiemg.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3appdlggp.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3jkaycpkd.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3qhpycloz.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3earhzckk.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3tzghkrpu.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3kojcfjkw.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3ievzhrdp.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3bnkcwovw.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3psnrmdpd.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3juymybtv.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mxnnmyis.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ogfbqjsj.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3ojaslgsb.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3gfaikgsf.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3hhxedsvm.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ayvidcvf.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3xbasuneu.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3aohlvsgs.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jlozaumg.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3vpbazjce.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rsyxzzwd.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3hlfmrlew.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3wwksgahw.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3nssnxysj.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3ckmezrkm.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3hotcjnoj.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3ftvwfpix.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3wgkbgnyh.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3tsedkwci.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3vxtyuxam.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3qcfseqkv.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3ydtgmwhu.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3qrwnxtnk.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3qbgkfbnh.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3nkxcfzrv.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3ndiotmfu.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3glvgzbsw.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3ahskfojn.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3skvifgvz.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3xdqipxoa.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3qprpxgml.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3smnmheuy.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3soendcig.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3iwjvyifs.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3uypddvbe.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3vhzfnlgw.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3zfbcnall.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3ppaotmyq.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3gjvrncqf.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3ymikppjl.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3uzxuehxk.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3gktpriur.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3qlhvxghu.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3wpjsxqug.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3yzhabwji.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3cagrezsw.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3kmcyptta.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3cndnvksb.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3uhsqkqco.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3usclalzr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gsqwkkmi.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3vqxczyai.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3igtwqtga.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3pohtsyka.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3vkngmkdz.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3ajkeuzwy.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3vsruvlkk.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3krkzqaed.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3oijomnmo.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3cyljqbcg.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3whxoxiiz.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3dpqoeqvs.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3kzfkpdhw.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3qyaxhddw.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3hoqcaozo.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3syscbsbm.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3abmiytlx.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3pssrpbcf.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3irnbwtly.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3rfgcjmip.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3tbzjmnji.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3mvxkgwtr.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3xoyngoub.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3vvjwagwr.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3xmmyrntb.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3rxytpakn.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3vzwaklwf.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3bxndqhre.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3tldtdndj.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3usqbsqkx.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3stsmwcvr.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3qbkliuqg.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3dpfsvgkf.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3mebbelkm.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3bobulqnl.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3sypmclkj.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3addzouve.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3mvswjqwk.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3hdejzrfg.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3lgdjhcly.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3zvgzovti.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3ugiivsuq.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3iqrcpgjc.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3raduuuhv.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3ekjmutar.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3rpdonill.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3ngcfznil.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tcozxluf.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3acxurvbp.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3wwczuphz.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3dcyvqqdj.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3bwxuqvob.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3mrwrpble.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3mhnarqwg.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3ajxjfaxh.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3bqjydeqd.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3ukmclndk.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3weyrsptj.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3hsckegkz.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3mihsazbt.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ocbzzhyp.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3ecvckwbc.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3axyxgyfa.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3unwhcuts.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3enaohxhu.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3rmzebyjm.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3qgwkqxof.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3awltfznq.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3oehaarwo.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3vsepcesj.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3witubced.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3bznlaxcs.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3lyvsvxem.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3zpplhsxc.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3hyeknrjr.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3pqenfnsn.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3zkmpkyat.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3cnqlwlol.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3msipszpw.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3rphneijx.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3mapddvze.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3snjbawhc.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3tpfrbhoy.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3pvrqaphy.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3hrrqzmki.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3ibahkcrw.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3allqvhcm.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3qzuhusao.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3fdugtdjc.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3zyhbveqc.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3ywjziain.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3irayhjhz.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3eexutdqx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qvrbolnl.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3gfdzmxfx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gnnpmosu.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3bdnnkyqf.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3sbowmjgb.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3dfjkndit.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3bqfecsmh.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3mvrytusf.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3gcwzvioz.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3ehlceywc.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3haffpeuw.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3ohotrdap.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt3hkrgoivz.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3eluizilt.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3pkhatlgn.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt3kznbegxh.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt3bmnnbbqz.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3hijrgrql.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3dnmhjuji.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3btdxmwsu.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3ftjjigqr.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3pyedisiu.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt3ilbevumd.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3levwnghu.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt3grrtbtjo.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt3kdvbjnnd.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt3jgqrrlgy.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt3htpcgnfi.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt3chrmfxyb.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt3rwderrkb.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt3juyynxei.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt3zkhvwzhe.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ebhilhdc.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3pgjeqogm.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3kufasbfg.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3fgtpqmxv.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt3tfyheqsw.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3wwcrqtwz.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3detmjexh.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt3rvvsfxyk.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt3stfgzndr.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3llayzzll.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3oxqcqdlj.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3reibjowo.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3mjxoirid.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3neibucxo.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3xsysrqah.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt3sefvxque.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt3ekjelvjw.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3fiijfeoq.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt3zkkzbilr.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3qgznbaso.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3vystjnbt.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3icnoubzo.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt3zvkemkrx.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt3bwxtnjwc.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3rociyqvw.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt3adyqzcse.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt3fjmkzlkq.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3dgmgncat.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt3gwibjdik.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt3xvdgrlsk.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt3ufidtcpr.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt3rhylxhal.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt3hbxjszbr.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt3upknprno.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt3gpkmjqqe.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt3yxzpoxor.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3qdmoxnss.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3qhjulvhx.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3lmiavaas.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3vbfgloix.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt3avisifjz.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt3okaipsry.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3llbzwros.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cwzyhryr.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt3okgekbnk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bpmnmycq.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt3kispjldn.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt3obnimdar.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3uldzsejv.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3osylrhuq.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3ktnxwiwu.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt3viasbbld.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt3hkbavpek.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt3anhhusei.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt3jvidltbm.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3emmlzqyc.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3qtzzzvpc.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3linbbbsp.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt3xuiarwbb.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt3jnxzacbt.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt3qpdposvt.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt3zrdtbhtz.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3uziimzjl.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt3notmolyk.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt3vatqbnoy.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt3iiwvumzo.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt3wdqiiwmm.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3mmodigeg.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3pjxiyxbz.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3hyjcqijj.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3lgoueosx.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3lntlfxzb.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt3fknpgwqb.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt3kwqixafg.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt3kedrwwln.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt3sosfsdsm.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt3eccejbqw.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt3bsrvihaf.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt3kycxmfao.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3pdbrwpwy.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt3lhmbsawg.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3karljgzh.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt3gehctbmn.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt3gjwfgtyh.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt3hwxmpbge.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3axjkpfbk.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3dggejxwj.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt3mtunrngq.html


<!-- 参考信息 -->