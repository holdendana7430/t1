代发 wailian999

TS:   greet(): string { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/grqqzcrbm.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.hesvh.cn/Article/details/glzivswwu.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.hesvh.cn/Article/details/gqpfpnohw.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.hesvh.cn/Article/details/gbvitwuaa.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.hesvh.cn/Article/details/ggjokisvy.sHtML

[G07] 调用父类方法
来源：http://www.share.fehbvm.com/Article/details/gzawnacsn.sHtML

Py:   super().greet()
来源：http://baike.fehbvm.com/Article/details/gnmmpospl.sHtML

PHP:  parent::greet();
来源：http://www.share.hesvh.cn/Article/details/gknssjpjs.sHtML

JS:   super.greet();
来源：http://www.share.fehbvm.com/Article/details/gkguiivkv.sHtML

TS:   super.greet();
来源：http://mobile.zdbjq.cn/Article/details/gbsfmtaix.sHtML

Java: super.greet();
来源：http://www.blog.zdbjq.cn/Article/details/gwyjpqeei.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.fehbvm.com/Article/details/gyqnkmxxu.sHtML

Ruby: super
来源：http://baike.zdbjq.cn/Article/details/gukgblisp.sHtML

C#:   base.Greet();
来源：http://www.m.share.hesvh.cn/Article/details/gadizwgrp.sHtML

[G08] 静态方法与属性
来源：http://wap.zdbjq.cn/Article/details/ggmsewrmu.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.hesvh.cn/Article/details/gmxvebksp.sHtML

PHP:  public static function f() {}
来源：http://www.share.zdbjq.cn/Article/details/gdemcodmw.sHtML

JS:   static f() {}
来源：http://read.share.hesvh.cn/Article/details/gfvcxnghb.sHtML

TS:   static f(): void {}
来源：http://mobile.fehbvm.com/Article/details/ggtkbvaxh.sHtML

Java: static void f() {}
来源：http://m.share.fehbvm.com/Article/details/gfntxdyqx.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.fehbvm.com/Article/details/gaadpftek.sHtML

Ruby: def self.f; end
来源：http://mobile.zdbjq.cn/Article/details/gfcznkbsy.sHtML

C#:   public static void F() {}
来源：http://blog.hesvh.cn/Article/details/gdqouarhl.sHtML

[G09] 接口 / 抽象类
来源：http://blog.hesvh.cn/Article/details/gocljlgmv.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.hesvh.cn/Article/details/gnbdhekup.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.hesvh.cn/Article/details/gjkdmiqgy.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.hesvh.cn/Article/details/gcfxdjeri.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.hesvh.cn/Article/details/gcsvkwpzp.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.hesvh.cn/Article/details/gijjrzzrt.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.fehbvm.com/Article/details/gbbjpoilw.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.hesvh.cn/Article/details/gblomnpae.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.hesvh.cn/Article/details/gllbhyvcd.sHtML

[G10] 访问控制
来源：http://3g.zdbjq.cn/Article/details/ggraceiae.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.hesvh.cn/Article/details/gtfauoquu.sHtML

PHP:  public / protected / private
来源：http://blog.fehbvm.com/Article/details/gqbomgzed.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.zdbjq.cn/Article/details/gavfqrrhb.sHtML

TS:   public / protected / private
来源：http://www.m.share.hesvh.cn/Article/details/gcxndajvw.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.fehbvm.com/Article/details/gaumdojel.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.fehbvm.com/Article/details/giapyhcrm.sHtML

Ruby: public / protected / private
来源：http://www.blog.fehbvm.com/Article/details/grdjafvyc.sHtML

C#:   public / protected / private / internal
来源：http://m.share.hesvh.cn/Article/details/gvogmedms.sHtML

[G11] getter / setter
来源：http://www.blog.hesvh.cn/Article/details/gnzyxzrqf.sHtML

Py:   @property 与 @x.setter
来源：http://blog.zdbjq.cn/Article/details/ggyqvqmtk.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.zdbjq.cn/Article/details/gckhjpgni.sHtML

JS:   get name() { return this._name; }
来源：http://3g.fehbvm.com/Article/details/gsenzgutp.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.zdbjq.cn/Article/details/gbjqjazlt.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gxnzxcvnz.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.zdbjq.cn/Article/details/gdszfcnmo.sHtML

Ruby: attr_accessor :name
来源：http://baike.fehbvm.com/Article/details/gwkhttvhn.sHtML

C#:   public string Name { get; set; }
来源：http://baike.zdbjq.cn/Article/details/gnermwoos.sHtML

[G12] 对象转字符串
来源：http://mobile.hesvh.cn/Article/details/grdzdlmul.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.fehbvm.com/Article/details/gyeewgtnt.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.hesvh.cn/Article/details/gfndkvnye.sHtML

JS:   toString() { return this.name; }
来源：http://blog.fehbvm.com/Article/details/gfswqvwmp.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/gqewhskgk.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.hesvh.cn/Article/details/gsnjuzqcg.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.zdbjq.cn/Article/details/gfprfkpqt.sHtML

Ruby: def to_s; @name; end
来源：http://blog.zdbjq.cn/Article/details/ggaxecohl.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.hesvh.cn/Article/details/gkhodujhj.sHtML

[G13] 判断对象类型
来源：http://blog.hesvh.cn/Article/details/gawkgtdky.sHtML

Py:   isinstance(u, User)
来源：http://m.share.fehbvm.com/Article/details/gfmmhrapz.sHtML

PHP:  $u instanceof User
来源：http://www.share.fehbvm.com/Article/details/gnjglqell.sHtML

JS:   u instanceof User
来源：http://baike.zdbjq.cn/Article/details/gjhqtpazb.sHtML

TS:   u instanceof User
来源：http://baike.hesvh.cn/Article/details/gljndgtml.sHtML

Java: u instanceof User
来源：http://baike.fehbvm.com/Article/details/gdczgklde.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.hesvh.cn/Article/details/grcgutjep.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.zdbjq.cn/Article/details/gmxrxnhov.sHtML

C#:   u is User
来源：http://3g.fehbvm.com/Article/details/gykerohyf.sHtML

[G14] 数据类 / record
来源：http://blog.fehbvm.com/Article/details/gvdmfkmhf.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://baike.fehbvm.com/Article/details/gtmdgpkqh.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.fehbvm.com/Article/details/gscagpjdf.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.fehbvm.com/Article/details/gzjtijrek.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.zdbjq.cn/Article/details/gjlpmlqew.sHtML

Java: record User(String name, int age) {}
来源：http://mobile.hesvh.cn/Article/details/gvnljyhwg.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.hesvh.cn/Article/details/gymrbyehl.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.zdbjq.cn/Article/details/gsddmpepr.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.hesvh.cn/Article/details/gmrrsswiy.sHtML

[G15] 枚举
来源：http://mobile.hesvh.cn/Article/details/gqzectuud.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.zdbjq.cn/Article/details/gaiycdavk.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://wap.hesvh.cn/Article/details/gdnztolyr.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.zdbjq.cn/Article/details/gkqbrdxfq.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.fehbvm.com/Article/details/guvaaidoh.sHtML

Java: enum Color { RED, GREEN }
来源：http://blog.hesvh.cn/Article/details/gcwtprfsr.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.blog.hesvh.cn/Article/details/gkovyjiyc.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.fehbvm.com/Article/details/gtdhkhsrf.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.zdbjq.cn/Article/details/gavuyxhci.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.zdbjq.cn/Article/details/gvfyjalll.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.blog.hesvh.cn/Article/details/gjtrajofh.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.hesvh.cn/Article/details/gzvvjqspk.sHtML

JS:   Object.entries(obj)
来源：http://wap.fehbvm.com/Article/details/gmwjrismj.sHtML

TS:   Object.entries(obj)
来源：http://www.share.zdbjq.cn/Article/details/gmcmrcnue.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.zdbjq.cn/Article/details/gxmjkwtgg.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.hesvh.cn/Article/details/gwufpcpxi.sHtML

Ruby: obj.instance_variables
来源：http://read.share.zdbjq.cn/Article/details/gjocrmmkt.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.zdbjq.cn/Article/details/gepoxdbzh.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gfhxmohgb.sHtML

H. 异常与错误处理
来源：http://3g.fehbvm.com/Article/details/gnfgqbpya.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gjtobygfg.sHtML

[H01] try / catch 基础
来源：http://blog.fehbvm.com/Article/details/glgkrqdfh.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.hesvh.cn/Article/details/gfxfmatvy.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.hesvh.cn/Article/details/ghdwtjkua.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.zdbjq.cn/Article/details/gxhqytyhl.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.hesvh.cn/Article/details/gcaxptreq.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.zdbjq.cn/Article/details/gpqdfajfe.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.fehbvm.com/Article/details/gyanblrcq.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://3g.fehbvm.com/Article/details/gswaxnuzx.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.fehbvm.com/Article/details/gvxlsevng.sHtML

[H02] finally / ensure 收尾
来源：http://baike.fehbvm.com/Article/details/gahresilz.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.fehbvm.com/Article/details/gnfahzqge.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.share.fehbvm.com/Article/details/gjggsmiik.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://wap.hesvh.cn/Article/details/gbldppycz.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.fehbvm.com/Article/details/gcsqrfear.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.hesvh.cn/Article/details/gukajmjlt.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.fehbvm.com/Article/details/gxpxhjnly.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://read.share.zdbjq.cn/Article/details/gqjllsdld.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://m.share.zdbjq.cn/Article/details/gksvkdcix.sHtML

[H03] 主动抛出异常
来源：http://3g.hesvh.cn/Article/details/gduxvrgks.sHtML

Py:   raise ValueError("错误信息")
来源：http://baike.fehbvm.com/Article/details/gphwzovuj.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://3g.fehbvm.com/Article/details/gemykgrpr.sHtML

JS:   throw new Error("错误信息");
来源：http://www.share.fehbvm.com/Article/details/gxgfbnvgs.sHtML

TS:   throw new Error("错误信息");
来源：http://www.m.share.zdbjq.cn/Article/details/grclyetcf.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.fehbvm.com/Article/details/grqqybrnq.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.blog.zdbjq.cn/Article/details/gwvwaxaqp.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://baike.zdbjq.cn/Article/details/gyxtgicpv.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://m.share.fehbvm.com/Article/details/gjmmwbzqs.sHtML

[H04] 自定义异常类型
来源：http://read.share.hesvh.cn/Article/details/gimfwefgb.sHtML

Py:   class MyError(Exception): pass
来源：http://m.share.zdbjq.cn/Article/details/gjuocfocy.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://mobile.fehbvm.com/Article/details/gtfdiomzz.sHtML

JS:   class MyError extends Error {}
来源：http://read.share.fehbvm.com/Article/details/gvqfxbunf.sHtML

TS:   class MyError extends Error {}
来源：http://www.share.hesvh.cn/Article/details/gnhfjaroe.sHtML

Java: class MyException extends RuntimeException {}
来源：http://mobile.fehbvm.com/Article/details/gtoieiede.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wap.zdbjq.cn/Article/details/gkeoyupsj.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.zdbjq.cn/Article/details/gppgwahto.sHtML

C#:   class MyException : Exception {}
来源：http://www.blog.fehbvm.com/Article/details/gstykcwwh.sHtML

[H05] 捕获特定类型
来源：http://www.blog.fehbvm.com/Article/details/ghdouadaa.sHtML

Py:   except ValueError as e:
来源：http://www.blog.hesvh.cn/Article/details/grwjzvzlg.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://blog.zdbjq.cn/Article/details/gtacxeqpc.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://baike.hesvh.cn/Article/details/gpscwlnqi.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.blog.zdbjq.cn/Article/details/gpfvklvca.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.zdbjq.cn/Article/details/gvdlgwlbx.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.share.fehbvm.com/Article/details/grdkuketq.sHtML

Ruby: rescue ArgumentError => e
来源：http://read.share.hesvh.cn/Article/details/gviusuiox.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gaoybvepd.sHtML

[H06] 可选值 / 空值安全访问
来源：http://wap.fehbvm.com/Article/details/gkzpsplbr.sHtML

Py:   value = d.get("k") or default
来源：http://www.blog.zdbjq.cn/Article/details/gibekcuyu.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://m.share.hesvh.cn/Article/details/gzadfctrp.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://blog.fehbvm.com/Article/details/gsuzkgvtq.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.share.fehbvm.com/Article/details/gsqrsmopf.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wap.zdbjq.cn/Article/details/gobburdyv.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://m.share.fehbvm.com/Article/details/gpaizcstr.sHtML

Ruby: d&.dig(:a, :b)
来源：http://mobile.hesvh.cn/Article/details/gdufrdpfq.sHtML

C#:   obj?.A?.B ?? default
来源：http://baike.fehbvm.com/Article/details/gvijdfyjd.sHtML

[H07] 断言
来源：http://www.share.fehbvm.com/Article/details/gbbzkuklz.sHtML

Py:   assert x > 0, "必须为正"
来源：http://read.share.fehbvm.com/Article/details/gmxrqpicm.sHtML

PHP:  assert($x > 0);
来源：http://mobile.hesvh.cn/Article/details/gggnjbbpe.sHtML

JS:   console.assert(x > 0);
来源：http://mobile.hesvh.cn/Article/details/gmziuywsh.sHtML

TS:   console.assert(x > 0);
来源：http://m.share.fehbvm.com/Article/details/gryjgcyve.sHtML

Java: assert x > 0 : "必须为正";
来源：http://m.share.hesvh.cn/Article/details/gaqmhaffc.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.m.share.fehbvm.com/Article/details/gkqyuszyz.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.blog.fehbvm.com/Article/details/gygfhlgcl.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.blog.hesvh.cn/Article/details/giwbmzvhk.sHtML

[H08] 获取错误信息与堆栈
来源：http://blog.hesvh.cn/Article/details/gbmtzcciz.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://m.share.zdbjq.cn/Article/details/gckmmddpe.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.m.share.fehbvm.com/Article/details/gooyuxuoj.sHtML

JS:   e.message;  e.stack
来源：http://mobile.zdbjq.cn/Article/details/gkbwxdkjd.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://baike.fehbvm.com/Article/details/gewoacwzp.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.share.zdbjq.cn/Article/details/glhkgkrmp.sHtML

Go:   err.Error()
来源：http://mobile.fehbvm.com/Article/details/gzinwzvwp.sHtML

Ruby: e.message;  e.backtrace
来源：http://blog.fehbvm.com/Article/details/gzlhhneeo.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.blog.fehbvm.com/Article/details/gwxkwngot.sHtML

[H09] 带错误码的异常
来源：http://www.m.share.zdbjq.cn/Article/details/giqqumxfv.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.m.share.hesvh.cn/Article/details/gcieenthb.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://read.share.zdbjq.cn/Article/details/gpkbcljjk.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://blog.zdbjq.cn/Article/details/ggqespzxv.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://read.share.fehbvm.com/Article/details/gensmisvx.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://m.share.fehbvm.com/Article/details/ganqlzsxq.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://m.share.zdbjq.cn/Article/details/gbatzookn.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://mobile.zdbjq.cn/Article/details/gvsxlecsq.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://wap.fehbvm.com/Article/details/ggdxhwqln.sHtML

[H10] 资源自动释放
来源：http://baike.hesvh.cn/Article/details/gdhdfrvog.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://mobile.hesvh.cn/Article/details/gmskdufsc.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.share.zdbjq.cn/Article/details/glukcrfwa.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.zdbjq.cn/Article/details/gqlavrgyw.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.zdbjq.cn/Article/details/gqjyaqtyo.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://read.share.fehbvm.com/Article/details/gimaoatkx.sHtML

Go:   defer f.Close()
来源：http://read.share.zdbjq.cn/Article/details/goysezpcc.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://baike.fehbvm.com/Article/details/gmzzdjifr.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://baike.hesvh.cn/Article/details/ghoxfphle.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gntchkxhb.sHtML

I. 正则表达式
来源：http://blog.hesvh.cn/Article/details/gmbuyidzl.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gyihatrjv.sHtML

[I01] 判断是否匹配
来源：http://www.m.share.zdbjq.cn/Article/details/glkfsbuwj.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mobile.hesvh.cn/Article/details/giidxesre.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://mobile.hesvh.cn/Article/details/gqlzqhadx.sHtML

JS:   /\d+/.test(s)
来源：http://3g.hesvh.cn/Article/details/gumfstzvj.sHtML

TS:   /\d+/.test(s)
来源：http://www.m.share.fehbvm.com/Article/details/gmgertrbr.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.share.hesvh.cn/Article/details/gqohcebew.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://read.share.hesvh.cn/Article/details/gplwwmeoa.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.m.share.fehbvm.com/Article/details/gxxbndnwb.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://blog.fehbvm.com/Article/details/gpocxbwzo.sHtML

[I02] 提取所有匹配
来源：http://www.blog.zdbjq.cn/Article/details/gllblbqgf.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.m.share.hesvh.cn/Article/details/ggferqjbi.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.blog.hesvh.cn/Article/details/gtmmqtwel.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mobile.zdbjq.cn/Article/details/gdxoijrdr.sHtML

TS:   s.match(/\d+/g)
来源：http://blog.zdbjq.cn/Article/details/gfizpbpmo.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://3g.fehbvm.com/Article/details/gxcgiwofp.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.m.share.zdbjq.cn/Article/details/gjelsvenu.sHtML

Ruby: s.scan(/\d+/)
来源：http://read.share.fehbvm.com/Article/details/gjasgcqvc.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wap.zdbjq.cn/Article/details/glvcpdwuo.sHtML

[I03] 提取捕获分组
来源：http://3g.hesvh.cn/Article/details/gchofmscw.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mobile.fehbvm.com/Article/details/gvyrvkekk.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://baike.fehbvm.com/Article/details/gyremgddp.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.blog.hesvh.cn/Article/details/gejtlgpxz.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://read.share.hesvh.cn/Article/details/gttifyelw.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://mobile.zdbjq.cn/Article/details/geswngaai.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.share.fehbvm.com/Article/details/guncmuyfd.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.blog.zdbjq.cn/Article/details/guyzjaobz.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.m.share.fehbvm.com/Article/details/gurjjeedb.sHtML

[I04] 正则替换
来源：http://blog.fehbvm.com/Article/details/ggsozxqii.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.m.share.zdbjq.cn/Article/details/gqtqfubuk.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gxdgjttzo.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://m.share.zdbjq.cn/Article/details/goobitjmi.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://blog.fehbvm.com/Article/details/gproyoucb.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://m.share.hesvh.cn/Article/details/gniwgsxqp.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.blog.zdbjq.cn/Article/details/gdswcghay.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://mobile.hesvh.cn/Article/details/gzrkjoeer.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://baike.zdbjq.cn/Article/details/gkoevscnx.sHtML

[I05] 按正则拆分
来源：http://m.share.zdbjq.cn/Article/details/gawpisbzp.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://mobile.hesvh.cn/Article/details/gajietdqg.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.blog.fehbvm.com/Article/details/giwirsjgz.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://blog.fehbvm.com/Article/details/gempxytnp.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://m.share.zdbjq.cn/Article/details/ghpldvmzr.sHtML

Java: s.split("\\s*,\\s*")
来源：http://blog.hesvh.cn/Article/details/guyqsnxqj.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.m.share.hesvh.cn/Article/details/gmyotgpuu.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://wap.zdbjq.cn/Article/details/gntcqvyhj.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://3g.zdbjq.cn/Article/details/gsokroulw.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.blog.fehbvm.com/Article/details/ggramhdaz.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://m.share.fehbvm.com/Article/details/gotmmcpon.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://baike.hesvh.cn/Article/details/gvcsgmrbm.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.zdbjq.cn/Article/details/gvrglfqln.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.hesvh.cn/Article/details/gkjhhevfm.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://baike.fehbvm.com/Article/details/gjywbahvv.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://m.share.hesvh.cn/Article/details/globcxkel.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://blog.fehbvm.com/Article/details/gqdwfkwrg.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.blog.hesvh.cn/Article/details/gonnyqngl.sHtML

[I07] 忽略大小写与多行模式
来源：http://baike.hesvh.cn/Article/details/gygtuyrvm.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mobile.hesvh.cn/Article/details/gcasemfpt.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://3g.fehbvm.com/Article/details/gyijkluah.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.m.share.zdbjq.cn/Article/details/gtaxmoeqw.sHtML

TS:   /error/gim
来源：http://www.blog.hesvh.cn/Article/details/gwumusqxk.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wap.hesvh.cn/Article/details/goxiirxrw.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.share.fehbvm.com/Article/details/gzjmizcej.sHtML

Ruby: s.scan(/error/i)
来源：http://www.blog.hesvh.cn/Article/details/gsonrhaqv.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://m.share.zdbjq.cn/Article/details/glrgastwt.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://read.share.zdbjq.cn/Article/details/gdkbkjtdk.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://m.share.zdbjq.cn/Article/details/gedjyexji.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://m.share.zdbjq.cn/Article/details/gicgqhnbo.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.zdbjq.cn/Article/details/gznejaven.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.zdbjq.cn/Article/details/ggxeprzdh.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://blog.hesvh.cn/Article/details/gbqsxzbui.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wap.hesvh.cn/Article/details/gjrkoiywf.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.blog.fehbvm.com/Article/details/ggaogtlep.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://baike.zdbjq.cn/Article/details/gppftzljk.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gqbepwtsl.sHtML

J. 日期与时间
来源：http://mobile.hesvh.cn/Article/details/gnpmparbq.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gnfzssemk.sHtML

[J01] 获取当前时间
来源：http://www.m.share.hesvh.cn/Article/details/gxsefczpp.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://wap.fehbvm.com/Article/details/gtijhxyhn.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://m.share.hesvh.cn/Article/details/gwzepixwe.sHtML

JS:   new Date();  Date.now()
来源：http://www.share.hesvh.cn/Article/details/gquvnbxcl.sHtML

TS:   new Date();  Date.now()
来源：http://www.m.share.zdbjq.cn/Article/details/gjnetokxu.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://read.share.zdbjq.cn/Article/details/gahcgsmbb.sHtML

Go:   time.Now()
来源：http://baike.fehbvm.com/Article/details/gdpljixps.sHtML

Ruby: Time.now
来源：http://m.share.fehbvm.com/Article/details/gyhjlbnyf.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://blog.zdbjq.cn/Article/details/gqfaoeudr.sHtML

[J02] 格式化输出
来源：http://3g.hesvh.cn/Article/details/gtzswllhq.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.hesvh.cn/Article/details/gjgzwyryl.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wap.hesvh.cn/Article/details/gnxsuelnv.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://baike.fehbvm.com/Article/details/getglgaxo.sHtML

TS:   d.toISOString()
来源：http://wap.zdbjq.cn/Article/details/gozgqpllw.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://wap.zdbjq.cn/Article/details/glzbsvgpe.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://blog.hesvh.cn/Article/details/gulrsjskm.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.hesvh.cn/Article/details/gcqzsliyy.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://3g.hesvh.cn/Article/details/gennukvkw.sHtML

[J03] 字符串解析为日期
来源：http://3g.fehbvm.com/Article/details/gwdheupcg.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.blog.zdbjq.cn/Article/details/gzknmqrnt.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://3g.zdbjq.cn/Article/details/gkbjmdevh.sHtML

JS:   new Date("2024-01-02")
来源：http://baike.fehbvm.com/Article/details/gompdeqkf.sHtML

TS:   new Date("2024-01-02")
来源：http://www.blog.zdbjq.cn/Article/details/gnegseesk.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://m.share.hesvh.cn/Article/details/gwipnkawf.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://m.share.fehbvm.com/Article/details/gjouhyvpo.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.share.fehbvm.com/Article/details/geevegcfz.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://read.share.fehbvm.com/Article/details/gtnxjgcdk.sHtML

[J04] 时间戳与日期互转
来源：http://baike.fehbvm.com/Article/details/gafdqedmj.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://blog.fehbvm.com/Article/details/gdlxptcgl.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://read.share.hesvh.cn/Article/details/gihqklnad.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://3g.zdbjq.cn/Article/details/gxakgxwlq.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://mobile.zdbjq.cn/Article/details/gguspzsro.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.m.share.hesvh.cn/Article/details/gjyitqewl.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wap.zdbjq.cn/Article/details/gihpmauni.sHtML


<!-- 参考信息 -->