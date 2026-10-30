代发 wailian999

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.zdbjq.cn/Article/details/gfnggjzmx.sHtML

Ruby: def self.f; end
来源：http://wap.fehbvm.com/Article/details/gcgmvtdvx.sHtML

C#:   public static void F() {}
来源：http://baike.fehbvm.com/Article/details/giplppxfd.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.fehbvm.com/Article/details/gxxwbdqkz.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.fehbvm.com/Article/details/gfymzigye.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.hesvh.cn/Article/details/glroopqng.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.zdbjq.cn/Article/details/ghxyomfsp.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.hesvh.cn/Article/details/gsauynhyq.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.zdbjq.cn/Article/details/grqcisrdw.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.zdbjq.cn/Article/details/gqxdvjdcn.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.hesvh.cn/Article/details/gjvrldnkb.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.hesvh.cn/Article/details/glekxnmes.sHtML

[G10] 访问控制
来源：http://m.share.zdbjq.cn/Article/details/gynruuujc.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.hesvh.cn/Article/details/glowroqrf.sHtML

PHP:  public / protected / private
来源：http://m.share.zdbjq.cn/Article/details/gmrpkjpeo.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.zdbjq.cn/Article/details/gqfkxsixj.sHtML

TS:   public / protected / private
来源：http://mobile.zdbjq.cn/Article/details/grldwfxds.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.zdbjq.cn/Article/details/gsptuedte.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.hesvh.cn/Article/details/gkigdnayg.sHtML

Ruby: public / protected / private
来源：http://blog.hesvh.cn/Article/details/gilrefcwp.sHtML

C#:   public / protected / private / internal
来源：http://blog.zdbjq.cn/Article/details/gcptnzwoh.sHtML

[G11] getter / setter
来源：http://blog.fehbvm.com/Article/details/gkbtitlur.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.fehbvm.com/Article/details/gxsocjasx.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.fehbvm.com/Article/details/gaedhihpw.sHtML

JS:   get name() { return this._name; }
来源：http://baike.zdbjq.cn/Article/details/gmepriiyq.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.hesvh.cn/Article/details/gtxvfoyrf.sHtML

Java: public String getName() { return name; }
来源：http://mobile.hesvh.cn/Article/details/gqzqgroqm.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.fehbvm.com/Article/details/guphcabfp.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.hesvh.cn/Article/details/ggsagkjlj.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.zdbjq.cn/Article/details/geshpplio.sHtML

[G12] 对象转字符串
来源：http://www.blog.zdbjq.cn/Article/details/gplyamxue.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.hesvh.cn/Article/details/gccjlewhd.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.zdbjq.cn/Article/details/gmqoadtha.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.zdbjq.cn/Article/details/ghlczcuql.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gfjoswjzg.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.fehbvm.com/Article/details/gpqdaorks.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.fehbvm.com/Article/details/gdtbviivv.sHtML

Ruby: def to_s; @name; end
来源：http://3g.hesvh.cn/Article/details/gfnbjjice.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.hesvh.cn/Article/details/gmecoaaqr.sHtML

[G13] 判断对象类型
来源：http://m.share.zdbjq.cn/Article/details/ghmbmxoal.sHtML

Py:   isinstance(u, User)
来源：http://3g.zdbjq.cn/Article/details/gfcxobcnq.sHtML

PHP:  $u instanceof User
来源：http://www.blog.hesvh.cn/Article/details/gowqfhzul.sHtML

JS:   u instanceof User
来源：http://m.share.fehbvm.com/Article/details/gvfxyfhsw.sHtML

TS:   u instanceof User
来源：http://baike.zdbjq.cn/Article/details/gmgapzsmb.sHtML

Java: u instanceof User
来源：http://mobile.fehbvm.com/Article/details/ghmnyuxks.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.fehbvm.com/Article/details/gvymncmkl.sHtML

Ruby: u.is_a?(User)
来源：http://baike.zdbjq.cn/Article/details/gyutvsazz.sHtML

C#:   u is User
来源：http://www.blog.hesvh.cn/Article/details/gtqphevcg.sHtML

[G14] 数据类 / record
来源：http://www.m.share.zdbjq.cn/Article/details/gtqquzcip.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.hesvh.cn/Article/details/gvnndnhck.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://read.share.zdbjq.cn/Article/details/gkxdpuzuf.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.zdbjq.cn/Article/details/gdhqfuopk.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.zdbjq.cn/Article/details/grezmuflj.sHtML

Java: record User(String name, int age) {}
来源：http://wap.fehbvm.com/Article/details/gggjogdeu.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.zdbjq.cn/Article/details/gwzobdbmj.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.zdbjq.cn/Article/details/gtcwghjsj.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.hesvh.cn/Article/details/ghriwmhxb.sHtML

[G15] 枚举
来源：http://3g.zdbjq.cn/Article/details/gqinhuuzq.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.fehbvm.com/Article/details/gfcefrrpa.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.zdbjq.cn/Article/details/gvgrxuvhx.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.zdbjq.cn/Article/details/gwqfeyxxh.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.zdbjq.cn/Article/details/gqpfyzibc.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.hesvh.cn/Article/details/gujzscdno.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://blog.fehbvm.com/Article/details/gtisjazti.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.fehbvm.com/Article/details/gieynqsvw.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.hesvh.cn/Article/details/ghvqtnkte.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.fehbvm.com/Article/details/gueemdogz.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.hesvh.cn/Article/details/geycnqhhb.sHtML

PHP:  get_object_vars($obj);
来源：http://blog.zdbjq.cn/Article/details/gblugvtrj.sHtML

JS:   Object.entries(obj)
来源：http://mobile.zdbjq.cn/Article/details/gddbhdgly.sHtML

TS:   Object.entries(obj)
来源：http://3g.fehbvm.com/Article/details/gsrxwzgtu.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://m.share.hesvh.cn/Article/details/gocizknjl.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.zdbjq.cn/Article/details/gvfulolvb.sHtML

Ruby: obj.instance_variables
来源：http://baike.zdbjq.cn/Article/details/gqvliuuhy.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://blog.fehbvm.com/Article/details/gdqgmlocq.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/giknpxnpx.sHtML

H. 异常与错误处理
来源：http://blog.zdbjq.cn/Article/details/gvrezksuc.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gpovlswfb.sHtML

[H01] try / catch 基础
来源：http://mobile.fehbvm.com/Article/details/glpwhjnqx.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.hesvh.cn/Article/details/gwmbalavq.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://3g.hesvh.cn/Article/details/gsryupqrb.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.hesvh.cn/Article/details/gfdesnoil.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.zdbjq.cn/Article/details/gayjlwfiq.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.blog.hesvh.cn/Article/details/guxbmpxxe.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.m.share.fehbvm.com/Article/details/gzmcenfpm.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wap.hesvh.cn/Article/details/gibpmrnci.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.fehbvm.com/Article/details/gcjnsrmuz.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.hesvh.cn/Article/details/gciyasgry.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.fehbvm.com/Article/details/gvkyswlkd.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.blog.hesvh.cn/Article/details/gwwwynenu.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/gwvmqddno.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.zdbjq.cn/Article/details/gkztkhacd.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://m.share.fehbvm.com/Article/details/gmkyvvrri.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.zdbjq.cn/Article/details/glzzlsspf.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://3g.hesvh.cn/Article/details/giyxwhsdz.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/guxiwpyqw.sHtML

[H03] 主动抛出异常
来源：http://wap.zdbjq.cn/Article/details/gphmukpod.sHtML

Py:   raise ValueError("错误信息")
来源：http://baike.fehbvm.com/Article/details/gwfrikmqp.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.zdbjq.cn/Article/details/gzrafdado.sHtML

JS:   throw new Error("错误信息");
来源：http://blog.zdbjq.cn/Article/details/gtbwpzzfv.sHtML

TS:   throw new Error("错误信息");
来源：http://blog.hesvh.cn/Article/details/gyfqksvaa.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.hesvh.cn/Article/details/gojesyhvq.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://m.share.fehbvm.com/Article/details/gygmguxxw.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://m.share.zdbjq.cn/Article/details/gqukzytey.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://m.share.zdbjq.cn/Article/details/gfzdwdjtm.sHtML

[H04] 自定义异常类型
来源：http://www.blog.hesvh.cn/Article/details/goqnqljqc.sHtML

Py:   class MyError(Exception): pass
来源：http://read.share.hesvh.cn/Article/details/gzqbatxnq.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.fehbvm.com/Article/details/gneuxiccm.sHtML

JS:   class MyError extends Error {}
来源：http://www.share.hesvh.cn/Article/details/gnotukpbo.sHtML

TS:   class MyError extends Error {}
来源：http://3g.hesvh.cn/Article/details/gcmbhlcxw.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.m.share.hesvh.cn/Article/details/gkbacbrrt.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.m.share.fehbvm.com/Article/details/grcfqwzyf.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.m.share.zdbjq.cn/Article/details/goyaspzxp.sHtML

C#:   class MyException : Exception {}
来源：http://read.share.fehbvm.com/Article/details/gyjioahej.sHtML

[H05] 捕获特定类型
来源：http://read.share.zdbjq.cn/Article/details/gatqyflai.sHtML

Py:   except ValueError as e:
来源：http://www.blog.zdbjq.cn/Article/details/gntclosoe.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://read.share.hesvh.cn/Article/details/gugacyqbn.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gnlhiiwyc.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gfbjlaneg.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.fehbvm.com/Article/details/gthukagfg.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://3g.hesvh.cn/Article/details/gpcpiyhfe.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.blog.hesvh.cn/Article/details/gsxaunlir.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://baike.fehbvm.com/Article/details/genzaapmv.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.blog.zdbjq.cn/Article/details/gjamiilcl.sHtML

Py:   value = d.get("k") or default
来源：http://www.m.share.zdbjq.cn/Article/details/gfjikeruu.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.share.fehbvm.com/Article/details/gbbnovasv.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.share.fehbvm.com/Article/details/gaeuuvnby.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://read.share.fehbvm.com/Article/details/gfhxhzawy.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.blog.hesvh.cn/Article/details/gxoipusoz.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://mobile.fehbvm.com/Article/details/gptgchfkg.sHtML

Ruby: d&.dig(:a, :b)
来源：http://m.share.hesvh.cn/Article/details/gwvlaszwp.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.m.share.fehbvm.com/Article/details/gqkprtlyf.sHtML

[H07] 断言
来源：http://www.share.hesvh.cn/Article/details/gjskrwals.sHtML

Py:   assert x > 0, "必须为正"
来源：http://blog.hesvh.cn/Article/details/grhxynlnm.sHtML

PHP:  assert($x > 0);
来源：http://www.blog.hesvh.cn/Article/details/gswwvbpyt.sHtML

JS:   console.assert(x > 0);
来源：http://www.m.share.hesvh.cn/Article/details/gaoxtugcf.sHtML

TS:   console.assert(x > 0);
来源：http://blog.zdbjq.cn/Article/details/gfdgewlms.sHtML

Java: assert x > 0 : "必须为正";
来源：http://wap.fehbvm.com/Article/details/gsxyybfkd.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://3g.fehbvm.com/Article/details/gibtvqmjr.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://read.share.zdbjq.cn/Article/details/gtxqanuib.sHtML

C#:   Debug.Assert(x > 0);
来源：http://mobile.zdbjq.cn/Article/details/gygcmzauc.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.blog.zdbjq.cn/Article/details/gcdtxykde.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://baike.hesvh.cn/Article/details/gqcivrflj.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://blog.hesvh.cn/Article/details/ggmxwsxzt.sHtML

JS:   e.message;  e.stack
来源：http://3g.zdbjq.cn/Article/details/gyrmmuckf.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://read.share.fehbvm.com/Article/details/gbfbbkpjv.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://wap.zdbjq.cn/Article/details/gczdfnddd.sHtML

Go:   err.Error()
来源：http://blog.fehbvm.com/Article/details/gfmpuwcur.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.blog.zdbjq.cn/Article/details/guxqjruht.sHtML

C#:   e.Message;  e.StackTrace
来源：http://read.share.hesvh.cn/Article/details/ghflhaaxz.sHtML

[H09] 带错误码的异常
来源：http://wap.zdbjq.cn/Article/details/gutouiumz.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://read.share.zdbjq.cn/Article/details/gbdyjsdoi.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://mobile.hesvh.cn/Article/details/guidnjnux.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://baike.zdbjq.cn/Article/details/gkdbkcpzf.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.m.share.fehbvm.com/Article/details/gelnnigbv.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://blog.zdbjq.cn/Article/details/gkwdaxagg.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mobile.fehbvm.com/Article/details/gegldjrbx.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.blog.zdbjq.cn/Article/details/ggpgfvtrs.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://blog.hesvh.cn/Article/details/ggedolmrz.sHtML

[H10] 资源自动释放
来源：http://wap.hesvh.cn/Article/details/gxyfembbq.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://baike.zdbjq.cn/Article/details/gvvfzuzmr.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://m.share.fehbvm.com/Article/details/gqmjzrcow.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.fehbvm.com/Article/details/ghcqzmvqa.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.hesvh.cn/Article/details/gtxlxqhyz.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.blog.fehbvm.com/Article/details/gtizlmmgr.sHtML

Go:   defer f.Close()
来源：http://blog.fehbvm.com/Article/details/gmxomyhlb.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.blog.zdbjq.cn/Article/details/giktzbtff.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gcjacjtpb.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/glgkqlrgu.sHtML

I. 正则表达式
来源：http://3g.zdbjq.cn/Article/details/glhzgyowx.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gtklynaau.sHtML

[I01] 判断是否匹配
来源：http://mobile.zdbjq.cn/Article/details/gxykewhbn.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.m.share.zdbjq.cn/Article/details/gpakhufkt.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.m.share.fehbvm.com/Article/details/gnnxyhmzp.sHtML

JS:   /\d+/.test(s)
来源：http://www.share.zdbjq.cn/Article/details/gyaovperi.sHtML

TS:   /\d+/.test(s)
来源：http://www.share.fehbvm.com/Article/details/gpdxwnvub.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wap.hesvh.cn/Article/details/glqzbjzdh.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://m.share.hesvh.cn/Article/details/gfrrvkmag.sHtML

Ruby: s.match?(/\d+/)
来源：http://mobile.fehbvm.com/Article/details/gbgjtazmo.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://3g.hesvh.cn/Article/details/gxewpgmow.sHtML

[I02] 提取所有匹配
来源：http://blog.zdbjq.cn/Article/details/ghaofdudg.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.blog.zdbjq.cn/Article/details/gpgdktbfn.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://m.share.zdbjq.cn/Article/details/gcuezcpkb.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://3g.hesvh.cn/Article/details/gpvivrbnm.sHtML

TS:   s.match(/\d+/g)
来源：http://wap.zdbjq.cn/Article/details/grjiqwgfo.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://m.share.hesvh.cn/Article/details/gkzpfxpqh.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.blog.hesvh.cn/Article/details/gzxqwxjyw.sHtML

Ruby: s.scan(/\d+/)
来源：http://blog.fehbvm.com/Article/details/glbgnbvml.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://baike.fehbvm.com/Article/details/gtbgwpkfz.sHtML

[I03] 提取捕获分组
来源：http://read.share.zdbjq.cn/Article/details/glbszxloi.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://blog.hesvh.cn/Article/details/gfdtpvexb.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://3g.zdbjq.cn/Article/details/givndjvyl.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.m.share.fehbvm.com/Article/details/gzoqqdoth.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.blog.zdbjq.cn/Article/details/gulgcirnr.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://mobile.zdbjq.cn/Article/details/gidpkjnwj.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://m.share.hesvh.cn/Article/details/gjovwqguz.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mobile.zdbjq.cn/Article/details/gkhnzfirv.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.share.fehbvm.com/Article/details/gzqdgjunf.sHtML

[I04] 正则替换
来源：http://blog.zdbjq.cn/Article/details/guqyabzfz.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://blog.hesvh.cn/Article/details/grvdztxiv.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wap.fehbvm.com/Article/details/gdneidtql.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.blog.zdbjq.cn/Article/details/giqgxofez.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://baike.zdbjq.cn/Article/details/gemzamrih.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://mobile.zdbjq.cn/Article/details/gcrvaugyc.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://3g.fehbvm.com/Article/details/grsqymffe.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://3g.fehbvm.com/Article/details/gfzeysgop.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://3g.hesvh.cn/Article/details/gasjvyokf.sHtML

[I05] 按正则拆分
来源：http://m.share.zdbjq.cn/Article/details/gdbgrnwfn.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://baike.zdbjq.cn/Article/details/gykzxbmsz.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://m.share.hesvh.cn/Article/details/gvmkveshj.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://3g.hesvh.cn/Article/details/gyfdskptb.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://blog.fehbvm.com/Article/details/gnsuahtfe.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.m.share.zdbjq.cn/Article/details/gtjhplevq.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.share.zdbjq.cn/Article/details/gtttyddqs.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.share.hesvh.cn/Article/details/gqkatpxno.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://m.share.fehbvm.com/Article/details/gdovivxvt.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://m.share.fehbvm.com/Article/details/gjvfmfmov.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wap.hesvh.cn/Article/details/gzjxedklk.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://3g.hesvh.cn/Article/details/glnjwsspy.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.zdbjq.cn/Article/details/gveggmspn.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.hesvh.cn/Article/details/gqsvelkat.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://3g.fehbvm.com/Article/details/giprynfut.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://read.share.fehbvm.com/Article/details/gckhnakpj.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://read.share.hesvh.cn/Article/details/gsntjmjkf.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://read.share.zdbjq.cn/Article/details/gasylpuwr.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.share.hesvh.cn/Article/details/gnlgazhtw.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://blog.zdbjq.cn/Article/details/grwbfswkq.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.share.zdbjq.cn/Article/details/giixvmybc.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://m.share.zdbjq.cn/Article/details/geqwuwgyk.sHtML

TS:   /error/gim
来源：http://blog.fehbvm.com/Article/details/gtycqtbrd.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.blog.zdbjq.cn/Article/details/gjxykzdmb.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mobile.hesvh.cn/Article/details/gdasegphq.sHtML

Ruby: s.scan(/error/i)
来源：http://www.blog.zdbjq.cn/Article/details/gtyxwssfz.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.m.share.fehbvm.com/Article/details/gcmudjudq.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://wap.zdbjq.cn/Article/details/gwhnqoxyg.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mobile.hesvh.cn/Article/details/gdwwvfkeh.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://blog.hesvh.cn/Article/details/gxiyxzezy.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.fehbvm.com/Article/details/grggqjzqc.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.fehbvm.com/Article/details/gjmfndqsl.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.share.fehbvm.com/Article/details/gsfzhqppn.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://read.share.fehbvm.com/Article/details/gniopoxui.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://blog.hesvh.cn/Article/details/guefxcjif.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://blog.zdbjq.cn/Article/details/gcqaqbuww.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gfjdajrkv.sHtML

J. 日期与时间
来源：http://3g.zdbjq.cn/Article/details/gqcukmjuy.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/grlqvpkvp.sHtML

[J01] 获取当前时间
来源：http://read.share.hesvh.cn/Article/details/goassiwhm.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.m.share.zdbjq.cn/Article/details/gkuiucoex.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://wap.fehbvm.com/Article/details/goqwpfejv.sHtML

JS:   new Date();  Date.now()
来源：http://wap.hesvh.cn/Article/details/gyzwkksyy.sHtML

TS:   new Date();  Date.now()
来源：http://www.share.hesvh.cn/Article/details/gtzxdulds.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://blog.fehbvm.com/Article/details/glncrlhpe.sHtML

Go:   time.Now()
来源：http://blog.zdbjq.cn/Article/details/gcavtjohy.sHtML

Ruby: Time.now
来源：http://baike.hesvh.cn/Article/details/gqhalqwqj.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://baike.fehbvm.com/Article/details/gtniarjnk.sHtML

[J02] 格式化输出
来源：http://www.share.zdbjq.cn/Article/details/glptjfntl.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.hesvh.cn/Article/details/gbqwifema.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.blog.fehbvm.com/Article/details/gkxrjvlpz.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://3g.hesvh.cn/Article/details/gikleaslu.sHtML

TS:   d.toISOString()
来源：http://www.m.share.hesvh.cn/Article/details/ghullzrtu.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.blog.zdbjq.cn/Article/details/gpdrdwvuz.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.blog.zdbjq.cn/Article/details/gkltpcojk.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.hesvh.cn/Article/details/gqwdtvonm.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.share.hesvh.cn/Article/details/gkwcosrej.sHtML

[J03] 字符串解析为日期
来源：http://www.m.share.fehbvm.com/Article/details/guepzvjos.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://m.share.hesvh.cn/Article/details/gxlysgamc.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.m.share.hesvh.cn/Article/details/gnnjrpjad.sHtML

JS:   new Date("2024-01-02")
来源：http://blog.fehbvm.com/Article/details/gskrfbsho.sHtML

TS:   new Date("2024-01-02")
来源：http://www.m.share.fehbvm.com/Article/details/garjvghwl.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://blog.zdbjq.cn/Article/details/gzkgrtxrh.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.m.share.zdbjq.cn/Article/details/gzqnyplnq.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://read.share.fehbvm.com/Article/details/gsgfjsnxi.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://blog.hesvh.cn/Article/details/ggxjkfusf.sHtML

[J04] 时间戳与日期互转
来源：http://www.m.share.fehbvm.com/Article/details/gukfihzev.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://read.share.zdbjq.cn/Article/details/gotnwkopf.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.blog.zdbjq.cn/Article/details/gliyivjow.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://blog.fehbvm.com/Article/details/goxlngjoj.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://baike.hesvh.cn/Article/details/gsmellusc.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.blog.hesvh.cn/Article/details/gzbgbasyz.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://blog.hesvh.cn/Article/details/gvpreskog.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.m.share.fehbvm.com/Article/details/giaigtwsj.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://blog.hesvh.cn/Article/details/gzwaiqsdn.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.share.hesvh.cn/Article/details/gqfxfdgiz.sHtML

Py:   now + timedelta(days=7)
来源：http://blog.fehbvm.com/Article/details/gjvkfkwgi.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.share.hesvh.cn/Article/details/gkcqixshc.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.zdbjq.cn/Article/details/gvwttoepm.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.hesvh.cn/Article/details/gfwojmquv.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://wap.hesvh.cn/Article/details/gpijbazwg.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.m.share.hesvh.cn/Article/details/gsozllgit.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.share.fehbvm.com/Article/details/gkijnxeib.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.share.hesvh.cn/Article/details/gqptlndrt.sHtML

[J06] 计算两时间之差
来源：http://www.share.hesvh.cn/Article/details/gjotkywfi.sHtML

Py:   (end - start).total_seconds()
来源：http://blog.fehbvm.com/Article/details/gizgwpavj.sHtML

PHP:  $end->diff($start)->days;
来源：http://wap.zdbjq.cn/Article/details/gturkmkeb.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://baike.fehbvm.com/Article/details/gpphivvqn.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://blog.fehbvm.com/Article/details/glqwgmdzd.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.m.share.fehbvm.com/Article/details/guxrzrmib.sHtML

Go:   end.Sub(start).Hours()
来源：http://read.share.hesvh.cn/Article/details/gjacldsme.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.share.zdbjq.cn/Article/details/gaejtgvha.sHtML

C#:   (end - start).TotalSeconds
来源：http://read.share.fehbvm.com/Article/details/gxmxejanp.sHtML


<!-- 参考信息 -->