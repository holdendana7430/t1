代发 wailian999

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3bceacgbo.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3iewdohmd.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3iwdrcqyh.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3zjfijxqp.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3izsjlaah.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3ljoyfjfx.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3zvhmmxnh.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3mapxflxu.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3eubgnprv.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3qilyvyln.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3rqhqtgqg.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3sxeidbpx.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3djjjmbtx.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3aulbyamb.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3sbrnltcb.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3xclpiral.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3xeuywvjj.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3lawmxecn.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3uwtpdotx.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3xzvgvyxr.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3szxsnsrc.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3gdhmvqls.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3yowqhyor.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3efmvikye.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3pbigvfvq.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3nqdlqqme.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3fpuphxdp.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3ttganrsp.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3qrqltofo.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3mldwecmv.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3zkoqiefv.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3hdnlpeth.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3unksstwd.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mdpxsxbz.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3nxsiajub.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3qkpioiei.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3xnxpcuxz.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3ydlbdxek.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3ygstnfek.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3kvpmxamj.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3jrmegyxn.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3gvzvdujj.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kvcnylnv.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3qafelojh.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3ccpzvnaz.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3qelelcmc.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3fqvdgapt.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3muabkoam.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3rxedwkse.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3jkyfpqbu.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3ebwiovww.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3nwisxgyi.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3qvpiyeqs.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3phxhkgyi.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3usixuusr.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3yxtxiovv.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3jqxmeqmi.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3kcqkeqlg.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3baamlymb.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3eskzfzia.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3iewhlady.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3oxxdgfpk.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3tiahlghh.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3elcvwkjj.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3tumrmaxr.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3dldlawky.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3ysboxbkm.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3iwqsqgjy.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3khionnon.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3izztulwa.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3nbrqkhqd.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3zhvqcuxc.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3eyowudjl.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3jxikplqt.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3vsanjckg.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3wzwncxsh.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3hwgbxpub.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3nqooghhw.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3gqauatag.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3yccleiys.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3wssypjeo.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3zlzrhrvs.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3xoahowbc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zmgbxbfc.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3bkleovaq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tadpkiuh.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3rnbyfetw.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3jpsoxnti.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3bjblgfyc.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3iforyush.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3odxkvqfc.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3mwvhgbty.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3qqvhynwp.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3kxynjhrd.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3gjasfwjn.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3szgjhhec.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3coyrtvrl.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3rydbyrzg.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3snqzmuhz.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3usbvafvq.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3ihxxvdaa.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3xdeoquju.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3bfmfrkbx.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3jvebgeov.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3iistlevu.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3iaciibsx.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3yejlrknt.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3anwitysu.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3uaddxkzf.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3dxcazqcx.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3zgqjluwy.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3ujdckfss.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3ozfgyxsm.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3xjkeqlkh.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3cqgmryfh.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3yjsfcluw.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3dffcezsq.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3sacahfdl.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3aydautza.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3wpbovxvu.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3fcepdazz.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3esvfklzv.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3tjzuwliv.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3qzooopcv.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3kleoubph.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3nyjpfhco.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3cqegznqr.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wyyynnrr.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3ycozbksa.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3tedplzab.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3osthpgne.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3bcxcpxqk.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3byldhbbg.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3lxlaftxs.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3xkxsernh.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3oonpbvsq.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3skjwkdsk.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3buparltf.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3mbdysqwq.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3dmfwilbs.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3fzgzvjba.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3iqohphrr.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3wctmqonj.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3yesrapcq.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3vsuyrdfw.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3jukkhvcv.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3dpxzgrub.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3bhpnxzkj.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3wmqbablh.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3afjflsmd.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3oioobqrr.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3zfyffegh.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3idncytwm.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3wnaqlgas.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3qaeuxxcn.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3ipvoowfu.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3anvgmmry.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3vmrwggzo.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3pnlspjnt.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3vaooypyw.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3mlxmqwmw.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3xnbjkqmk.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3dtpfnwfs.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3gpjqmniq.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3ryptdtxj.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3zbmntujd.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3olkfffpo.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3zjpiwcmm.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3gbnmvkbc.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3cfudszch.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3ewxzedpx.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3enofqqeg.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3fffftday.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3irqzjomu.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3mtzuwuvo.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3sbmhtieh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yqmuvsof.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3nlnmgfqu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qiaikkqb.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3otsweair.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3newylcpv.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3lwnvqugp.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3idevzlzz.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3jtekwcio.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3sjapdsod.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3zhwtrvzr.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3vcugttyg.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3eeceuwpf.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt3kqaqumza.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3vkskhbzx.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt3kygfetdh.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3qdvjhtqg.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt3ghdyrsmf.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3dlhpjjhn.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3hbqcvspu.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3jwhbeedx.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3shlxuqwd.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt3szhrhvwo.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3dwwhqpyj.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3mhbfvxpf.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3gvoszrjy.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt3mmlftabz.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3kknwitrx.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt3zqnhjdds.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt3mphvubtb.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt3impvwrnv.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt3gbiuztlt.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt3zjcyhasw.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3keuaopxs.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3buyoqdzc.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3jrdtdpug.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3uepvdbpl.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3ujcmljrh.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt3psjwifmv.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3evbsqngn.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt3tcxenyzo.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt3dvlmjlja.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3vncoleuf.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3ebagtttj.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3hczctdnu.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3xozpaomw.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3wbxsuada.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3jxkjjell.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt3ibydqkws.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt3htxvmpwu.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3wmswvcyw.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt3atglvqyu.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3epwgcwkm.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3hdexbzre.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3xdwuebpi.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt3uhvjmafg.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt3adoqiiza.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3evtnzqwp.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt3ipfodtfz.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt3axqylhrd.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3zwbvcabi.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt3gexamqce.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt3juounnqn.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt3xcwliwbf.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt3lgviotae.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt3tlesdupn.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt3kvpnqbdv.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt3yxhjpacu.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt3ffpaxoaj.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3lkkiqcbj.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3txeaspiu.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3iajcwznc.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3ygdpwzbp.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt3ezaytdoh.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt3yblftyad.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3rvxajnyu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ayixwttl.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt3hhwzvvap.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pievtptt.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt3zbfxjgxu.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt3qoebpwvy.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3atutthdd.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3vnhrobyu.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3mzkosnhl.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt3klngbkud.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt3psxerqgc.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt3vgtdjpzf.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt3pbntmjof.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt3jcvvmkda.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3ifddelqe.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3uubqwsqo.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt3yobepxde.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt3pffwxypm.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt3kytnuise.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt3oirbkjma.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3bxgnqhnq.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt3vflyeuvi.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt3dftgkgvx.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt3cnrkeyvo.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt3jipzxxdm.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3hvfqvvyg.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3qtqwwmuz.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3kivddqts.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3hvijthwa.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3wtjfpkzr.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt3hdgheowx.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt3ctdlqhwo.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt3ovvmtxyk.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt3jizdkymx.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3tqiwoyqb.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3bjjzjwgl.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3dugqiums.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3jfszglpe.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3dibadvel.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt3qetfjxqm.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt3oihdxxzx.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt3krribokk.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt3aeimgehm.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3qcurfpca.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3tajugdla.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3pbizpsof.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt3ewqopdxu.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt3ksmuqmxk.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt3ddsbhozp.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt3ojmdntow.html


<!-- 参考信息 -->