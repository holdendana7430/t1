代发 wailian999

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnqpbktuv.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzhuewtsr.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gedjjytgw.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.fanxiaobao.xyz/Article/details/gzbmkzcqa.sHtML

Java: interface Shape { double area(); }
来源：http://wap.fanxiaobao.xyz/Article/details/glzndefsa.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.fanxiaobao.xyz/Article/details/gigpiqwib.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.fanxiaobao.xyz/Article/details/gdipjeswq.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gmcysocgp.sHtML

[G10] 访问控制
来源：http://3g.fanxiaobao.xyz/Article/details/gsniygufu.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goesemktb.sHtML

PHP:  public / protected / private
来源：http://mobile.fanxiaobao.xyz/Article/details/gkpiuusku.sHtML

JS:   #private 字段；其余公开
来源：http://blog.fanxiaobao.xyz/Article/details/gxlzfvmer.sHtML

TS:   public / protected / private
来源：http://www.share.fanxiaobao.xyz/Article/details/gzptrhkas.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.fanxiaobao.xyz/Article/details/gicznclhg.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.fanxiaobao.xyz/Article/details/giwdcficc.sHtML

Ruby: public / protected / private
来源：http://baike.fanxiaobao.xyz/Article/details/grgtbxaie.sHtML

C#:   public / protected / private / internal
来源：http://m.share.fanxiaobao.xyz/Article/details/gadcdbqpz.sHtML

[G11] getter / setter
来源：http://baike.fanxiaobao.xyz/Article/details/gpuwiival.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.fanxiaobao.xyz/Article/details/gctujingi.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzeapbuwq.sHtML

JS:   get name() { return this._name; }
来源：http://3g.fanxiaobao.xyz/Article/details/gecjvfbjy.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gxcodkkki.sHtML

Java: public String getName() { return name; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gnyubkxtt.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.fanxiaobao.xyz/Article/details/gklvxqvow.sHtML

Ruby: attr_accessor :name
来源：http://baike.fanxiaobao.xyz/Article/details/glecozcji.sHtML

C#:   public string Name { get; set; }
来源：http://baike.fanxiaobao.xyz/Article/details/gviwjxfhh.sHtML

[G12] 对象转字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gweniaztp.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcikkxdmc.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.fanxiaobao.xyz/Article/details/gfcxvoikt.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwwvibtts.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.fanxiaobao.xyz/Article/details/gltzeopoj.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.fanxiaobao.xyz/Article/details/ghgqksdto.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.fanxiaobao.xyz/Article/details/gksjiscmr.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxkhowudc.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.fanxiaobao.xyz/Article/details/gryqvbdjr.sHtML

[G13] 判断对象类型
来源：http://baike.fanxiaobao.xyz/Article/details/gmlswhcbt.sHtML

Py:   isinstance(u, User)
来源：http://m.share.fanxiaobao.xyz/Article/details/gpjkxcclf.sHtML

PHP:  $u instanceof User
来源：http://www.share.fanxiaobao.xyz/Article/details/gthiyyblu.sHtML

JS:   u instanceof User
来源：http://www.blog.fanxiaobao.xyz/Article/details/gttrrnlqc.sHtML

TS:   u instanceof User
来源：http://m.share.fanxiaobao.xyz/Article/details/gwmmglgqh.sHtML

Java: u instanceof User
来源：http://3g.fanxiaobao.xyz/Article/details/gxjkssaaw.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.fanxiaobao.xyz/Article/details/gkultpqpo.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbxoiooyq.sHtML

C#:   u is User
来源：http://baike.fanxiaobao.xyz/Article/details/gpmzybtbq.sHtML

[G14] 数据类 / record
来源：http://wap.fanxiaobao.xyz/Article/details/gyzjzwoke.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://3g.fanxiaobao.xyz/Article/details/gnfhmizqj.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.fanxiaobao.xyz/Article/details/gbvmkgads.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.fanxiaobao.xyz/Article/details/gnwzexsqh.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.fanxiaobao.xyz/Article/details/gxjetnrps.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpqpzybsi.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.fanxiaobao.xyz/Article/details/gzdlibiyy.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.fanxiaobao.xyz/Article/details/gubyehgpj.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwiebkzie.sHtML

[G15] 枚举
来源：http://m.share.fanxiaobao.xyz/Article/details/giwuixify.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.fanxiaobao.xyz/Article/details/gfbmkkrem.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsvcjshvj.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mobile.fanxiaobao.xyz/Article/details/gwfgdclfl.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gkzeheezo.sHtML

Java: enum Color { RED, GREEN }
来源：http://m.share.fanxiaobao.xyz/Article/details/gapvsnhlv.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.fanxiaobao.xyz/Article/details/gvgstssez.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqgowinyx.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.fanxiaobao.xyz/Article/details/gyctquyvh.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.fanxiaobao.xyz/Article/details/gthwmfeyn.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.fanxiaobao.xyz/Article/details/gubtugawy.sHtML

PHP:  get_object_vars($obj);
来源：http://wap.fanxiaobao.xyz/Article/details/gjovuyypi.sHtML

JS:   Object.entries(obj)
来源：http://wap.fanxiaobao.xyz/Article/details/gxyjfnudf.sHtML

TS:   Object.entries(obj)
来源：http://blog.fanxiaobao.xyz/Article/details/gucepvfnc.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grkvgddcz.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.fanxiaobao.xyz/Article/details/glmvinddd.sHtML

Ruby: obj.instance_variables
来源：http://baike.fanxiaobao.xyz/Article/details/gnxuzugca.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.fanxiaobao.xyz/Article/details/gzpzsmwqa.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gjffcockw.sHtML

H. 异常与错误处理
来源：http://mobile.fanxiaobao.xyz/Article/details/gjutptnfl.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnnnvzira.sHtML

[H01] try / catch 基础
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyvlljrjg.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.fanxiaobao.xyz/Article/details/gnsqsctuq.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.fanxiaobao.xyz/Article/details/gizcxyqtx.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.fanxiaobao.xyz/Article/details/givamilpu.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gxrcmhcnm.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvwfohhjx.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.blog.fanxiaobao.xyz/Article/details/gchnqmxmi.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wap.fanxiaobao.xyz/Article/details/gtccrllmo.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gflefmaeh.sHtML

[H02] finally / ensure 收尾
来源：http://wap.fanxiaobao.xyz/Article/details/gxjjkkrcp.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.share.fanxiaobao.xyz/Article/details/gvnokhrfx.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://baike.fanxiaobao.xyz/Article/details/gohcdpmeu.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://baike.fanxiaobao.xyz/Article/details/gxfwgofur.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://baike.fanxiaobao.xyz/Article/details/gfkbmvfbc.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gtwaqoqxw.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.fanxiaobao.xyz/Article/details/gizkphqwx.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghtkorylx.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjcsncvoy.sHtML

[H03] 主动抛出异常
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goskcouac.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.fanxiaobao.xyz/Article/details/gnxqfvxda.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blog.fanxiaobao.xyz/Article/details/gnviqxjmq.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.fanxiaobao.xyz/Article/details/gekujtikk.sHtML

TS:   throw new Error("错误信息");
来源：http://wap.fanxiaobao.xyz/Article/details/gvfjfxqbl.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://baike.fanxiaobao.xyz/Article/details/gajvqowwi.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://3g.fanxiaobao.xyz/Article/details/ghincntku.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://wap.fanxiaobao.xyz/Article/details/gwcxmkict.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://baike.fanxiaobao.xyz/Article/details/gtkmghfcs.sHtML

[H04] 自定义异常类型
来源：http://baike.fanxiaobao.xyz/Article/details/gwvjptdgc.sHtML

Py:   class MyError(Exception): pass
来源：http://3g.fanxiaobao.xyz/Article/details/ggqcuiffd.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://blog.fanxiaobao.xyz/Article/details/ghmockibh.sHtML

JS:   class MyError extends Error {}
来源：http://m.share.fanxiaobao.xyz/Article/details/goiktetfn.sHtML

TS:   class MyError extends Error {}
来源：http://blog.fanxiaobao.xyz/Article/details/gzgzuafzo.sHtML

Java: class MyException extends RuntimeException {}
来源：http://wap.fanxiaobao.xyz/Article/details/ggmkndyso.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://m.share.fanxiaobao.xyz/Article/details/gflelwyjc.sHtML

Ruby: class MyError < StandardError; end
来源：http://m.share.fanxiaobao.xyz/Article/details/gkmcgknwr.sHtML

C#:   class MyException : Exception {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gsrrfeuyn.sHtML

[H05] 捕获特定类型
来源：http://blog.fanxiaobao.xyz/Article/details/gycdiogff.sHtML

Py:   except ValueError as e:
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfhnwugbt.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://m.share.fanxiaobao.xyz/Article/details/ghouozabj.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://3g.fanxiaobao.xyz/Article/details/gbxmmsmuw.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gpxzfbbfx.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gbvbngeyx.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://baike.fanxiaobao.xyz/Article/details/gjsmmvbfo.sHtML

Ruby: rescue ArgumentError => e
来源：http://wap.fanxiaobao.xyz/Article/details/goswhqjly.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gsuqmxpkt.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.fanxiaobao.xyz/Article/details/gorqyixld.sHtML

Py:   value = d.get("k") or default
来源：http://baike.fanxiaobao.xyz/Article/details/grkgibwmg.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.fanxiaobao.xyz/Article/details/gafupslbg.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geunkgipa.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://wap.fanxiaobao.xyz/Article/details/gtmmpanjw.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grxpbcjmz.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/godqxdkpt.sHtML

Ruby: d&.dig(:a, :b)
来源：http://m.share.fanxiaobao.xyz/Article/details/gmjomiyql.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.share.fanxiaobao.xyz/Article/details/gvyeawxlz.sHtML

[H07] 断言
来源：http://m.share.fanxiaobao.xyz/Article/details/grmlpytgn.sHtML

Py:   assert x > 0, "必须为正"
来源：http://read.share.fanxiaobao.xyz/Article/details/gcbmrfduy.sHtML

PHP:  assert($x > 0);
来源：http://baike.fanxiaobao.xyz/Article/details/gzsptthux.sHtML

JS:   console.assert(x > 0);
来源：http://baike.fanxiaobao.xyz/Article/details/gaiabxnby.sHtML

TS:   console.assert(x > 0);
来源：http://baike.fanxiaobao.xyz/Article/details/gnbwzqlyw.sHtML

Java: assert x > 0 : "必须为正";
来源：http://blog.fanxiaobao.xyz/Article/details/gcywkowlg.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://blog.fanxiaobao.xyz/Article/details/glunbyqqz.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.blog.fanxiaobao.xyz/Article/details/gubhqaugc.sHtML

C#:   Debug.Assert(x > 0);
来源：http://wap.fanxiaobao.xyz/Article/details/guwmiwfzk.sHtML

[H08] 获取错误信息与堆栈
来源：http://wap.fanxiaobao.xyz/Article/details/gpbiqxhqc.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://mobile.fanxiaobao.xyz/Article/details/gihyrrvfe.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.share.fanxiaobao.xyz/Article/details/gosaivtox.sHtML

JS:   e.message;  e.stack
来源：http://mobile.fanxiaobao.xyz/Article/details/gunugbrvx.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://baike.fanxiaobao.xyz/Article/details/gsaxrsprd.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://wap.fanxiaobao.xyz/Article/details/gkgsugkye.sHtML

Go:   err.Error()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyozrkthp.sHtML

Ruby: e.message;  e.backtrace
来源：http://3g.fanxiaobao.xyz/Article/details/gvyeadzaq.sHtML

C#:   e.Message;  e.StackTrace
来源：http://3g.fanxiaobao.xyz/Article/details/gxfztkrqv.sHtML

[H09] 带错误码的异常
来源：http://baike.fanxiaobao.xyz/Article/details/gmtlnpbyy.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://3g.fanxiaobao.xyz/Article/details/gjbhcyobd.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://wap.fanxiaobao.xyz/Article/details/gqtzxdzfv.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkgzhsyxc.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gybtqjlcv.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://m.share.fanxiaobao.xyz/Article/details/ggldzbsor.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://blog.fanxiaobao.xyz/Article/details/guthkdwjt.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://read.share.fanxiaobao.xyz/Article/details/grmmcfsod.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://blog.fanxiaobao.xyz/Article/details/gsbgqpyic.sHtML

[H10] 资源自动释放
来源：http://3g.fanxiaobao.xyz/Article/details/glprehfpc.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://wap.fanxiaobao.xyz/Article/details/ggsvwdmyh.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://m.share.fanxiaobao.xyz/Article/details/gzyxeiszf.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyfywxzfg.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.fanxiaobao.xyz/Article/details/gwyqsisex.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://m.share.fanxiaobao.xyz/Article/details/gqqbcmvwr.sHtML

Go:   defer f.Close()
来源：http://www.share.fanxiaobao.xyz/Article/details/gjhfhvhxa.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.share.fanxiaobao.xyz/Article/details/goatzwgby.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wap.fanxiaobao.xyz/Article/details/gkejwrvjk.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gicaktqlq.sHtML

I. 正则表达式
来源：http://baike.fanxiaobao.xyz/Article/details/gkenybtts.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gvfsaewew.sHtML

[I01] 判断是否匹配
来源：http://mobile.fanxiaobao.xyz/Article/details/gdfemogvq.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gepcshlew.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnvyeijje.sHtML

JS:   /\d+/.test(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gqfmwivuh.sHtML

TS:   /\d+/.test(s)
来源：http://3g.fanxiaobao.xyz/Article/details/gjaxuyeap.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://blog.fanxiaobao.xyz/Article/details/gzgdzgwsx.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gvvqrfcdo.sHtML

Ruby: s.match?(/\d+/)
来源：http://wap.fanxiaobao.xyz/Article/details/gezakcsgi.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://baike.fanxiaobao.xyz/Article/details/gvgimrfmy.sHtML

[I02] 提取所有匹配
来源：http://m.share.fanxiaobao.xyz/Article/details/gtujyiamg.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gokafmioz.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.share.fanxiaobao.xyz/Article/details/gmvgmflje.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://read.share.fanxiaobao.xyz/Article/details/gtifdvxpz.sHtML

TS:   s.match(/\d+/g)
来源：http://read.share.fanxiaobao.xyz/Article/details/gqgejhxnt.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://read.share.fanxiaobao.xyz/Article/details/gbqlmxegp.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gnonqmjbz.sHtML

Ruby: s.scan(/\d+/)
来源：http://3g.fanxiaobao.xyz/Article/details/gftohhbic.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://baike.fanxiaobao.xyz/Article/details/gposejpqi.sHtML

[I03] 提取捕获分组
来源：http://www.blog.fanxiaobao.xyz/Article/details/grxpjpiwa.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzsxbryqi.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://blog.fanxiaobao.xyz/Article/details/gpsehydyl.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://m.share.fanxiaobao.xyz/Article/details/gclutvlas.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://m.share.fanxiaobao.xyz/Article/details/ggqykwcgz.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://blog.fanxiaobao.xyz/Article/details/gtstihrcz.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://read.share.fanxiaobao.xyz/Article/details/gissbkmgm.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://m.share.fanxiaobao.xyz/Article/details/gjiaikkbr.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://read.share.fanxiaobao.xyz/Article/details/gqyurdmdp.sHtML

[I04] 正则替换
来源：http://m.share.fanxiaobao.xyz/Article/details/giklronje.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://wap.fanxiaobao.xyz/Article/details/gktuwmhox.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://baike.fanxiaobao.xyz/Article/details/gvcchkmwv.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://m.share.fanxiaobao.xyz/Article/details/gdhtrwubb.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://mobile.fanxiaobao.xyz/Article/details/grrfgkwew.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzsklmozc.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.share.fanxiaobao.xyz/Article/details/gzkyaovje.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqfbfnvuf.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://blog.fanxiaobao.xyz/Article/details/gyicvyezo.sHtML

[I05] 按正则拆分
来源：http://baike.fanxiaobao.xyz/Article/details/gsifhxqtk.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://blog.fanxiaobao.xyz/Article/details/gaysnuypx.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://baike.fanxiaobao.xyz/Article/details/gajtbyoef.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://blog.fanxiaobao.xyz/Article/details/grhynbovs.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaklqccfj.sHtML

Java: s.split("\\s*,\\s*")
来源：http://read.share.fanxiaobao.xyz/Article/details/gtpxugejg.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gubwaidni.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://wap.fanxiaobao.xyz/Article/details/gqdbkdqsm.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wap.fanxiaobao.xyz/Article/details/gsqnuwoex.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.share.fanxiaobao.xyz/Article/details/gtrqeeslr.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://mobile.fanxiaobao.xyz/Article/details/gwgaumdbz.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfgqkufnt.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.fanxiaobao.xyz/Article/details/gpozytvab.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.fanxiaobao.xyz/Article/details/guqxtsckk.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://blog.fanxiaobao.xyz/Article/details/gqtsenloe.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.share.fanxiaobao.xyz/Article/details/guinkjgky.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://m.share.fanxiaobao.xyz/Article/details/gwvbueifl.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mobile.fanxiaobao.xyz/Article/details/gmonkoxqd.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.share.fanxiaobao.xyz/Article/details/gtwpgqumv.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://blog.fanxiaobao.xyz/Article/details/gmrurwkjc.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://read.share.fanxiaobao.xyz/Article/details/gvadyzgnf.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwaukfawc.sHtML

TS:   /error/gim
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpfyumtsx.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.share.fanxiaobao.xyz/Article/details/gnbvofiok.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://baike.fanxiaobao.xyz/Article/details/gropglzdq.sHtML

Ruby: s.scan(/error/i)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmgldvgzj.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://read.share.fanxiaobao.xyz/Article/details/gtknciwzl.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://mobile.fanxiaobao.xyz/Article/details/gehfqaqaf.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://blog.fanxiaobao.xyz/Article/details/glhpoijmh.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggszqwkos.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcaklnspy.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.fanxiaobao.xyz/Article/details/gwhfjxzdn.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.share.fanxiaobao.xyz/Article/details/gxbwfqzmx.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://m.share.fanxiaobao.xyz/Article/details/glwgqbpxx.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wap.fanxiaobao.xyz/Article/details/gdewkciwr.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mobile.fanxiaobao.xyz/Article/details/gmjvvpevh.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gumbvjkpp.sHtML

J. 日期与时间
来源：http://mobile.fanxiaobao.xyz/Article/details/garyoryfz.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gbzdjfvto.sHtML

[J01] 获取当前时间
来源：http://www.share.fanxiaobao.xyz/Article/details/gjlmtuvky.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://wap.fanxiaobao.xyz/Article/details/gqbibcdju.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://baike.fanxiaobao.xyz/Article/details/glzzgypzf.sHtML

JS:   new Date();  Date.now()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gptivxhld.sHtML

TS:   new Date();  Date.now()
来源：http://baike.fanxiaobao.xyz/Article/details/gibdcteda.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://wap.fanxiaobao.xyz/Article/details/gfnrfqtsy.sHtML

Go:   time.Now()
来源：http://read.share.fanxiaobao.xyz/Article/details/gbzfsuiic.sHtML

Ruby: Time.now
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvgwfhflo.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://mobile.fanxiaobao.xyz/Article/details/gzdqogtux.sHtML

[J02] 格式化输出
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfhnugezo.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpjcfldxp.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://m.share.fanxiaobao.xyz/Article/details/gutwtymot.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wap.fanxiaobao.xyz/Article/details/gzxqjytoa.sHtML

TS:   d.toISOString()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gedibtmvo.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://baike.fanxiaobao.xyz/Article/details/gafsnhrnv.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://blog.fanxiaobao.xyz/Article/details/gvxereekj.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gztlqutfb.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://m.share.fanxiaobao.xyz/Article/details/ghfanfubs.sHtML

[J03] 字符串解析为日期
来源：http://mobile.fanxiaobao.xyz/Article/details/gpidkilgp.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://mobile.fanxiaobao.xyz/Article/details/glcngccil.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://read.share.fanxiaobao.xyz/Article/details/gbgcjjlbe.sHtML

JS:   new Date("2024-01-02")
来源：http://m.share.fanxiaobao.xyz/Article/details/grudosvgj.sHtML

TS:   new Date("2024-01-02")
来源：http://www.share.fanxiaobao.xyz/Article/details/gejkacxnf.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://baike.fanxiaobao.xyz/Article/details/gxcurrhig.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.share.fanxiaobao.xyz/Article/details/ghsbpfccg.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://wap.fanxiaobao.xyz/Article/details/gtqydhtnv.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://m.share.fanxiaobao.xyz/Article/details/gswtdaypu.sHtML

[J04] 时间戳与日期互转
来源：http://blog.fanxiaobao.xyz/Article/details/gkjiblygw.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gilqffayq.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://read.share.fanxiaobao.xyz/Article/details/gsqahcjtc.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://m.share.fanxiaobao.xyz/Article/details/gbakdfgjs.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzlhxyjso.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbhutxnse.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://read.share.fanxiaobao.xyz/Article/details/gppphyyzg.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://3g.fanxiaobao.xyz/Article/details/gboakgmdf.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://read.share.fanxiaobao.xyz/Article/details/guytrpplf.sHtML

[J05] 时间加减（加 7 天）
来源：http://baike.fanxiaobao.xyz/Article/details/grnanqiql.sHtML

Py:   now + timedelta(days=7)
来源：http://www.blog.fanxiaobao.xyz/Article/details/glvzgecgy.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://baike.fanxiaobao.xyz/Article/details/glhlnkpzk.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.fanxiaobao.xyz/Article/details/gzpawypeg.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.fanxiaobao.xyz/Article/details/gbvjgnxov.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzahzonut.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mobile.fanxiaobao.xyz/Article/details/grgeerzll.sHtML

Ruby: Time.now + 7 * 86400
来源：http://blog.fanxiaobao.xyz/Article/details/goithbsnu.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://read.share.fanxiaobao.xyz/Article/details/gpjytopap.sHtML

[J06] 计算两时间之差
来源：http://m.share.fanxiaobao.xyz/Article/details/geuroxmjz.sHtML

Py:   (end - start).total_seconds()
来源：http://read.share.fanxiaobao.xyz/Article/details/gedwcvywl.sHtML

PHP:  $end->diff($start)->days;
来源：http://read.share.fanxiaobao.xyz/Article/details/gmyrfbczb.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdfgkxpiu.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://3g.fanxiaobao.xyz/Article/details/gwttrqvku.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://read.share.fanxiaobao.xyz/Article/details/grinknxvb.sHtML

Go:   end.Sub(start).Hours()
来源：http://baike.fanxiaobao.xyz/Article/details/gxnrksvwx.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.share.fanxiaobao.xyz/Article/details/gajcprtzn.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.blog.fanxiaobao.xyz/Article/details/gubhormre.sHtML

[J07] 比较两个日期
来源：http://3g.fanxiaobao.xyz/Article/details/gcjkfazlm.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://blog.fanxiaobao.xyz/Article/details/giddhdqho.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://blog.fanxiaobao.xyz/Article/details/gilrppikt.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://blog.fanxiaobao.xyz/Article/details/giolzyhqm.sHtML


<!-- 参考信息 -->