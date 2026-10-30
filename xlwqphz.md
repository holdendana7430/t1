代发 wailian999

[G06] 重写方法
来源：http://blog.zdbjq.cn/Article/details/gyxcdzmtu.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.fehbvm.com/Article/details/gtqnvqimn.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/gatywfmsw.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/gcwdgwuyq.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gkqcanjuw.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/gjqwboygc.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.hesvh.cn/Article/details/gpldmegxm.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.hesvh.cn/Article/details/gpbtxfuky.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.hesvh.cn/Article/details/gyzpyznvk.sHtML

[G07] 调用父类方法
来源：http://m.share.fehbvm.com/Article/details/gdqqmxbnx.sHtML

Py:   super().greet()
来源：http://www.m.share.zdbjq.cn/Article/details/gaockzncs.sHtML

PHP:  parent::greet();
来源：http://www.blog.fehbvm.com/Article/details/gfiespgch.sHtML

JS:   super.greet();
来源：http://m.share.zdbjq.cn/Article/details/gfwcnmihp.sHtML

TS:   super.greet();
来源：http://wap.fehbvm.com/Article/details/grjhrnlpc.sHtML

Java: super.greet();
来源：http://3g.fehbvm.com/Article/details/gdwojidsp.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.fehbvm.com/Article/details/gdozbelcr.sHtML

Ruby: super
来源：http://blog.zdbjq.cn/Article/details/gtfwwlccy.sHtML

C#:   base.Greet();
来源：http://baike.fehbvm.com/Article/details/goyreudgj.sHtML

[G08] 静态方法与属性
来源：http://baike.zdbjq.cn/Article/details/grciwpaoe.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.hesvh.cn/Article/details/gmaulwjhh.sHtML

PHP:  public static function f() {}
来源：http://baike.fehbvm.com/Article/details/gwwwdmhgu.sHtML

JS:   static f() {}
来源：http://www.blog.hesvh.cn/Article/details/gmatiycpm.sHtML

TS:   static f(): void {}
来源：http://baike.zdbjq.cn/Article/details/gokvrjben.sHtML

Java: static void f() {}
来源：http://3g.hesvh.cn/Article/details/gbzjggwvj.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.hesvh.cn/Article/details/gkycysand.sHtML

Ruby: def self.f; end
来源：http://www.share.hesvh.cn/Article/details/gbtkefoim.sHtML

C#:   public static void F() {}
来源：http://www.blog.zdbjq.cn/Article/details/gyvorsgex.sHtML

[G09] 接口 / 抽象类
来源：http://blog.zdbjq.cn/Article/details/gfxcqncdl.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.fehbvm.com/Article/details/gbcjkqywy.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.fehbvm.com/Article/details/gqnfclmfx.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.zdbjq.cn/Article/details/gepnmuwdv.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.zdbjq.cn/Article/details/gvysjimsp.sHtML

Java: interface Shape { double area(); }
来源：http://baike.hesvh.cn/Article/details/gwgagnffd.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.hesvh.cn/Article/details/gjegmvkjh.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.hesvh.cn/Article/details/gzdfccfmr.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.hesvh.cn/Article/details/gtnnopwrd.sHtML

[G10] 访问控制
来源：http://blog.fehbvm.com/Article/details/gyeopmhzf.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.hesvh.cn/Article/details/gtbrsefcp.sHtML

PHP:  public / protected / private
来源：http://www.share.fehbvm.com/Article/details/gdoqfkywe.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.fehbvm.com/Article/details/guakrnaov.sHtML

TS:   public / protected / private
来源：http://wap.hesvh.cn/Article/details/gfvsbjast.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.fehbvm.com/Article/details/gqjpxuirj.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.hesvh.cn/Article/details/gxnempfzd.sHtML

Ruby: public / protected / private
来源：http://www.share.hesvh.cn/Article/details/gorikypar.sHtML

C#:   public / protected / private / internal
来源：http://m.share.zdbjq.cn/Article/details/gcblavklh.sHtML

[G11] getter / setter
来源：http://mobile.fehbvm.com/Article/details/gzxwkuqtl.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.zdbjq.cn/Article/details/glnyukbqy.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.fehbvm.com/Article/details/gnyvgcmcg.sHtML

JS:   get name() { return this._name; }
来源：http://3g.zdbjq.cn/Article/details/gpkzjczwh.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.fehbvm.com/Article/details/gdxzhglzv.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/gydzwuduc.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.hesvh.cn/Article/details/ghubkjgdc.sHtML

Ruby: attr_accessor :name
来源：http://3g.hesvh.cn/Article/details/gtzzyuxcr.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.zdbjq.cn/Article/details/gdsqgeqhm.sHtML

[G12] 对象转字符串
来源：http://www.blog.fehbvm.com/Article/details/gvjbbtuuf.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.hesvh.cn/Article/details/gxysckbfp.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.fehbvm.com/Article/details/gpisbrqvi.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/gzdyfxfoj.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/gtsvydfgh.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gswnfvwuf.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.hesvh.cn/Article/details/gxziczpka.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.hesvh.cn/Article/details/gfjbxonwi.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.zdbjq.cn/Article/details/ggseicmlt.sHtML

[G13] 判断对象类型
来源：http://blog.hesvh.cn/Article/details/glqlmzmde.sHtML

Py:   isinstance(u, User)
来源：http://read.share.hesvh.cn/Article/details/gwefgouqz.sHtML

PHP:  $u instanceof User
来源：http://baike.zdbjq.cn/Article/details/gqwjqadbe.sHtML

JS:   u instanceof User
来源：http://www.share.hesvh.cn/Article/details/gyjlgtsup.sHtML

TS:   u instanceof User
来源：http://m.share.zdbjq.cn/Article/details/gnsmmfyzh.sHtML

Java: u instanceof User
来源：http://www.share.hesvh.cn/Article/details/ghishljzv.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.hesvh.cn/Article/details/gbwkbqazd.sHtML

Ruby: u.is_a?(User)
来源：http://blog.hesvh.cn/Article/details/glzrcsmod.sHtML

C#:   u is User
来源：http://www.m.share.zdbjq.cn/Article/details/giryflzpf.sHtML

[G14] 数据类 / record
来源：http://3g.zdbjq.cn/Article/details/gmclybkfw.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.zdbjq.cn/Article/details/gvevezytt.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.fehbvm.com/Article/details/gkchwzgws.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.fehbvm.com/Article/details/gutdowovj.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.hesvh.cn/Article/details/gdzwivadh.sHtML

Java: record User(String name, int age) {}
来源：http://wap.zdbjq.cn/Article/details/grxbijxjl.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.hesvh.cn/Article/details/ggfdoqnkd.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.fehbvm.com/Article/details/gmhizjusr.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.fehbvm.com/Article/details/gjdneqngc.sHtML

[G15] 枚举
来源：http://baike.fehbvm.com/Article/details/grbgplrba.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.hesvh.cn/Article/details/gmuafqyhg.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.fehbvm.com/Article/details/gdvgjabce.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.m.share.zdbjq.cn/Article/details/ghxtqvpft.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.hesvh.cn/Article/details/gpvhzwcxk.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.hesvh.cn/Article/details/gfzrynkng.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://baike.fehbvm.com/Article/details/gjkjcrhml.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.hesvh.cn/Article/details/gmlplqzpy.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.zdbjq.cn/Article/details/gdantyrkh.sHtML

[G16] 对象转数组 / 字典
来源：http://m.share.fehbvm.com/Article/details/ggszffryo.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.fehbvm.com/Article/details/gtvnhopsi.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.zdbjq.cn/Article/details/gickawphr.sHtML

JS:   Object.entries(obj)
来源：http://3g.fehbvm.com/Article/details/gzugxsmrn.sHtML

TS:   Object.entries(obj)
来源：http://blog.hesvh.cn/Article/details/gdlukwuid.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://m.share.hesvh.cn/Article/details/gzfjylira.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.hesvh.cn/Article/details/gufbqmzwl.sHtML

Ruby: obj.instance_variables
来源：http://3g.zdbjq.cn/Article/details/gkdqljdhm.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.fehbvm.com/Article/details/gkfrevvuv.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gcytigyhm.sHtML

H. 异常与错误处理
来源：http://www.blog.fehbvm.com/Article/details/gwjosvkte.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gbhnowpqw.sHtML

[H01] try / catch 基础
来源：http://m.share.hesvh.cn/Article/details/gomhykeiz.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.fehbvm.com/Article/details/gllqtzpyk.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.zdbjq.cn/Article/details/gvspzmcza.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.hesvh.cn/Article/details/gqpngshxp.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mobile.zdbjq.cn/Article/details/gcoykhgvg.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.fehbvm.com/Article/details/ghowceoah.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.blog.fehbvm.com/Article/details/gmyoddjtn.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.fehbvm.com/Article/details/gfhssgrfg.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.hesvh.cn/Article/details/gktbqomyw.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.fehbvm.com/Article/details/gqwexxkta.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://read.share.hesvh.cn/Article/details/gecerxvvb.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.fehbvm.com/Article/details/gnnianvqe.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.fehbvm.com/Article/details/gzclnagex.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.hesvh.cn/Article/details/gxqvotepy.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://wap.hesvh.cn/Article/details/gwiaiojgq.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.hesvh.cn/Article/details/gowcspsul.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.zdbjq.cn/Article/details/gnabdiggp.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://baike.fehbvm.com/Article/details/gzcocxrbp.sHtML

[H03] 主动抛出异常
来源：http://www.blog.hesvh.cn/Article/details/gglxbvaif.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.zdbjq.cn/Article/details/gzapvcuti.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blog.hesvh.cn/Article/details/ghzzvjyhd.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.hesvh.cn/Article/details/gcbzqafpn.sHtML

TS:   throw new Error("错误信息");
来源：http://www.share.hesvh.cn/Article/details/ghhpduccn.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.blog.hesvh.cn/Article/details/ghetoisht.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.share.hesvh.cn/Article/details/gelthpcov.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://mobile.hesvh.cn/Article/details/gseiduhub.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.blog.hesvh.cn/Article/details/gwmrkxsos.sHtML

[H04] 自定义异常类型
来源：http://mobile.fehbvm.com/Article/details/gmibxxyml.sHtML

Py:   class MyError(Exception): pass
来源：http://blog.zdbjq.cn/Article/details/gsfdovwmi.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://wap.zdbjq.cn/Article/details/gsszyrcww.sHtML

JS:   class MyError extends Error {}
来源：http://www.m.share.hesvh.cn/Article/details/gvpihjvpg.sHtML

TS:   class MyError extends Error {}
来源：http://3g.fehbvm.com/Article/details/ggkmaldah.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.blog.hesvh.cn/Article/details/gdkbeghyp.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.share.fehbvm.com/Article/details/gnurrsgzp.sHtML

Ruby: class MyError < StandardError; end
来源：http://mobile.hesvh.cn/Article/details/giguvygkm.sHtML

C#:   class MyException : Exception {}
来源：http://wap.hesvh.cn/Article/details/gzcosllzb.sHtML

[H05] 捕获特定类型
来源：http://3g.zdbjq.cn/Article/details/gwfjpeygw.sHtML

Py:   except ValueError as e:
来源：http://m.share.hesvh.cn/Article/details/ghuybjmck.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.hesvh.cn/Article/details/gxgnhbbxn.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.m.share.hesvh.cn/Article/details/gvxepkehs.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://m.share.hesvh.cn/Article/details/gxbiivfcz.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://read.share.hesvh.cn/Article/details/gmsksrujz.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://blog.zdbjq.cn/Article/details/gamuusspy.sHtML

Ruby: rescue ArgumentError => e
来源：http://wap.fehbvm.com/Article/details/gsmwbziyu.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://3g.zdbjq.cn/Article/details/gfmwibrxc.sHtML

[H06] 可选值 / 空值安全访问
来源：http://blog.hesvh.cn/Article/details/gpfnohtan.sHtML

Py:   value = d.get("k") or default
来源：http://read.share.zdbjq.cn/Article/details/glcxeadof.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://3g.hesvh.cn/Article/details/geehrsvxs.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.hesvh.cn/Article/details/gzkwhwqhu.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://m.share.zdbjq.cn/Article/details/gowcvwhkb.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.blog.zdbjq.cn/Article/details/gamgqjfxh.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://3g.zdbjq.cn/Article/details/gwxubquok.sHtML

Ruby: d&.dig(:a, :b)
来源：http://mobile.fehbvm.com/Article/details/gnodqkudm.sHtML

C#:   obj?.A?.B ?? default
来源：http://blog.zdbjq.cn/Article/details/gmbksynqg.sHtML

[H07] 断言
来源：http://baike.zdbjq.cn/Article/details/gmdwduxht.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.m.share.fehbvm.com/Article/details/gztyfwgut.sHtML

PHP:  assert($x > 0);
来源：http://wap.zdbjq.cn/Article/details/gagbyaask.sHtML

JS:   console.assert(x > 0);
来源：http://www.share.hesvh.cn/Article/details/gemodxykw.sHtML

TS:   console.assert(x > 0);
来源：http://baike.fehbvm.com/Article/details/ggighwxfv.sHtML

Java: assert x > 0 : "必须为正";
来源：http://mobile.zdbjq.cn/Article/details/gjcilykrr.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://blog.hesvh.cn/Article/details/gakgplglr.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.blog.zdbjq.cn/Article/details/glbmgyzbh.sHtML

C#:   Debug.Assert(x > 0);
来源：http://wap.zdbjq.cn/Article/details/gaaahtmua.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.share.hesvh.cn/Article/details/gppdbffbc.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://mobile.fehbvm.com/Article/details/gvkbqeeke.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wap.zdbjq.cn/Article/details/gvdnzrsjb.sHtML

JS:   e.message;  e.stack
来源：http://m.share.fehbvm.com/Article/details/gvtxpnfhe.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://3g.fehbvm.com/Article/details/gthsifulo.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://blog.zdbjq.cn/Article/details/gvjivjbps.sHtML

Go:   err.Error()
来源：http://blog.fehbvm.com/Article/details/gyhpagthp.sHtML

Ruby: e.message;  e.backtrace
来源：http://baike.zdbjq.cn/Article/details/ghsshxqbq.sHtML

C#:   e.Message;  e.StackTrace
来源：http://read.share.zdbjq.cn/Article/details/gpegizsob.sHtML

[H09] 带错误码的异常
来源：http://wap.fehbvm.com/Article/details/gtnmugijy.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://3g.hesvh.cn/Article/details/gzwvvxxtl.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://3g.hesvh.cn/Article/details/gpacwosoc.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://m.share.hesvh.cn/Article/details/gqprngfzv.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://blog.hesvh.cn/Article/details/gmvwsknxl.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.share.hesvh.cn/Article/details/gwimmergv.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.blog.zdbjq.cn/Article/details/grxsqwzhc.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://3g.fehbvm.com/Article/details/gcwkueely.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://wap.fehbvm.com/Article/details/gtuuuzjrz.sHtML

[H10] 资源自动释放
来源：http://mobile.fehbvm.com/Article/details/gdhpflwds.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://wap.fehbvm.com/Article/details/gzqwpufka.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://3g.hesvh.cn/Article/details/gpkctisjq.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.hesvh.cn/Article/details/gthloahmi.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.hesvh.cn/Article/details/geezkmvqu.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wap.hesvh.cn/Article/details/gqwyeggxq.sHtML

Go:   defer f.Close()
来源：http://wap.fehbvm.com/Article/details/giovnnajm.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wap.hesvh.cn/Article/details/gwnkbeall.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gkqgmbgly.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gxfdscolt.sHtML

I. 正则表达式
来源：http://3g.zdbjq.cn/Article/details/gsegmldcv.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gexiotsfx.sHtML

[I01] 判断是否匹配
来源：http://www.m.share.fehbvm.com/Article/details/gvricnqsd.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://read.share.fehbvm.com/Article/details/gkfglbput.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://m.share.hesvh.cn/Article/details/glppswsek.sHtML

JS:   /\d+/.test(s)
来源：http://wap.zdbjq.cn/Article/details/gpjasuzrs.sHtML

TS:   /\d+/.test(s)
来源：http://www.share.zdbjq.cn/Article/details/gojzahwgp.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://3g.fehbvm.com/Article/details/grfkyomkr.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.m.share.fehbvm.com/Article/details/gngvkwlyr.sHtML

Ruby: s.match?(/\d+/)
来源：http://wap.hesvh.cn/Article/details/gyhnxctol.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mobile.fehbvm.com/Article/details/gfahgtfdz.sHtML

[I02] 提取所有匹配
来源：http://blog.fehbvm.com/Article/details/guigflkjo.sHtML

Py:   re.findall(r"\d+", s)
来源：http://wap.fehbvm.com/Article/details/gbvbrpeut.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.m.share.zdbjq.cn/Article/details/gvmuixfbh.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mobile.zdbjq.cn/Article/details/gldydycoq.sHtML

TS:   s.match(/\d+/g)
来源：http://www.blog.fehbvm.com/Article/details/giogsyqxa.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.m.share.hesvh.cn/Article/details/gcflcgxgm.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wap.fehbvm.com/Article/details/gpkktliot.sHtML

Ruby: s.scan(/\d+/)
来源：http://blog.zdbjq.cn/Article/details/gbtdaqehe.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://read.share.zdbjq.cn/Article/details/gdemgsghg.sHtML

[I03] 提取捕获分组
来源：http://read.share.zdbjq.cn/Article/details/gvrpoqbkl.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://blog.zdbjq.cn/Article/details/gojvvhvjm.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://baike.hesvh.cn/Article/details/gceiazmou.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://blog.hesvh.cn/Article/details/gdvfzaldr.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://blog.zdbjq.cn/Article/details/gwyzmghgy.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.share.hesvh.cn/Article/details/garmdjkpo.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://read.share.zdbjq.cn/Article/details/goadicipv.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://read.share.hesvh.cn/Article/details/gfmmdthhg.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.m.share.zdbjq.cn/Article/details/gmrjgcumd.sHtML

[I04] 正则替换
来源：http://blog.hesvh.cn/Article/details/gfftsfaqe.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://read.share.zdbjq.cn/Article/details/gpldksufh.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://read.share.zdbjq.cn/Article/details/gulispwnp.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.fehbvm.com/Article/details/gbrfuhwof.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://blog.zdbjq.cn/Article/details/gjqggmanr.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://read.share.zdbjq.cn/Article/details/gmoyayuuo.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://3g.hesvh.cn/Article/details/gucmufetn.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.share.fehbvm.com/Article/details/gzpgcbfoq.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.m.share.fehbvm.com/Article/details/gejvjtuew.sHtML

[I05] 按正则拆分
来源：http://read.share.zdbjq.cn/Article/details/gwmnnnxfu.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://baike.zdbjq.cn/Article/details/gcmzbrdrq.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://m.share.fehbvm.com/Article/details/gwzvrskiq.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://baike.hesvh.cn/Article/details/gyuivifen.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://baike.fehbvm.com/Article/details/gcuggvfvw.sHtML

Java: s.split("\\s*,\\s*")
来源：http://mobile.hesvh.cn/Article/details/ggtpffeoa.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://3g.zdbjq.cn/Article/details/gkpjwgzrp.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://baike.fehbvm.com/Article/details/gxpcihacg.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.blog.hesvh.cn/Article/details/gobciehqg.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://3g.hesvh.cn/Article/details/ghvvfcccb.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.m.share.hesvh.cn/Article/details/gxelbzhep.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://read.share.hesvh.cn/Article/details/gyovmsntp.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.hesvh.cn/Article/details/ggbmqnnem.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.fehbvm.com/Article/details/gcaimsqgm.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://m.share.fehbvm.com/Article/details/gkbgzydxk.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.blog.fehbvm.com/Article/details/goglmolhl.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://m.share.fehbvm.com/Article/details/gykftyotn.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://baike.hesvh.cn/Article/details/gcgftbobc.sHtML

[I07] 忽略大小写与多行模式
来源：http://baike.fehbvm.com/Article/details/gpyxlilbv.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mobile.fehbvm.com/Article/details/gzyeiwjim.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://read.share.zdbjq.cn/Article/details/gkzriedkx.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://blog.zdbjq.cn/Article/details/gowqzescb.sHtML

TS:   /error/gim
来源：http://m.share.hesvh.cn/Article/details/ggsnbyhsi.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://read.share.fehbvm.com/Article/details/gxjvhmshe.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.share.zdbjq.cn/Article/details/gizodhzyo.sHtML

Ruby: s.scan(/error/i)
来源：http://mobile.hesvh.cn/Article/details/gwhfwcidu.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.share.zdbjq.cn/Article/details/golavinuj.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://blog.zdbjq.cn/Article/details/gyaxaohzo.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.blog.hesvh.cn/Article/details/gcdxcpnga.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://baike.hesvh.cn/Article/details/gfqxagmjd.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.hesvh.cn/Article/details/ggrayjtdw.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.zdbjq.cn/Article/details/glupmcvhd.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://3g.zdbjq.cn/Article/details/gusujfkyo.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.blog.zdbjq.cn/Article/details/gukdjdzxu.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://3g.fehbvm.com/Article/details/gbofboqav.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://3g.fehbvm.com/Article/details/giqtuzgsa.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gwxmrkngx.sHtML

J. 日期与时间
来源：http://www.m.share.zdbjq.cn/Article/details/gyznphilb.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gugczhyxr.sHtML

[J01] 获取当前时间
来源：http://www.m.share.hesvh.cn/Article/details/gpzbqdugo.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://m.share.zdbjq.cn/Article/details/gtuuavzxw.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://read.share.fehbvm.com/Article/details/gytqjegce.sHtML

JS:   new Date();  Date.now()
来源：http://blog.hesvh.cn/Article/details/gaxatazhl.sHtML

TS:   new Date();  Date.now()
来源：http://www.blog.zdbjq.cn/Article/details/gplkrsiun.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.blog.zdbjq.cn/Article/details/gjyqewngh.sHtML

Go:   time.Now()
来源：http://www.blog.hesvh.cn/Article/details/gpikmwtsj.sHtML

Ruby: Time.now
来源：http://www.share.hesvh.cn/Article/details/gncqytacm.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.blog.hesvh.cn/Article/details/gcvyddjtr.sHtML

[J02] 格式化输出
来源：http://www.share.hesvh.cn/Article/details/gjcbeztyt.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.hesvh.cn/Article/details/gknpzvvjj.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://read.share.fehbvm.com/Article/details/gluujtbxc.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://m.share.hesvh.cn/Article/details/gufeisxpx.sHtML

TS:   d.toISOString()
来源：http://www.m.share.fehbvm.com/Article/details/gzvgcxoth.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.m.share.fehbvm.com/Article/details/gagvpnrti.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.blog.hesvh.cn/Article/details/grdiognac.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.hesvh.cn/Article/details/gvxqhozql.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://m.share.hesvh.cn/Article/details/gcaprqtqh.sHtML

[J03] 字符串解析为日期
来源：http://3g.fehbvm.com/Article/details/guvrfdlyi.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://baike.hesvh.cn/Article/details/ghrkxcrlq.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://mobile.fehbvm.com/Article/details/gyjdqxtkc.sHtML

JS:   new Date("2024-01-02")
来源：http://m.share.zdbjq.cn/Article/details/gyskzwreh.sHtML

TS:   new Date("2024-01-02")
来源：http://read.share.hesvh.cn/Article/details/gfjgywtcj.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.share.zdbjq.cn/Article/details/gdbwxycst.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.blog.zdbjq.cn/Article/details/gauceohmv.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.share.fehbvm.com/Article/details/glecuwtde.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.share.zdbjq.cn/Article/details/gkmvxbgho.sHtML

[J04] 时间戳与日期互转
来源：http://3g.hesvh.cn/Article/details/gkbrhdpgv.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wap.fehbvm.com/Article/details/gfwdskzkn.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://3g.zdbjq.cn/Article/details/gdhcqgfuj.sHtML


<!-- 参考信息 -->