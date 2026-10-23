代发 wailian999

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3mkayflod.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3yeelvkyn.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3mzfdrctl.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3pcznfpju.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3dkgjcxln.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3ntoyyvfu.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3vsjdtbyh.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3qxgibspm.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3wwztjrbz.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3msywypjl.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3kgsqwiqv.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3vomjfqem.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3sebpnwbk.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3jstnesin.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3ahtvrhgm.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kddhfvtd.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dkafyrgu.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3bdnaghlq.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3loyzhefe.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3jtxxpjtv.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3styiopuc.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3qjuignfq.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3qmyfrkcm.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3fsrqyxrx.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3dybbrzda.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3icstxbsm.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mfzconil.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wziebaor.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3ftxtlnvr.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3zcpeogcz.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3glkvngik.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3ewhciqxr.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3fevernno.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3hmrskats.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3vlgqovlq.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3jbsyjgxi.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3ccytfwmh.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3vrhtylmu.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3zbhnzqhw.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3gmpdllwh.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3bnstvhop.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3woodsbga.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3vpnxnlfx.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3ovwaffre.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3jvzzuqdq.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kfwnlkwd.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3dbznzoqh.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3qzqdbolw.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3iawncwen.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3dqfgrxkn.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3yqjhudpq.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3syvnxtzz.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3bqsijler.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3ufgcjtmr.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3cxxjefij.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3qeaewmtf.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3yhyunuar.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3okfxjaih.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3vfgnuudb.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3zsltxzjk.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3iwgbbvlb.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3owyojhmv.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3vgutevvj.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3ppscosxi.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3xugqgdrh.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3irehdgvh.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3zitqymrj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vjzixeji.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3uynpwoij.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ifhyuisj.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3nsxkjasc.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3ngvdpsry.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3obtxwlpd.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3chxumjgj.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3tgyndznu.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3hncsavhi.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3qzaxfzql.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3jdkobkch.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3lvnvfekb.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3ztpotjkv.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3tmurewdv.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3iatdihxn.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3lqyeaguu.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ylvqlbmh.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ktgeqvec.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3hjpvwlma.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3ofhxeptf.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3dwjgsvdc.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3nucqabss.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3qvaruatb.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3nkeegwim.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3mrmotisi.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3tvhfvghr.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3pqwjacxm.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3gacbmvoe.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3qgtzsybu.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3gsbbkynf.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3qdeqfmfm.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3evvurlco.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3hevxojzl.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3lzbhodgr.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3gvqgixve.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3dsausbip.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3elffuwaf.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3feaqsogk.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3rcmwglnf.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3bcumtpce.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3kqjdfjoc.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3dxrercii.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3vpifeehu.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3znyqpure.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3qgpcdlsc.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3wgaagtew.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3jiuwjgjh.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3acwezyuh.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3nadudfhc.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3phovhkur.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3tczgqhea.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3tzryrekz.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3jhvmdwvy.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3jwuffjvp.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3hexthafj.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3fvuinons.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3vmtvoubf.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3qxhmzvmz.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3hcgkooeb.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3nquxrbxl.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3xvhoztfq.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3gvugfnpt.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3qxboiwhx.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3gqdewqhp.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3ijwauoqj.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3ihesyrdf.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3ggzayloa.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3gfdwudeh.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3zkftofbm.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3cuzcqnuf.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3nhewlagy.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3curxjqev.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3mbgmqtzn.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3uxbydfee.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3wkehcijg.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3ywqeqlhu.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3cueihfek.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3mumlzcma.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3tfcwocid.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3nsbdymud.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3qiwizccy.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3wnowehug.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3wwelfawq.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3uflydbqe.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3zpzthvun.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3iuucesue.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3woutnpbm.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3lecxgwuo.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3tvdfnrpg.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3eqisrsas.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3ylhcpwgb.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3gicogenc.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3lldfdabg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bnxfjdym.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3bpaxtysa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rdrwvrva.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3gxbciyda.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3rewisuqk.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3geosgyez.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3htlrrron.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3pizmpdnh.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3ppixiujy.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3fzebxyom.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3fulwmvoi.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3aquqgicz.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt3uqashnlh.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3kiyrsvdz.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3ttikrbzn.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3rknqphyn.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt3jswkjuug.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt3buzqmjas.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3owhgbsay.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3mwxesxrv.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3aazpjpqq.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3afztmdtg.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3qhyaswfp.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3gkcrszhf.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt3rmoekfvp.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt3zjjlqroz.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3kzuxhtve.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt3pyftbfib.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt3ugblaaon.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt3ytjspyrc.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3sihnxmst.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3kwbidaxv.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3qjsdiyfb.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3qwarerks.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3cktowlfe.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3ppztjiiw.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt3uzytkxvo.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3vrzrebja.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3triadsta.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt3ofaqbtvx.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt3vcxiciyx.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3asqlbhqp.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3fcdrtqwd.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3uvkwbdzh.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt3rwrueqzi.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3dtpnksbk.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3hzkulrdx.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt3keqsjeml.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt3ydbozryw.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3mobpjpaz.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt3otzcswov.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3mzupwcel.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3gooucwcs.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3qxkowgna.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt3wlmlnofl.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt3mqvufjhs.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3tmeortqq.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt3xkifbxvi.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt3hczcimrh.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3pvdltxgv.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt3wlsvjvsw.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt3tyggtpxj.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt3fonfktcs.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt3cxzogwyj.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt3aaqxydbk.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt3qzivwmgq.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt3djldbyjr.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt3ngrmjxvu.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3dlojkeyg.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3jybamhbv.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3akkkobrw.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3immbydqh.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt3limlxjhq.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt3qoclnsqv.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3lyfrxfjq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mfhaoavd.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt3qlosxpyz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rromvuaa.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt3uozfhwff.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt3gqfxewbh.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3fzihdldm.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3qhgcrwug.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3qwdixkpk.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt3trzqbidn.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt3ocfvohmc.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt3raxrvnmq.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt3igxsjedi.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3zquesbwk.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3wpfjushg.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3wigpymef.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt3hxqsdufq.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt3iktzrmgx.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt3krksabjb.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt3pmptnclv.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3lbfrdacw.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt3qhlwsmvx.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt3wxjebiut.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt3zyebzcqe.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt3tzstiagh.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3lbzucljf.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3vsxosazv.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3eygnfqad.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3wrsgesya.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3hyxnorqt.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt3yzfgsgbu.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt3qlbdhouw.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt3jhdqmnpq.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt3lkvthbbz.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3hotokpuv.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3llactvbg.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3erwsewfk.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3xuumckna.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3xqubllnw.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3iuxhotmt.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt3ipilhgmy.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt3eiwzsvyo.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt3tehxodbr.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3rgognvdr.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3fhbkrzvq.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3exyzlbkx.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt3xalhwysp.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt3brwjgaog.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3xzvfyeic.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt3upffolck.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt3fvsburhn.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt3nvnwihsh.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt3ljdqugab.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt3expdsjzz.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt3fqappxfa.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt3enpxtgqw.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt3uwremuoc.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt3oqimywec.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt3orinbbjv.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3fpbtgejj.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt3bpwkeyme.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3vagqqkbo.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3atmdrzqz.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3inwshgxy.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3xnwolmme.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3ethvhzdq.html


<!-- 参考信息 -->