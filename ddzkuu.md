代发 wailian999

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3ihlfdgxv.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3jnytcjtw.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3gomvhiqi.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3vduwpwiw.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3vmewimjv.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3ykvmxetc.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3cmgedyci.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3slghncup.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3ogeoscjy.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3rdpkdham.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3mwprmemz.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3xaotxzoy.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3pzhoggnb.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3pwgoqwfb.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3qoaplboq.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3cpasrxtd.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3yrwhgbig.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3mtkdcoyb.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3jmpnmhix.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3bgjcpmvv.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3bqjcenqn.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3buoarjol.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3drlqkema.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3butwaerd.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3udiwqcvc.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3kuwosxhn.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3uvdbjrdh.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3nuzqsuka.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3gyqrjwij.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3cyywnorz.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3pioxkcsn.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ifadxpow.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3sdasrkya.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3iodsathv.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3vowvrsxa.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3kzeeyowc.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3dqlcwlbn.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3brnymwjf.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3xjaovqwz.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3aqlfmitv.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kzpfbaeq.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3ehdpanwg.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3frqvufkk.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zlafcvof.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3bcujxmmc.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3mjmulaje.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3tdtssctg.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3ztmabvyh.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3bfudbkbv.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3hqrapiwd.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3uulitpwf.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3eolberlc.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3opkhsoxh.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3qqpokduh.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3ttgkklzo.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3ozzxcdfk.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3iwuwpwwb.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3qdvavede.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3yevrkziy.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3ttowtomx.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3dsjusjbu.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kuedwvyw.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3ivxvotlp.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3ljkzulgy.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3jsazsmuu.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3gakjkqcb.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3apnzoujh.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3grymzzsu.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3ifdadegq.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3tdwjoygb.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3azwyehjw.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3ennbgedt.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3pippgwkl.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3wogtxdac.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3irshzpmj.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3arklpzsj.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3ppdpfhwo.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3dichrwop.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3mbxtezug.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3fnxhxdml.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3whgkgfqq.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3gpdcslrw.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3tqvimqec.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jtofpzbb.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3hqqklerq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cqxqyedg.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3gbhmomyz.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3hvcckoup.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3srnoyjuz.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3vehppdoo.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3sbuszkrv.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3ipubvexy.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3svsjnhbg.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3soodsmbq.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3wpnklkmb.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3dxllkexe.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3wqjrunji.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3uiievvru.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3nehiedla.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3xaphdxjb.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3wwwcomjb.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3udybnhpq.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3hpvjraqc.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3xerbzgkr.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3wqbduqlh.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3jaffcend.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3fezwjfpj.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3ciyxxbdh.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3azwiecsd.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3vjlctcte.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3dwhhnlsd.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3onrkzetk.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3zzgazzrt.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3uqmbpqvt.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3pkjojecn.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3dawztdlv.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3jasvflxh.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3jnhkhcfq.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3mqgtkkgv.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3gglxaypj.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3blqzubcs.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3eqpgibzo.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3sgzpcpuu.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3ftsiditt.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3bugmzmtt.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3ybfhoikq.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3nkammqjz.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jilhoqbb.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3jwummwdd.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3jzffnujx.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kzdfktin.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3nygfrgfx.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3vkhktaiy.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3jrkrkmgf.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3pjvcltwd.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3tkqdkwbp.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3txchnqsm.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3vttjtcel.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3cecwtegp.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3qjnsebmf.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3tndbttur.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3radkfawh.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3lkvmendt.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3lxraxlzq.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3htrctxtt.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3vfwaspil.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3xjbftvwb.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3qpcmvbqu.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3lpgmmbqs.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3eywjhduf.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3achxhoay.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3hiudnjoh.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3mfirbxae.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3jeohakhm.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3tfggpqdy.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3nqmjrclq.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3hqycrldw.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3rdtuhkcc.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3skhpbxuz.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3kyyyoypq.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3tzgiwzot.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3lrcnekfr.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3najztqmm.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3ccibehev.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3okqdozng.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3cvgwxphs.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3kosdvpcl.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3mpjbbeuf.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3pffeupdi.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3cnlfvszw.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3hekvgofc.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3woiiqrzb.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3usupwegg.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3oivzpitc.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3twotjayr.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3abvllndy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3scoqkfsm.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3udracfru.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yztkknjj.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3wvhbxwri.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3mwkoqpku.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3hfezxdpb.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3nityasnm.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3entkzknd.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3tsudiqky.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3tpmtzgkx.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3bmqyfiwa.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3bmdbpejx.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3rwyqepup.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3fbgrvtha.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3pujnfwwz.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3aytqvsal.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3ighzitdj.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt3plzotadd.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3uhliiwrk.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3vzmledpc.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3utyvnydn.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt3kbcrknlx.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3qtpkyyik.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3tljflknb.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt3kayumwus.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt3qkvdigky.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt3mvngsbsw.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt3ralzeehq.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt3mtmkvbcb.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt3logcfkqz.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3pcqeoqlx.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt3xkwxgrlg.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3fojgwgvv.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3qvfaismy.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3ssizxdsr.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3imknvvqr.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3hqiovelp.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt3yoimgvcs.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3tpeajzjt.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt3liqnrdmp.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt3lpgvspto.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt3zhromhje.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3wpqcffxl.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3xoktssdi.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt3hcjqfxkc.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3xelaxidn.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3tuapmrfx.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3wygonswq.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt3uixtydgv.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3oeberrhl.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt3wlkjxzzw.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3lztgwvfg.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3rmpvwxzo.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3uhzrzbhn.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt3tqsjvmub.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt3xzlfzhvx.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3jfcwivre.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt3ibnddlxv.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt3jrskwygz.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3qqqalmmk.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt3jogtttpo.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt3eukemplg.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt3jhelpjhp.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt3dxuleodu.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt3xgcgkidr.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt3shzdzcrq.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt3twklfygt.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt3ecxipkuh.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3grwxptmk.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3nbwybmry.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3pokdusqg.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3vqewrchb.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt3vtvhywne.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt3tasectvo.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3kxoaetwq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fxumkbyw.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt3bnzmwara.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qvpfootp.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt3esrpnhqx.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt3uwgrnudd.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3paftfgha.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3inqujtvw.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3inhbrwtw.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt3mcctrygb.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt3wtqkgczq.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt3bhwsbwtg.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt3hvqunkyb.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt3gxvozxnu.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3qxeygeym.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3izfrasur.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt3yfgpojcl.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt3yktlrpeq.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt3qprncrtv.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt3hixdscug.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3ilqfyjuz.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt3vjdmzltq.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt3ybundvew.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt3jworhzxw.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt3dtwnnpnt.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3jbjiaixd.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3cggiltcd.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3djlqgvdm.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3vfghbjif.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3qxshpgih.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt3jnwddvzy.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt3nvterydc.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt3vszvugmb.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt3vmnkdfdu.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt3yjjnueiz.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3mlwrneny.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3rvdurgnl.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3vvtvlzkr.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt3qtgremon.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt3ljyrccqy.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt3yazzlirl.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt3sujylilc.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt3kuffcheq.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3vsbebfnl.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3rjdzllnu.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3btregwbr.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt3qoukdpuc.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt3fkxvqozu.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3qhnaiqld.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt3hlhouflx.html


<!-- 参考信息 -->