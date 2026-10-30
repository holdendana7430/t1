代发 wailian999

Py:   from abc import ABC, abstractmethod
来源：http://m.share.fehbvm.com/Article/details/gnhxtrkor.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.hesvh.cn/Article/details/grzmenugr.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.fehbvm.com/Article/details/gqnodfmih.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.hesvh.cn/Article/details/gjfmklfaq.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.hesvh.cn/Article/details/grugavhgo.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.zdbjq.cn/Article/details/guxutzyqt.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.hesvh.cn/Article/details/gpyexqijs.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.fehbvm.com/Article/details/guylfwfcy.sHtML

[G10] 访问控制
来源：http://wap.fehbvm.com/Article/details/gildikukp.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.fehbvm.com/Article/details/gslvhdokj.sHtML

PHP:  public / protected / private
来源：http://wap.fehbvm.com/Article/details/gwhrwvkku.sHtML

JS:   #private 字段；其余公开
来源：http://3g.fehbvm.com/Article/details/gtgpjywik.sHtML

TS:   public / protected / private
来源：http://wap.zdbjq.cn/Article/details/gnzzfizzl.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.fehbvm.com/Article/details/gsudctxkj.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.hesvh.cn/Article/details/gbturafzr.sHtML

Ruby: public / protected / private
来源：http://3g.zdbjq.cn/Article/details/gxvdjauav.sHtML

C#:   public / protected / private / internal
来源：http://mobile.fehbvm.com/Article/details/gyfjnmohx.sHtML

[G11] getter / setter
来源：http://www.share.fehbvm.com/Article/details/gqdamslub.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.fehbvm.com/Article/details/gvcuqwybu.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.hesvh.cn/Article/details/gmzjsbtxt.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.zdbjq.cn/Article/details/gyrcyjujm.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.hesvh.cn/Article/details/gviqhknuy.sHtML

Java: public String getName() { return name; }
来源：http://m.share.zdbjq.cn/Article/details/gxpmambwe.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.hesvh.cn/Article/details/gqeteckov.sHtML

Ruby: attr_accessor :name
来源：http://wap.hesvh.cn/Article/details/ghiyalddd.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.hesvh.cn/Article/details/gnnmkziht.sHtML

[G12] 对象转字符串
来源：http://wap.hesvh.cn/Article/details/gotrmzneq.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.hesvh.cn/Article/details/gmiqbrwcf.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.zdbjq.cn/Article/details/gtfblwvdj.sHtML

JS:   toString() { return this.name; }
来源：http://3g.fehbvm.com/Article/details/gpobjggvf.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.zdbjq.cn/Article/details/gyjndmncw.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/gupizyihy.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.zdbjq.cn/Article/details/gllfijtti.sHtML

Ruby: def to_s; @name; end
来源：http://blog.zdbjq.cn/Article/details/gaacmhslv.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.hesvh.cn/Article/details/gawigjgns.sHtML

[G13] 判断对象类型
来源：http://www.share.zdbjq.cn/Article/details/gpsnvbwpe.sHtML

Py:   isinstance(u, User)
来源：http://3g.zdbjq.cn/Article/details/gfdrnhwox.sHtML

PHP:  $u instanceof User
来源：http://blog.zdbjq.cn/Article/details/geityfrts.sHtML

JS:   u instanceof User
来源：http://www.share.fehbvm.com/Article/details/gunmzoxlf.sHtML

TS:   u instanceof User
来源：http://mobile.fehbvm.com/Article/details/ghnoepcyh.sHtML

Java: u instanceof User
来源：http://wap.fehbvm.com/Article/details/golvyewpx.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.zdbjq.cn/Article/details/gikeayvjs.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.zdbjq.cn/Article/details/gmebimeqo.sHtML

C#:   u is User
来源：http://3g.zdbjq.cn/Article/details/gayvxxraz.sHtML

[G14] 数据类 / record
来源：http://wap.hesvh.cn/Article/details/gzwqnzpqa.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://3g.hesvh.cn/Article/details/gomylbizw.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.zdbjq.cn/Article/details/gmjbybogv.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.fehbvm.com/Article/details/gvnbbgkpa.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.zdbjq.cn/Article/details/glohbxznv.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.zdbjq.cn/Article/details/gtvqllfad.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.zdbjq.cn/Article/details/giebphccb.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.zdbjq.cn/Article/details/gdpxzgbpt.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.hesvh.cn/Article/details/gbztwoyzg.sHtML

[G15] 枚举
来源：http://mobile.hesvh.cn/Article/details/gavsjohlm.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.zdbjq.cn/Article/details/glyjmwxjj.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://baike.zdbjq.cn/Article/details/gmycbjdyo.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.hesvh.cn/Article/details/gmlyckpfg.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.hesvh.cn/Article/details/gyuoxkjrd.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.hesvh.cn/Article/details/gxsqptvli.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.fehbvm.com/Article/details/gqrpiwtwb.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.hesvh.cn/Article/details/ghzoiytvc.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.fehbvm.com/Article/details/gamxczzrg.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.hesvh.cn/Article/details/gdgqlnvxv.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.hesvh.cn/Article/details/gtzemqbwg.sHtML

PHP:  get_object_vars($obj);
来源：http://blog.hesvh.cn/Article/details/grilepaso.sHtML

JS:   Object.entries(obj)
来源：http://www.share.hesvh.cn/Article/details/gtnhsbyfq.sHtML

TS:   Object.entries(obj)
来源：http://www.blog.fehbvm.com/Article/details/giruabsyl.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.hesvh.cn/Article/details/gpqeykygc.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.zdbjq.cn/Article/details/grflixkre.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.hesvh.cn/Article/details/gfsybqinl.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.zdbjq.cn/Article/details/gaodlyvhq.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gctrliuvq.sHtML

H. 异常与错误处理
来源：http://wap.fehbvm.com/Article/details/ghnoygldu.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gpkjiphoj.sHtML

[H01] try / catch 基础
来源：http://read.share.fehbvm.com/Article/details/gfwoqpcid.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://read.share.zdbjq.cn/Article/details/ghdqcgjrz.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.fehbvm.com/Article/details/gpquebxjn.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://m.share.fehbvm.com/Article/details/gbhewublu.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.hesvh.cn/Article/details/gscpfrqmz.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://baike.zdbjq.cn/Article/details/gndkfuutc.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.m.share.fehbvm.com/Article/details/gxyhfgmor.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.m.share.hesvh.cn/Article/details/ganovqxik.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.fehbvm.com/Article/details/giqmafola.sHtML

[H02] finally / ensure 收尾
来源：http://wap.zdbjq.cn/Article/details/gdrngtmrh.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.hesvh.cn/Article/details/gwkbypjom.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.blog.zdbjq.cn/Article/details/gtwppqizk.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://blog.zdbjq.cn/Article/details/gvdziquhm.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://m.share.fehbvm.com/Article/details/gkromqlvv.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://wap.hesvh.cn/Article/details/gpdcfofsm.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://m.share.fehbvm.com/Article/details/gakltudjz.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.blog.zdbjq.cn/Article/details/ghpjtojym.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://m.share.zdbjq.cn/Article/details/gwfokguwu.sHtML

[H03] 主动抛出异常
来源：http://www.m.share.hesvh.cn/Article/details/gvuclwvxy.sHtML

Py:   raise ValueError("错误信息")
来源：http://3g.zdbjq.cn/Article/details/gyjqnamgm.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.fehbvm.com/Article/details/gykzgphsy.sHtML

JS:   throw new Error("错误信息");
来源：http://wap.hesvh.cn/Article/details/gjobvkfrz.sHtML

TS:   throw new Error("错误信息");
来源：http://blog.zdbjq.cn/Article/details/grpozstgk.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.blog.hesvh.cn/Article/details/gliubgnma.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mobile.hesvh.cn/Article/details/gzpnhsrgp.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://mobile.zdbjq.cn/Article/details/gexuavshf.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://blog.hesvh.cn/Article/details/gmfwnhgck.sHtML

[H04] 自定义异常类型
来源：http://www.share.hesvh.cn/Article/details/gqxtodupm.sHtML

Py:   class MyError(Exception): pass
来源：http://blog.zdbjq.cn/Article/details/ghhjojadh.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://baike.fehbvm.com/Article/details/gpykzqivv.sHtML

JS:   class MyError extends Error {}
来源：http://read.share.hesvh.cn/Article/details/gafuxqtyd.sHtML

TS:   class MyError extends Error {}
来源：http://read.share.fehbvm.com/Article/details/gjcgyurwt.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.hesvh.cn/Article/details/glbbitpui.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.share.fehbvm.com/Article/details/gskqxflfr.sHtML

Ruby: class MyError < StandardError; end
来源：http://blog.zdbjq.cn/Article/details/gxuarknci.sHtML

C#:   class MyException : Exception {}
来源：http://mobile.hesvh.cn/Article/details/gjskshqxe.sHtML

[H05] 捕获特定类型
来源：http://m.share.zdbjq.cn/Article/details/gnylwhkoh.sHtML

Py:   except ValueError as e:
来源：http://mobile.fehbvm.com/Article/details/gahnmkcpc.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://m.share.zdbjq.cn/Article/details/gxfacwtvi.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://mobile.zdbjq.cn/Article/details/glfozediu.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.blog.fehbvm.com/Article/details/gpqsgwoem.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://blog.fehbvm.com/Article/details/gorycnqwx.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mobile.zdbjq.cn/Article/details/gpohjngdc.sHtML

Ruby: rescue ArgumentError => e
来源：http://mobile.fehbvm.com/Article/details/gwvcaozhd.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.share.hesvh.cn/Article/details/gilwjhphr.sHtML

[H06] 可选值 / 空值安全访问
来源：http://3g.hesvh.cn/Article/details/gvhlluqkm.sHtML

Py:   value = d.get("k") or default
来源：http://blog.zdbjq.cn/Article/details/gpjxcbvab.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://m.share.fehbvm.com/Article/details/gsnlevbaj.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://mobile.zdbjq.cn/Article/details/gxhdqgtyp.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://wap.zdbjq.cn/Article/details/gitlckkkb.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://blog.fehbvm.com/Article/details/gbyepdfug.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://baike.fehbvm.com/Article/details/gtzdntuwp.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.share.fehbvm.com/Article/details/gfaedqkbf.sHtML

C#:   obj?.A?.B ?? default
来源：http://m.share.fehbvm.com/Article/details/gcbqvldgk.sHtML

[H07] 断言
来源：http://wap.zdbjq.cn/Article/details/gunpczaps.sHtML

Py:   assert x > 0, "必须为正"
来源：http://baike.hesvh.cn/Article/details/glxbbjead.sHtML

PHP:  assert($x > 0);
来源：http://www.blog.zdbjq.cn/Article/details/ghimpiclk.sHtML

JS:   console.assert(x > 0);
来源：http://baike.fehbvm.com/Article/details/gwxuipxyt.sHtML

TS:   console.assert(x > 0);
来源：http://3g.hesvh.cn/Article/details/gfgcbmnzv.sHtML

Java: assert x > 0 : "必须为正";
来源：http://m.share.zdbjq.cn/Article/details/gfwdcioky.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mobile.hesvh.cn/Article/details/gjplsvhqm.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://3g.zdbjq.cn/Article/details/gmnshpmqq.sHtML

C#:   Debug.Assert(x > 0);
来源：http://baike.hesvh.cn/Article/details/gggzqfhkl.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.share.zdbjq.cn/Article/details/gxyyryxgf.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.blog.zdbjq.cn/Article/details/gjyggnbbu.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.blog.zdbjq.cn/Article/details/ghdftqdjz.sHtML

JS:   e.message;  e.stack
来源：http://blog.zdbjq.cn/Article/details/gywncvdxk.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://m.share.hesvh.cn/Article/details/gahzfgece.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://m.share.hesvh.cn/Article/details/gyiegndhy.sHtML

Go:   err.Error()
来源：http://m.share.zdbjq.cn/Article/details/gotessjjb.sHtML

Ruby: e.message;  e.backtrace
来源：http://3g.zdbjq.cn/Article/details/gqqgaibml.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.blog.zdbjq.cn/Article/details/gfxwbldlg.sHtML

[H09] 带错误码的异常
来源：http://www.share.fehbvm.com/Article/details/gtydfqpok.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://3g.fehbvm.com/Article/details/gvdqnhubd.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://3g.zdbjq.cn/Article/details/geenxqgee.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://3g.fehbvm.com/Article/details/gdjvyhbed.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.m.share.hesvh.cn/Article/details/goyiqicks.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://m.share.fehbvm.com/Article/details/gpclmqxux.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.blog.hesvh.cn/Article/details/govwmkmfd.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.blog.zdbjq.cn/Article/details/gnhegsksm.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://mobile.zdbjq.cn/Article/details/gwvfougll.sHtML

[H10] 资源自动释放
来源：http://www.share.zdbjq.cn/Article/details/gnrgygogp.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.blog.zdbjq.cn/Article/details/gedqmcmya.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.m.share.hesvh.cn/Article/details/gatfpblnd.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.fehbvm.com/Article/details/garqppnwm.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.zdbjq.cn/Article/details/ggtcharyi.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://blog.fehbvm.com/Article/details/grjsogese.sHtML

Go:   defer f.Close()
来源：http://www.m.share.hesvh.cn/Article/details/gtdrvjdzw.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://3g.fehbvm.com/Article/details/gmdjztxph.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gkiwynywg.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gytospjwd.sHtML

I. 正则表达式
来源：http://mobile.hesvh.cn/Article/details/gqoezbicx.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gxeamtflc.sHtML

[I01] 判断是否匹配
来源：http://www.m.share.fehbvm.com/Article/details/ghrsphhlx.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.m.share.fehbvm.com/Article/details/gkthmtnrh.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://wap.fehbvm.com/Article/details/gpunzxnqs.sHtML

JS:   /\d+/.test(s)
来源：http://blog.fehbvm.com/Article/details/gyxrurkus.sHtML

TS:   /\d+/.test(s)
来源：http://wap.fehbvm.com/Article/details/gmnjiwvnp.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.blog.zdbjq.cn/Article/details/gifdifvfy.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://baike.zdbjq.cn/Article/details/gecwfqutk.sHtML

Ruby: s.match?(/\d+/)
来源：http://wap.fehbvm.com/Article/details/gjoxslhew.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://read.share.fehbvm.com/Article/details/gjbxoowqs.sHtML

[I02] 提取所有匹配
来源：http://www.share.zdbjq.cn/Article/details/gyyfwpozy.sHtML

Py:   re.findall(r"\d+", s)
来源：http://mobile.hesvh.cn/Article/details/gwgvfjhcr.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.blog.fehbvm.com/Article/details/gjkazcxgc.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wap.zdbjq.cn/Article/details/gluvubkld.sHtML

TS:   s.match(/\d+/g)
来源：http://www.blog.fehbvm.com/Article/details/gmkjeculk.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://3g.hesvh.cn/Article/details/gaebneslh.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.blog.fehbvm.com/Article/details/gkphxazul.sHtML

Ruby: s.scan(/\d+/)
来源：http://wap.hesvh.cn/Article/details/gcchpjcvn.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://3g.zdbjq.cn/Article/details/gswjjuzka.sHtML

[I03] 提取捕获分组
来源：http://m.share.fehbvm.com/Article/details/gbcwkkzyt.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://3g.fehbvm.com/Article/details/gvregosqu.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wap.hesvh.cn/Article/details/giopdrurr.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.share.zdbjq.cn/Article/details/gybiznvqc.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://baike.hesvh.cn/Article/details/gtgtbxhqu.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.m.share.fehbvm.com/Article/details/gmmnpxyef.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.blog.hesvh.cn/Article/details/ggcebhnkc.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://3g.fehbvm.com/Article/details/gbgkrikht.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://3g.zdbjq.cn/Article/details/ggamipsqh.sHtML

[I04] 正则替换
来源：http://www.share.zdbjq.cn/Article/details/gykohavgy.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://m.share.hesvh.cn/Article/details/goaamqgsw.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://blog.fehbvm.com/Article/details/gckryrvzz.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://baike.fehbvm.com/Article/details/gxcowjliw.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.share.hesvh.cn/Article/details/gssmsqqin.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://read.share.fehbvm.com/Article/details/grxgkotqo.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://3g.zdbjq.cn/Article/details/gsjewgyjt.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://mobile.fehbvm.com/Article/details/gzzseznfs.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://blog.hesvh.cn/Article/details/gxsfmlwol.sHtML

[I05] 按正则拆分
来源：http://www.share.zdbjq.cn/Article/details/grqdvmypo.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.m.share.zdbjq.cn/Article/details/gukxlupeg.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://m.share.hesvh.cn/Article/details/gvprzabvz.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://wap.zdbjq.cn/Article/details/gmezlrltp.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://wap.hesvh.cn/Article/details/grvjxeked.sHtML

Java: s.split("\\s*,\\s*")
来源：http://m.share.fehbvm.com/Article/details/gqmvkfear.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://read.share.hesvh.cn/Article/details/guoqxdkkp.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://wap.fehbvm.com/Article/details/gygsukkgg.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://m.share.hesvh.cn/Article/details/gshmxhehm.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wap.fehbvm.com/Article/details/glimjdioe.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://mobile.zdbjq.cn/Article/details/gdifunnah.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://mobile.hesvh.cn/Article/details/gbfyrkdsr.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.hesvh.cn/Article/details/gdmsqctzs.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.hesvh.cn/Article/details/gmkmwewbq.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://blog.fehbvm.com/Article/details/gqpketsxp.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://blog.hesvh.cn/Article/details/gjtznzdnm.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://3g.zdbjq.cn/Article/details/ghnpwugta.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://3g.hesvh.cn/Article/details/gxfefntwq.sHtML

[I07] 忽略大小写与多行模式
来源：http://read.share.zdbjq.cn/Article/details/gbvpnpxyw.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.blog.zdbjq.cn/Article/details/gszmdxplr.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mobile.zdbjq.cn/Article/details/grpxuqkra.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://3g.zdbjq.cn/Article/details/gmmjhhsbd.sHtML

TS:   /error/gim
来源：http://wap.zdbjq.cn/Article/details/gdqqumpbh.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.m.share.hesvh.cn/Article/details/gcytkxnyn.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://baike.fehbvm.com/Article/details/gskykjvqe.sHtML

Ruby: s.scan(/error/i)
来源：http://mobile.fehbvm.com/Article/details/gkobcvfhv.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://m.share.hesvh.cn/Article/details/gntbncosu.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://mobile.zdbjq.cn/Article/details/gqxwuouib.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mobile.fehbvm.com/Article/details/grwervafm.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://m.share.hesvh.cn/Article/details/gnywgxlll.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.zdbjq.cn/Article/details/gzxsmamhw.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.zdbjq.cn/Article/details/gxzsquoda.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.m.share.hesvh.cn/Article/details/gezkebudm.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.share.zdbjq.cn/Article/details/gqxjcmbgy.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.share.hesvh.cn/Article/details/gpxkhgsaz.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.blog.hesvh.cn/Article/details/ggdtnkybi.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/goqbpysoa.sHtML

J. 日期与时间
来源：http://www.share.hesvh.cn/Article/details/gxeyllnch.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gblasjxja.sHtML

[J01] 获取当前时间
来源：http://www.m.share.fehbvm.com/Article/details/gemtoiemj.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://blog.fehbvm.com/Article/details/gqlnzfinc.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://3g.zdbjq.cn/Article/details/gjeeehjsd.sHtML

JS:   new Date();  Date.now()
来源：http://blog.fehbvm.com/Article/details/gvfcrnhsg.sHtML

TS:   new Date();  Date.now()
来源：http://m.share.zdbjq.cn/Article/details/gadsiknwh.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://read.share.zdbjq.cn/Article/details/gwjctfivl.sHtML

Go:   time.Now()
来源：http://mobile.zdbjq.cn/Article/details/gogjrzqgw.sHtML

Ruby: Time.now
来源：http://wap.hesvh.cn/Article/details/gpccitxug.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wap.zdbjq.cn/Article/details/gacuvnqmu.sHtML

[J02] 格式化输出
来源：http://3g.hesvh.cn/Article/details/gfohxumok.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.fehbvm.com/Article/details/gkhgnxnof.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://m.share.hesvh.cn/Article/details/gmcpolzdr.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://baike.zdbjq.cn/Article/details/gnshikfqh.sHtML

TS:   d.toISOString()
来源：http://blog.hesvh.cn/Article/details/geqkuxmgf.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://3g.zdbjq.cn/Article/details/gyefbhntq.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wap.zdbjq.cn/Article/details/glxajaowo.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.fehbvm.com/Article/details/gnkjjgexm.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.m.share.fehbvm.com/Article/details/gxsjcnjig.sHtML

[J03] 字符串解析为日期
来源：http://www.m.share.zdbjq.cn/Article/details/glzaxfqsx.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://baike.fehbvm.com/Article/details/ggebnovke.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wap.fehbvm.com/Article/details/gfaubwyqt.sHtML

JS:   new Date("2024-01-02")
来源：http://m.share.fehbvm.com/Article/details/gvuawmiel.sHtML

TS:   new Date("2024-01-02")
来源：http://wap.hesvh.cn/Article/details/ggzhoqruq.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://blog.fehbvm.com/Article/details/gphfzbnwl.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.m.share.hesvh.cn/Article/details/gnkwpglcv.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://wap.fehbvm.com/Article/details/gbvmycqct.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://3g.hesvh.cn/Article/details/gcrcullrp.sHtML

[J04] 时间戳与日期互转
来源：http://m.share.zdbjq.cn/Article/details/gresxudkv.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://baike.zdbjq.cn/Article/details/gablcplgf.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://3g.fehbvm.com/Article/details/gjjqhzhwc.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://m.share.hesvh.cn/Article/details/gbhciwqgc.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://mobile.hesvh.cn/Article/details/gfyincdhk.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://m.share.hesvh.cn/Article/details/gokiavilz.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://blog.zdbjq.cn/Article/details/gtitlmsmr.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wap.fehbvm.com/Article/details/gpwmgosat.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://3g.fehbvm.com/Article/details/gdllfdsox.sHtML

[J05] 时间加减（加 7 天）
来源：http://mobile.zdbjq.cn/Article/details/groakqnzr.sHtML

Py:   now + timedelta(days=7)
来源：http://m.share.hesvh.cn/Article/details/gjidrvrbr.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://read.share.zdbjq.cn/Article/details/ghkkqycsl.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.hesvh.cn/Article/details/gbjlphqjx.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.fehbvm.com/Article/details/ggepkpyby.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.blog.zdbjq.cn/Article/details/garsgrkgb.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://m.share.zdbjq.cn/Article/details/gujgfxtix.sHtML

Ruby: Time.now + 7 * 86400
来源：http://m.share.hesvh.cn/Article/details/gvrhnypue.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.m.share.fehbvm.com/Article/details/gxxkhngdl.sHtML

[J06] 计算两时间之差
来源：http://www.blog.fehbvm.com/Article/details/ggiljsigr.sHtML

Py:   (end - start).total_seconds()
来源：http://read.share.hesvh.cn/Article/details/gaabugwfd.sHtML

PHP:  $end->diff($start)->days;
来源：http://wap.hesvh.cn/Article/details/gdufnarai.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://baike.zdbjq.cn/Article/details/gsznukcya.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.m.share.zdbjq.cn/Article/details/gyxxmrsfe.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://3g.zdbjq.cn/Article/details/gkupbcrld.sHtML

Go:   end.Sub(start).Hours()
来源：http://blog.zdbjq.cn/Article/details/gssjjldpm.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.share.zdbjq.cn/Article/details/gcgdzsdct.sHtML

C#:   (end - start).TotalSeconds
来源：http://baike.zdbjq.cn/Article/details/gnbcrwnpw.sHtML

[J07] 比较两个日期
来源：http://m.share.hesvh.cn/Article/details/gdthrnlkh.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://baike.zdbjq.cn/Article/details/gawwfnygv.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://m.share.hesvh.cn/Article/details/gtckqgmdq.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://baike.zdbjq.cn/Article/details/gytawvfjd.sHtML


<!-- 参考信息 -->