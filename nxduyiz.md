代发 wailian999

Py:   from abc import ABC, abstractmethod
来源：http://www.share.zdbjq.cn/Article/details/gqirpyshq.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.hesvh.cn/Article/details/gcgfwyfjx.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.hesvh.cn/Article/details/gndrlkugo.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.hesvh.cn/Article/details/gzjaibmtr.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.fehbvm.com/Article/details/glhgicsbx.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.hesvh.cn/Article/details/ggmgmhoka.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.zdbjq.cn/Article/details/gpwszkzgk.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.fehbvm.com/Article/details/gdswunxvw.sHtML

[G10] 访问控制
来源：http://www.blog.hesvh.cn/Article/details/gweppwzsn.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.fehbvm.com/Article/details/gvcoubibz.sHtML

PHP:  public / protected / private
来源：http://www.blog.zdbjq.cn/Article/details/gdqawwtwl.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.hesvh.cn/Article/details/gddwhhmen.sHtML

TS:   public / protected / private
来源：http://www.blog.hesvh.cn/Article/details/gsqfyerzp.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.zdbjq.cn/Article/details/gbxceijdr.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.zdbjq.cn/Article/details/gqrypyysr.sHtML

Ruby: public / protected / private
来源：http://mobile.hesvh.cn/Article/details/gcjfzecii.sHtML

C#:   public / protected / private / internal
来源：http://m.share.hesvh.cn/Article/details/gsqgdejef.sHtML

[G11] getter / setter
来源：http://m.share.fehbvm.com/Article/details/gjtclshnd.sHtML

Py:   @property 与 @x.setter
来源：http://wap.zdbjq.cn/Article/details/ghoolmsgq.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.zdbjq.cn/Article/details/giuwngxqf.sHtML

JS:   get name() { return this._name; }
来源：http://blog.zdbjq.cn/Article/details/gfnjvsdsh.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.hesvh.cn/Article/details/gdursgiyv.sHtML

Java: public String getName() { return name; }
来源：http://baike.fehbvm.com/Article/details/gloefwluu.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.fehbvm.com/Article/details/gdmzwggjn.sHtML

Ruby: attr_accessor :name
来源：http://read.share.hesvh.cn/Article/details/gbyyksxox.sHtML

C#:   public string Name { get; set; }
来源：http://wap.fehbvm.com/Article/details/gqvgecpii.sHtML

[G12] 对象转字符串
来源：http://www.blog.zdbjq.cn/Article/details/gqaewxsgd.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.fehbvm.com/Article/details/gvudokhrn.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.fehbvm.com/Article/details/gqoxrlhsl.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/gydqksoeo.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.hesvh.cn/Article/details/ghjpxnpno.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.hesvh.cn/Article/details/gwkpcjdet.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.hesvh.cn/Article/details/grdiiiukb.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.zdbjq.cn/Article/details/gcohdzhas.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.zdbjq.cn/Article/details/gszwznfbw.sHtML

[G13] 判断对象类型
来源：http://wap.zdbjq.cn/Article/details/gjkzwntjs.sHtML

Py:   isinstance(u, User)
来源：http://m.share.fehbvm.com/Article/details/gprufwpyo.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.hesvh.cn/Article/details/gdtqahsqj.sHtML

JS:   u instanceof User
来源：http://blog.hesvh.cn/Article/details/gdhdmzlbj.sHtML

TS:   u instanceof User
来源：http://www.blog.fehbvm.com/Article/details/gltefvroz.sHtML

Java: u instanceof User
来源：http://read.share.fehbvm.com/Article/details/guxhiojvk.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.share.zdbjq.cn/Article/details/gocigatcw.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.fehbvm.com/Article/details/ggpnpyccm.sHtML

C#:   u is User
来源：http://3g.fehbvm.com/Article/details/gbocvnbds.sHtML

[G14] 数据类 / record
来源：http://baike.fehbvm.com/Article/details/gomfktzxk.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.zdbjq.cn/Article/details/gjasuumst.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.zdbjq.cn/Article/details/glnvctqji.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.hesvh.cn/Article/details/gihzqjihc.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.share.fehbvm.com/Article/details/gckzqnyra.sHtML

Java: record User(String name, int age) {}
来源：http://read.share.fehbvm.com/Article/details/gzxzvwzru.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.fehbvm.com/Article/details/gpthxownk.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.hesvh.cn/Article/details/gysoprdkt.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.fehbvm.com/Article/details/gvmoksbio.sHtML

[G15] 枚举
来源：http://wap.hesvh.cn/Article/details/gsbgrxdcw.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.hesvh.cn/Article/details/gaoihukbi.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://baike.fehbvm.com/Article/details/gbphegxgl.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.fehbvm.com/Article/details/gacccxvpl.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.zdbjq.cn/Article/details/gtukhieab.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.fehbvm.com/Article/details/gctpsunkx.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.hesvh.cn/Article/details/gbcfvolnn.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.zdbjq.cn/Article/details/gjknxdxrt.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.fehbvm.com/Article/details/gdeitigia.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.zdbjq.cn/Article/details/gmgflhrsu.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.fehbvm.com/Article/details/giohocehu.sHtML

PHP:  get_object_vars($obj);
来源：http://wap.hesvh.cn/Article/details/gvjkbgopg.sHtML

JS:   Object.entries(obj)
来源：http://blog.zdbjq.cn/Article/details/gdygzxrgt.sHtML

TS:   Object.entries(obj)
来源：http://read.share.zdbjq.cn/Article/details/gxluwmdqb.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.hesvh.cn/Article/details/gdzqdzoyy.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://3g.zdbjq.cn/Article/details/gqtxfugzp.sHtML

Ruby: obj.instance_variables
来源：http://blog.zdbjq.cn/Article/details/gqqzbynsp.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.fehbvm.com/Article/details/gqhtgyvbq.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gadjrpwib.sHtML

H. 异常与错误处理
来源：http://m.share.hesvh.cn/Article/details/gaaokmmzp.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gejhiankp.sHtML

[H01] try / catch 基础
来源：http://wap.hesvh.cn/Article/details/gpjukohsx.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.hesvh.cn/Article/details/glcufovbw.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.fehbvm.com/Article/details/gzcjgjoxn.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.fehbvm.com/Article/details/guhbezrhc.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.m.share.fehbvm.com/Article/details/gxpmloakm.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.blog.fehbvm.com/Article/details/goqvwzgqa.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://read.share.fehbvm.com/Article/details/glpvczuph.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.zdbjq.cn/Article/details/gwmyhpjsk.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.m.share.zdbjq.cn/Article/details/gaoawhfwo.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.zdbjq.cn/Article/details/givbfceuq.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.m.share.fehbvm.com/Article/details/gtlummjxx.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.fehbvm.com/Article/details/grwaxfxmb.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.hesvh.cn/Article/details/gtiimwvnv.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://m.share.hesvh.cn/Article/details/gmizgkxtu.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.m.share.hesvh.cn/Article/details/geqcpyucv.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.zdbjq.cn/Article/details/gzexlunre.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.hesvh.cn/Article/details/gltqjlnvs.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.share.hesvh.cn/Article/details/gzqlybhot.sHtML

[H03] 主动抛出异常
来源：http://blog.zdbjq.cn/Article/details/glrkgmrsj.sHtML

Py:   raise ValueError("错误信息")
来源：http://baike.fehbvm.com/Article/details/gaczdtzjz.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mobile.fehbvm.com/Article/details/gblrrwmbx.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.fehbvm.com/Article/details/gdwmwykbs.sHtML

TS:   throw new Error("错误信息");
来源：http://baike.hesvh.cn/Article/details/gxbqwqjce.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.m.share.hesvh.cn/Article/details/glvjqjjpy.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.hesvh.cn/Article/details/gttyhzzwk.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.m.share.zdbjq.cn/Article/details/geyuxxcby.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://m.share.zdbjq.cn/Article/details/gdrjhhxig.sHtML

[H04] 自定义异常类型
来源：http://blog.zdbjq.cn/Article/details/glwjhmmpp.sHtML

Py:   class MyError(Exception): pass
来源：http://3g.hesvh.cn/Article/details/gsgoxnzic.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.fehbvm.com/Article/details/gzreqtdfq.sHtML

JS:   class MyError extends Error {}
来源：http://m.share.hesvh.cn/Article/details/gficwhhgm.sHtML

TS:   class MyError extends Error {}
来源：http://wap.fehbvm.com/Article/details/gjazqjlbr.sHtML

Java: class MyException extends RuntimeException {}
来源：http://3g.fehbvm.com/Article/details/geswzplka.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.m.share.fehbvm.com/Article/details/gopmjzasj.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.share.fehbvm.com/Article/details/gyoclyqwi.sHtML

C#:   class MyException : Exception {}
来源：http://www.m.share.hesvh.cn/Article/details/gvwfxarfo.sHtML

[H05] 捕获特定类型
来源：http://www.blog.hesvh.cn/Article/details/gkxapspba.sHtML

Py:   except ValueError as e:
来源：http://www.m.share.hesvh.cn/Article/details/gytneseoq.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://baike.fehbvm.com/Article/details/glevfzgoj.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://baike.zdbjq.cn/Article/details/ghgndgqxa.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://3g.zdbjq.cn/Article/details/gddkcabwz.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.fehbvm.com/Article/details/grthtjzbw.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mobile.zdbjq.cn/Article/details/guemrjylf.sHtML

Ruby: rescue ArgumentError => e
来源：http://3g.zdbjq.cn/Article/details/goksxsyha.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://3g.fehbvm.com/Article/details/gqnnndska.sHtML

[H06] 可选值 / 空值安全访问
来源：http://wap.fehbvm.com/Article/details/gvxchcyyq.sHtML

Py:   value = d.get("k") or default
来源：http://mobile.fehbvm.com/Article/details/gtnubdwrd.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://mobile.zdbjq.cn/Article/details/gytewudnn.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.zdbjq.cn/Article/details/ghrwrdmya.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://read.share.fehbvm.com/Article/details/gyowxffwu.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wap.zdbjq.cn/Article/details/gnphhmexs.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://read.share.hesvh.cn/Article/details/gctrynhag.sHtML

Ruby: d&.dig(:a, :b)
来源：http://3g.hesvh.cn/Article/details/gsixvqimm.sHtML

C#:   obj?.A?.B ?? default
来源：http://m.share.hesvh.cn/Article/details/gtuyjlzqh.sHtML

[H07] 断言
来源：http://3g.fehbvm.com/Article/details/gxjqncptx.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.m.share.zdbjq.cn/Article/details/gzmepnkiq.sHtML

PHP:  assert($x > 0);
来源：http://www.m.share.hesvh.cn/Article/details/gaseitbjy.sHtML

JS:   console.assert(x > 0);
来源：http://3g.fehbvm.com/Article/details/gbciukvqk.sHtML

TS:   console.assert(x > 0);
来源：http://www.blog.zdbjq.cn/Article/details/gcslevplr.sHtML

Java: assert x > 0 : "必须为正";
来源：http://read.share.hesvh.cn/Article/details/gmbxmhhkv.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://3g.hesvh.cn/Article/details/gushvpmkh.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://blog.hesvh.cn/Article/details/gsnkgytor.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.blog.fehbvm.com/Article/details/gueovlqax.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.m.share.fehbvm.com/Article/details/glutdczmm.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.blog.zdbjq.cn/Article/details/gxwrdtcul.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mobile.zdbjq.cn/Article/details/gxzvlvfrz.sHtML

JS:   e.message;  e.stack
来源：http://blog.zdbjq.cn/Article/details/gexgznskb.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://blog.fehbvm.com/Article/details/gpxxvelav.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.blog.fehbvm.com/Article/details/ghonzaobg.sHtML

Go:   err.Error()
来源：http://mobile.fehbvm.com/Article/details/gdcyastaz.sHtML

Ruby: e.message;  e.backtrace
来源：http://mobile.fehbvm.com/Article/details/gnihxigku.sHtML

C#:   e.Message;  e.StackTrace
来源：http://m.share.fehbvm.com/Article/details/gqqegmhkv.sHtML

[H09] 带错误码的异常
来源：http://blog.zdbjq.cn/Article/details/gfaklbycd.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://blog.hesvh.cn/Article/details/gpmkalxeg.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://3g.fehbvm.com/Article/details/godqdeajt.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://read.share.hesvh.cn/Article/details/gnfxeojsu.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mobile.hesvh.cn/Article/details/gjnszjhri.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mobile.zdbjq.cn/Article/details/gmclsujxf.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.m.share.fehbvm.com/Article/details/gpmnfqorz.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://baike.hesvh.cn/Article/details/glyiqkndb.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.blog.zdbjq.cn/Article/details/gemhsrqzm.sHtML

[H10] 资源自动释放
来源：http://www.share.hesvh.cn/Article/details/gpodlgkut.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://m.share.fehbvm.com/Article/details/gbopgpzsr.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://read.share.zdbjq.cn/Article/details/guifrjngv.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.fehbvm.com/Article/details/gzqqfzmpg.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.zdbjq.cn/Article/details/gytrvbmbq.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.share.fehbvm.com/Article/details/gboytoysf.sHtML

Go:   defer f.Close()
来源：http://3g.zdbjq.cn/Article/details/gxsywcjcu.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wap.zdbjq.cn/Article/details/gsbgydosm.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://baike.hesvh.cn/Article/details/gluamqsdp.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gnhfzvgtt.sHtML

I. 正则表达式
来源：http://www.blog.fehbvm.com/Article/details/gukazntso.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/ghinzbwfc.sHtML

[I01] 判断是否匹配
来源：http://mobile.hesvh.cn/Article/details/gowviwyfv.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.m.share.hesvh.cn/Article/details/gxebygdbk.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.share.hesvh.cn/Article/details/gcvhgcwec.sHtML

JS:   /\d+/.test(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gkfbsgjqi.sHtML

TS:   /\d+/.test(s)
来源：http://mobile.hesvh.cn/Article/details/gwsvtmzyc.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.share.zdbjq.cn/Article/details/gmklfvece.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.blog.zdbjq.cn/Article/details/gyxytdrvl.sHtML

Ruby: s.match?(/\d+/)
来源：http://wap.zdbjq.cn/Article/details/gfxgogwof.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://baike.hesvh.cn/Article/details/gmpekhptv.sHtML

[I02] 提取所有匹配
来源：http://read.share.zdbjq.cn/Article/details/gtrrdnihg.sHtML

Py:   re.findall(r"\d+", s)
来源：http://baike.fehbvm.com/Article/details/gxpsqozoh.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wap.zdbjq.cn/Article/details/gsljgwipa.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.blog.fehbvm.com/Article/details/gyuzqmnzs.sHtML

TS:   s.match(/\d+/g)
来源：http://baike.fehbvm.com/Article/details/gdxgkcgav.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://m.share.fehbvm.com/Article/details/gcfsmamhl.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://3g.zdbjq.cn/Article/details/gypevcpoy.sHtML

Ruby: s.scan(/\d+/)
来源：http://blog.zdbjq.cn/Article/details/gwantqbtv.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://3g.fehbvm.com/Article/details/gtyieowgh.sHtML

[I03] 提取捕获分组
来源：http://m.share.fehbvm.com/Article/details/gpcptqaci.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://blog.zdbjq.cn/Article/details/guqfuklzk.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://3g.hesvh.cn/Article/details/gjdqfoiwn.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.share.hesvh.cn/Article/details/guiymyeoh.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mobile.hesvh.cn/Article/details/gtbpcwupv.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://baike.hesvh.cn/Article/details/gdaqifyfl.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wap.zdbjq.cn/Article/details/gdfookvcq.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://m.share.hesvh.cn/Article/details/gpfahnyav.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://baike.fehbvm.com/Article/details/gnufabrdm.sHtML

[I04] 正则替换
来源：http://m.share.hesvh.cn/Article/details/gxftadtha.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://blog.fehbvm.com/Article/details/gwuepljbs.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mobile.hesvh.cn/Article/details/gdfplrhoi.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.share.zdbjq.cn/Article/details/gtpibujcq.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://baike.hesvh.cn/Article/details/gzbcjjjqt.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://m.share.fehbvm.com/Article/details/gddfwnwmp.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://wap.hesvh.cn/Article/details/ggkplfdey.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.m.share.hesvh.cn/Article/details/grxmcnhch.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://blog.zdbjq.cn/Article/details/glypaivay.sHtML

[I05] 按正则拆分
来源：http://www.blog.zdbjq.cn/Article/details/gcolxbubi.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://blog.fehbvm.com/Article/details/gbiexdygn.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.share.zdbjq.cn/Article/details/gqwhzzpwy.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.share.fehbvm.com/Article/details/gfnmxidpe.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://3g.fehbvm.com/Article/details/gbpstccph.sHtML

Java: s.split("\\s*,\\s*")
来源：http://wap.fehbvm.com/Article/details/gplbntmul.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.share.fehbvm.com/Article/details/guticnsgw.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://m.share.hesvh.cn/Article/details/gmfyaafyr.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.m.share.hesvh.cn/Article/details/gcczjsigj.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mobile.zdbjq.cn/Article/details/gupygjcyr.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wap.hesvh.cn/Article/details/glmjijjmi.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://mobile.hesvh.cn/Article/details/ggpkjeitn.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.hesvh.cn/Article/details/geijuncpd.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.fehbvm.com/Article/details/gxmtkjujf.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.m.share.fehbvm.com/Article/details/gtwordwlv.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://mobile.hesvh.cn/Article/details/gvmdapyks.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.share.fehbvm.com/Article/details/gtnpevsua.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.blog.fehbvm.com/Article/details/gykxlogzk.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.share.zdbjq.cn/Article/details/gnftcotxj.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.blog.fehbvm.com/Article/details/gmofpviua.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://read.share.fehbvm.com/Article/details/grlzgsbsf.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://3g.hesvh.cn/Article/details/glstwipve.sHtML

TS:   /error/gim
来源：http://www.blog.zdbjq.cn/Article/details/gltxnietq.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://blog.hesvh.cn/Article/details/gafgynlle.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://3g.fehbvm.com/Article/details/ggcivclol.sHtML

Ruby: s.scan(/error/i)
来源：http://m.share.zdbjq.cn/Article/details/gqjipfmoa.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.blog.zdbjq.cn/Article/details/gisucowpg.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.blog.zdbjq.cn/Article/details/guuileuqs.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.blog.fehbvm.com/Article/details/goybuyzjr.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wap.hesvh.cn/Article/details/gkrpezlff.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.hesvh.cn/Article/details/gkyygfubs.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.zdbjq.cn/Article/details/gzjtzgzcc.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.m.share.hesvh.cn/Article/details/gzgdzrxai.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://baike.zdbjq.cn/Article/details/gdatojtqn.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mobile.hesvh.cn/Article/details/getxikora.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://baike.zdbjq.cn/Article/details/gkkoazfyy.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gtvzghjsy.sHtML

J. 日期与时间
来源：http://wap.fehbvm.com/Article/details/gmfayspjo.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gvdzuafpj.sHtML

[J01] 获取当前时间
来源：http://3g.hesvh.cn/Article/details/gpcdodfzb.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://read.share.fehbvm.com/Article/details/glgjxuopt.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://read.share.fehbvm.com/Article/details/grcgnmgbp.sHtML

JS:   new Date();  Date.now()
来源：http://read.share.zdbjq.cn/Article/details/gahsiimvp.sHtML

TS:   new Date();  Date.now()
来源：http://read.share.zdbjq.cn/Article/details/goadwgnjm.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://wap.fehbvm.com/Article/details/girissvik.sHtML

Go:   time.Now()
来源：http://read.share.hesvh.cn/Article/details/gceqhcghl.sHtML

Ruby: Time.now
来源：http://m.share.fehbvm.com/Article/details/gulgzsina.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://read.share.zdbjq.cn/Article/details/gvygwayqk.sHtML

[J02] 格式化输出
来源：http://wap.hesvh.cn/Article/details/gruoxuncx.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.zdbjq.cn/Article/details/gktbznzuu.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.blog.fehbvm.com/Article/details/gxhcpfvgh.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://m.share.hesvh.cn/Article/details/glfbxqzhp.sHtML

TS:   d.toISOString()
来源：http://m.share.zdbjq.cn/Article/details/gzkjlimyl.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.m.share.zdbjq.cn/Article/details/gegmtzscw.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://m.share.fehbvm.com/Article/details/gvtffwwgj.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.hesvh.cn/Article/details/gcymbzlni.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://3g.fehbvm.com/Article/details/gpayvpiwa.sHtML

[J03] 字符串解析为日期
来源：http://m.share.hesvh.cn/Article/details/giafhkikv.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.blog.zdbjq.cn/Article/details/gjmjnxhqh.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://m.share.hesvh.cn/Article/details/ghsalkweg.sHtML

JS:   new Date("2024-01-02")
来源：http://3g.hesvh.cn/Article/details/gkfrzruyk.sHtML

TS:   new Date("2024-01-02")
来源：http://m.share.zdbjq.cn/Article/details/gohnyfxyh.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://mobile.fehbvm.com/Article/details/gtpotocyu.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.blog.fehbvm.com/Article/details/ghhkyigyw.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://m.share.hesvh.cn/Article/details/ggasgmnfb.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://read.share.zdbjq.cn/Article/details/gatmkydts.sHtML

[J04] 时间戳与日期互转
来源：http://www.share.zdbjq.cn/Article/details/gfofdhhmr.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.share.fehbvm.com/Article/details/gckuwkerw.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.m.share.hesvh.cn/Article/details/ghbcrepar.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://baike.zdbjq.cn/Article/details/gccepjlnc.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://m.share.fehbvm.com/Article/details/gqhjpenxa.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.share.hesvh.cn/Article/details/gaxmovxjc.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://mobile.zdbjq.cn/Article/details/gsohrraqz.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.blog.fehbvm.com/Article/details/gumqroknf.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.blog.hesvh.cn/Article/details/gqihcezog.sHtML

[J05] 时间加减（加 7 天）
来源：http://blog.zdbjq.cn/Article/details/gsiteaglb.sHtML

Py:   now + timedelta(days=7)
来源：http://wap.zdbjq.cn/Article/details/gqjbzamoh.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://blog.hesvh.cn/Article/details/gzpstppjt.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.hesvh.cn/Article/details/gdfemenwe.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.fehbvm.com/Article/details/gjwnesiwq.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.share.zdbjq.cn/Article/details/gjivogypk.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.blog.zdbjq.cn/Article/details/gebfxqlyk.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.m.share.zdbjq.cn/Article/details/gtgdbafvr.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://wap.fehbvm.com/Article/details/gljbnvqli.sHtML

[J06] 计算两时间之差
来源：http://3g.fehbvm.com/Article/details/gezoszyed.sHtML

Py:   (end - start).total_seconds()
来源：http://baike.hesvh.cn/Article/details/gpfzamqzb.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.blog.zdbjq.cn/Article/details/gbzciubii.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://baike.hesvh.cn/Article/details/gadkrofrg.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://blog.zdbjq.cn/Article/details/gkdrwqsej.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.blog.hesvh.cn/Article/details/gbqyepuku.sHtML

Go:   end.Sub(start).Hours()
来源：http://mobile.fehbvm.com/Article/details/gbiqixwtk.sHtML

Ruby: end - start                 # 返回秒数
来源：http://read.share.zdbjq.cn/Article/details/gdbhjcnnw.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.blog.fehbvm.com/Article/details/gyempgpil.sHtML

[J07] 比较两个日期
来源：http://www.share.hesvh.cn/Article/details/ggwoljwio.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://read.share.zdbjq.cn/Article/details/gsqhdquxr.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.share.fehbvm.com/Article/details/gfirdvblu.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://baike.zdbjq.cn/Article/details/gxvdoiize.sHtML


<!-- 参考信息 -->