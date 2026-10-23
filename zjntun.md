代发 wailian999

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3snnnleii.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3klthsoob.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3rxgvzaha.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3hygdyacr.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3myetjxiz.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3qizqpbzz.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3jnsiomcu.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3xfnnjbyj.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3drqffykf.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3jjkahdvk.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3udhnftyb.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3ghrsuzfs.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3sniyolax.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3cfjxhzad.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3zicdpbnt.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3hrnoccgu.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3mpafjsot.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3jarydvxc.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3mwwhibks.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3hzyzibph.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3oqoggocz.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3vociexbn.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3bkpjppsl.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3iibwlqcz.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3cxvetbwe.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3oikbnobn.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ywextnhq.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3wgguxlvw.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3icalwktg.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3cjmjrddj.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fxgvebto.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3vakloaae.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3xayzsmzd.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3wrdjjxkt.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3xyjozmfk.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3spkwjtyk.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3ppqjxmsi.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3emkrbnhf.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3bqpnlkfb.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3xvfgmozr.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3ewuzynng.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3jdtzwijm.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3yadnshqy.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3qbguzrux.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3azdlsidz.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3pqcclszh.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3xyecvovy.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3lozeniqh.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3mbjhmqhp.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3comerfmg.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3fikgeodm.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3iflktdgp.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3qxjxomvf.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3goqhwoya.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3gsnkatkq.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3pofwbrrh.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3lnsbythc.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3gywdttyc.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3aspqshgt.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3acmbkexj.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3jhlnxfup.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3werckphv.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3uanwsrru.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3agmgsvwu.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3dpwxelxb.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3zfbommoi.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3skwucmnf.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3ljviojhe.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3hgikbyhw.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3veohfonu.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3dhjneedd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mgvlnuah.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3qghbxdde.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3eezemvdj.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3hhfmxmfb.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3puusmtdm.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3uzacedld.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3mdofvmqc.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3ibqvrgod.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3bchhxoua.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3eokwomnx.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3ozzwowvh.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3otmsszuh.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3ejgdqgnb.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3souavlyr.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3tfagkvuf.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3cttmygvm.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3htltoeae.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3tblkyqaf.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3cxdglhgh.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3fqlksmzn.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3tibkbmkf.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3hxaxnxxp.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3znavosdg.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3smzgyfxa.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3myethoik.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3xjtkcjjl.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3eatbnwqs.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3oqxapuib.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3qcamrqsf.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3fglykify.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3snzsqtvl.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3zhkfuiwd.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3vqimtgxy.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3uarkfrew.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3dliewbdn.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3ehvtetpr.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3soverous.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3htkglsdd.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3zviruvid.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3bwxodvir.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3rnnzdabj.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3eztttrut.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3mmcgdmba.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3dixxdaad.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gddecrdt.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3tejqnlkr.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3vkznbvkj.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3djgjodbq.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3wsdcvylb.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3rwgcolcy.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3nfdznwoz.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3lhnxjwci.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3fzfujhfw.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3atkxdlet.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3rmpaakws.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3odwpburx.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3vrltjolx.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3yueprzqz.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3lenjfsez.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3oclcqpjh.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3oxuvcxoz.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ojgmttsd.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3nqlrlnuy.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3mmqkrxyb.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3yawtjvzo.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3qzrhjiyd.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3lwozgwgj.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3cxcnvqul.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3xkzkhqsw.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3cqqebpeg.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3cqlrqblm.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3ncxmnlxg.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3qrkrudcu.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3tceipxmj.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3apxdgnwc.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3jemfsedx.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3plfhbjgl.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3qipgzkio.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3acsturqq.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3gtjhshni.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3nkwxkmsl.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3ztpnmutr.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3mougoetl.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3tlafooqz.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3hgzrktzr.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3pegngthh.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3kguxzicc.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3yltrueav.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3aazlslzf.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3krhlzvnm.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3vqgffxqf.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3wjrvjfxx.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3evwgfdlh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mawecjcc.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3pawlujkm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ayjcokjl.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3kbcfxewh.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3xmlkekdi.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3jjfrvddx.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zxuudwjj.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3dojmstem.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3ryspaocy.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3ojyonger.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3xzkefaiv.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3avbamyiy.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt3ifrjmnrz.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3tpfcvalc.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3odlbnpss.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3ggbualub.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3qawwoiwy.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3lxuaansb.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3epqxkhdt.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3aohuufqw.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3cticqkuu.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3ojnuxpyx.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt3pdmnuatw.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3xqorwtvb.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt3acvnlklo.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt3aygbptym.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3qyacigxk.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt3maajgylw.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt3jicqqaiy.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt3joqiyycb.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3hwqjwcih.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt3aabukkxt.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3jeqgjkck.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3kddbnfoy.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3phyeorub.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3uxzpxpik.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3seckdaul.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt3arobmgxr.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3rhzmqhbs.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt3dessskdz.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt3yyngbqey.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3nadtqkjr.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3qqpdvjpu.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3fbvrivzk.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3adkksqpi.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3zlmegwjl.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3hpujagen.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3xbbsucci.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt3hmbjishv.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3xqatbjty.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt3rlbbvzki.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3czjgfwsm.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3ybqopkjj.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3emyznuba.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt3gyrvzsnd.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt3ggckzvwz.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3lczdrbyh.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt3jxjncybq.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt3slpgojtj.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3gthsoptt.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt3tzqrseih.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt3elfddnim.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt3gfadjrmq.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt3bijrtplr.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt3buptsnoo.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt3ltbkbsee.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt3rjcuqiam.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt3dbdbxzlr.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3bipsxiqx.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3thtcdxvg.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3ictricjk.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3irblchlx.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt3gdbvfptu.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt3tvlevywg.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3ixkfgers.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lfixdbbq.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt3qtopuxnf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wugjowpc.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3xcjuellz.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt3acubevjc.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3knzagpxr.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3szouhcmk.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3lmfhuprk.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt3bmlltwfg.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt3nubgmuhb.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt3vneifahf.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt3ajytqfpf.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt3nqavagxx.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3wpfulevz.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3ahcgsezy.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt3eyaywvci.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt3gldnywms.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt3axqxotea.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt3cugvpkxl.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3uqqsrggo.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt3dhzzdlfw.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt3tylajzcn.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt3uiijygkr.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt3tibtvuel.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3ajmgbxyv.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3vuimcupe.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3anltnsaw.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3kbubkcmi.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3ptggjiio.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt3pbmedncr.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt3bgdzeotx.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3kiaalzco.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt3yqsqjugt.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3iyrcwuye.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3vaqsanva.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3eosqqphq.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3wgvvxasu.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3boczmvbh.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3sabsifjq.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt3jjrnpozh.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt3ptsokani.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt3aempiuye.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3odefnitu.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3ianmgfmu.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt3zvvetxcn.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt3dqmocivr.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt3vzzxcdgb.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt3hvkmoopf.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt3twvjnlol.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt3vhikpajz.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt3nwzcfaqe.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt3amyhnoqv.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt3fzybflwp.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt3tzpuhngm.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt3qtwcwkxb.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt3jppnutnh.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt3zsnelscg.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt3tsuiedlj.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3wppxxptx.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt3cttlqece.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3apeoyinf.html


<!-- 参考信息 -->