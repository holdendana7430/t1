代发 wailian999

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.hesvh.cn/Article/details/gemcdfwen.sHtML

Ruby: def self.f; end
来源：http://read.share.zdbjq.cn/Article/details/gbisqulhp.sHtML

C#:   public static void F() {}
来源：http://baike.fehbvm.com/Article/details/ghfmveaab.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.fehbvm.com/Article/details/gqdctlbus.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.fehbvm.com/Article/details/gkrcylkxm.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.fehbvm.com/Article/details/gpvoimjkj.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.fehbvm.com/Article/details/gvmmshxud.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.hesvh.cn/Article/details/glcsncksd.sHtML

Java: interface Shape { double area(); }
来源：http://wap.hesvh.cn/Article/details/grhlnampi.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.fehbvm.com/Article/details/gmkwdnmzi.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.fehbvm.com/Article/details/gwgjjhlrc.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.hesvh.cn/Article/details/gwarhqcjp.sHtML

[G10] 访问控制
来源：http://read.share.zdbjq.cn/Article/details/gcpfmdfcc.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.fehbvm.com/Article/details/gzlopzefa.sHtML

PHP:  public / protected / private
来源：http://m.share.hesvh.cn/Article/details/gdffjjwbw.sHtML

JS:   #private 字段；其余公开
来源：http://blog.zdbjq.cn/Article/details/ggzpamhdt.sHtML

TS:   public / protected / private
来源：http://www.blog.hesvh.cn/Article/details/ggfjmhyqu.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.hesvh.cn/Article/details/gmzxhwdro.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.hesvh.cn/Article/details/glprsnkul.sHtML

Ruby: public / protected / private
来源：http://www.share.hesvh.cn/Article/details/gfblhjnwi.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.hesvh.cn/Article/details/gjifxrrhq.sHtML

[G11] getter / setter
来源：http://baike.hesvh.cn/Article/details/goxvuiesy.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.fehbvm.com/Article/details/gakqrhcfo.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.zdbjq.cn/Article/details/gwduhvesv.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.fehbvm.com/Article/details/gjzseuquj.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.fehbvm.com/Article/details/goihazfyu.sHtML

Java: public String getName() { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gckfhhkau.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.hesvh.cn/Article/details/gucsyhmnr.sHtML

Ruby: attr_accessor :name
来源：http://blog.hesvh.cn/Article/details/gwkanavou.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.fehbvm.com/Article/details/gibpscnje.sHtML

[G12] 对象转字符串
来源：http://3g.fehbvm.com/Article/details/gnpfkoust.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.zdbjq.cn/Article/details/gtijsbsqk.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.hesvh.cn/Article/details/gbzoctcnt.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.fehbvm.com/Article/details/gwenhejli.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/gqukefvdt.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/gjwlnbnaf.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.fehbvm.com/Article/details/gewpbyelx.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.zdbjq.cn/Article/details/gbyzglklk.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.fehbvm.com/Article/details/ggrexlabt.sHtML

[G13] 判断对象类型
来源：http://www.blog.hesvh.cn/Article/details/gpolfynwu.sHtML

Py:   isinstance(u, User)
来源：http://m.share.hesvh.cn/Article/details/gfkkjfmsd.sHtML

PHP:  $u instanceof User
来源：http://mobile.fehbvm.com/Article/details/gmsrhmkme.sHtML

JS:   u instanceof User
来源：http://wap.zdbjq.cn/Article/details/gbxxoxgkl.sHtML

TS:   u instanceof User
来源：http://m.share.fehbvm.com/Article/details/ghgpabdbf.sHtML

Java: u instanceof User
来源：http://wap.hesvh.cn/Article/details/gcxqnhqaf.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.hesvh.cn/Article/details/gqpvtyskc.sHtML

Ruby: u.is_a?(User)
来源：http://wap.zdbjq.cn/Article/details/giehxjvnr.sHtML

C#:   u is User
来源：http://wap.zdbjq.cn/Article/details/gawrhmldl.sHtML

[G14] 数据类 / record
来源：http://www.share.hesvh.cn/Article/details/gkfeyqroa.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.zdbjq.cn/Article/details/gsobrrjwa.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.fehbvm.com/Article/details/guxerkmol.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.fehbvm.com/Article/details/gcghwywvz.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.fehbvm.com/Article/details/gklqkktpy.sHtML

Java: record User(String name, int age) {}
来源：http://mobile.hesvh.cn/Article/details/gyogntukd.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.hesvh.cn/Article/details/ggijqlqpw.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.zdbjq.cn/Article/details/ggkqizkev.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.zdbjq.cn/Article/details/gwjiiybjf.sHtML

[G15] 枚举
来源：http://mobile.fehbvm.com/Article/details/gdldprgcw.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.hesvh.cn/Article/details/gjpwfwqau.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.hesvh.cn/Article/details/goecxrbwq.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.fehbvm.com/Article/details/gqcqkoakn.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.fehbvm.com/Article/details/ghdhtiihy.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.fehbvm.com/Article/details/gnjopbtff.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.fehbvm.com/Article/details/gagyoxbyl.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.hesvh.cn/Article/details/gqoektrpp.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.hesvh.cn/Article/details/gffuajmkr.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.fehbvm.com/Article/details/geczpofyd.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.fehbvm.com/Article/details/gsagrkcah.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.hesvh.cn/Article/details/gpbiszynd.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gnjplyltk.sHtML

TS:   Object.entries(obj)
来源：http://m.share.zdbjq.cn/Article/details/grqloixah.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.zdbjq.cn/Article/details/gfzjxtkjx.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://3g.hesvh.cn/Article/details/gpsgzlwsz.sHtML

Ruby: obj.instance_variables
来源：http://baike.hesvh.cn/Article/details/gahmwhvxh.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.fehbvm.com/Article/details/gbijoqiud.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gnrtmaxof.sHtML

H. 异常与错误处理
来源：http://3g.hesvh.cn/Article/details/gnzqfpbhz.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gwijdobml.sHtML

[H01] try / catch 基础
来源：http://wap.hesvh.cn/Article/details/ggwozifwy.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.fehbvm.com/Article/details/glohpqfmi.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.zdbjq.cn/Article/details/ghyldncau.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.fehbvm.com/Article/details/gbhicgeyw.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.zdbjq.cn/Article/details/gcymklcwi.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://baike.fehbvm.com/Article/details/gycbwigbq.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.blog.fehbvm.com/Article/details/gsxdvgyiq.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.share.zdbjq.cn/Article/details/gynueblub.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mobile.zdbjq.cn/Article/details/gfyozxheq.sHtML

[H02] finally / ensure 收尾
来源：http://baike.hesvh.cn/Article/details/girwznnyy.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.hesvh.cn/Article/details/gcsrfwemt.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.hesvh.cn/Article/details/gxxodzcrc.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/gewhuzipo.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/gudfdizno.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.m.share.fehbvm.com/Article/details/gjrpkkxwl.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.fehbvm.com/Article/details/gheezxybv.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://blog.fehbvm.com/Article/details/giotgupxp.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/gsabvslvo.sHtML

[H03] 主动抛出异常
来源：http://m.share.zdbjq.cn/Article/details/gaxsfbjwt.sHtML

Py:   raise ValueError("错误信息")
来源：http://wap.zdbjq.cn/Article/details/gpvgcethi.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.zdbjq.cn/Article/details/gyoxuftxg.sHtML

JS:   throw new Error("错误信息");
来源：http://wap.zdbjq.cn/Article/details/gdzfxawxa.sHtML

TS:   throw new Error("错误信息");
来源：http://www.m.share.zdbjq.cn/Article/details/gffneujjq.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.zdbjq.cn/Article/details/gadbarlql.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.m.share.hesvh.cn/Article/details/ghmdzqmbd.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.zdbjq.cn/Article/details/gtawyptfz.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://blog.zdbjq.cn/Article/details/gstkaimrg.sHtML

[H04] 自定义异常类型
来源：http://www.m.share.fehbvm.com/Article/details/gyieidijs.sHtML

Py:   class MyError(Exception): pass
来源：http://baike.zdbjq.cn/Article/details/gsdoozwee.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.m.share.hesvh.cn/Article/details/gonnfbxsh.sHtML

JS:   class MyError extends Error {}
来源：http://baike.fehbvm.com/Article/details/gaumaczaf.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.hesvh.cn/Article/details/grjvubjct.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.hesvh.cn/Article/details/gclmmafah.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.blog.hesvh.cn/Article/details/gmzxaisfg.sHtML

Ruby: class MyError < StandardError; end
来源：http://blog.zdbjq.cn/Article/details/goohhkihv.sHtML

C#:   class MyException : Exception {}
来源：http://wap.hesvh.cn/Article/details/gtxajcyxq.sHtML

[H05] 捕获特定类型
来源：http://mobile.fehbvm.com/Article/details/gjzactykw.sHtML

Py:   except ValueError as e:
来源：http://www.blog.zdbjq.cn/Article/details/gqbkgtxbj.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://m.share.fehbvm.com/Article/details/gfpjgtxel.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://mobile.zdbjq.cn/Article/details/gpujyzwma.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.m.share.fehbvm.com/Article/details/gqufrjfsu.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://mobile.zdbjq.cn/Article/details/gofmhhqiz.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://blog.zdbjq.cn/Article/details/gbngwfxri.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.blog.fehbvm.com/Article/details/gatmfmbrg.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.share.zdbjq.cn/Article/details/gjbwcchtz.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.blog.fehbvm.com/Article/details/gxmkmejjx.sHtML

Py:   value = d.get("k") or default
来源：http://3g.zdbjq.cn/Article/details/gmdqdddgf.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.share.fehbvm.com/Article/details/givntndjn.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://blog.hesvh.cn/Article/details/gjouzuyex.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://m.share.hesvh.cn/Article/details/gxpzlndze.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://blog.fehbvm.com/Article/details/gmahoglmh.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.m.share.zdbjq.cn/Article/details/gbxvgykzv.sHtML

Ruby: d&.dig(:a, :b)
来源：http://mobile.fehbvm.com/Article/details/glnfqnpol.sHtML

C#:   obj?.A?.B ?? default
来源：http://read.share.fehbvm.com/Article/details/ginixcubr.sHtML

[H07] 断言
来源：http://baike.zdbjq.cn/Article/details/ghmymuvkx.sHtML

Py:   assert x > 0, "必须为正"
来源：http://wap.fehbvm.com/Article/details/glkdtftwf.sHtML

PHP:  assert($x > 0);
来源：http://www.blog.hesvh.cn/Article/details/gsiqwqfqw.sHtML

JS:   console.assert(x > 0);
来源：http://wap.hesvh.cn/Article/details/glvtzppjw.sHtML

TS:   console.assert(x > 0);
来源：http://blog.zdbjq.cn/Article/details/grudexvld.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.blog.fehbvm.com/Article/details/gtshdmfqh.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://baike.fehbvm.com/Article/details/gurlviygm.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.share.hesvh.cn/Article/details/gwyoqtmtq.sHtML

C#:   Debug.Assert(x > 0);
来源：http://m.share.fehbvm.com/Article/details/ggxnzsetp.sHtML

[H08] 获取错误信息与堆栈
来源：http://wap.fehbvm.com/Article/details/galngnxeb.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://mobile.hesvh.cn/Article/details/gwmkmsdyf.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://3g.fehbvm.com/Article/details/gspxnmayv.sHtML

JS:   e.message;  e.stack
来源：http://m.share.hesvh.cn/Article/details/gazqsuhrr.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://read.share.zdbjq.cn/Article/details/gnbeqnyiv.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://wap.fehbvm.com/Article/details/gqpzerrgo.sHtML

Go:   err.Error()
来源：http://blog.zdbjq.cn/Article/details/gqipyrcrk.sHtML

Ruby: e.message;  e.backtrace
来源：http://blog.zdbjq.cn/Article/details/gshwfaqmf.sHtML

C#:   e.Message;  e.StackTrace
来源：http://mobile.fehbvm.com/Article/details/glhwfexsf.sHtML

[H09] 带错误码的异常
来源：http://m.share.zdbjq.cn/Article/details/gofjgfmvs.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://m.share.fehbvm.com/Article/details/gteytmtvi.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.share.fehbvm.com/Article/details/getsxflzk.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://baike.hesvh.cn/Article/details/gqmxmwcxj.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.m.share.fehbvm.com/Article/details/grsewmscq.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wap.zdbjq.cn/Article/details/gpajlsdev.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wap.hesvh.cn/Article/details/gtiupieoj.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://mobile.fehbvm.com/Article/details/gnjtjflob.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://baike.zdbjq.cn/Article/details/gqphcsoei.sHtML

[H10] 资源自动释放
来源：http://read.share.hesvh.cn/Article/details/gbtuargvu.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.share.zdbjq.cn/Article/details/gudxkpazj.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.blog.zdbjq.cn/Article/details/gilfgduyn.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.zdbjq.cn/Article/details/gdmvunscx.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.zdbjq.cn/Article/details/gvfbyoaom.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.blog.hesvh.cn/Article/details/gczwiyigd.sHtML

Go:   defer f.Close()
来源：http://wap.zdbjq.cn/Article/details/gjvhuvtuh.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://read.share.fehbvm.com/Article/details/gqpokpqco.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gjkramlhu.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/grrhsvkym.sHtML

I. 正则表达式
来源：http://read.share.fehbvm.com/Article/details/gvnkqukld.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/ggnbimrgm.sHtML

[I01] 判断是否匹配
来源：http://www.blog.fehbvm.com/Article/details/gsewifqki.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://blog.fehbvm.com/Article/details/gtvklsgwk.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://blog.fehbvm.com/Article/details/gvzkcthcx.sHtML

JS:   /\d+/.test(s)
来源：http://www.share.hesvh.cn/Article/details/gnolpvxxe.sHtML

TS:   /\d+/.test(s)
来源：http://www.share.zdbjq.cn/Article/details/gvwshmahg.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wap.hesvh.cn/Article/details/guhkbiyyk.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://3g.fehbvm.com/Article/details/guefiobep.sHtML

Ruby: s.match?(/\d+/)
来源：http://m.share.fehbvm.com/Article/details/gccgdajpz.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://baike.hesvh.cn/Article/details/ghekjlaqa.sHtML

[I02] 提取所有匹配
来源：http://www.share.fehbvm.com/Article/details/gogjmpxss.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.share.hesvh.cn/Article/details/gydqfbfwp.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://m.share.zdbjq.cn/Article/details/ghdnymslu.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mobile.hesvh.cn/Article/details/gjzlhhoox.sHtML

TS:   s.match(/\d+/g)
来源：http://www.share.zdbjq.cn/Article/details/gtlpdvria.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://3g.zdbjq.cn/Article/details/ghtlwfscc.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://3g.fehbvm.com/Article/details/gbcakrcgv.sHtML

Ruby: s.scan(/\d+/)
来源：http://m.share.zdbjq.cn/Article/details/gydeqrfkk.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mobile.hesvh.cn/Article/details/gxjathrcw.sHtML

[I03] 提取捕获分组
来源：http://read.share.fehbvm.com/Article/details/gecarpgfy.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.blog.fehbvm.com/Article/details/gdfcnavnb.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://read.share.zdbjq.cn/Article/details/ggstbdajc.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mobile.hesvh.cn/Article/details/gjehlznkq.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://3g.hesvh.cn/Article/details/gpekdozjr.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://mobile.zdbjq.cn/Article/details/gbyljgyxx.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://baike.hesvh.cn/Article/details/gtegehqdi.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://blog.zdbjq.cn/Article/details/gldcetlas.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://blog.fehbvm.com/Article/details/glewpsonb.sHtML

[I04] 正则替换
来源：http://www.m.share.hesvh.cn/Article/details/gquilbtfo.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://baike.fehbvm.com/Article/details/glazwzwji.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.fehbvm.com/Article/details/guxflotiv.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.fehbvm.com/Article/details/gaogprmkf.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://wap.hesvh.cn/Article/details/gopgmmalb.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://mobile.fehbvm.com/Article/details/gyvpbzjov.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.blog.zdbjq.cn/Article/details/gvoenfseb.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://read.share.zdbjq.cn/Article/details/gvdqvxqch.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.share.zdbjq.cn/Article/details/guyxvnirv.sHtML

[I05] 按正则拆分
来源：http://mobile.fehbvm.com/Article/details/gxydhnvrw.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://blog.fehbvm.com/Article/details/ghpyhgreo.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.blog.zdbjq.cn/Article/details/gtpgkfygf.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://read.share.zdbjq.cn/Article/details/gofbzayei.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://blog.zdbjq.cn/Article/details/gcfjayadc.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.share.hesvh.cn/Article/details/gddyrcyqr.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.share.zdbjq.cn/Article/details/gxgmnbxyo.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://blog.fehbvm.com/Article/details/gdckrvdau.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.m.share.fehbvm.com/Article/details/gbzjjovnm.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.share.fehbvm.com/Article/details/gcqwmeddu.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://mobile.hesvh.cn/Article/details/gjlbibbdw.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.blog.zdbjq.cn/Article/details/gnqqmtpfg.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.fehbvm.com/Article/details/gsuacynyg.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.hesvh.cn/Article/details/gpfjyhfaq.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mobile.fehbvm.com/Article/details/geoanbfmp.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://blog.fehbvm.com/Article/details/gmvagyeqo.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://3g.zdbjq.cn/Article/details/gspjtcqww.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://blog.hesvh.cn/Article/details/gsfryfyvu.sHtML

[I07] 忽略大小写与多行模式
来源：http://3g.fehbvm.com/Article/details/glomxkbdt.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://baike.fehbvm.com/Article/details/gacaufqdp.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://m.share.hesvh.cn/Article/details/goyziponk.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://3g.fehbvm.com/Article/details/goaysxuls.sHtML

TS:   /error/gim
来源：http://mobile.zdbjq.cn/Article/details/gqqpuriws.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wap.hesvh.cn/Article/details/gveuzvdoi.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mobile.fehbvm.com/Article/details/gnvewvwku.sHtML

Ruby: s.scan(/error/i)
来源：http://m.share.hesvh.cn/Article/details/gdjdvyeqg.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.m.share.zdbjq.cn/Article/details/gkejfntuc.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://baike.zdbjq.cn/Article/details/glgqfrdmi.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.m.share.fehbvm.com/Article/details/gvylbgmic.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wap.zdbjq.cn/Article/details/ghhsjwqnk.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.hesvh.cn/Article/details/gsqrmdxqw.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.hesvh.cn/Article/details/gvwrwyifr.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.m.share.fehbvm.com/Article/details/gyzhvrrtp.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://3g.zdbjq.cn/Article/details/gfzzcggcl.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.blog.hesvh.cn/Article/details/grsczhenl.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.blog.fehbvm.com/Article/details/gligqsuna.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gpzkdahmo.sHtML

J. 日期与时间
来源：http://mobile.hesvh.cn/Article/details/gmapxcidx.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gvriksmsr.sHtML

[J01] 获取当前时间
来源：http://www.share.fehbvm.com/Article/details/gueduecak.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://read.share.hesvh.cn/Article/details/gvjpxbuef.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://m.share.fehbvm.com/Article/details/gajkhhbvc.sHtML

JS:   new Date();  Date.now()
来源：http://blog.hesvh.cn/Article/details/gvrernysl.sHtML

TS:   new Date();  Date.now()
来源：http://baike.zdbjq.cn/Article/details/glcynlazo.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.m.share.zdbjq.cn/Article/details/gluuyvrkx.sHtML

Go:   time.Now()
来源：http://baike.hesvh.cn/Article/details/gvrqkkxsg.sHtML

Ruby: Time.now
来源：http://read.share.hesvh.cn/Article/details/glhqxmrhu.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://read.share.hesvh.cn/Article/details/gureqpjnh.sHtML

[J02] 格式化输出
来源：http://baike.zdbjq.cn/Article/details/guqugdwkn.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.zdbjq.cn/Article/details/gfyhajvcf.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://m.share.fehbvm.com/Article/details/gsqzrsemu.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://read.share.hesvh.cn/Article/details/gxqwzsjar.sHtML

TS:   d.toISOString()
来源：http://baike.zdbjq.cn/Article/details/giobthhqg.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://baike.fehbvm.com/Article/details/gsgbwfnfj.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.blog.hesvh.cn/Article/details/glhlkydxj.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.hesvh.cn/Article/details/gvunqzazk.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://blog.fehbvm.com/Article/details/genpxrkpw.sHtML

[J03] 字符串解析为日期
来源：http://m.share.fehbvm.com/Article/details/gzvmanqsz.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://baike.zdbjq.cn/Article/details/gwmvswtuy.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.blog.fehbvm.com/Article/details/geuvfklzz.sHtML

JS:   new Date("2024-01-02")
来源：http://3g.hesvh.cn/Article/details/gsupsacdh.sHtML

TS:   new Date("2024-01-02")
来源：http://blog.hesvh.cn/Article/details/guzctgmeq.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://3g.zdbjq.cn/Article/details/gdmhyjifz.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wap.fehbvm.com/Article/details/gynjwidqv.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.m.share.hesvh.cn/Article/details/gbbgipgnz.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://m.share.hesvh.cn/Article/details/gzbteftlt.sHtML

[J04] 时间戳与日期互转
来源：http://www.blog.zdbjq.cn/Article/details/gayxizhmr.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://m.share.fehbvm.com/Article/details/gnznjjgnc.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.share.zdbjq.cn/Article/details/gpoturfsd.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://blog.zdbjq.cn/Article/details/gudyufmhr.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://wap.zdbjq.cn/Article/details/gwbhklrdu.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://blog.fehbvm.com/Article/details/gmauuacsa.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://3g.fehbvm.com/Article/details/gibntwhhy.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wap.fehbvm.com/Article/details/gbaqdpmzm.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wap.fehbvm.com/Article/details/gnuwfxsoq.sHtML

[J05] 时间加减（加 7 天）
来源：http://baike.hesvh.cn/Article/details/gxxogpqsu.sHtML

Py:   now + timedelta(days=7)
来源：http://baike.hesvh.cn/Article/details/gtdnjmzfl.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.blog.fehbvm.com/Article/details/gxrsqvkjp.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.hesvh.cn/Article/details/gfdpthogj.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.fehbvm.com/Article/details/gdptzpigd.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.share.zdbjq.cn/Article/details/gevkniari.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.m.share.fehbvm.com/Article/details/gkbnbcysz.sHtML

Ruby: Time.now + 7 * 86400
来源：http://baike.fehbvm.com/Article/details/gmoitefgk.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.share.hesvh.cn/Article/details/gtpsmyxvn.sHtML

[J06] 计算两时间之差
来源：http://www.share.hesvh.cn/Article/details/gujetmykd.sHtML

Py:   (end - start).total_seconds()
来源：http://mobile.fehbvm.com/Article/details/gwjrxwosr.sHtML

PHP:  $end->diff($start)->days;
来源：http://m.share.fehbvm.com/Article/details/guoflawja.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://m.share.fehbvm.com/Article/details/gwuywgizz.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://blog.zdbjq.cn/Article/details/gcsxnmwcg.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://baike.zdbjq.cn/Article/details/gzhymzszo.sHtML

Go:   end.Sub(start).Hours()
来源：http://baike.hesvh.cn/Article/details/glharzsep.sHtML

Ruby: end - start                 # 返回秒数
来源：http://m.share.zdbjq.cn/Article/details/ggveebelu.sHtML

C#:   (end - start).TotalSeconds
来源：http://baike.zdbjq.cn/Article/details/gmekgigxn.sHtML


<!-- 参考信息 -->