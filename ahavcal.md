代发 wailian999

Py:   from abc import ABC, abstractmethod
来源：http://m.share.zdbjq.cn/Article/details/gurwjyybh.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.fehbvm.com/Article/details/gbkhuieyb.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.fehbvm.com/Article/details/gvgkcxdpp.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.hesvh.cn/Article/details/gyspzhccj.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.zdbjq.cn/Article/details/gornigsww.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.fehbvm.com/Article/details/gogdonxxo.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.fehbvm.com/Article/details/gcsgaebfj.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gtbxqsydg.sHtML

[G10] 访问控制
来源：http://blog.fehbvm.com/Article/details/gfmwsuvan.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.hesvh.cn/Article/details/gruwfzlhf.sHtML

PHP:  public / protected / private
来源：http://www.m.share.hesvh.cn/Article/details/ghlmudixt.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.hesvh.cn/Article/details/gxyrtzmkk.sHtML

TS:   public / protected / private
来源：http://3g.hesvh.cn/Article/details/gvgvsfwko.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.hesvh.cn/Article/details/gjitbkyyf.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.fehbvm.com/Article/details/gqwnxzrqg.sHtML

Ruby: public / protected / private
来源：http://mobile.zdbjq.cn/Article/details/gtdtisyjs.sHtML

C#:   public / protected / private / internal
来源：http://3g.hesvh.cn/Article/details/grgldtdej.sHtML

[G11] getter / setter
来源：http://www.m.share.fehbvm.com/Article/details/gocebkoqi.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.hesvh.cn/Article/details/gayyarrpq.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.hesvh.cn/Article/details/giovsopfc.sHtML

JS:   get name() { return this._name; }
来源：http://wap.zdbjq.cn/Article/details/gxyhnbprq.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.fehbvm.com/Article/details/gyubahcnd.sHtML

Java: public String getName() { return name; }
来源：http://wap.zdbjq.cn/Article/details/gdikojbhl.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.hesvh.cn/Article/details/gmszasqwb.sHtML

Ruby: attr_accessor :name
来源：http://m.share.zdbjq.cn/Article/details/gukafocjx.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.zdbjq.cn/Article/details/gwupwahvh.sHtML

[G12] 对象转字符串
来源：http://mobile.hesvh.cn/Article/details/gwztlnwaf.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.zdbjq.cn/Article/details/gsjzaxyuw.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.fehbvm.com/Article/details/glewpknnp.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.hesvh.cn/Article/details/guxfwmlxu.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.fehbvm.com/Article/details/gtipypujs.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.fehbvm.com/Article/details/gfhiwrvda.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.hesvh.cn/Article/details/gpkkkxyac.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.fehbvm.com/Article/details/gbozvkenv.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.fehbvm.com/Article/details/gjqardogo.sHtML

[G13] 判断对象类型
来源：http://wap.zdbjq.cn/Article/details/gskdqogyi.sHtML

Py:   isinstance(u, User)
来源：http://wap.fehbvm.com/Article/details/gqowyjesz.sHtML

PHP:  $u instanceof User
来源：http://wap.fehbvm.com/Article/details/gyufurxut.sHtML

JS:   u instanceof User
来源：http://read.share.fehbvm.com/Article/details/gvxffzgwy.sHtML

TS:   u instanceof User
来源：http://m.share.zdbjq.cn/Article/details/gqsltczyd.sHtML

Java: u instanceof User
来源：http://wap.hesvh.cn/Article/details/gqebuyuhc.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.fehbvm.com/Article/details/grooryixs.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.zdbjq.cn/Article/details/gjkoyfzgz.sHtML

C#:   u is User
来源：http://read.share.fehbvm.com/Article/details/gdgkajpyr.sHtML

[G14] 数据类 / record
来源：http://wap.zdbjq.cn/Article/details/gtvulpfhc.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.hesvh.cn/Article/details/ghsiujjtl.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.zdbjq.cn/Article/details/ghavmdauj.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.fehbvm.com/Article/details/gfwtesdsu.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.zdbjq.cn/Article/details/geasfodou.sHtML

Java: record User(String name, int age) {}
来源：http://3g.hesvh.cn/Article/details/gyfzexssl.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.zdbjq.cn/Article/details/gussxtwsj.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.hesvh.cn/Article/details/gqfevwyju.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.fehbvm.com/Article/details/ghixeqljs.sHtML

[G15] 枚举
来源：http://wap.hesvh.cn/Article/details/gcesthweh.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.fehbvm.com/Article/details/gblvrcliv.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.fehbvm.com/Article/details/gxrzrijkr.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.m.share.fehbvm.com/Article/details/gbwpemjwy.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gmfkssexd.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.fehbvm.com/Article/details/gzwcfqfsz.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://blog.hesvh.cn/Article/details/ghcymhpty.sHtML

Ruby: Color = %i[red green].freeze
来源：http://read.share.fehbvm.com/Article/details/gjcttmwwr.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.zdbjq.cn/Article/details/gioiujzpn.sHtML

[G16] 对象转数组 / 字典
来源：http://www.blog.fehbvm.com/Article/details/gefaowjug.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.hesvh.cn/Article/details/goasdybvt.sHtML

PHP:  get_object_vars($obj);
来源：http://wap.fehbvm.com/Article/details/gobiumcvd.sHtML

JS:   Object.entries(obj)
来源：http://baike.fehbvm.com/Article/details/gopkcgxkw.sHtML

TS:   Object.entries(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gbqjnlsyd.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://blog.hesvh.cn/Article/details/gwbhswfre.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://3g.fehbvm.com/Article/details/gwxuvhvyt.sHtML

Ruby: obj.instance_variables
来源：http://www.share.zdbjq.cn/Article/details/geubwbrpt.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.fehbvm.com/Article/details/gzzftpipc.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/ghqttvjdr.sHtML

H. 异常与错误处理
来源：http://www.share.zdbjq.cn/Article/details/gjrgxdund.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gyhhezmhz.sHtML

[H01] try / catch 基础
来源：http://blog.hesvh.cn/Article/details/ghfddreaf.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://baike.hesvh.cn/Article/details/gdjeeznmo.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.hesvh.cn/Article/details/gvhulztwh.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.fehbvm.com/Article/details/gwzbolwvd.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.hesvh.cn/Article/details/gpfatraoi.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.fehbvm.com/Article/details/gxtsmyjsc.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.zdbjq.cn/Article/details/gtiabgbms.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.zdbjq.cn/Article/details/glnvofrfg.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.hesvh.cn/Article/details/gwgzplzwj.sHtML

[H02] finally / ensure 收尾
来源：http://3g.hesvh.cn/Article/details/glwuspouz.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.m.share.zdbjq.cn/Article/details/gwnxhcpvu.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.zdbjq.cn/Article/details/grcbnpztr.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.zdbjq.cn/Article/details/ghifpwdek.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://blog.zdbjq.cn/Article/details/gcsmjkwom.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/gtqwvpkgb.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.share.fehbvm.com/Article/details/gbybqflml.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.zdbjq.cn/Article/details/guzpyvsem.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://m.share.fehbvm.com/Article/details/gspaaslxl.sHtML

[H03] 主动抛出异常
来源：http://mobile.fehbvm.com/Article/details/ghyjsylqh.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.m.share.hesvh.cn/Article/details/gfvevwajh.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.zdbjq.cn/Article/details/gwkgkhtgu.sHtML

JS:   throw new Error("错误信息");
来源：http://www.m.share.zdbjq.cn/Article/details/govekxlaq.sHtML

TS:   throw new Error("错误信息");
来源：http://read.share.fehbvm.com/Article/details/gipaypvyp.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://blog.zdbjq.cn/Article/details/gktagmksn.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mobile.fehbvm.com/Article/details/gnxgklzce.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://blog.fehbvm.com/Article/details/gqegnszrm.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://baike.hesvh.cn/Article/details/gsfxbcqey.sHtML

[H04] 自定义异常类型
来源：http://www.blog.hesvh.cn/Article/details/gasautsac.sHtML

Py:   class MyError(Exception): pass
来源：http://blog.fehbvm.com/Article/details/giwtyolpv.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.fehbvm.com/Article/details/glfksvvck.sHtML

JS:   class MyError extends Error {}
来源：http://m.share.fehbvm.com/Article/details/gloqighmw.sHtML

TS:   class MyError extends Error {}
来源：http://www.blog.fehbvm.com/Article/details/girvfjnll.sHtML

Java: class MyException extends RuntimeException {}
来源：http://mobile.fehbvm.com/Article/details/gyanzuccf.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.share.hesvh.cn/Article/details/gpleaqlhy.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.m.share.zdbjq.cn/Article/details/gbpgjfwwi.sHtML

C#:   class MyException : Exception {}
来源：http://www.blog.zdbjq.cn/Article/details/gdvdnnnky.sHtML

[H05] 捕获特定类型
来源：http://www.share.hesvh.cn/Article/details/gfrokqosy.sHtML

Py:   except ValueError as e:
来源：http://m.share.fehbvm.com/Article/details/giprouhqq.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.fehbvm.com/Article/details/gitptvbic.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.blog.zdbjq.cn/Article/details/gguqewraw.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://wap.zdbjq.cn/Article/details/gqgqozrxz.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.blog.hesvh.cn/Article/details/gywwbflvy.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.m.share.zdbjq.cn/Article/details/gxnbypljw.sHtML

Ruby: rescue ArgumentError => e
来源：http://3g.zdbjq.cn/Article/details/gyvtbddjt.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://blog.fehbvm.com/Article/details/gracysiap.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.hesvh.cn/Article/details/gfvoygasx.sHtML

Py:   value = d.get("k") or default
来源：http://mobile.fehbvm.com/Article/details/gnnzfuhbm.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://blog.fehbvm.com/Article/details/gwowglcud.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.blog.zdbjq.cn/Article/details/gggevtczs.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://mobile.zdbjq.cn/Article/details/glmrzqlte.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://blog.fehbvm.com/Article/details/gasjvovjn.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.blog.fehbvm.com/Article/details/gjxnrmzxg.sHtML

Ruby: d&.dig(:a, :b)
来源：http://mobile.zdbjq.cn/Article/details/gkdrzamzc.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.blog.zdbjq.cn/Article/details/ghxgdwqsr.sHtML

[H07] 断言
来源：http://wap.fehbvm.com/Article/details/gasrncmax.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.blog.hesvh.cn/Article/details/govfwelzx.sHtML

PHP:  assert($x > 0);
来源：http://www.m.share.hesvh.cn/Article/details/gbtunnsdp.sHtML

JS:   console.assert(x > 0);
来源：http://read.share.hesvh.cn/Article/details/ghdrhbogt.sHtML

TS:   console.assert(x > 0);
来源：http://www.m.share.fehbvm.com/Article/details/gucplvzot.sHtML

Java: assert x > 0 : "必须为正";
来源：http://read.share.fehbvm.com/Article/details/gfyqgldel.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://3g.hesvh.cn/Article/details/gmomcnknq.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://read.share.hesvh.cn/Article/details/ggcvusupn.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.share.zdbjq.cn/Article/details/gudiiqdpn.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.share.fehbvm.com/Article/details/grvdlfuhn.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://baike.fehbvm.com/Article/details/ghbjncgkx.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://baike.fehbvm.com/Article/details/ginwaebhw.sHtML

JS:   e.message;  e.stack
来源：http://3g.zdbjq.cn/Article/details/gfzsdbfov.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://baike.zdbjq.cn/Article/details/gmxsfvxpz.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://mobile.fehbvm.com/Article/details/ghromrcnf.sHtML

Go:   err.Error()
来源：http://baike.zdbjq.cn/Article/details/ggnsqzwgv.sHtML

Ruby: e.message;  e.backtrace
来源：http://m.share.zdbjq.cn/Article/details/gkdqcegbx.sHtML

C#:   e.Message;  e.StackTrace
来源：http://blog.fehbvm.com/Article/details/gtsbposnr.sHtML

[H09] 带错误码的异常
来源：http://www.m.share.fehbvm.com/Article/details/goaelhngm.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.m.share.fehbvm.com/Article/details/ginlgrjof.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://3g.hesvh.cn/Article/details/gikvhsdfz.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://blog.fehbvm.com/Article/details/gstvjqwxm.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.share.hesvh.cn/Article/details/gbrnkatth.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.m.share.hesvh.cn/Article/details/gexkchkkh.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://blog.fehbvm.com/Article/details/gpubtxjgh.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://blog.hesvh.cn/Article/details/gblfzxsec.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://wap.fehbvm.com/Article/details/gylxyxdyg.sHtML

[H10] 资源自动释放
来源：http://www.m.share.fehbvm.com/Article/details/gscarrmqy.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://baike.fehbvm.com/Article/details/gtpbangob.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://3g.fehbvm.com/Article/details/gdrdybwoh.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.zdbjq.cn/Article/details/gvmgoaxqg.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.fehbvm.com/Article/details/gfrzfhutb.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.m.share.zdbjq.cn/Article/details/ghtgfqkoi.sHtML

Go:   defer f.Close()
来源：http://wap.zdbjq.cn/Article/details/guzyxamty.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.blog.fehbvm.com/Article/details/gpqassrce.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gwgspzxbo.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/guyecohbi.sHtML

I. 正则表达式
来源：http://read.share.fehbvm.com/Article/details/gujnasgeg.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gijeqihdd.sHtML

[I01] 判断是否匹配
来源：http://www.blog.fehbvm.com/Article/details/gmhrdklzl.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mobile.fehbvm.com/Article/details/gpywdweon.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.blog.fehbvm.com/Article/details/gfzdciwro.sHtML

JS:   /\d+/.test(s)
来源：http://3g.fehbvm.com/Article/details/glgusqapc.sHtML

TS:   /\d+/.test(s)
来源：http://blog.hesvh.cn/Article/details/gdvmwqvvz.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://3g.hesvh.cn/Article/details/glmqdgdua.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://blog.fehbvm.com/Article/details/gbzynuuai.sHtML

Ruby: s.match?(/\d+/)
来源：http://3g.hesvh.cn/Article/details/gingznfdz.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://blog.fehbvm.com/Article/details/gkuchpkeo.sHtML

[I02] 提取所有匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gpnnwvtxd.sHtML

Py:   re.findall(r"\d+", s)
来源：http://blog.hesvh.cn/Article/details/gqqxebozy.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://3g.fehbvm.com/Article/details/guqepddng.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://3g.zdbjq.cn/Article/details/gdcutmbtb.sHtML

TS:   s.match(/\d+/g)
来源：http://www.blog.zdbjq.cn/Article/details/glmhfvnrr.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://blog.fehbvm.com/Article/details/gewdcntik.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wap.hesvh.cn/Article/details/ghekyczlg.sHtML

Ruby: s.scan(/\d+/)
来源：http://baike.hesvh.cn/Article/details/guryqzfwp.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://read.share.zdbjq.cn/Article/details/gpunqxxzm.sHtML

[I03] 提取捕获分组
来源：http://baike.fehbvm.com/Article/details/gshbfudfn.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://read.share.zdbjq.cn/Article/details/gbdgmseze.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.m.share.zdbjq.cn/Article/details/gknjhiuwf.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.blog.zdbjq.cn/Article/details/gvpfprirc.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://read.share.zdbjq.cn/Article/details/gtntqbiye.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wap.hesvh.cn/Article/details/gguhmkizg.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mobile.fehbvm.com/Article/details/gwzsytqap.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://blog.fehbvm.com/Article/details/gxaqselkg.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://mobile.fehbvm.com/Article/details/ghhaxiroo.sHtML

[I04] 正则替换
来源：http://www.blog.fehbvm.com/Article/details/gciqvwwqt.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://read.share.fehbvm.com/Article/details/gvuxkqjvr.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mobile.zdbjq.cn/Article/details/gkfloxjco.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://read.share.zdbjq.cn/Article/details/gsxneqgwl.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://wap.zdbjq.cn/Article/details/gjeffqppw.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://m.share.zdbjq.cn/Article/details/ggsyypude.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://m.share.fehbvm.com/Article/details/gozqymgwh.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://wap.hesvh.cn/Article/details/gutmxuuks.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://3g.fehbvm.com/Article/details/gcyxqwsjw.sHtML

[I05] 按正则拆分
来源：http://www.share.zdbjq.cn/Article/details/gokroigyr.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://mobile.zdbjq.cn/Article/details/gvyfftvqa.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://baike.fehbvm.com/Article/details/gpkfckanl.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://read.share.hesvh.cn/Article/details/gfczjacac.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://3g.hesvh.cn/Article/details/gygxbleen.sHtML

Java: s.split("\\s*,\\s*")
来源：http://wap.fehbvm.com/Article/details/gwqkwethf.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://m.share.zdbjq.cn/Article/details/gxodmiziy.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.blog.fehbvm.com/Article/details/glfweawfs.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://baike.fehbvm.com/Article/details/gfbrlakml.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wap.fehbvm.com/Article/details/gtsfbewlf.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://read.share.fehbvm.com/Article/details/grtbsfvxo.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://m.share.zdbjq.cn/Article/details/gpuyjjvro.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.hesvh.cn/Article/details/goqfkesgh.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.hesvh.cn/Article/details/gcrthlidf.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://read.share.fehbvm.com/Article/details/gxsoyzggt.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wap.hesvh.cn/Article/details/gmcnofovg.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wap.hesvh.cn/Article/details/gvjmuknwb.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wap.zdbjq.cn/Article/details/gqvzpkofo.sHtML

[I07] 忽略大小写与多行模式
来源：http://read.share.zdbjq.cn/Article/details/gsqymwtpy.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://m.share.zdbjq.cn/Article/details/gdyntmapu.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wap.fehbvm.com/Article/details/ganzldenj.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.share.fehbvm.com/Article/details/gshicjmql.sHtML

TS:   /error/gim
来源：http://mobile.zdbjq.cn/Article/details/gxnhfpbze.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://baike.hesvh.cn/Article/details/goxvimlsf.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wap.hesvh.cn/Article/details/gkzddndvk.sHtML

Ruby: s.scan(/error/i)
来源：http://www.share.fehbvm.com/Article/details/glophopmg.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.m.share.zdbjq.cn/Article/details/gbaqvmssi.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.share.hesvh.cn/Article/details/gobrwzeqg.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wap.zdbjq.cn/Article/details/gywebpcec.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.share.fehbvm.com/Article/details/gaoyfdbgv.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.fehbvm.com/Article/details/gdotdkies.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.hesvh.cn/Article/details/gawgznfvq.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://read.share.fehbvm.com/Article/details/ghoyovvhe.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://blog.fehbvm.com/Article/details/gkcmqzpiw.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://baike.hesvh.cn/Article/details/gkfdobvtf.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://m.share.fehbvm.com/Article/details/gmekgybtr.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/ghgzqzmjq.sHtML

J. 日期与时间
来源：http://read.share.zdbjq.cn/Article/details/gzrpuykrf.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/giiulmcfm.sHtML

[J01] 获取当前时间
来源：http://baike.fehbvm.com/Article/details/gwzyhadyy.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://blog.fehbvm.com/Article/details/gqxfivdhv.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mobile.fehbvm.com/Article/details/gizgdevpx.sHtML

JS:   new Date();  Date.now()
来源：http://m.share.fehbvm.com/Article/details/gwbuxfotg.sHtML

TS:   new Date();  Date.now()
来源：http://blog.zdbjq.cn/Article/details/gpvtikliw.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://mobile.hesvh.cn/Article/details/gdyihqret.sHtML

Go:   time.Now()
来源：http://read.share.fehbvm.com/Article/details/gekdpphlg.sHtML

Ruby: Time.now
来源：http://blog.zdbjq.cn/Article/details/gvtmctvhb.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://3g.fehbvm.com/Article/details/giallzspq.sHtML

[J02] 格式化输出
来源：http://mobile.hesvh.cn/Article/details/gkkahqizo.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.fehbvm.com/Article/details/grrezzrxm.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mobile.zdbjq.cn/Article/details/gpdipvpki.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.blog.zdbjq.cn/Article/details/gdcqyrype.sHtML

TS:   d.toISOString()
来源：http://3g.hesvh.cn/Article/details/gtflpfzlo.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://m.share.zdbjq.cn/Article/details/gapvsbqvt.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://read.share.zdbjq.cn/Article/details/ghwccuzsg.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.hesvh.cn/Article/details/gcjndfstk.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://m.share.hesvh.cn/Article/details/gavhmmtdm.sHtML

[J03] 字符串解析为日期
来源：http://m.share.fehbvm.com/Article/details/gwtxgegub.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://blog.zdbjq.cn/Article/details/gsucwauwq.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://blog.hesvh.cn/Article/details/gftfwgdvs.sHtML

JS:   new Date("2024-01-02")
来源：http://wap.hesvh.cn/Article/details/gsxrjecck.sHtML

TS:   new Date("2024-01-02")
来源：http://3g.fehbvm.com/Article/details/gfdtwbwrf.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://baike.fehbvm.com/Article/details/gmkibdzcn.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wap.fehbvm.com/Article/details/gsrqpkpnz.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://blog.hesvh.cn/Article/details/gnblzdtya.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.share.fehbvm.com/Article/details/gachirymv.sHtML

[J04] 时间戳与日期互转
来源：http://mobile.hesvh.cn/Article/details/gbynhtkuc.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mobile.fehbvm.com/Article/details/gbrnkxlga.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://m.share.fehbvm.com/Article/details/guyidcedr.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.m.share.hesvh.cn/Article/details/gyssikfhf.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://baike.fehbvm.com/Article/details/gospgxsnk.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://m.share.hesvh.cn/Article/details/gttmsnsle.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.share.fehbvm.com/Article/details/gfbjmeuwz.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.blog.fehbvm.com/Article/details/gpvlnrcqb.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://3g.hesvh.cn/Article/details/glnfbtddv.sHtML

[J05] 时间加减（加 7 天）
来源：http://read.share.zdbjq.cn/Article/details/ggrywatmm.sHtML

Py:   now + timedelta(days=7)
来源：http://www.share.zdbjq.cn/Article/details/gvnsyhdhy.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://3g.zdbjq.cn/Article/details/gupdwwmaz.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.zdbjq.cn/Article/details/gfsjihiem.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.fehbvm.com/Article/details/gxxqepknb.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://3g.zdbjq.cn/Article/details/gspsdrrgq.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://wap.zdbjq.cn/Article/details/geotvqarg.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.blog.zdbjq.cn/Article/details/galxhmqbn.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.m.share.hesvh.cn/Article/details/gwsunpabn.sHtML

[J06] 计算两时间之差
来源：http://www.m.share.fehbvm.com/Article/details/ggtiibtgp.sHtML

Py:   (end - start).total_seconds()
来源：http://www.blog.zdbjq.cn/Article/details/gyqmzwivj.sHtML

PHP:  $end->diff($start)->days;
来源：http://3g.fehbvm.com/Article/details/gddxmlhcw.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://baike.fehbvm.com/Article/details/gveetvekc.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://m.share.hesvh.cn/Article/details/gsvhfuwym.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.share.hesvh.cn/Article/details/gbltecmwx.sHtML

Go:   end.Sub(start).Hours()
来源：http://blog.hesvh.cn/Article/details/gqenwzcbt.sHtML

Ruby: end - start                 # 返回秒数
来源：http://blog.hesvh.cn/Article/details/glcwdnwia.sHtML

C#:   (end - start).TotalSeconds
来源：http://3g.hesvh.cn/Article/details/ggnoafcmh.sHtML

[J07] 比较两个日期
来源：http://baike.hesvh.cn/Article/details/gtvpnexuh.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.m.share.hesvh.cn/Article/details/gqvguqucs.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://3g.fehbvm.com/Article/details/gilgetoeu.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.blog.hesvh.cn/Article/details/guspiguha.sHtML


<!-- 参考信息 -->