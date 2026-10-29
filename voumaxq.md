代发 wailian999

TS:   greet(): string { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/gntfisyxm.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/gufmiafvx.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.zdbjq.cn/Article/details/gipekuukv.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.hesvh.cn/Article/details/gjhyequsp.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.hesvh.cn/Article/details/glglpoolf.sHtML

[G07] 调用父类方法
来源：http://wap.hesvh.cn/Article/details/grifazpcq.sHtML

Py:   super().greet()
来源：http://www.m.share.zdbjq.cn/Article/details/gbedeztna.sHtML

PHP:  parent::greet();
来源：http://mobile.hesvh.cn/Article/details/gafqijbsb.sHtML

JS:   super.greet();
来源：http://mobile.zdbjq.cn/Article/details/gdmuphjul.sHtML

TS:   super.greet();
来源：http://3g.hesvh.cn/Article/details/gjfrhylpj.sHtML

Java: super.greet();
来源：http://wap.fehbvm.com/Article/details/gnlrzgmli.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.hesvh.cn/Article/details/ggmgdqrub.sHtML

Ruby: super
来源：http://read.share.fehbvm.com/Article/details/gcuezzstv.sHtML

C#:   base.Greet();
来源：http://mobile.zdbjq.cn/Article/details/gboldtrfz.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.fehbvm.com/Article/details/ggtpptibf.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.fehbvm.com/Article/details/gctjnpuas.sHtML

PHP:  public static function f() {}
来源：http://read.share.zdbjq.cn/Article/details/gmvejcqze.sHtML

JS:   static f() {}
来源：http://www.blog.fehbvm.com/Article/details/gywxccubm.sHtML

TS:   static f(): void {}
来源：http://mobile.hesvh.cn/Article/details/ghaayruwq.sHtML

Java: static void f() {}
来源：http://www.share.hesvh.cn/Article/details/gcvcdyblf.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.hesvh.cn/Article/details/gibkgziaz.sHtML

Ruby: def self.f; end
来源：http://www.blog.zdbjq.cn/Article/details/gpfijuben.sHtML

C#:   public static void F() {}
来源：http://www.blog.fehbvm.com/Article/details/gcuoqjywg.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.fehbvm.com/Article/details/gvdgthphd.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.fehbvm.com/Article/details/ggpnulxpi.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.hesvh.cn/Article/details/gxnregnve.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.fehbvm.com/Article/details/gvtheqmiv.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.fehbvm.com/Article/details/goqfnwlqm.sHtML

Java: interface Shape { double area(); }
来源：http://blog.zdbjq.cn/Article/details/gotwelfof.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.fehbvm.com/Article/details/gmyjhvuut.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.zdbjq.cn/Article/details/gejgavxvl.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.fehbvm.com/Article/details/gszptekxa.sHtML

[G10] 访问控制
来源：http://3g.zdbjq.cn/Article/details/gnyfqwoxd.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.zdbjq.cn/Article/details/gjmwgstps.sHtML

PHP:  public / protected / private
来源：http://blog.hesvh.cn/Article/details/gtysxgvvo.sHtML

JS:   #private 字段；其余公开
来源：http://3g.fehbvm.com/Article/details/gohqplknm.sHtML

TS:   public / protected / private
来源：http://m.share.zdbjq.cn/Article/details/gxjsggguk.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.hesvh.cn/Article/details/grvuuywmq.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.hesvh.cn/Article/details/gijmnehjg.sHtML

Ruby: public / protected / private
来源：http://www.m.share.fehbvm.com/Article/details/gioaxspbe.sHtML

C#:   public / protected / private / internal
来源：http://3g.hesvh.cn/Article/details/gdpbjthvi.sHtML

[G11] getter / setter
来源：http://m.share.zdbjq.cn/Article/details/gxyblduva.sHtML

Py:   @property 与 @x.setter
来源：http://baike.hesvh.cn/Article/details/ghvezyodp.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.zdbjq.cn/Article/details/gjxnqwdan.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gyqkjbxwp.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.fehbvm.com/Article/details/ggupzuhrc.sHtML

Java: public String getName() { return name; }
来源：http://blog.zdbjq.cn/Article/details/ggbinbnan.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.hesvh.cn/Article/details/gllmuyobt.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.fehbvm.com/Article/details/ghpezhpjk.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.hesvh.cn/Article/details/gckchuezl.sHtML

[G12] 对象转字符串
来源：http://baike.zdbjq.cn/Article/details/gvikkjadz.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.hesvh.cn/Article/details/gqmcuymot.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.fehbvm.com/Article/details/gitztoqbb.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/gwjnjutei.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/gmvhxgqln.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.fehbvm.com/Article/details/gpaufkluz.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.hesvh.cn/Article/details/gdhfjxgyd.sHtML

Ruby: def to_s; @name; end
来源：http://3g.zdbjq.cn/Article/details/gxilvvmxk.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.zdbjq.cn/Article/details/gdqaeicyu.sHtML

[G13] 判断对象类型
来源：http://www.share.zdbjq.cn/Article/details/gkpdegebo.sHtML

Py:   isinstance(u, User)
来源：http://read.share.fehbvm.com/Article/details/gcroudhad.sHtML

PHP:  $u instanceof User
来源：http://www.blog.hesvh.cn/Article/details/gcilyozfo.sHtML

JS:   u instanceof User
来源：http://blog.fehbvm.com/Article/details/gmnacigzg.sHtML

TS:   u instanceof User
来源：http://www.m.share.hesvh.cn/Article/details/gsnpdoxgg.sHtML

Java: u instanceof User
来源：http://3g.hesvh.cn/Article/details/gldjewgje.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.fehbvm.com/Article/details/gfeqnvwls.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.fehbvm.com/Article/details/ghivblocy.sHtML

C#:   u is User
来源：http://www.share.zdbjq.cn/Article/details/gtcxxqqfz.sHtML

[G14] 数据类 / record
来源：http://baike.fehbvm.com/Article/details/gvfccfpjf.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://baike.zdbjq.cn/Article/details/gzxyzddmy.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.zdbjq.cn/Article/details/giewiphuc.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.zdbjq.cn/Article/details/gqvglxfkc.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.fehbvm.com/Article/details/glelcwgvz.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.fehbvm.com/Article/details/gmoyxdguh.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.fehbvm.com/Article/details/gjdsotycj.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.zdbjq.cn/Article/details/gyziwgsgk.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.zdbjq.cn/Article/details/gmqqbxivf.sHtML

[G15] 枚举
来源：http://wap.hesvh.cn/Article/details/gosvzlekd.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.fehbvm.com/Article/details/gwfsrjoje.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gjhxvvyqb.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.zdbjq.cn/Article/details/gnaeciopx.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.hesvh.cn/Article/details/gobircktg.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.zdbjq.cn/Article/details/guokhmams.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://baike.zdbjq.cn/Article/details/gsbndsplj.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.m.share.hesvh.cn/Article/details/gagupzrxj.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.zdbjq.cn/Article/details/gtlaxgcwt.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.hesvh.cn/Article/details/ghxdgpqxr.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.fehbvm.com/Article/details/gxxfwvyxj.sHtML

PHP:  get_object_vars($obj);
来源：http://3g.hesvh.cn/Article/details/gtabifgjw.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gwlapmunj.sHtML

TS:   Object.entries(obj)
来源：http://3g.hesvh.cn/Article/details/ghoypfrjx.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.fehbvm.com/Article/details/gektyeius.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.fehbvm.com/Article/details/gxjsbxqtc.sHtML

Ruby: obj.instance_variables
来源：http://read.share.zdbjq.cn/Article/details/gapcwfouh.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.zdbjq.cn/Article/details/gzckxjzgt.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/ggbudizhl.sHtML

H. 异常与错误处理
来源：http://www.share.hesvh.cn/Article/details/gatdznsrn.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gwhfjzvbg.sHtML

[H01] try / catch 基础
来源：http://www.blog.zdbjq.cn/Article/details/gfpnonhqb.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.hesvh.cn/Article/details/ghuasihol.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.fehbvm.com/Article/details/gqfxhqwik.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://blog.fehbvm.com/Article/details/gngezgcpx.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.hesvh.cn/Article/details/glgbohazm.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.zdbjq.cn/Article/details/gfyqcplvr.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.zdbjq.cn/Article/details/goxypoked.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.hesvh.cn/Article/details/gpwpiyfrl.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.hesvh.cn/Article/details/gblxuwmfp.sHtML

[H02] finally / ensure 收尾
来源：http://mobile.fehbvm.com/Article/details/gzqdwqica.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://3g.fehbvm.com/Article/details/guypbakoj.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://blog.hesvh.cn/Article/details/gtndwdjco.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.fehbvm.com/Article/details/gztpwyvkq.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gictdvwcr.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.blog.hesvh.cn/Article/details/gxbmsnpaa.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.share.zdbjq.cn/Article/details/ghvdkfaeo.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.fehbvm.com/Article/details/gnboeukbo.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://3g.zdbjq.cn/Article/details/gvgbsrlpi.sHtML

[H03] 主动抛出异常
来源：http://mobile.fehbvm.com/Article/details/gepjwbiki.sHtML

Py:   raise ValueError("错误信息")
来源：http://baike.zdbjq.cn/Article/details/gkzftttfr.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://m.share.zdbjq.cn/Article/details/glkzaqzmx.sHtML

JS:   throw new Error("错误信息");
来源：http://www.blog.fehbvm.com/Article/details/gqwwnstzy.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.zdbjq.cn/Article/details/gtwgvjpkb.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://mobile.zdbjq.cn/Article/details/gdvcudfgz.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://read.share.hesvh.cn/Article/details/gjljlryfj.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://wap.hesvh.cn/Article/details/germvtbqa.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.share.zdbjq.cn/Article/details/gbvqldxlo.sHtML

[H04] 自定义异常类型
来源：http://www.share.zdbjq.cn/Article/details/gygsgdudp.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.fehbvm.com/Article/details/gqgkomglv.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.share.fehbvm.com/Article/details/grbrqorqv.sHtML

JS:   class MyError extends Error {}
来源：http://www.share.zdbjq.cn/Article/details/gighpppdh.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.zdbjq.cn/Article/details/gqowaifyh.sHtML

Java: class MyException extends RuntimeException {}
来源：http://baike.hesvh.cn/Article/details/gwjmuyphm.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.zdbjq.cn/Article/details/gclcnpzuf.sHtML

Ruby: class MyError < StandardError; end
来源：http://m.share.zdbjq.cn/Article/details/gaorvppdh.sHtML

C#:   class MyException : Exception {}
来源：http://baike.fehbvm.com/Article/details/gvasvwrbh.sHtML

[H05] 捕获特定类型
来源：http://www.m.share.hesvh.cn/Article/details/gdsvaktay.sHtML

Py:   except ValueError as e:
来源：http://www.m.share.hesvh.cn/Article/details/gkcsjizdp.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.blog.zdbjq.cn/Article/details/grjzsuafv.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://mobile.fehbvm.com/Article/details/gssbsiemw.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://wap.fehbvm.com/Article/details/grlbgacyv.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.blog.hesvh.cn/Article/details/gotvpupzs.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.share.fehbvm.com/Article/details/gmgquvfka.sHtML

Ruby: rescue ArgumentError => e
来源：http://blog.zdbjq.cn/Article/details/gryeshthx.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mobile.hesvh.cn/Article/details/gfjtdrpkm.sHtML

[H06] 可选值 / 空值安全访问
来源：http://read.share.fehbvm.com/Article/details/gfblgqszr.sHtML

Py:   value = d.get("k") or default
来源：http://baike.hesvh.cn/Article/details/gjxwemunl.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.zdbjq.cn/Article/details/ghplxnjeh.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.blog.fehbvm.com/Article/details/gxhgrsudf.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://3g.fehbvm.com/Article/details/gnylgjkol.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.m.share.zdbjq.cn/Article/details/gvifmvvnh.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://wap.zdbjq.cn/Article/details/gvqqvzujm.sHtML

Ruby: d&.dig(:a, :b)
来源：http://read.share.hesvh.cn/Article/details/gnedkjlne.sHtML

C#:   obj?.A?.B ?? default
来源：http://m.share.zdbjq.cn/Article/details/gvoyhvgtk.sHtML

[H07] 断言
来源：http://3g.fehbvm.com/Article/details/gpidufzie.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.share.hesvh.cn/Article/details/gjeoxbbmk.sHtML

PHP:  assert($x > 0);
来源：http://read.share.fehbvm.com/Article/details/gnlannydv.sHtML

JS:   console.assert(x > 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gedmpcmjk.sHtML

TS:   console.assert(x > 0);
来源：http://3g.hesvh.cn/Article/details/gkgtbyyht.sHtML

Java: assert x > 0 : "必须为正";
来源：http://m.share.hesvh.cn/Article/details/gtuetoazr.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://read.share.zdbjq.cn/Article/details/gcsaxoiqg.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://read.share.fehbvm.com/Article/details/gbwunywxu.sHtML

C#:   Debug.Assert(x > 0);
来源：http://3g.zdbjq.cn/Article/details/gttmgqgnh.sHtML

[H08] 获取错误信息与堆栈
来源：http://3g.zdbjq.cn/Article/details/gppneijic.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://blog.hesvh.cn/Article/details/gnltetrtr.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mobile.zdbjq.cn/Article/details/gjjfdlrpo.sHtML

JS:   e.message;  e.stack
来源：http://baike.fehbvm.com/Article/details/gwjjrznbg.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://wap.hesvh.cn/Article/details/gizzryvhm.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://read.share.fehbvm.com/Article/details/gmmlvuheo.sHtML

Go:   err.Error()
来源：http://3g.zdbjq.cn/Article/details/gjdieaivy.sHtML

Ruby: e.message;  e.backtrace
来源：http://baike.zdbjq.cn/Article/details/gwfzlouej.sHtML

C#:   e.Message;  e.StackTrace
来源：http://blog.zdbjq.cn/Article/details/gmsnojkoi.sHtML

[H09] 带错误码的异常
来源：http://read.share.zdbjq.cn/Article/details/gkwunozdz.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://baike.zdbjq.cn/Article/details/gmzhrltqw.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.m.share.fehbvm.com/Article/details/gflimsfra.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://m.share.hesvh.cn/Article/details/ghtsiipoh.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://blog.fehbvm.com/Article/details/gevhkghdi.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://baike.zdbjq.cn/Article/details/gzmipdnya.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://m.share.fehbvm.com/Article/details/gejkuuakc.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.blog.zdbjq.cn/Article/details/ggpxrncxv.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://blog.fehbvm.com/Article/details/goxfduskc.sHtML

[H10] 资源自动释放
来源：http://www.share.zdbjq.cn/Article/details/giiaasoye.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://m.share.fehbvm.com/Article/details/ggdetvkrg.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://baike.hesvh.cn/Article/details/gfwgxafyl.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.hesvh.cn/Article/details/gbnjgsgpx.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.fehbvm.com/Article/details/gxfjxlqma.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://3g.zdbjq.cn/Article/details/gozdxcvkp.sHtML

Go:   defer f.Close()
来源：http://wap.hesvh.cn/Article/details/gvvctzvkv.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mobile.hesvh.cn/Article/details/gwqvoqsho.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gonhrfnrz.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gvdkhnkij.sHtML

I. 正则表达式
来源：http://www.m.share.zdbjq.cn/Article/details/gnovbffcf.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gpcbwxvvq.sHtML

[I01] 判断是否匹配
来源：http://mobile.fehbvm.com/Article/details/gyobcdrfh.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://m.share.hesvh.cn/Article/details/gxxmmbydx.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.share.hesvh.cn/Article/details/gkdgzzosc.sHtML

JS:   /\d+/.test(s)
来源：http://www.share.fehbvm.com/Article/details/ghztgilfr.sHtML

TS:   /\d+/.test(s)
来源：http://www.blog.fehbvm.com/Article/details/gvvvqmfrs.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://m.share.fehbvm.com/Article/details/gicywilos.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://m.share.zdbjq.cn/Article/details/gjuouggrs.sHtML

Ruby: s.match?(/\d+/)
来源：http://blog.hesvh.cn/Article/details/gjjwegvxl.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.m.share.hesvh.cn/Article/details/gucgoffej.sHtML

[I02] 提取所有匹配
来源：http://wap.fehbvm.com/Article/details/grndkwnmc.sHtML

Py:   re.findall(r"\d+", s)
来源：http://m.share.hesvh.cn/Article/details/gaeqoazui.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.blog.hesvh.cn/Article/details/gfoanarre.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.m.share.fehbvm.com/Article/details/grajnetlo.sHtML

TS:   s.match(/\d+/g)
来源：http://www.share.zdbjq.cn/Article/details/gguhmanvd.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.m.share.fehbvm.com/Article/details/gghzqsmow.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.m.share.fehbvm.com/Article/details/gfkoivblo.sHtML

Ruby: s.scan(/\d+/)
来源：http://3g.fehbvm.com/Article/details/gadtrnymj.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://m.share.fehbvm.com/Article/details/gtoehjwfn.sHtML

[I03] 提取捕获分组
来源：http://read.share.zdbjq.cn/Article/details/gycliqccs.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://3g.fehbvm.com/Article/details/gdzkvqxxg.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.blog.hesvh.cn/Article/details/ghbygxjxh.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://3g.hesvh.cn/Article/details/gpietomso.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mobile.hesvh.cn/Article/details/gzaicanla.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://baike.fehbvm.com/Article/details/gvlvxuyom.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.blog.fehbvm.com/Article/details/gibdgtllo.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://3g.hesvh.cn/Article/details/gnrodrzbw.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://3g.zdbjq.cn/Article/details/ggrvmsybu.sHtML

[I04] 正则替换
来源：http://baike.zdbjq.cn/Article/details/gnlpekvvr.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.m.share.fehbvm.com/Article/details/gufhexrqw.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://blog.hesvh.cn/Article/details/ghwcxnnbr.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://3g.hesvh.cn/Article/details/gupvzkvag.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://read.share.fehbvm.com/Article/details/gyjfgffto.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://read.share.zdbjq.cn/Article/details/grmjvlqta.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.m.share.fehbvm.com/Article/details/gcxbpiafo.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://baike.fehbvm.com/Article/details/ghfvdthws.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.m.share.hesvh.cn/Article/details/gjjrzeeww.sHtML

[I05] 按正则拆分
来源：http://www.blog.zdbjq.cn/Article/details/gvsogcpqb.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://3g.fehbvm.com/Article/details/gbjdlfzek.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://m.share.zdbjq.cn/Article/details/gpcylmwbm.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.share.hesvh.cn/Article/details/gfguruqbe.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://wap.fehbvm.com/Article/details/gsmgpenxf.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.m.share.hesvh.cn/Article/details/glpgfyjnj.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.share.fehbvm.com/Article/details/gzjkgncqv.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://wap.hesvh.cn/Article/details/gsvocwori.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wap.zdbjq.cn/Article/details/gylneognu.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.blog.zdbjq.cn/Article/details/gsfzdelyb.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.share.hesvh.cn/Article/details/gbxlifxff.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://read.share.fehbvm.com/Article/details/gvnuicsnd.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.fehbvm.com/Article/details/gwjevwytn.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.fehbvm.com/Article/details/gzgidnyvn.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://blog.fehbvm.com/Article/details/gcqjtyqid.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://baike.fehbvm.com/Article/details/gttpfvdje.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://3g.zdbjq.cn/Article/details/gksdywdig.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://baike.fehbvm.com/Article/details/gttnolppz.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.share.fehbvm.com/Article/details/gsihhwxhz.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mobile.fehbvm.com/Article/details/grmfbnaps.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.blog.zdbjq.cn/Article/details/gyqekhkae.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mobile.hesvh.cn/Article/details/guoimfmdu.sHtML

TS:   /error/gim
来源：http://www.m.share.fehbvm.com/Article/details/grijxakvk.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mobile.zdbjq.cn/Article/details/gclouxuaa.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.share.hesvh.cn/Article/details/glspraagd.sHtML

Ruby: s.scan(/error/i)
来源：http://www.blog.fehbvm.com/Article/details/gudusalcr.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mobile.zdbjq.cn/Article/details/gegnllupv.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.m.share.hesvh.cn/Article/details/galhkcpvv.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.share.zdbjq.cn/Article/details/glyppkjcx.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://m.share.fehbvm.com/Article/details/gcoelaphn.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.fehbvm.com/Article/details/gmiovnldo.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.zdbjq.cn/Article/details/gnhaklyxs.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://3g.hesvh.cn/Article/details/gbxscgnfd.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wap.hesvh.cn/Article/details/gabgfxurk.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.blog.hesvh.cn/Article/details/gwfgsabmk.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://read.share.fehbvm.com/Article/details/gohubfvvl.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gzrjunbpr.sHtML

J. 日期与时间
来源：http://baike.hesvh.cn/Article/details/gdtbfmmjg.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/guvejticf.sHtML

[J01] 获取当前时间
来源：http://baike.hesvh.cn/Article/details/guredrimi.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://read.share.zdbjq.cn/Article/details/gxgbuzwhl.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://blog.fehbvm.com/Article/details/gfkltqdcq.sHtML

JS:   new Date();  Date.now()
来源：http://m.share.zdbjq.cn/Article/details/gwefvtbim.sHtML

TS:   new Date();  Date.now()
来源：http://blog.hesvh.cn/Article/details/gdhvqrmco.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.blog.zdbjq.cn/Article/details/ggnpgxnit.sHtML

Go:   time.Now()
来源：http://read.share.zdbjq.cn/Article/details/gnpzxatwp.sHtML

Ruby: Time.now
来源：http://read.share.zdbjq.cn/Article/details/gsupxvsxw.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://mobile.hesvh.cn/Article/details/gphhnxjub.sHtML

[J02] 格式化输出
来源：http://baike.hesvh.cn/Article/details/gvokjjrvd.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.zdbjq.cn/Article/details/gswzwpgpq.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.share.zdbjq.cn/Article/details/gwpakluce.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.m.share.zdbjq.cn/Article/details/gqnmcbspl.sHtML

TS:   d.toISOString()
来源：http://mobile.hesvh.cn/Article/details/gpkfntwis.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://read.share.hesvh.cn/Article/details/gbackkuuy.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.share.zdbjq.cn/Article/details/gqfoauedj.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.zdbjq.cn/Article/details/gecjulaot.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.blog.fehbvm.com/Article/details/gptjgynib.sHtML

[J03] 字符串解析为日期
来源：http://blog.hesvh.cn/Article/details/guazswrep.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://blog.zdbjq.cn/Article/details/glyixapzc.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://mobile.fehbvm.com/Article/details/gzfqwlnsj.sHtML

JS:   new Date("2024-01-02")
来源：http://3g.fehbvm.com/Article/details/gswzjtlfq.sHtML

TS:   new Date("2024-01-02")
来源：http://3g.fehbvm.com/Article/details/grcgjmthd.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.m.share.fehbvm.com/Article/details/gbdurgqaq.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wap.zdbjq.cn/Article/details/gbsoyopbb.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.blog.fehbvm.com/Article/details/gagwseopm.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.share.fehbvm.com/Article/details/gemjgdhem.sHtML

[J04] 时间戳与日期互转
来源：http://3g.hesvh.cn/Article/details/gkuukxqxs.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://baike.zdbjq.cn/Article/details/gmzjnleqp.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.m.share.fehbvm.com/Article/details/gwulnwwpj.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://baike.fehbvm.com/Article/details/gorpbntet.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://baike.hesvh.cn/Article/details/gxqycveek.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.share.zdbjq.cn/Article/details/ggjnsqpxt.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://read.share.zdbjq.cn/Article/details/ggrbatpzk.sHtML


<!-- 参考信息 -->