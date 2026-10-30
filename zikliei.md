代发 wailian999

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.hesvh.cn/Article/details/gadhebhdi.sHtML

Ruby: def self.f; end
来源：http://mobile.zdbjq.cn/Article/details/gvfhtuvea.sHtML

C#:   public static void F() {}
来源：http://mobile.hesvh.cn/Article/details/ghoomllmz.sHtML

[G09] 接口 / 抽象类
来源：http://blog.fehbvm.com/Article/details/gqsikimee.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.zdbjq.cn/Article/details/gvucwvmox.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.fehbvm.com/Article/details/gtaznsfhi.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.zdbjq.cn/Article/details/gzdckbxay.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.hesvh.cn/Article/details/ggixqdaos.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.zdbjq.cn/Article/details/gkzgnypmw.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.zdbjq.cn/Article/details/ghawgjwmn.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.zdbjq.cn/Article/details/ggxcgrggh.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.hesvh.cn/Article/details/gcxwhkzad.sHtML

[G10] 访问控制
来源：http://www.share.zdbjq.cn/Article/details/gaxfhvjth.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.zdbjq.cn/Article/details/gxxniqnsf.sHtML

PHP:  public / protected / private
来源：http://mobile.zdbjq.cn/Article/details/gsjwypcyy.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.fehbvm.com/Article/details/gxffizpla.sHtML

TS:   public / protected / private
来源：http://mobile.zdbjq.cn/Article/details/gfztdbkkf.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.zdbjq.cn/Article/details/gixidddpq.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.hesvh.cn/Article/details/gpeqnkorp.sHtML

Ruby: public / protected / private
来源：http://m.share.fehbvm.com/Article/details/gxkecemka.sHtML

C#:   public / protected / private / internal
来源：http://blog.hesvh.cn/Article/details/gvnzqchzj.sHtML

[G11] getter / setter
来源：http://3g.fehbvm.com/Article/details/gfzgdesbk.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.zdbjq.cn/Article/details/gbiujsbis.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.hesvh.cn/Article/details/gsipzvupy.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.hesvh.cn/Article/details/gilaogiau.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.hesvh.cn/Article/details/gsnjdimtd.sHtML

Java: public String getName() { return name; }
来源：http://read.share.hesvh.cn/Article/details/gplirbczk.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.zdbjq.cn/Article/details/gmjytyjvg.sHtML

Ruby: attr_accessor :name
来源：http://www.share.zdbjq.cn/Article/details/gwjsmlihg.sHtML

C#:   public string Name { get; set; }
来源：http://baike.hesvh.cn/Article/details/gvbysvgli.sHtML

[G12] 对象转字符串
来源：http://read.share.zdbjq.cn/Article/details/gxsxyznan.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.fehbvm.com/Article/details/gjihlejgw.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.fehbvm.com/Article/details/gbtxddufb.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/gtfohsmhu.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gdgznuacl.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.fehbvm.com/Article/details/gchpjmdjk.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.fehbvm.com/Article/details/gabxxkhhj.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.zdbjq.cn/Article/details/gmpalsmwt.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.zdbjq.cn/Article/details/gocfmbnmi.sHtML

[G13] 判断对象类型
来源：http://m.share.zdbjq.cn/Article/details/gvhmqkwfw.sHtML

Py:   isinstance(u, User)
来源：http://blog.fehbvm.com/Article/details/gycencahh.sHtML

PHP:  $u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/gxzzcvtno.sHtML

JS:   u instanceof User
来源：http://wap.fehbvm.com/Article/details/gtdpbqdzt.sHtML

TS:   u instanceof User
来源：http://blog.zdbjq.cn/Article/details/gmiazargf.sHtML

Java: u instanceof User
来源：http://read.share.fehbvm.com/Article/details/gdlmnmtks.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.hesvh.cn/Article/details/glnazmxvj.sHtML

Ruby: u.is_a?(User)
来源：http://blog.hesvh.cn/Article/details/gesjtxcop.sHtML

C#:   u is User
来源：http://m.share.fehbvm.com/Article/details/gyhthgflg.sHtML

[G14] 数据类 / record
来源：http://3g.fehbvm.com/Article/details/gsskaenii.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.zdbjq.cn/Article/details/gviwsmxkm.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.fehbvm.com/Article/details/gcnsqfbyh.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.zdbjq.cn/Article/details/gerpifahg.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.hesvh.cn/Article/details/gyzrpjvtz.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.fehbvm.com/Article/details/gdjcbntgg.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.zdbjq.cn/Article/details/gywkqfmis.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.zdbjq.cn/Article/details/ghqscahcd.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.zdbjq.cn/Article/details/gkpkobnfq.sHtML

[G15] 枚举
来源：http://baike.fehbvm.com/Article/details/gkyowgvtr.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.hesvh.cn/Article/details/gbfcssggd.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.hesvh.cn/Article/details/gkndwkgrf.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.hesvh.cn/Article/details/gbgvoduyl.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.zdbjq.cn/Article/details/gfsqingwn.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.fehbvm.com/Article/details/genyrsgoq.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.fehbvm.com/Article/details/gdgsjzawl.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.fehbvm.com/Article/details/gxabnqfwe.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.zdbjq.cn/Article/details/gxohpsnhg.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.hesvh.cn/Article/details/gjnbllnkn.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.blog.fehbvm.com/Article/details/grhewsmye.sHtML

PHP:  get_object_vars($obj);
来源：http://wap.fehbvm.com/Article/details/gewtslulf.sHtML

JS:   Object.entries(obj)
来源：http://mobile.zdbjq.cn/Article/details/glaheomcd.sHtML

TS:   Object.entries(obj)
来源：http://mobile.fehbvm.com/Article/details/gjdsltxoa.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.fehbvm.com/Article/details/garqlnglt.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.fehbvm.com/Article/details/gpefmdofs.sHtML

Ruby: obj.instance_variables
来源：http://baike.fehbvm.com/Article/details/gnxwenpgn.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.hesvh.cn/Article/details/grarwacmn.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gixykakin.sHtML

H. 异常与错误处理
来源：http://blog.zdbjq.cn/Article/details/giyzmnjxi.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gggprlqkr.sHtML

[H01] try / catch 基础
来源：http://mobile.fehbvm.com/Article/details/gvtarobyy.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.hesvh.cn/Article/details/gfjrvbyaz.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.blog.fehbvm.com/Article/details/ghsudbria.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.share.fehbvm.com/Article/details/gujgefphk.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://m.share.fehbvm.com/Article/details/gokrkeocn.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://baike.hesvh.cn/Article/details/grsrvlfrk.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://read.share.zdbjq.cn/Article/details/gzvfjtiof.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wap.hesvh.cn/Article/details/geghzcoyv.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mobile.fehbvm.com/Article/details/gyqslhhls.sHtML

[H02] finally / ensure 收尾
来源：http://wap.fehbvm.com/Article/details/gjummwoxe.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.fehbvm.com/Article/details/gmnkhuegh.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://3g.zdbjq.cn/Article/details/gjivvkvqu.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://mobile.zdbjq.cn/Article/details/gysxtiktq.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://baike.hesvh.cn/Article/details/gkklhwwfp.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/gfrwxurdd.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://m.share.zdbjq.cn/Article/details/gwpihmxgk.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.zdbjq.cn/Article/details/gwgsfxfvd.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.share.fehbvm.com/Article/details/ggbilufoy.sHtML

[H03] 主动抛出异常
来源：http://www.share.fehbvm.com/Article/details/gfliqociq.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.share.fehbvm.com/Article/details/goiejckrw.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.hesvh.cn/Article/details/gsomwjjfb.sHtML

JS:   throw new Error("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/gemevkqtx.sHtML

TS:   throw new Error("错误信息");
来源：http://www.blog.zdbjq.cn/Article/details/genonkkqp.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.blog.fehbvm.com/Article/details/gspgraixp.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://baike.zdbjq.cn/Article/details/gcgmhgrbp.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://wap.zdbjq.cn/Article/details/gkqvhltsf.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://blog.zdbjq.cn/Article/details/gocbioddf.sHtML

[H04] 自定义异常类型
来源：http://blog.hesvh.cn/Article/details/ghbkrtqyq.sHtML

Py:   class MyError(Exception): pass
来源：http://baike.hesvh.cn/Article/details/gnkzxfddu.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://baike.hesvh.cn/Article/details/gjhkmqwaj.sHtML

JS:   class MyError extends Error {}
来源：http://m.share.hesvh.cn/Article/details/gsqvwnaeu.sHtML

TS:   class MyError extends Error {}
来源：http://blog.fehbvm.com/Article/details/gkwugbzjf.sHtML

Java: class MyException extends RuntimeException {}
来源：http://m.share.fehbvm.com/Article/details/gxtblmfzt.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mobile.hesvh.cn/Article/details/gozhxsusf.sHtML

Ruby: class MyError < StandardError; end
来源：http://m.share.zdbjq.cn/Article/details/gddtqdhmo.sHtML

C#:   class MyException : Exception {}
来源：http://wap.zdbjq.cn/Article/details/goaredzoc.sHtML

[H05] 捕获特定类型
来源：http://3g.zdbjq.cn/Article/details/gahngvfwh.sHtML

Py:   except ValueError as e:
来源：http://m.share.fehbvm.com/Article/details/gkhbfdzqs.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.m.share.zdbjq.cn/Article/details/grzduihiu.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.blog.zdbjq.cn/Article/details/grcydfhoc.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://3g.zdbjq.cn/Article/details/gupjkhhxo.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://read.share.hesvh.cn/Article/details/gdwcfrrcj.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://3g.hesvh.cn/Article/details/gmubmpkbd.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.blog.fehbvm.com/Article/details/gibtbwjmo.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://m.share.zdbjq.cn/Article/details/grkucurpk.sHtML

[H06] 可选值 / 空值安全访问
来源：http://read.share.hesvh.cn/Article/details/gqqdvxgvs.sHtML

Py:   value = d.get("k") or default
来源：http://baike.zdbjq.cn/Article/details/gughojjhg.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://mobile.hesvh.cn/Article/details/gpmltvbnc.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://blog.fehbvm.com/Article/details/gwbnnblxb.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://blog.fehbvm.com/Article/details/gfcmrnfjq.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://3g.hesvh.cn/Article/details/gyzvcijcp.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://3g.zdbjq.cn/Article/details/gmtijkldr.sHtML

Ruby: d&.dig(:a, :b)
来源：http://3g.zdbjq.cn/Article/details/gyoicxzzz.sHtML

C#:   obj?.A?.B ?? default
来源：http://3g.hesvh.cn/Article/details/geihvkvky.sHtML

[H07] 断言
来源：http://mobile.fehbvm.com/Article/details/gmidohmpx.sHtML

Py:   assert x > 0, "必须为正"
来源：http://blog.zdbjq.cn/Article/details/gduagycnw.sHtML

PHP:  assert($x > 0);
来源：http://3g.hesvh.cn/Article/details/gcvuvqqgc.sHtML

JS:   console.assert(x > 0);
来源：http://3g.hesvh.cn/Article/details/gcpyiifym.sHtML

TS:   console.assert(x > 0);
来源：http://www.blog.hesvh.cn/Article/details/gaakriucb.sHtML

Java: assert x > 0 : "必须为正";
来源：http://blog.hesvh.cn/Article/details/gbrnovtij.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.blog.zdbjq.cn/Article/details/ganbprleu.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://blog.fehbvm.com/Article/details/gtjrmkugu.sHtML

C#:   Debug.Assert(x > 0);
来源：http://blog.fehbvm.com/Article/details/gcbzkbysb.sHtML

[H08] 获取错误信息与堆栈
来源：http://mobile.fehbvm.com/Article/details/gbezwnccp.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://mobile.hesvh.cn/Article/details/gbaeqmnse.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://read.share.hesvh.cn/Article/details/grkhfgvrp.sHtML

JS:   e.message;  e.stack
来源：http://www.blog.fehbvm.com/Article/details/gzuddwssc.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://read.share.zdbjq.cn/Article/details/grlxbvqme.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.blog.hesvh.cn/Article/details/gkbakkjhx.sHtML

Go:   err.Error()
来源：http://m.share.zdbjq.cn/Article/details/gdehopysb.sHtML

Ruby: e.message;  e.backtrace
来源：http://mobile.fehbvm.com/Article/details/gmogkrhxu.sHtML

C#:   e.Message;  e.StackTrace
来源：http://mobile.hesvh.cn/Article/details/gueuafxvd.sHtML

[H09] 带错误码的异常
来源：http://mobile.zdbjq.cn/Article/details/gcrtvsfoj.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.blog.fehbvm.com/Article/details/gqawvolhl.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.share.zdbjq.cn/Article/details/gdkicsbvr.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.blog.hesvh.cn/Article/details/gaydcufmk.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.blog.fehbvm.com/Article/details/ghhitbsud.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://m.share.fehbvm.com/Article/details/gptccnvli.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.m.share.fehbvm.com/Article/details/gotdnlanm.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://wap.zdbjq.cn/Article/details/gvnmnxgxm.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://read.share.hesvh.cn/Article/details/gdldaztju.sHtML

[H10] 资源自动释放
来源：http://www.blog.zdbjq.cn/Article/details/gsytoqoxa.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.blog.zdbjq.cn/Article/details/gcnyulwlb.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://blog.hesvh.cn/Article/details/gdxqnfubn.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.hesvh.cn/Article/details/gngzaqjpv.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.fehbvm.com/Article/details/gibkacbyn.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://m.share.hesvh.cn/Article/details/ghbpdxmof.sHtML

Go:   defer f.Close()
来源：http://wap.fehbvm.com/Article/details/gmqrujjhv.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.share.fehbvm.com/Article/details/gddhcdtts.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gbihxfzuj.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/glybcaorq.sHtML

I. 正则表达式
来源：http://www.blog.fehbvm.com/Article/details/gigfdgwrf.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gscnhqyld.sHtML

[I01] 判断是否匹配
来源：http://www.share.fehbvm.com/Article/details/gvnhzvdyr.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mobile.fehbvm.com/Article/details/gtglfyoiu.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.m.share.hesvh.cn/Article/details/guumaywax.sHtML

JS:   /\d+/.test(s)
来源：http://mobile.hesvh.cn/Article/details/golbxamra.sHtML

TS:   /\d+/.test(s)
来源：http://3g.zdbjq.cn/Article/details/guijyfzdy.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mobile.hesvh.cn/Article/details/gtlbnslov.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://3g.zdbjq.cn/Article/details/gkfkggfvf.sHtML

Ruby: s.match?(/\d+/)
来源：http://mobile.hesvh.cn/Article/details/gisihmxnd.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://baike.zdbjq.cn/Article/details/gcetdtdxn.sHtML

[I02] 提取所有匹配
来源：http://blog.zdbjq.cn/Article/details/gfmwgbsxh.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.share.fehbvm.com/Article/details/gyxoexahs.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://3g.zdbjq.cn/Article/details/gvvdffqwb.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.blog.hesvh.cn/Article/details/ggmeqzvni.sHtML

TS:   s.match(/\d+/g)
来源：http://baike.fehbvm.com/Article/details/gtukqftei.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.m.share.hesvh.cn/Article/details/gsgppdftx.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://baike.zdbjq.cn/Article/details/grxchkgnh.sHtML

Ruby: s.scan(/\d+/)
来源：http://blog.zdbjq.cn/Article/details/grudduvli.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gdwolyalw.sHtML

[I03] 提取捕获分组
来源：http://www.m.share.fehbvm.com/Article/details/gsjrzvflk.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.share.fehbvm.com/Article/details/gtmbrsccq.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.m.share.zdbjq.cn/Article/details/gqmykldsy.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mobile.zdbjq.cn/Article/details/ggaklcsyg.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://baike.hesvh.cn/Article/details/glgnapeso.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://m.share.fehbvm.com/Article/details/gbunkajbi.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wap.hesvh.cn/Article/details/gclutsxub.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://baike.fehbvm.com/Article/details/gcrkxpjvf.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://blog.zdbjq.cn/Article/details/gzeoldwtk.sHtML

[I04] 正则替换
来源：http://www.m.share.fehbvm.com/Article/details/gpyquhkzu.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://mobile.fehbvm.com/Article/details/geluwbent.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.fehbvm.com/Article/details/gzvwpbdbr.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://read.share.fehbvm.com/Article/details/ghcsiqwka.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://3g.fehbvm.com/Article/details/gmwedmugw.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.blog.fehbvm.com/Article/details/goceydjhm.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://mobile.zdbjq.cn/Article/details/grotejrih.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.blog.fehbvm.com/Article/details/gbqfzvprl.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.share.hesvh.cn/Article/details/gjfialclg.sHtML

[I05] 按正则拆分
来源：http://www.m.share.hesvh.cn/Article/details/gskbnkswe.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://baike.hesvh.cn/Article/details/gfczstjds.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://blog.zdbjq.cn/Article/details/gurzyoezt.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.m.share.hesvh.cn/Article/details/gqzycpqgx.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://blog.zdbjq.cn/Article/details/gavpfubyg.sHtML

Java: s.split("\\s*,\\s*")
来源：http://wap.zdbjq.cn/Article/details/glmhhsxsf.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.share.hesvh.cn/Article/details/gdqqtvoty.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://mobile.zdbjq.cn/Article/details/gbdbhzomf.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mobile.zdbjq.cn/Article/details/gpbwsmsvh.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://m.share.fehbvm.com/Article/details/gukoxusgl.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://m.share.zdbjq.cn/Article/details/grsyayeim.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://read.share.zdbjq.cn/Article/details/gekyjmjqz.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.hesvh.cn/Article/details/gllfohmvg.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.fehbvm.com/Article/details/gyibnohaw.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wap.zdbjq.cn/Article/details/gjpggcgrd.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://blog.zdbjq.cn/Article/details/gkctyxhch.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wap.fehbvm.com/Article/details/giudunszp.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://read.share.hesvh.cn/Article/details/gtnzrhnkx.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.m.share.zdbjq.cn/Article/details/gfzxnmqtc.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wap.hesvh.cn/Article/details/gqyeyrxok.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.share.fehbvm.com/Article/details/gddotyfgv.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.blog.hesvh.cn/Article/details/ggvwxcutz.sHtML

TS:   /error/gim
来源：http://baike.zdbjq.cn/Article/details/glrocxswv.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://3g.fehbvm.com/Article/details/gfinivfmo.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://m.share.fehbvm.com/Article/details/gntufuadq.sHtML

Ruby: s.scan(/error/i)
来源：http://wap.fehbvm.com/Article/details/gwbxymnee.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://wap.fehbvm.com/Article/details/gtcquhhsw.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.share.hesvh.cn/Article/details/glgprmgae.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.blog.hesvh.cn/Article/details/geoqtkvnx.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wap.zdbjq.cn/Article/details/gxwggaekr.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.hesvh.cn/Article/details/gulucuyeg.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.zdbjq.cn/Article/details/gbmrubica.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://m.share.zdbjq.cn/Article/details/giolvgcmg.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.share.fehbvm.com/Article/details/gkupehqvc.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.m.share.zdbjq.cn/Article/details/gtjcjqwhj.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://read.share.hesvh.cn/Article/details/gjttzzqqm.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gnltfigni.sHtML

J. 日期与时间
来源：http://wap.fehbvm.com/Article/details/gisnfzxtr.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/grejbmuto.sHtML

[J01] 获取当前时间
来源：http://www.blog.zdbjq.cn/Article/details/gvozdkfle.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://read.share.zdbjq.cn/Article/details/gieqiwtku.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.m.share.hesvh.cn/Article/details/gecgjfpzz.sHtML

JS:   new Date();  Date.now()
来源：http://blog.fehbvm.com/Article/details/gzbwoxrkc.sHtML

TS:   new Date();  Date.now()
来源：http://wap.hesvh.cn/Article/details/gshqcpydh.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://blog.zdbjq.cn/Article/details/gitqztreo.sHtML

Go:   time.Now()
来源：http://www.blog.hesvh.cn/Article/details/ghhhumjky.sHtML

Ruby: Time.now
来源：http://mobile.hesvh.cn/Article/details/guwlplxus.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.blog.fehbvm.com/Article/details/gfxlzucdl.sHtML

[J02] 格式化输出
来源：http://www.share.fehbvm.com/Article/details/grhylylwa.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.zdbjq.cn/Article/details/gsdbvkptv.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.share.hesvh.cn/Article/details/gkhptgefz.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mobile.zdbjq.cn/Article/details/gaamhkwcb.sHtML

TS:   d.toISOString()
来源：http://read.share.hesvh.cn/Article/details/gzmswnqot.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.blog.zdbjq.cn/Article/details/gpdkcrpzo.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.blog.hesvh.cn/Article/details/gspourakx.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.hesvh.cn/Article/details/gwadforwx.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.share.zdbjq.cn/Article/details/gbdobwtyd.sHtML

[J03] 字符串解析为日期
来源：http://baike.zdbjq.cn/Article/details/gucadpiai.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://blog.hesvh.cn/Article/details/gzlmtlirt.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.m.share.hesvh.cn/Article/details/gfwetmobg.sHtML

JS:   new Date("2024-01-02")
来源：http://3g.fehbvm.com/Article/details/guesyxiin.sHtML

TS:   new Date("2024-01-02")
来源：http://www.m.share.zdbjq.cn/Article/details/gjuqihccv.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.share.zdbjq.cn/Article/details/gnwsrufrq.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://m.share.hesvh.cn/Article/details/gkbwdmhbx.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.share.zdbjq.cn/Article/details/geykgyqww.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mobile.fehbvm.com/Article/details/ghcdhpnxs.sHtML

[J04] 时间戳与日期互转
来源：http://www.share.zdbjq.cn/Article/details/gwgxvlups.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.share.fehbvm.com/Article/details/gkvvynkls.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://m.share.fehbvm.com/Article/details/gheeuydrg.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://read.share.hesvh.cn/Article/details/goqzcmvpv.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.blog.fehbvm.com/Article/details/gwyhookiz.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.blog.fehbvm.com/Article/details/gyjmycwhz.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wap.zdbjq.cn/Article/details/gcjpzvtyf.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.share.hesvh.cn/Article/details/gqomezhke.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://mobile.hesvh.cn/Article/details/gidyaoran.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.m.share.fehbvm.com/Article/details/gglyodtuh.sHtML

Py:   now + timedelta(days=7)
来源：http://wap.zdbjq.cn/Article/details/gtzstgbtu.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://3g.hesvh.cn/Article/details/gmzdelpxu.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.zdbjq.cn/Article/details/gwrjsgufh.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.zdbjq.cn/Article/details/glfdjaktc.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://mobile.fehbvm.com/Article/details/gylgdscjm.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://3g.hesvh.cn/Article/details/gtkrooqfo.sHtML

Ruby: Time.now + 7 * 86400
来源：http://3g.hesvh.cn/Article/details/gfprzcknu.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://read.share.fehbvm.com/Article/details/gtxuamcep.sHtML

[J06] 计算两时间之差
来源：http://wap.fehbvm.com/Article/details/geryqwxcs.sHtML

Py:   (end - start).total_seconds()
来源：http://mobile.fehbvm.com/Article/details/gulmjjfyh.sHtML

PHP:  $end->diff($start)->days;
来源：http://baike.hesvh.cn/Article/details/gzbwyoffd.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://blog.fehbvm.com/Article/details/gsygjhowk.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://baike.zdbjq.cn/Article/details/gdqjiestv.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://wap.zdbjq.cn/Article/details/gwjtdbhxx.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.m.share.zdbjq.cn/Article/details/gdmsjpztv.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.m.share.zdbjq.cn/Article/details/gxirpiqxv.sHtML

C#:   (end - start).TotalSeconds
来源：http://baike.hesvh.cn/Article/details/ghxepioai.sHtML


<!-- 参考信息 -->