代发 wailian999

Py:   from abc import ABC, abstractmethod
来源：http://mobile.zdbjq.cn/Article/details/gtvepabxa.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.fehbvm.com/Article/details/gntotllzz.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.zdbjq.cn/Article/details/giigtyhje.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.fehbvm.com/Article/details/gabitshaj.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.hesvh.cn/Article/details/gizjhpcwa.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.hesvh.cn/Article/details/gehitezlc.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.fehbvm.com/Article/details/gvundqkgs.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.fehbvm.com/Article/details/glolvdoma.sHtML

[G10] 访问控制
来源：http://3g.hesvh.cn/Article/details/ggtkyklhl.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.hesvh.cn/Article/details/ghciyqrvn.sHtML

PHP:  public / protected / private
来源：http://www.m.share.zdbjq.cn/Article/details/gcnxgsbwr.sHtML

JS:   #private 字段；其余公开
来源：http://wap.zdbjq.cn/Article/details/gtcefyoui.sHtML

TS:   public / protected / private
来源：http://blog.zdbjq.cn/Article/details/gkqnfquua.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.zdbjq.cn/Article/details/gnbjdpnjj.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.fehbvm.com/Article/details/ggsckrayu.sHtML

Ruby: public / protected / private
来源：http://wap.zdbjq.cn/Article/details/ggbhmihnn.sHtML

C#:   public / protected / private / internal
来源：http://baike.zdbjq.cn/Article/details/guebrqtlm.sHtML

[G11] getter / setter
来源：http://3g.hesvh.cn/Article/details/gdssveyfo.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.fehbvm.com/Article/details/ghphrqpaa.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.zdbjq.cn/Article/details/gketrtxpj.sHtML

JS:   get name() { return this._name; }
来源：http://wap.zdbjq.cn/Article/details/govtvwwmu.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.zdbjq.cn/Article/details/gsffbywzb.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gznpidfuc.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.fehbvm.com/Article/details/gwjfwdvps.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.fehbvm.com/Article/details/gtkhgfitv.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.fehbvm.com/Article/details/grqjwebbf.sHtML

[G12] 对象转字符串
来源：http://m.share.fehbvm.com/Article/details/gbcqxasuf.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.fehbvm.com/Article/details/gljhxnwoz.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.hesvh.cn/Article/details/gwckbhjqs.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.fehbvm.com/Article/details/gkyulones.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/gsviwckoi.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.fehbvm.com/Article/details/gdepbhpbg.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.fehbvm.com/Article/details/glwlarsis.sHtML

Ruby: def to_s; @name; end
来源：http://baike.zdbjq.cn/Article/details/gqswjhrzr.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.zdbjq.cn/Article/details/gdszznnfp.sHtML

[G13] 判断对象类型
来源：http://wap.hesvh.cn/Article/details/gkgawifcx.sHtML

Py:   isinstance(u, User)
来源：http://baike.fehbvm.com/Article/details/gcyoelqkm.sHtML

PHP:  $u instanceof User
来源：http://read.share.hesvh.cn/Article/details/gnojsctgj.sHtML

JS:   u instanceof User
来源：http://3g.fehbvm.com/Article/details/gektuulow.sHtML

TS:   u instanceof User
来源：http://blog.zdbjq.cn/Article/details/gsdjbbuom.sHtML

Java: u instanceof User
来源：http://www.m.share.hesvh.cn/Article/details/gypiwzckm.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.hesvh.cn/Article/details/gilemqoyq.sHtML

Ruby: u.is_a?(User)
来源：http://baike.zdbjq.cn/Article/details/gwdxmmtea.sHtML

C#:   u is User
来源：http://read.share.zdbjq.cn/Article/details/gxegkofye.sHtML

[G14] 数据类 / record
来源：http://3g.fehbvm.com/Article/details/gtkzvxxsa.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.zdbjq.cn/Article/details/gzpgeidzk.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.fehbvm.com/Article/details/gcvjbijbg.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.hesvh.cn/Article/details/gzaeiyksi.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.hesvh.cn/Article/details/glqrktirj.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.hesvh.cn/Article/details/gaqydauzq.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.zdbjq.cn/Article/details/ghoconvum.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.fehbvm.com/Article/details/gltdhbxmh.sHtML

C#:   record User(string Name, int Age);
来源：http://m.share.hesvh.cn/Article/details/gddzveyzu.sHtML

[G15] 枚举
来源：http://www.blog.hesvh.cn/Article/details/gqcrozece.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.hesvh.cn/Article/details/gyqeahkkl.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://baike.zdbjq.cn/Article/details/gnmqpeluy.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.fehbvm.com/Article/details/gzhdywpgr.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.hesvh.cn/Article/details/gdfhfkjee.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.fehbvm.com/Article/details/gvtpunwcy.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.hesvh.cn/Article/details/gtesgopxv.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.hesvh.cn/Article/details/goyfbrmke.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.zdbjq.cn/Article/details/gkykaxksm.sHtML

[G16] 对象转数组 / 字典
来源：http://www.m.share.zdbjq.cn/Article/details/gnfihjimu.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.zdbjq.cn/Article/details/gxkcthomz.sHtML

PHP:  get_object_vars($obj);
来源：http://3g.hesvh.cn/Article/details/gautmdamx.sHtML

JS:   Object.entries(obj)
来源：http://blog.fehbvm.com/Article/details/gwwirxvyn.sHtML

TS:   Object.entries(obj)
来源：http://wap.zdbjq.cn/Article/details/gjpxowbhl.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://read.share.zdbjq.cn/Article/details/guiryqded.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://wap.zdbjq.cn/Article/details/gfzbrnmsz.sHtML

Ruby: obj.instance_variables
来源：http://www.m.share.fehbvm.com/Article/details/gcjggcizc.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.hesvh.cn/Article/details/ghslkixhu.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/ggaqmrznn.sHtML

H. 异常与错误处理
来源：http://3g.zdbjq.cn/Article/details/gwlzzgzaa.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gcipdgcvy.sHtML

[H01] try / catch 基础
来源：http://www.m.share.zdbjq.cn/Article/details/gdrvfjwir.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.zdbjq.cn/Article/details/gabheqbtt.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.hesvh.cn/Article/details/gwqffryqj.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://blog.hesvh.cn/Article/details/grporicsf.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.zdbjq.cn/Article/details/gabpmpgpr.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.hesvh.cn/Article/details/gfreqnazs.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.hesvh.cn/Article/details/gzfqyiaub.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.hesvh.cn/Article/details/gdphfmahy.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mobile.zdbjq.cn/Article/details/gbzufrajx.sHtML

[H02] finally / ensure 收尾
来源：http://baike.fehbvm.com/Article/details/gdkqhfaob.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://mobile.hesvh.cn/Article/details/gonljjsqz.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.m.share.fehbvm.com/Article/details/gpqfnxoph.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://3g.fehbvm.com/Article/details/gwmsrvclq.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.fehbvm.com/Article/details/gmwfskuwv.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/geqqlmpja.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.zdbjq.cn/Article/details/gpzjrqmcf.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.m.share.hesvh.cn/Article/details/gvaarlhjr.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.share.zdbjq.cn/Article/details/gcvotxurv.sHtML

[H03] 主动抛出异常
来源：http://m.share.hesvh.cn/Article/details/glvttpwez.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.m.share.zdbjq.cn/Article/details/gwazxlsqc.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.fehbvm.com/Article/details/gtvwijxer.sHtML

JS:   throw new Error("错误信息");
来源：http://baike.zdbjq.cn/Article/details/gkihawvck.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.fehbvm.com/Article/details/gnnnftoax.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.hesvh.cn/Article/details/gkcxowova.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.m.share.fehbvm.com/Article/details/ggvdivpgg.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.zdbjq.cn/Article/details/gvtiejwvc.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.blog.hesvh.cn/Article/details/gmangebtr.sHtML

[H04] 自定义异常类型
来源：http://mobile.fehbvm.com/Article/details/glgbbqnkx.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.fehbvm.com/Article/details/gczsfjxel.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://baike.hesvh.cn/Article/details/gbjqrgpib.sHtML

JS:   class MyError extends Error {}
来源：http://read.share.hesvh.cn/Article/details/gborupmvq.sHtML

TS:   class MyError extends Error {}
来源：http://3g.fehbvm.com/Article/details/ghfkynmog.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.m.share.hesvh.cn/Article/details/gczwwrjzm.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.fehbvm.com/Article/details/gmxwopbse.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.hesvh.cn/Article/details/gohzqophi.sHtML

C#:   class MyException : Exception {}
来源：http://mobile.zdbjq.cn/Article/details/goavmuwzx.sHtML

[H05] 捕获特定类型
来源：http://www.blog.zdbjq.cn/Article/details/gtakpxmit.sHtML

Py:   except ValueError as e:
来源：http://www.m.share.hesvh.cn/Article/details/gwunsywot.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://read.share.fehbvm.com/Article/details/gphtipkrc.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://m.share.zdbjq.cn/Article/details/gglfdrqjm.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://3g.fehbvm.com/Article/details/gfcmhytmu.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://wap.fehbvm.com/Article/details/grevtxhwi.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.blog.hesvh.cn/Article/details/guuicdple.sHtML

Ruby: rescue ArgumentError => e
来源：http://read.share.zdbjq.cn/Article/details/geodjntct.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.share.fehbvm.com/Article/details/gxpmwdaro.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.zdbjq.cn/Article/details/gqgymdtjd.sHtML

Py:   value = d.get("k") or default
来源：http://wap.hesvh.cn/Article/details/gzxyebfic.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.blog.fehbvm.com/Article/details/gdcvojfgb.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.zdbjq.cn/Article/details/ghkgaddhv.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.blog.hesvh.cn/Article/details/gprtailhf.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.m.share.hesvh.cn/Article/details/gmdxleuuz.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.share.hesvh.cn/Article/details/gnwazuejr.sHtML

Ruby: d&.dig(:a, :b)
来源：http://3g.zdbjq.cn/Article/details/gwcdyblmc.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.m.share.fehbvm.com/Article/details/gakrbwjbg.sHtML

[H07] 断言
来源：http://www.m.share.fehbvm.com/Article/details/gjcoixehl.sHtML

Py:   assert x > 0, "必须为正"
来源：http://blog.hesvh.cn/Article/details/guifxafsz.sHtML

PHP:  assert($x > 0);
来源：http://wap.fehbvm.com/Article/details/ggibmapfb.sHtML

JS:   console.assert(x > 0);
来源：http://www.m.share.hesvh.cn/Article/details/gguqvjvcg.sHtML

TS:   console.assert(x > 0);
来源：http://www.m.share.hesvh.cn/Article/details/gfsttuwuj.sHtML

Java: assert x > 0 : "必须为正";
来源：http://baike.fehbvm.com/Article/details/gnkcehrlb.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://baike.hesvh.cn/Article/details/grmndwwtq.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.blog.zdbjq.cn/Article/details/gzutpdosk.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.share.fehbvm.com/Article/details/gtlsvozqc.sHtML

[H08] 获取错误信息与堆栈
来源：http://3g.fehbvm.com/Article/details/gwgstkppu.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.blog.fehbvm.com/Article/details/gcjckmtqu.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wap.zdbjq.cn/Article/details/gqnjrnyce.sHtML

JS:   e.message;  e.stack
来源：http://mobile.fehbvm.com/Article/details/gvbbhsitu.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://wap.zdbjq.cn/Article/details/gwgnoqxvu.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://baike.hesvh.cn/Article/details/gbjjaewrt.sHtML

Go:   err.Error()
来源：http://baike.fehbvm.com/Article/details/gfdfujwfm.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.m.share.zdbjq.cn/Article/details/gtryzcldg.sHtML

C#:   e.Message;  e.StackTrace
来源：http://m.share.hesvh.cn/Article/details/gmbjbnpvn.sHtML

[H09] 带错误码的异常
来源：http://read.share.hesvh.cn/Article/details/gdznidljq.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://read.share.zdbjq.cn/Article/details/goouysiju.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.blog.hesvh.cn/Article/details/geclzjslc.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mobile.fehbvm.com/Article/details/giiegijjm.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://baike.fehbvm.com/Article/details/gnwtbxyuv.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.share.zdbjq.cn/Article/details/gbhsohmuu.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://baike.fehbvm.com/Article/details/grhkhtwkf.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://blog.fehbvm.com/Article/details/gcmdgbcad.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.m.share.zdbjq.cn/Article/details/grhgtgagz.sHtML

[H10] 资源自动释放
来源：http://www.m.share.zdbjq.cn/Article/details/gpehpyqrg.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://baike.hesvh.cn/Article/details/gvrhtzqwn.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wap.fehbvm.com/Article/details/gkdubpyzc.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.zdbjq.cn/Article/details/gbafgaczu.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.hesvh.cn/Article/details/grzeowrax.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://3g.hesvh.cn/Article/details/godpfrolj.sHtML

Go:   defer f.Close()
来源：http://m.share.zdbjq.cn/Article/details/gbozgsmux.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://blog.fehbvm.com/Article/details/gbcprxdud.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://read.share.fehbvm.com/Article/details/ggbfllrhy.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gqrzmdlbs.sHtML

I. 正则表达式
来源：http://read.share.zdbjq.cn/Article/details/gacetffls.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gzahribre.sHtML

[I01] 判断是否匹配
来源：http://wap.fehbvm.com/Article/details/gtijsgyoc.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://3g.fehbvm.com/Article/details/gyjecjpjy.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://3g.fehbvm.com/Article/details/gcmeyjkyl.sHtML

JS:   /\d+/.test(s)
来源：http://wap.fehbvm.com/Article/details/gnpdfitkg.sHtML

TS:   /\d+/.test(s)
来源：http://www.blog.zdbjq.cn/Article/details/gysgdhvrk.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.m.share.hesvh.cn/Article/details/gcieuyxay.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.blog.hesvh.cn/Article/details/ggkcpoxdm.sHtML

Ruby: s.match?(/\d+/)
来源：http://blog.zdbjq.cn/Article/details/gumivlypj.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://3g.fehbvm.com/Article/details/gapatpryy.sHtML

[I02] 提取所有匹配
来源：http://3g.fehbvm.com/Article/details/gpunjfucd.sHtML

Py:   re.findall(r"\d+", s)
来源：http://blog.hesvh.cn/Article/details/gbgoxgdbm.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.blog.fehbvm.com/Article/details/guqlwobpp.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://blog.fehbvm.com/Article/details/gbqzainhq.sHtML

TS:   s.match(/\d+/g)
来源：http://www.m.share.zdbjq.cn/Article/details/gezwwmiwg.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://m.share.fehbvm.com/Article/details/gwqajints.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.share.zdbjq.cn/Article/details/gycmmcgns.sHtML

Ruby: s.scan(/\d+/)
来源：http://3g.fehbvm.com/Article/details/gskgazgmv.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.share.zdbjq.cn/Article/details/gtvqxjjzg.sHtML

[I03] 提取捕获分组
来源：http://mobile.hesvh.cn/Article/details/grekqseps.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.blog.fehbvm.com/Article/details/gojgekqyd.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.blog.zdbjq.cn/Article/details/gkqejbnok.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://m.share.fehbvm.com/Article/details/gcrfyetix.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mobile.hesvh.cn/Article/details/gucrpkorb.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://baike.zdbjq.cn/Article/details/getuhcnyk.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://3g.fehbvm.com/Article/details/gurqhbuda.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wap.hesvh.cn/Article/details/ghyfmbjra.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://blog.hesvh.cn/Article/details/ghqkorkuu.sHtML

[I04] 正则替换
来源：http://wap.hesvh.cn/Article/details/gxdnqdczb.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://blog.hesvh.cn/Article/details/gtxtijnwk.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://m.share.fehbvm.com/Article/details/gsxwohnrn.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://wap.hesvh.cn/Article/details/gjietkrqs.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.blog.fehbvm.com/Article/details/gmtaywpym.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://wap.fehbvm.com/Article/details/gywvgglry.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://mobile.fehbvm.com/Article/details/grexmdbgl.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://baike.hesvh.cn/Article/details/gkqhmrowi.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://blog.fehbvm.com/Article/details/gtidjzgyf.sHtML

[I05] 按正则拆分
来源：http://m.share.hesvh.cn/Article/details/gohbzaxbj.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.share.hesvh.cn/Article/details/gouuaosrd.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.share.zdbjq.cn/Article/details/gfvpmpuee.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://m.share.zdbjq.cn/Article/details/goouyxtgp.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://m.share.hesvh.cn/Article/details/gosvofowm.sHtML

Java: s.split("\\s*,\\s*")
来源：http://wap.fehbvm.com/Article/details/gboneylea.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://3g.hesvh.cn/Article/details/gjkuhmylg.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://baike.zdbjq.cn/Article/details/geyllxpse.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://m.share.hesvh.cn/Article/details/gswpftzer.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://blog.fehbvm.com/Article/details/gouhgiqmk.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://baike.hesvh.cn/Article/details/gohratzwr.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wap.zdbjq.cn/Article/details/gmyipprkz.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.fehbvm.com/Article/details/gcevqhecz.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.hesvh.cn/Article/details/gcnifxgas.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wap.zdbjq.cn/Article/details/gmzhkzbqo.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://m.share.zdbjq.cn/Article/details/gkapzjufv.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wap.zdbjq.cn/Article/details/grnsktgmp.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mobile.zdbjq.cn/Article/details/gmijrwpac.sHtML

[I07] 忽略大小写与多行模式
来源：http://wap.fehbvm.com/Article/details/gxwaddpbq.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://read.share.zdbjq.cn/Article/details/gzokhtrux.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://m.share.zdbjq.cn/Article/details/gvgarzuuu.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.m.share.hesvh.cn/Article/details/gwyomlniz.sHtML

TS:   /error/gim
来源：http://wap.hesvh.cn/Article/details/gkxechkkn.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://3g.hesvh.cn/Article/details/gtoukfkhj.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://baike.hesvh.cn/Article/details/gijzxldzq.sHtML

Ruby: s.scan(/error/i)
来源：http://baike.fehbvm.com/Article/details/gopodrdmd.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://blog.zdbjq.cn/Article/details/gueyzkjqq.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://3g.hesvh.cn/Article/details/ghhxixwou.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mobile.zdbjq.cn/Article/details/gqodznjdc.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wap.hesvh.cn/Article/details/gzukonwyt.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.fehbvm.com/Article/details/gnwourrvz.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.fehbvm.com/Article/details/ghnyhbove.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.share.zdbjq.cn/Article/details/gtfcsccra.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.blog.fehbvm.com/Article/details/gjlvpaxxi.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://3g.fehbvm.com/Article/details/genzoaajt.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.share.hesvh.cn/Article/details/gzyiopcan.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gbtuzgprj.sHtML

J. 日期与时间
来源：http://wap.zdbjq.cn/Article/details/ggqunudfd.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gigkhirmx.sHtML

[J01] 获取当前时间
来源：http://wap.fehbvm.com/Article/details/gudctvsew.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.share.zdbjq.cn/Article/details/gnonjbfuz.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mobile.hesvh.cn/Article/details/goladbejf.sHtML

JS:   new Date();  Date.now()
来源：http://wap.hesvh.cn/Article/details/gvizuvnmy.sHtML

TS:   new Date();  Date.now()
来源：http://m.share.hesvh.cn/Article/details/gmjjwuvxs.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://baike.zdbjq.cn/Article/details/gnkzqtmzy.sHtML

Go:   time.Now()
来源：http://wap.zdbjq.cn/Article/details/gymrgugrt.sHtML

Ruby: Time.now
来源：http://wap.fehbvm.com/Article/details/gpqoxgeuy.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://mobile.hesvh.cn/Article/details/gswkkodsv.sHtML

[J02] 格式化输出
来源：http://mobile.zdbjq.cn/Article/details/gdojbjmju.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.hesvh.cn/Article/details/gjujutzgq.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.blog.zdbjq.cn/Article/details/gvktbewtr.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://baike.hesvh.cn/Article/details/grrisajni.sHtML

TS:   d.toISOString()
来源：http://wap.hesvh.cn/Article/details/grejmxhql.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://m.share.zdbjq.cn/Article/details/gozdhfhon.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.share.fehbvm.com/Article/details/gltdibpfl.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.zdbjq.cn/Article/details/gryhauqpj.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.blog.fehbvm.com/Article/details/gxnlytlxk.sHtML

[J03] 字符串解析为日期
来源：http://www.m.share.hesvh.cn/Article/details/gcybymqfk.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://read.share.fehbvm.com/Article/details/gwynynvin.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wap.zdbjq.cn/Article/details/goxdccqml.sHtML

JS:   new Date("2024-01-02")
来源：http://baike.hesvh.cn/Article/details/gtwymiayw.sHtML

TS:   new Date("2024-01-02")
来源：http://3g.hesvh.cn/Article/details/gxjqlqdum.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://baike.zdbjq.cn/Article/details/gwvkzmctm.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://3g.hesvh.cn/Article/details/gdsvpgpdx.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://wap.hesvh.cn/Article/details/gydrveclu.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mobile.zdbjq.cn/Article/details/gnrvgphio.sHtML

[J04] 时间戳与日期互转
来源：http://wap.zdbjq.cn/Article/details/gfzsxwdzb.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://m.share.hesvh.cn/Article/details/guqvxmcmr.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.blog.zdbjq.cn/Article/details/gwpiqsfvv.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.blog.zdbjq.cn/Article/details/glwzznouq.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://read.share.hesvh.cn/Article/details/gesouhyua.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.blog.hesvh.cn/Article/details/gwelkhxyq.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.share.hesvh.cn/Article/details/gggclmcld.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.share.hesvh.cn/Article/details/gzhqrhqdu.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://read.share.zdbjq.cn/Article/details/goferwghq.sHtML

[J05] 时间加减（加 7 天）
来源：http://m.share.fehbvm.com/Article/details/gfzpjtrwm.sHtML

Py:   now + timedelta(days=7)
来源：http://m.share.hesvh.cn/Article/details/gciicoudc.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.blog.hesvh.cn/Article/details/ghjnnhcfv.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.fehbvm.com/Article/details/gaedtxbfk.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.zdbjq.cn/Article/details/gpccumtzs.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://3g.hesvh.cn/Article/details/geutmfaav.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://blog.fehbvm.com/Article/details/gagjfxvjn.sHtML

Ruby: Time.now + 7 * 86400
来源：http://mobile.fehbvm.com/Article/details/gsxcqnmar.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://blog.zdbjq.cn/Article/details/gblbdyyzk.sHtML

[J06] 计算两时间之差
来源：http://www.share.fehbvm.com/Article/details/gvxrqrxmg.sHtML

Py:   (end - start).total_seconds()
来源：http://3g.fehbvm.com/Article/details/gtkvuyhld.sHtML

PHP:  $end->diff($start)->days;
来源：http://baike.hesvh.cn/Article/details/gsollksan.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://baike.fehbvm.com/Article/details/gvolezhhy.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://m.share.hesvh.cn/Article/details/gcfjvabnh.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://wap.zdbjq.cn/Article/details/geppulcpm.sHtML

Go:   end.Sub(start).Hours()
来源：http://3g.hesvh.cn/Article/details/gvhmgqqmr.sHtML

Ruby: end - start                 # 返回秒数
来源：http://baike.hesvh.cn/Article/details/gvquawkae.sHtML

C#:   (end - start).TotalSeconds
来源：http://read.share.fehbvm.com/Article/details/guvuwdyvs.sHtML

[J07] 比较两个日期
来源：http://mobile.zdbjq.cn/Article/details/glqucuqrm.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.m.share.zdbjq.cn/Article/details/gcplenhtp.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://read.share.fehbvm.com/Article/details/gnfduystu.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://blog.zdbjq.cn/Article/details/gxbfuyrzr.sHtML


<!-- 参考信息 -->