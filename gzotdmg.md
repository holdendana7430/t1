代发 wailian999

Py:   from abc import ABC, abstractmethod
来源：http://blog.fehbvm.com/Article/details/gdepqlbvf.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.fehbvm.com/Article/details/ghvlixlqk.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.fehbvm.com/Article/details/gchdhewdc.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.fehbvm.com/Article/details/ghrgvulqa.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.fehbvm.com/Article/details/ggwollqjy.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.zdbjq.cn/Article/details/gewvzocxu.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.fehbvm.com/Article/details/gmpowsjfz.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.fehbvm.com/Article/details/gkkeheqgx.sHtML

[G10] 访问控制
来源：http://m.share.fehbvm.com/Article/details/gzkmgiilc.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.hesvh.cn/Article/details/gqqaqvspw.sHtML

PHP:  public / protected / private
来源：http://mobile.hesvh.cn/Article/details/gmutkjdns.sHtML

JS:   #private 字段；其余公开
来源：http://wap.zdbjq.cn/Article/details/ghjspeczc.sHtML

TS:   public / protected / private
来源：http://www.m.share.hesvh.cn/Article/details/ghtwbqdqb.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.fehbvm.com/Article/details/gftzengvm.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.fehbvm.com/Article/details/gtsjvpjrz.sHtML

Ruby: public / protected / private
来源：http://baike.fehbvm.com/Article/details/gylplcchz.sHtML

C#:   public / protected / private / internal
来源：http://www.share.zdbjq.cn/Article/details/grgxssswc.sHtML

[G11] getter / setter
来源：http://baike.fehbvm.com/Article/details/ggkgrdyle.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.fehbvm.com/Article/details/gxgamtzml.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.zdbjq.cn/Article/details/gtfgxjrhv.sHtML

JS:   get name() { return this._name; }
来源：http://blog.zdbjq.cn/Article/details/gxdcvjesl.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.fehbvm.com/Article/details/gtsftmtjg.sHtML

Java: public String getName() { return name; }
来源：http://m.share.hesvh.cn/Article/details/gjovaoghz.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.zdbjq.cn/Article/details/ggdwkyzbx.sHtML

Ruby: attr_accessor :name
来源：http://m.share.hesvh.cn/Article/details/gepyijuri.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.hesvh.cn/Article/details/gfygkvqly.sHtML

[G12] 对象转字符串
来源：http://mobile.fehbvm.com/Article/details/gyuyqqits.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.fehbvm.com/Article/details/gzaidoads.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.fehbvm.com/Article/details/ggzhbkbxf.sHtML

JS:   toString() { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/gspphoemd.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.fehbvm.com/Article/details/gmsjwsttd.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.fehbvm.com/Article/details/gmxewjpma.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.zdbjq.cn/Article/details/gdndrxfvx.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.fehbvm.com/Article/details/giqxqrwue.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.fehbvm.com/Article/details/gysrlnwsp.sHtML

[G13] 判断对象类型
来源：http://baike.fehbvm.com/Article/details/gwykeweym.sHtML

Py:   isinstance(u, User)
来源：http://baike.fehbvm.com/Article/details/ggtmljtvg.sHtML

PHP:  $u instanceof User
来源：http://baike.zdbjq.cn/Article/details/gaegspqyb.sHtML

JS:   u instanceof User
来源：http://3g.hesvh.cn/Article/details/gdwnudkfd.sHtML

TS:   u instanceof User
来源：http://baike.fehbvm.com/Article/details/gmmftskny.sHtML

Java: u instanceof User
来源：http://mobile.fehbvm.com/Article/details/gslvzrttc.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.hesvh.cn/Article/details/gitjwnyzv.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.zdbjq.cn/Article/details/gguevsodv.sHtML

C#:   u is User
来源：http://baike.zdbjq.cn/Article/details/grvwdzmyf.sHtML

[G14] 数据类 / record
来源：http://mobile.zdbjq.cn/Article/details/ghkbrjaws.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://3g.hesvh.cn/Article/details/grlrzwuqn.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.fehbvm.com/Article/details/gitnlqvtz.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.hesvh.cn/Article/details/gtvyimfyr.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.hesvh.cn/Article/details/gnytguaij.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.hesvh.cn/Article/details/gstzizuzq.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.zdbjq.cn/Article/details/gguvqvkpb.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.hesvh.cn/Article/details/gkafjlykl.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.hesvh.cn/Article/details/gnqggczxq.sHtML

[G15] 枚举
来源：http://read.share.zdbjq.cn/Article/details/gcotkfqwm.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.hesvh.cn/Article/details/ghbckvxhr.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.fehbvm.com/Article/details/gglaauzgl.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.hesvh.cn/Article/details/geoiluwip.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.zdbjq.cn/Article/details/gdgrqwgsc.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.hesvh.cn/Article/details/gwimqcswy.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.blog.zdbjq.cn/Article/details/grdixwvfc.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.zdbjq.cn/Article/details/gbtdaywhz.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.hesvh.cn/Article/details/gqqrujmlt.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.zdbjq.cn/Article/details/gxyxrvjzz.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.hesvh.cn/Article/details/gxvqojibk.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.zdbjq.cn/Article/details/gyttpemjm.sHtML

JS:   Object.entries(obj)
来源：http://mobile.fehbvm.com/Article/details/gizqupttm.sHtML

TS:   Object.entries(obj)
来源：http://baike.zdbjq.cn/Article/details/ggkmtetur.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.fehbvm.com/Article/details/gqsigqwrp.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.fehbvm.com/Article/details/gfmwhxzgb.sHtML

Ruby: obj.instance_variables
来源：http://blog.zdbjq.cn/Article/details/goggqqqsl.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.hesvh.cn/Article/details/gytewrraa.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gvixrurhv.sHtML

H. 异常与错误处理
来源：http://www.blog.zdbjq.cn/Article/details/gwhfsyxoo.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gdzxggpuf.sHtML

[H01] try / catch 基础
来源：http://blog.hesvh.cn/Article/details/ghewufnly.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.zdbjq.cn/Article/details/gavatdkco.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.zdbjq.cn/Article/details/gzafqybeg.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.hesvh.cn/Article/details/gobgepxoi.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.share.fehbvm.com/Article/details/ghkkaehpz.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.zdbjq.cn/Article/details/gkwnqdnmq.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://read.share.fehbvm.com/Article/details/glxfritpk.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://blog.fehbvm.com/Article/details/gpqvfuvaw.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://blog.zdbjq.cn/Article/details/gpferiwhv.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.zdbjq.cn/Article/details/gjltwjqor.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.m.share.zdbjq.cn/Article/details/gvjmxomxb.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.share.zdbjq.cn/Article/details/geaotkpzp.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://3g.fehbvm.com/Article/details/ghuzidmpf.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://blog.zdbjq.cn/Article/details/gxweliqus.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.share.zdbjq.cn/Article/details/gimqedrae.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://3g.zdbjq.cn/Article/details/gcfxzpeed.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://blog.hesvh.cn/Article/details/gtelaxfpf.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/gwphidtwy.sHtML

[H03] 主动抛出异常
来源：http://www.share.hesvh.cn/Article/details/gporffeai.sHtML

Py:   raise ValueError("错误信息")
来源：http://blog.hesvh.cn/Article/details/gwfpnhrza.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blog.zdbjq.cn/Article/details/gjonvbvbd.sHtML

JS:   throw new Error("错误信息");
来源：http://www.blog.fehbvm.com/Article/details/gpngszbsb.sHtML

TS:   throw new Error("错误信息");
来源：http://baike.hesvh.cn/Article/details/gawcctkev.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://mobile.zdbjq.cn/Article/details/gkopssznn.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.share.fehbvm.com/Article/details/gapsviaas.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.blog.hesvh.cn/Article/details/gtjbllkrt.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://blog.hesvh.cn/Article/details/gjpfhnpzq.sHtML

[H04] 自定义异常类型
来源：http://www.m.share.hesvh.cn/Article/details/glotjquux.sHtML

Py:   class MyError(Exception): pass
来源：http://wap.zdbjq.cn/Article/details/gvszpsffk.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://baike.fehbvm.com/Article/details/gnadxmokr.sHtML

JS:   class MyError extends Error {}
来源：http://www.m.share.zdbjq.cn/Article/details/gxbwnivlu.sHtML

TS:   class MyError extends Error {}
来源：http://mobile.hesvh.cn/Article/details/gyvoipdon.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.blog.fehbvm.com/Article/details/gnlxqgqsc.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.share.hesvh.cn/Article/details/gznnyreoa.sHtML

Ruby: class MyError < StandardError; end
来源：http://mobile.zdbjq.cn/Article/details/gqcftlwzs.sHtML

C#:   class MyException : Exception {}
来源：http://m.share.zdbjq.cn/Article/details/gzgfigkih.sHtML

[H05] 捕获特定类型
来源：http://3g.zdbjq.cn/Article/details/gqoowglko.sHtML

Py:   except ValueError as e:
来源：http://www.blog.fehbvm.com/Article/details/gpkpwktiz.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.hesvh.cn/Article/details/gnicvmiau.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://m.share.zdbjq.cn/Article/details/ggsplkcfh.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.share.hesvh.cn/Article/details/gszqhwjrt.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://wap.hesvh.cn/Article/details/gxiljaizj.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://read.share.hesvh.cn/Article/details/gokmfmmdh.sHtML

Ruby: rescue ArgumentError => e
来源：http://blog.fehbvm.com/Article/details/ghasuovik.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wap.zdbjq.cn/Article/details/gjejiortw.sHtML

[H06] 可选值 / 空值安全访问
来源：http://read.share.hesvh.cn/Article/details/gppshfmli.sHtML

Py:   value = d.get("k") or default
来源：http://blog.hesvh.cn/Article/details/gnhkhvbhz.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://3g.fehbvm.com/Article/details/gxrinlcuw.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://mobile.zdbjq.cn/Article/details/gtsdfwezk.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.blog.zdbjq.cn/Article/details/gxkwowvue.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mobile.zdbjq.cn/Article/details/glfjxfrtt.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.blog.hesvh.cn/Article/details/gcrcuxmwz.sHtML

Ruby: d&.dig(:a, :b)
来源：http://mobile.hesvh.cn/Article/details/gzbmkrsbi.sHtML

C#:   obj?.A?.B ?? default
来源：http://m.share.zdbjq.cn/Article/details/gwmqwlyhu.sHtML

[H07] 断言
来源：http://www.blog.hesvh.cn/Article/details/gtmnhffix.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.blog.hesvh.cn/Article/details/gklkvqgiu.sHtML

PHP:  assert($x > 0);
来源：http://read.share.fehbvm.com/Article/details/goihtjvzi.sHtML

JS:   console.assert(x > 0);
来源：http://www.share.fehbvm.com/Article/details/gcjsaofki.sHtML

TS:   console.assert(x > 0);
来源：http://wap.hesvh.cn/Article/details/glziyhveq.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.fehbvm.com/Article/details/ghhpmlods.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.share.zdbjq.cn/Article/details/ghmrbqiol.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.blog.fehbvm.com/Article/details/gcohboght.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.share.zdbjq.cn/Article/details/gtxbjokyc.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.share.fehbvm.com/Article/details/goqmegkyp.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.m.share.fehbvm.com/Article/details/gabjhhlts.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://3g.fehbvm.com/Article/details/gwpnjhntn.sHtML

JS:   e.message;  e.stack
来源：http://blog.fehbvm.com/Article/details/gmicnfcsf.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://3g.hesvh.cn/Article/details/ggzchpgcb.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://mobile.hesvh.cn/Article/details/gtkqtaydk.sHtML

Go:   err.Error()
来源：http://read.share.zdbjq.cn/Article/details/gogljdejm.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.m.share.hesvh.cn/Article/details/gvjgkljnd.sHtML

C#:   e.Message;  e.StackTrace
来源：http://m.share.fehbvm.com/Article/details/grkzjxcmq.sHtML

[H09] 带错误码的异常
来源：http://3g.fehbvm.com/Article/details/guocaysie.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://blog.fehbvm.com/Article/details/geulmrsdu.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://baike.fehbvm.com/Article/details/gcdvearvd.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.blog.fehbvm.com/Article/details/gqxxcewbd.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mobile.hesvh.cn/Article/details/ghtqidgby.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://blog.zdbjq.cn/Article/details/grczmaojt.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://3g.zdbjq.cn/Article/details/gqdnqdagy.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://wap.fehbvm.com/Article/details/gdfistdxh.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://3g.zdbjq.cn/Article/details/gabhfyisc.sHtML

[H10] 资源自动释放
来源：http://3g.zdbjq.cn/Article/details/giqouuahz.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://blog.fehbvm.com/Article/details/gdmizmklq.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://baike.fehbvm.com/Article/details/gvkmkmqee.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.fehbvm.com/Article/details/gskuhracw.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.hesvh.cn/Article/details/gjxhpoied.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mobile.hesvh.cn/Article/details/gsbokwcvy.sHtML

Go:   defer f.Close()
来源：http://read.share.hesvh.cn/Article/details/gaoqvvshq.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://baike.hesvh.cn/Article/details/gyraqtjjs.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gqzdsinsi.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/grrcaugxa.sHtML

I. 正则表达式
来源：http://wap.fehbvm.com/Article/details/gnzjddrjh.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/grmatokas.sHtML

[I01] 判断是否匹配
来源：http://read.share.hesvh.cn/Article/details/gsywielhu.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://baike.zdbjq.cn/Article/details/gvshdbguw.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gwxoziejm.sHtML

JS:   /\d+/.test(s)
来源：http://3g.fehbvm.com/Article/details/gaefliovy.sHtML

TS:   /\d+/.test(s)
来源：http://read.share.hesvh.cn/Article/details/gnzrejort.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mobile.zdbjq.cn/Article/details/gzisyyssr.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wap.zdbjq.cn/Article/details/gqmutdlyh.sHtML

Ruby: s.match?(/\d+/)
来源：http://3g.fehbvm.com/Article/details/gwrsnmoph.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mobile.zdbjq.cn/Article/details/ggbnjmcch.sHtML

[I02] 提取所有匹配
来源：http://3g.fehbvm.com/Article/details/gksrlfrpe.sHtML

Py:   re.findall(r"\d+", s)
来源：http://mobile.zdbjq.cn/Article/details/gqgckshtq.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://read.share.fehbvm.com/Article/details/gcyvrlejo.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.m.share.fehbvm.com/Article/details/gneiywivz.sHtML

TS:   s.match(/\d+/g)
来源：http://baike.hesvh.cn/Article/details/gjryfpzuv.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.share.zdbjq.cn/Article/details/gybfkwdca.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://baike.zdbjq.cn/Article/details/gofurvcsb.sHtML

Ruby: s.scan(/\d+/)
来源：http://blog.hesvh.cn/Article/details/gqkgtyggt.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.m.share.fehbvm.com/Article/details/gupagmkps.sHtML

[I03] 提取捕获分组
来源：http://www.blog.fehbvm.com/Article/details/gudcnbkmy.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://3g.zdbjq.cn/Article/details/ghyismjqo.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://m.share.hesvh.cn/Article/details/gncctzsbh.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://baike.zdbjq.cn/Article/details/gbeneftui.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://3g.fehbvm.com/Article/details/gfnodxuei.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://blog.hesvh.cn/Article/details/gupmuaocw.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://3g.fehbvm.com/Article/details/gsfrfuntl.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.m.share.hesvh.cn/Article/details/gauenqwyb.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://3g.fehbvm.com/Article/details/gesamrmdv.sHtML

[I04] 正则替换
来源：http://www.m.share.hesvh.cn/Article/details/gkaagvuwm.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.m.share.zdbjq.cn/Article/details/gvktssyyx.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.share.zdbjq.cn/Article/details/gkisrrtss.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://read.share.zdbjq.cn/Article/details/gpzxabqts.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://wap.hesvh.cn/Article/details/gdujlkizs.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://3g.zdbjq.cn/Article/details/glsakaxdy.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://read.share.fehbvm.com/Article/details/glqrobxrt.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://blog.zdbjq.cn/Article/details/grkxzjfib.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.m.share.hesvh.cn/Article/details/ggybfzvrl.sHtML

[I05] 按正则拆分
来源：http://blog.hesvh.cn/Article/details/gejedrkyr.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://mobile.hesvh.cn/Article/details/gpszhsima.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mobile.zdbjq.cn/Article/details/gjjzlueop.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.blog.hesvh.cn/Article/details/gxrhdrshm.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://blog.fehbvm.com/Article/details/gwzofletw.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.share.hesvh.cn/Article/details/giqklzaiy.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://m.share.fehbvm.com/Article/details/gklobrdrz.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://read.share.fehbvm.com/Article/details/glkfjdaft.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.blog.zdbjq.cn/Article/details/gwayznwpu.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://read.share.hesvh.cn/Article/details/gqewuieef.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://read.share.hesvh.cn/Article/details/gsncushlh.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.blog.zdbjq.cn/Article/details/gdhaympow.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.zdbjq.cn/Article/details/gbwljrhqd.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.zdbjq.cn/Article/details/gwnkrlshe.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://blog.zdbjq.cn/Article/details/gslhkccot.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://m.share.fehbvm.com/Article/details/guavkzmzj.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://m.share.fehbvm.com/Article/details/gvemntnkt.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wap.fehbvm.com/Article/details/giiwqzhyn.sHtML

[I07] 忽略大小写与多行模式
来源：http://read.share.fehbvm.com/Article/details/ghovjplub.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://read.share.hesvh.cn/Article/details/gtcjeuczk.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mobile.hesvh.cn/Article/details/gvvwqlmjs.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mobile.hesvh.cn/Article/details/ghqvrunul.sHtML

TS:   /error/gim
来源：http://wap.hesvh.cn/Article/details/gqszmbnzx.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.m.share.zdbjq.cn/Article/details/gsywecdvl.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.m.share.zdbjq.cn/Article/details/gfhyzysyy.sHtML

Ruby: s.scan(/error/i)
来源：http://3g.hesvh.cn/Article/details/gvyxnncwi.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://blog.hesvh.cn/Article/details/ghczpnmmr.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://read.share.zdbjq.cn/Article/details/gwjbvrpli.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://blog.zdbjq.cn/Article/details/gmoyxavvr.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.blog.fehbvm.com/Article/details/giafpgqct.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.zdbjq.cn/Article/details/gsmekewiw.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.fehbvm.com/Article/details/gyqtwibrw.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.blog.hesvh.cn/Article/details/gtubxjfxp.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://m.share.fehbvm.com/Article/details/guvztfqll.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://m.share.fehbvm.com/Article/details/gtkcqxhrp.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://read.share.hesvh.cn/Article/details/gmbequqwt.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gwfbdbqil.sHtML

J. 日期与时间
来源：http://read.share.hesvh.cn/Article/details/gqfmdnblh.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gduzrxrye.sHtML

[J01] 获取当前时间
来源：http://www.m.share.zdbjq.cn/Article/details/gunqfdnwd.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://read.share.fehbvm.com/Article/details/gvdwzhceo.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://3g.zdbjq.cn/Article/details/gabsepomq.sHtML

JS:   new Date();  Date.now()
来源：http://www.share.hesvh.cn/Article/details/gikcbcxgq.sHtML

TS:   new Date();  Date.now()
来源：http://www.m.share.fehbvm.com/Article/details/gzzwopolw.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.m.share.hesvh.cn/Article/details/gtzceeybm.sHtML

Go:   time.Now()
来源：http://m.share.hesvh.cn/Article/details/gyxrirllu.sHtML

Ruby: Time.now
来源：http://read.share.fehbvm.com/Article/details/gndmchzny.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://read.share.hesvh.cn/Article/details/gdbznfntm.sHtML

[J02] 格式化输出
来源：http://m.share.hesvh.cn/Article/details/gwksqodpf.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.zdbjq.cn/Article/details/gowwbojvv.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://3g.fehbvm.com/Article/details/goycorjvb.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mobile.fehbvm.com/Article/details/ghhusiuuh.sHtML

TS:   d.toISOString()
来源：http://wap.hesvh.cn/Article/details/gspoeyhrx.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://m.share.zdbjq.cn/Article/details/gnzckhmza.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.blog.zdbjq.cn/Article/details/gqlsoflny.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.zdbjq.cn/Article/details/gnplzkttx.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.share.hesvh.cn/Article/details/gskkbsiry.sHtML

[J03] 字符串解析为日期
来源：http://wap.fehbvm.com/Article/details/guarjhala.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.m.share.zdbjq.cn/Article/details/gmfvfdlpf.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.share.hesvh.cn/Article/details/gdjezgqwd.sHtML

JS:   new Date("2024-01-02")
来源：http://m.share.hesvh.cn/Article/details/gozlvilbk.sHtML

TS:   new Date("2024-01-02")
来源：http://3g.hesvh.cn/Article/details/gfaczljwf.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://wap.hesvh.cn/Article/details/gezyltxxd.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://3g.zdbjq.cn/Article/details/giqupmybg.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.share.zdbjq.cn/Article/details/gfltnhled.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mobile.fehbvm.com/Article/details/gqjjzkmjl.sHtML

[J04] 时间戳与日期互转
来源：http://www.share.hesvh.cn/Article/details/giftdlzpw.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://m.share.zdbjq.cn/Article/details/geoezeevq.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wap.fehbvm.com/Article/details/gpswgspfk.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.share.zdbjq.cn/Article/details/gxyqtceqz.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.share.hesvh.cn/Article/details/gtqcqnllg.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://wap.hesvh.cn/Article/details/gjiyqvxxz.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://3g.hesvh.cn/Article/details/gphdzzvnq.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.blog.zdbjq.cn/Article/details/gghfxvtgh.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://blog.zdbjq.cn/Article/details/gpyorlbfw.sHtML

[J05] 时间加减（加 7 天）
来源：http://m.share.zdbjq.cn/Article/details/ghleobolo.sHtML

Py:   now + timedelta(days=7)
来源：http://mobile.hesvh.cn/Article/details/gzstwynpz.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.m.share.fehbvm.com/Article/details/gsxpwdpkq.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.hesvh.cn/Article/details/gvhmwucgw.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.zdbjq.cn/Article/details/guxnashxb.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://m.share.hesvh.cn/Article/details/gzrddvguf.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://read.share.hesvh.cn/Article/details/gabdhbwuy.sHtML

Ruby: Time.now + 7 * 86400
来源：http://baike.hesvh.cn/Article/details/gxxoecwyg.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://wap.hesvh.cn/Article/details/giyvmcsfl.sHtML

[J06] 计算两时间之差
来源：http://www.blog.hesvh.cn/Article/details/gluwonnsu.sHtML

Py:   (end - start).total_seconds()
来源：http://baike.fehbvm.com/Article/details/gzjbfszbq.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.blog.fehbvm.com/Article/details/gnmuyzcuk.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://m.share.zdbjq.cn/Article/details/gmmgrlvwu.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wap.hesvh.cn/Article/details/gwyhdyyyy.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.share.zdbjq.cn/Article/details/gdssqmhnl.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.share.hesvh.cn/Article/details/gzmbpcpel.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.blog.hesvh.cn/Article/details/gbcxbvnsw.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.m.share.fehbvm.com/Article/details/gtvckagob.sHtML

[J07] 比较两个日期
来源：http://www.m.share.hesvh.cn/Article/details/gsrhinuaq.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://m.share.fehbvm.com/Article/details/gjkftosdp.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://read.share.hesvh.cn/Article/details/gvhrwseot.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://m.share.zdbjq.cn/Article/details/gehvqlixw.sHtML


<!-- 参考信息 -->