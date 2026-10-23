代发 wailian999

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3lwsboobj.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3hdcycpmz.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3smlkmthh.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3abmuwtvs.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3iawblibc.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3rxhmzscu.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3faepxzoi.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3njqoufxf.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3bknisgcr.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3iyjkpynr.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3qhkthrkj.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3uombiyym.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3ukvozsdd.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3xwpmsiuf.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3smzwmwvp.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3skvnrzfs.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3qhfnaapz.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3xojecwzk.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3yejiskax.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3vtsziffm.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3jwcncujh.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3qguzlpku.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3xlltnlkk.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3bttwhkei.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3hfbfaozc.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3mxngcqmh.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3bfbbquey.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3mskjwusu.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3pojdaqyk.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3ndnvoofa.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3drieaplk.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gipzixrb.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3dvafpwkq.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3adsycimw.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jztvmhke.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3esjwgcrx.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3vhfgqkra.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3skplxove.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3kzmgsjyn.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3fnkkvbxj.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3idkjlytm.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nkqlmrrm.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3yxhalcjd.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tezkyupe.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3rjnyrbwk.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3kjbsfers.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3gtcwjmjy.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3trlpkzpm.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3uokxlviw.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3mizabxdh.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3msvmudnw.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3espmcjzn.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3jhndvtgn.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3xjxmxvve.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3slvqikfn.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3dqnsvezx.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3goqhlvku.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3dyghlvxv.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3hgjgieio.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3popndjbt.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3rcilccdi.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3ancvfbnq.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3hhhqjyme.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3whlvrgkr.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3tmzwsbme.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3pyejwtdb.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3rrwphfwq.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dlkqtmui.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3nkplwckr.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3tiwthara.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3czbsoxqs.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3godsffsq.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3owkbirln.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3flcniuig.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3surjqduo.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3rpfbhbod.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3vvxbomvl.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3hltrzpef.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3bvzmornh.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3pnxifnzy.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3mwaavgwr.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3rxazjweo.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3liriquop.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ghbolbpm.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3feucnaqf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mboxiigp.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3jgimmpyx.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3ajjmfmvx.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3wzrlmdhg.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3rhxemciq.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3pqrmdpmk.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3xfunsozz.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3kwptluae.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3fidksosp.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3ectcnelp.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3dyzjppjn.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3dehedwkg.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3mksqiarm.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ucwuenld.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3xkshkzjv.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3svkommvz.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3dkoiqroi.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3anrqtqqs.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3rzcnfowq.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3uzvutuyf.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3fzvbcapr.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3sfwwvgjw.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3fufjtykv.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3pmoyylob.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3eerpcask.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3xvlpbwdw.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3rckkunzn.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3pryzmudk.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3bvarogle.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3fetpnlrj.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3qplxnhxv.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3lcrlitvc.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3xnxpgcar.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3lxxmdpmb.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3ixuqewur.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3muvbhmnn.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3umfgqsqn.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3ttoucjix.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3xahfyozo.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3njclstvk.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hkzckogv.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ywwiojxc.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3ymcywgou.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3ycmjlzby.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3vttshloa.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3eafyyadk.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3cwiipogt.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3hbcdketv.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3bmqbiifr.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3dtwmfklk.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3mjaywpqu.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3hbjebczr.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3zktpnlhz.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3ngfagock.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3taeyrtkd.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3tufpcxhl.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3qiulbjnc.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3tgogeswj.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3ifnswrjk.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3cnrtvvnf.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3sfbrnweu.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3wwemldfi.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3xdajmvwc.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3fgbyapvv.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3ignxaedx.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3helwcwaf.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3pioszlzp.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3gbirejgm.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3fivevutm.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3mzibuxuj.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3qzpxurkd.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3ctiksqqo.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3acojccwi.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3shalzgwe.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3uagcbiwm.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3ugxxghwt.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3swxvtfgx.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3rnchlcvc.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3ksorhxeu.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3epxsplrx.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3hvcnmmwt.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3zordcynj.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3sxydhanz.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3sagzstpc.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3vazrlxzv.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3scbkfonm.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3wujfftcl.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3grxhfgap.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3jurhcqjn.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3jdzdtsdi.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3bvtcylhw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ltwohzqv.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3dcawwojy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ojiaitws.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3mehegfha.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3roomefgd.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3dpfklmlo.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3nxirpnnz.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3arnguler.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3xwljtkeh.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3qqfmczdd.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3wtclixwq.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3lqcolxqt.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ncxasxbl.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3hpetcyls.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3urzcsupg.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3eifdlupx.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3wsoamavc.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3wamfzltn.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3blzvsyhb.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3xqukzare.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3tpyoogqx.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3lsipijsi.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt3zmobpmzy.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3gpzmfpvk.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3zkqlmtrj.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt3gssesjes.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3bvltevpm.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt3bpfpgkob.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt3nvgngyto.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt3obuifhaw.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3qjmlrsyd.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt3bxwestlm.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3tscdyzyb.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3yxpmewdp.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3ywkqbcte.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3fedvrddo.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt3finqufsw.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3gtxetjlx.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3dxihrvtn.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt3aayqxsec.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt3smlieacc.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt3gvvccphj.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3vuolngjc.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3pitgodcn.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt3uwetyqch.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3mbtaedud.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3mufgykrc.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt3odzktgjv.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt3scprshbt.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3iweqajgy.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt3ltnqnqvv.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3kwvkgzuw.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3gjzvuuch.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3ieasidnk.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt3tbcjizfx.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt3skrstsfr.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3tpazmrub.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt3cdrhzlso.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt3fgmprmhe.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3bhuaydfg.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt3cqhumylh.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt3yzzuiqwz.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt3zhkfhwnq.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt3hecotzwx.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt3heodhbtl.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt3gpjawdkq.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt3kajstjbl.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt3sxczvpwo.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3aoiydzye.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3sfnmfbbb.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3othjwsxp.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3gcbiscqr.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt3deeskdys.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt3dafaskot.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3bkofnvug.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ilbjidch.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt3ttrvlvdb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lzrhoikx.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt3jwoayjua.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt3sgqprrql.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3shxckvrn.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3qiavppkp.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3wuahigzy.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt3wnuxorsx.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt3bfxtsrwm.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt3pnindbhr.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt3kwmrkuic.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3xjgbyysu.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3ygtbpbbn.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3irjuhnzd.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt3hutlauuz.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt3yuohjnne.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt3khhkrjdq.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt3kpaggrtb.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3uvjmbvij.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt3tfolyzcv.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt3tansnqjp.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt3nviydazz.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt3emlxrhob.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3ziixfedo.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3oztancch.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3crsfxzwo.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3fdmogawf.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3bnkerzay.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt3qzfkjoow.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt3ezalbdpn.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt3kasgxgoo.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt3ktezixkv.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3iayruqnq.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt3tlfgcypo.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3pyvpdwbv.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt3tzfoxgdh.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3jwqykosn.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt3wirpjcly.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt3lumaikqu.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt3zgckzmnx.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt3yksxrhio.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3wipvwhtw.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3xafpttzy.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt3jcdevkdt.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt3sfmciquz.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt3tyzthngc.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3udtfocmw.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt3uphziani.html


<!-- 参考信息 -->