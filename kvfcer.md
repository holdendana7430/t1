代发 wailian999

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2zmfmqhoj.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2pctocpim.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2royuudwk.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2ljbgtuoq.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2dqjrqyhd.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2xkudgrnc.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2gvcezhkp.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2ovjjzgje.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2bmseftim.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2igtfytsu.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2varzersr.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2hungsvgi.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2xdtuvofb.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2tnvtpnuc.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2cwsjnrho.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2mmjhwjly.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2hvzmvahu.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2tltpttgo.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2bljqpmuw.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2azgkabgq.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2lbzcktyr.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2frglgbrd.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2ynbnfkob.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2xzymkcas.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gwcoldqu.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ilwfvekh.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ubtaatnt.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2pqaxnunh.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2nbmssayh.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2whhezwpk.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ezhqocfq.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2hgtzamod.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dlsvctcl.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2veewuimz.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2nkedqdqn.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dcmzzgwi.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2zsylupnu.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2ovwlrkuj.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2wudrpvva.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2ilvboibi.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2lltypxmp.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2veoyikyy.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2mtijxugn.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2xblpfzev.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2rsqbkbxz.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2jwbcjnmt.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2zoxvlkms.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2aijuxdaf.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2eebzpqlt.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2bfmdposx.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2kqqwxhnl.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2lgifvoit.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2tofugnur.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bcrasfzu.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2vaktorxl.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2uwkqetju.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2mluzrupu.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2svwocqkv.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2uwjmfkob.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vmjpveen.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2azjakhfw.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2gevuiwhx.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2lstnvxft.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2lwaaopds.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2lbbaqpbl.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2qwtogouk.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2ssqntxhg.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2nidktddm.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2tqhenwmm.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2lobstcgz.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2egxsbari.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2wukttemd.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2mduspnpt.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2wfdlxnkn.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2xjoghise.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sssqazfn.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2vlkpqftr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gyfqfzbk.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2tottczhh.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2zgpwsykb.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2nrdknuqq.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2sdjqonpk.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2tpmoimml.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2wfdtvqjl.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2lplsgnpd.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2yesakjkj.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2vvwewkyv.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2rtkbyqkw.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2macjpquw.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2uorphlcw.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2zrnbmanh.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2iufpzzfr.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2dngcsque.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2cvfodpkc.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2uhxuvdmm.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2aulqmnyr.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2conarklp.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2pjuaykqj.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2rnrijbbe.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2ytkmhfud.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2gijyzbyl.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2icfqejdc.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2ujiwkana.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2wepwbmuh.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2emotladt.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2oamjtoho.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2nuzzbsmn.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2jsrwhmgq.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2qhmwvypj.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2neskdnqx.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2ksjvmhxk.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2jjloiwvn.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2watagpqf.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2mkiybokh.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2hlhmtrnh.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2frrwjwpx.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2toiqtlje.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2uchknkcf.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gtlhdaag.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2ecjasfjc.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2vgpygfdm.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2qbsljwol.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xafqsrjp.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2zkjzgapg.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2kkfasrah.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2nrctlcqb.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2afiexxbc.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2etjhlwsw.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2jviucjfo.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2fxavlgbt.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2apfwjilt.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2llqhonfw.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2fczhabkm.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2bsfydevl.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2dgitudnl.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2sfehikxm.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2opycnrpe.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2cftyqame.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2rwmrykad.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2zubybrik.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2upqpfptk.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2zypmjyze.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2cwcbwirq.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2qidmligz.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2losioucd.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2ftivxhji.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2aczufmqj.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2qhljrcww.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2kdeathqw.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2kdwlabli.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2xazkrfcy.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2nqaluuku.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2mbmmwyig.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2qptuehms.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2hfwchjpk.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2vemdipoz.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2uaxtlaxv.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2yqkkompq.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2ydjkglfs.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2ongtxatt.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2nqrotfig.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2yzziaeob.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2moldxvpn.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2ahnqetqz.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2uuzbveht.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2crbliqxm.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2phrfetwv.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2usyzpisl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ruiiqmgs.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2plnnzqgc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fpufqsdo.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2oswhvsdh.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2bcszvdfl.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2bohjamfj.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2zvfuesus.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2cclqoxon.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2dvlcahzg.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vjehljvw.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2isxaxohr.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2cjomdocx.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2whvifodw.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2zlhhmvwh.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2jyghjpyy.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2ulsuxqxl.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2hzsbmnxg.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2fmbgswus.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2ksguzfjm.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2orxgkcqi.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2cqhtcwaq.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2hnglpifx.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2mvefqnna.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2bdzzgipd.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2qatktgkl.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2yedastmo.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2azwboyup.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2gzhnzczo.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2gnitzdeb.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2ygzjlqid.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2jcucmdnl.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2jdkklhjw.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2zlfvplhv.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2uaddbiyw.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2ryxkiqot.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2wsguvxvi.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2mcxjtxtv.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2lcoaywty.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2msfwznyd.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt2gmjrcdyj.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt2qsjuopbj.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2eorqsvfr.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2kxgfrqth.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2uncxlgts.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2janyjdls.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2nhrfemuz.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2xfumhpfs.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2yajtbdhi.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt2bipdxjob.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2hdlwpehb.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt2pruavzdv.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2olklfpjn.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2vcvutmfp.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2bxaeqmyy.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt2eaqbpsaw.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt2qjvpdgmm.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2pmhiixpz.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt2pdvjcfza.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt2uqrvgway.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2cvcxxyqi.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt2jcpsgjpx.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt2qbfequew.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt2rylghqvm.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt2zkqifadp.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt2nwmalqpz.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt2ttvclzgp.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt2xlpxdgoe.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt2tjiwyewm.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2unacjzgo.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2plqfqmgm.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2gjaxggap.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2hkhzmmvz.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt2xxxhkvvf.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt2qozrzscf.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2ffufzhfk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fovjbisy.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt2putkolwz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ykxprdvh.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2pkonduot.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt2zezblabl.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2zmxhlvma.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2ninnttzc.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2zsyyivyw.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt2jptihiri.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt2hydbwgpq.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt2ilpkqida.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt2ktqwgssq.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt2onrqlrdo.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2hgpjohip.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2zmnpygwx.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt2ddmmfuco.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt2tzykhpau.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt2tpaliqjj.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt2akhkplwj.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2zcqetalg.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt2qnkzubag.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt2ifzthvya.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt2gxosvghl.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt2ixorthkt.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2wxkcwanv.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2edispvoc.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2egwesqbb.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2gkrexmkr.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2poipiwij.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt2ycxjlhnz.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt2cfphtzii.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt2kovjjpmz.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt2txomfomp.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2jrhvdcxn.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt2ucynjhet.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2flmcdmam.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2xeccearv.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt2lxsqmhkx.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2sezfzbym.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt2xuzexaqv.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt2kvmenfrt.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt2jkpvhqvv.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2pnbjmrng.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2jtflvabm.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt2bixgemlw.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt2klyaemke.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt2xccsfmtz.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2ggfosqms.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt2vgtqlufo.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt2jdkveevu.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt2fxydejpw.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt2cdkaxkem.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt2xmlvzvir.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt2ychoyppr.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt2askqevbc.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2xvdxxywj.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt2orgdnxva.html


<!-- 参考信息 -->