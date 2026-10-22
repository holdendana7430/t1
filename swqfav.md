代发 wailian999

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2ymyppwjr.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2pyzjcgkm.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2cgfyrtoj.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2kdsvpkmi.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2fchaixlu.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2uquknspd.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2zvdfqzas.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2riaauqsb.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2aiqpbgbm.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2zclkfcdj.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2bellskhu.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2xvoahcaz.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2pqajudor.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2rvudqjrn.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2lqdndgxr.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2cnxhqest.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2ujncfjya.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2ssdbyvbq.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2jjnnhclr.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2kkayhjxq.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2ubscjmwy.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2lczathxq.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2kgjvbuwx.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xionwwcy.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2wmctulne.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2irmpqvmf.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2dckvijjj.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2zkduuitp.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2wbebzigh.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2nlqxssaa.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2pvqdjmhx.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2omqbalfn.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2crxurenl.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wfumhxbw.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rmisaaoe.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fjtgpemg.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2uenavxqz.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2ajuocsre.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2suuocvuc.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2xkmqurhe.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2oneqbhjc.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2ubtufwnf.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2bqfuoivd.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2ffutxtuh.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2plpjkldf.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2trchzowg.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2taiyjsnb.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2rljliylt.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2nownqggi.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2bxganjhc.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2dkltjfcv.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2kfwewsib.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2iemstclz.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2oflwzzev.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2yduslwfa.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2wndnzgns.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2rjrqmufu.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2zsjfkqua.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2vsipwyxp.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bprqluig.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2arfelias.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2ntrafhhf.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2gmimialo.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2tfuowutn.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2gmeuavxj.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2cqziuqzo.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2gkerrrlj.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2paczebrh.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2fdbgnvtu.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2meqnywuw.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2drkyyosh.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2jergoaeb.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2vthufubb.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2reitpimj.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2rffhtogl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zabkvcga.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2ammdrxlo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2iwbqqvwj.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2skjahzyd.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2uprvcpug.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2mgxkuduj.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2wtuatmkk.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2vxsjugjc.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2mzfnapny.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2mjivhyrh.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2yptvwvra.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2stqierxq.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2vcczsuuf.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2lstswqtz.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2julbwyhk.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2hfolfrgw.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ivlamfsr.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2wsjbwnvj.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2atmrteiy.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2xypfpxkz.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2yqvsgygn.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2sdbxhrqa.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2vjcwtzik.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2jsqqrlyd.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2bqvccass.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2xmdjjrds.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2mzubsjqp.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2ftiusmxt.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2chesxpjm.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2eadyulkz.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2dcjrrtiz.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2pogisdlr.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2mosaqcye.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2velvvlsm.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2fxzowaet.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2wbpeeoyt.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2rgbvkjuk.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2fipowgnw.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2ugpfyqmr.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2jduaxiil.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2fwpychcf.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2uffnedtc.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2etzeaubq.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2egfeisar.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2btzxybjj.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2uedcotqq.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2fhjahvod.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yqjyyfri.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2cqexvbif.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2xeprykao.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2koytvkze.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2tmihieqw.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2kzyabfnl.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2waianfae.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2hoeqwvgq.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2mulkbnfh.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2auuycfrf.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2cqyasnkq.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2bkyuemky.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2poktqgii.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2tfbzlhkd.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ppgrqkja.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2ywaxcbji.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2srrqbcfy.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2upthcqxw.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2cooqtbes.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2osprzkix.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2fvqbzodv.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2dswetugn.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2kaaxrqnd.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2nubrwzuu.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2xyeslxyt.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2fosflssw.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2fdqjdtaz.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2zggmowsc.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2jtontmsl.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2ppyzdhgr.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2nurdwnph.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2cdifpbjb.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2pxhtxufh.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2albgszbt.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2xjsnwqjf.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2uvpmrhmg.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2mzvpiizv.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2urgoscuj.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2jkgforpd.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2mihawyue.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2uylygksp.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2ehvvsmiy.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2gkfzoxsf.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2tkyzrumo.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2bytizqpa.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2zhczrvch.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ouvvlros.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2djyqepqs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qiaucshs.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2bkxkhgqm.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2fyiffadb.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2xjuqeums.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2vjejzhge.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2uofnbyhb.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2gfhzmyax.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tdgqqikm.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2ikmlrtya.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2phtdqbge.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2xwtyjcrp.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2hkudbppn.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2bjkwmvjj.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2mzgcmrhm.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2rgrlnwck.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2wpiadppm.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2kpmrbdok.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2genugjea.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2qglbbgez.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2ooozyorh.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2oqqsrsgw.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2kjnfdqlh.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2qltbrmrj.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2xiozucyu.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2eldtdouu.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2uumplciy.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2ikgrofzf.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2hrgjqevy.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2mgiksyzg.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2equnhhfz.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2nvwesiae.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2cblmhmmb.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2upjudojm.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2rxyjundl.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2twouxevw.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2nosovjwh.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2myldqlep.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt2eibcyctj.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt2cnhohipp.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt2usnnoqce.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2kyrwaook.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2vkhqmiax.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2nxqoayja.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2zczszbkb.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2pkkjegeq.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt2lnriwqjp.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt2mrzxhgjz.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2bakalnbq.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt2tufcsczh.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2lycymvzj.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2epzxawfo.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2mkrmrhjz.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt2tzajzgsd.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt2umaezxby.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2mbxsujmb.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt2xpiygqie.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt2wzcizqxx.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2whposjrp.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt2mubqycey.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt2vytntoen.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt2qpnwrrfi.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt2xpxlqmyb.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt2guiegapp.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt2idxtlfvw.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt2rgtottzo.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt2olkllogs.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2ijdapeqf.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2wikbjojr.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2tmbbcimz.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2pvrkwxtg.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt2exqitsmf.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt2oanydght.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2wzzsbyus.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vxatspwc.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt2zrytndyl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wzblpxts.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt2zsrundft.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt2sgipwjdu.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2vwhvuomy.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2nvikkbty.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2dxfuyexr.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt2svyjwonx.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt2szpvveyc.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt2dfjbukjh.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt2dzjdjigf.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt2layflngm.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2mmfnxmap.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2jbkvcnrk.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt2zzkmmarn.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt2dnwcmmum.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt2vssawpug.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2fafmrvqn.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2fbybrehu.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt2ilkrmdfs.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt2roxxlbji.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt2dpjelchg.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt2gjwzcxrt.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2oahlxwzn.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2dhbjedjm.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2grbskfbb.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2flxlmonr.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2zmrcuspj.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt2tbzvivfc.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt2apewnlfa.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2nxwuaghi.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt2qgkclhku.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2whslcglp.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2taamhulz.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt2njnepogj.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt2abihhsxy.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt2phzdfvci.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2monxhvek.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt2ptrfcqed.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt2gakgbmhx.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt2ubhfyglq.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2ceyakreb.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2qxzqonaj.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2locrxern.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt2ewismrlk.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt2dviykyhk.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2fthhdndu.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt2pburvtah.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt2acvtbfqk.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt2whncaqyo.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt2bjmtqeyz.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt2alkuerdc.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt2uoeeziij.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt2xblhxyuy.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt2yzyjgphs.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt2hlcxvemx.html


<!-- 参考信息 -->