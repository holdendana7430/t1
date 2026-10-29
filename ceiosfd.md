代发 wailian999

C#:   public override string Greet() => "admin";
来源：http://www.m.share.fehbvm.com/Article/details/gkeankrjp.sHtML

[G07] 调用父类方法
来源：http://baike.zdbjq.cn/Article/details/gwzuhmjwi.sHtML

Py:   super().greet()
来源：http://m.share.zdbjq.cn/Article/details/ghqvhnkwr.sHtML

PHP:  parent::greet();
来源：http://www.share.zdbjq.cn/Article/details/gspufbqbu.sHtML

JS:   super.greet();
来源：http://wap.hesvh.cn/Article/details/geujzqrbf.sHtML

TS:   super.greet();
来源：http://www.share.hesvh.cn/Article/details/gxkdsqulh.sHtML

Java: super.greet();
来源：http://www.share.hesvh.cn/Article/details/gptvohuzb.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.hesvh.cn/Article/details/gwxodgxyd.sHtML

Ruby: super
来源：http://www.m.share.fehbvm.com/Article/details/gjkzqdsbh.sHtML

C#:   base.Greet();
来源：http://3g.fehbvm.com/Article/details/gdizgtpfb.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.hesvh.cn/Article/details/giqpmsflj.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.fehbvm.com/Article/details/gevwgljfw.sHtML

PHP:  public static function f() {}
来源：http://baike.fehbvm.com/Article/details/gtbdtvwdw.sHtML

JS:   static f() {}
来源：http://www.blog.zdbjq.cn/Article/details/gnmmwpdzz.sHtML

TS:   static f(): void {}
来源：http://wap.hesvh.cn/Article/details/gvoeqwlso.sHtML

Java: static void f() {}
来源：http://read.share.zdbjq.cn/Article/details/gqvyqcove.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.zdbjq.cn/Article/details/gfzqukrya.sHtML

Ruby: def self.f; end
来源：http://mobile.zdbjq.cn/Article/details/gewfsnvkh.sHtML

C#:   public static void F() {}
来源：http://3g.hesvh.cn/Article/details/gdkahhicf.sHtML

[G09] 接口 / 抽象类
来源：http://baike.fehbvm.com/Article/details/gejaoxkwx.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.zdbjq.cn/Article/details/gqzdqfemz.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.hesvh.cn/Article/details/gogqtfmct.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.zdbjq.cn/Article/details/gglmplwfj.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.hesvh.cn/Article/details/gmrajnuwv.sHtML

Java: interface Shape { double area(); }
来源：http://wap.hesvh.cn/Article/details/gmrvxtqhl.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.zdbjq.cn/Article/details/gsstpemca.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.zdbjq.cn/Article/details/gyzqhrxpp.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.hesvh.cn/Article/details/gxodgpuja.sHtML

[G10] 访问控制
来源：http://www.blog.hesvh.cn/Article/details/grgnrwvbk.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.hesvh.cn/Article/details/gzqspxbew.sHtML

PHP:  public / protected / private
来源：http://wap.zdbjq.cn/Article/details/grhuwecwg.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.hesvh.cn/Article/details/gpcltrjpo.sHtML

TS:   public / protected / private
来源：http://blog.fehbvm.com/Article/details/gahqswtuh.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.hesvh.cn/Article/details/gahtbfleo.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.zdbjq.cn/Article/details/gnoaeiqfa.sHtML

Ruby: public / protected / private
来源：http://baike.zdbjq.cn/Article/details/gptuwfuaw.sHtML

C#:   public / protected / private / internal
来源：http://wap.fehbvm.com/Article/details/gxkczlffi.sHtML

[G11] getter / setter
来源：http://mobile.zdbjq.cn/Article/details/ggahnmmib.sHtML

Py:   @property 与 @x.setter
来源：http://wap.zdbjq.cn/Article/details/gtryhfleg.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.fehbvm.com/Article/details/gfoxxatde.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.zdbjq.cn/Article/details/gecslxrdu.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.fehbvm.com/Article/details/gyhqemtbx.sHtML

Java: public String getName() { return name; }
来源：http://m.share.fehbvm.com/Article/details/gclickafw.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.hesvh.cn/Article/details/gabsbqofn.sHtML

Ruby: attr_accessor :name
来源：http://blog.zdbjq.cn/Article/details/gxvqakwgf.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.fehbvm.com/Article/details/gnrxdiszz.sHtML

[G12] 对象转字符串
来源：http://mobile.fehbvm.com/Article/details/gmkogozfo.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.fehbvm.com/Article/details/gtkocdxwb.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.zdbjq.cn/Article/details/gztcyrqcn.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/gualilaph.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.fehbvm.com/Article/details/gybnciune.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.hesvh.cn/Article/details/gjktxygzz.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.fehbvm.com/Article/details/gkapvgvsw.sHtML

Ruby: def to_s; @name; end
来源：http://blog.fehbvm.com/Article/details/gduikxdgj.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.hesvh.cn/Article/details/geoufxuif.sHtML

[G13] 判断对象类型
来源：http://3g.zdbjq.cn/Article/details/gzirhcsat.sHtML

Py:   isinstance(u, User)
来源：http://read.share.zdbjq.cn/Article/details/ggqjpucro.sHtML

PHP:  $u instanceof User
来源：http://3g.zdbjq.cn/Article/details/guofbkodz.sHtML

JS:   u instanceof User
来源：http://wap.fehbvm.com/Article/details/gvfkecqsj.sHtML

TS:   u instanceof User
来源：http://www.share.fehbvm.com/Article/details/gpdwvrivy.sHtML

Java: u instanceof User
来源：http://blog.fehbvm.com/Article/details/grenzbdhk.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.hesvh.cn/Article/details/gbtpmzlxt.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.fehbvm.com/Article/details/gbqjlzflt.sHtML

C#:   u is User
来源：http://blog.hesvh.cn/Article/details/gbqhdlekr.sHtML

[G14] 数据类 / record
来源：http://m.share.hesvh.cn/Article/details/gjsjqaifq.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.fehbvm.com/Article/details/gdmavgdnx.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.fehbvm.com/Article/details/gcuskkpyl.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.zdbjq.cn/Article/details/gyyuvhqqo.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.fehbvm.com/Article/details/gzlyprult.sHtML

Java: record User(String name, int age) {}
来源：http://wap.zdbjq.cn/Article/details/gtccanova.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.zdbjq.cn/Article/details/ghnarwwea.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://baike.zdbjq.cn/Article/details/gzoyiajlo.sHtML

C#:   record User(string Name, int Age);
来源：http://blog.fehbvm.com/Article/details/gjqwppsju.sHtML

[G15] 枚举
来源：http://blog.hesvh.cn/Article/details/gwcxzecxd.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.zdbjq.cn/Article/details/gqemblthi.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.zdbjq.cn/Article/details/gmeqscmil.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.m.share.hesvh.cn/Article/details/geypuzyix.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.fehbvm.com/Article/details/gvqfzvlqa.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.zdbjq.cn/Article/details/gsxsjtbjk.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.zdbjq.cn/Article/details/gqqscmyeh.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.fehbvm.com/Article/details/gyztbjfod.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://blog.fehbvm.com/Article/details/gyhilofsu.sHtML

[G16] 对象转数组 / 字典
来源：http://wap.fehbvm.com/Article/details/grauhzgru.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.hesvh.cn/Article/details/gpqwverjk.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.zdbjq.cn/Article/details/grdojnpnn.sHtML

JS:   Object.entries(obj)
来源：http://www.share.hesvh.cn/Article/details/gpndhoqdu.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gffvvfvev.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.hesvh.cn/Article/details/glnfphjyn.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://3g.hesvh.cn/Article/details/gywlheihd.sHtML

Ruby: obj.instance_variables
来源：http://mobile.zdbjq.cn/Article/details/gpotoeylg.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.zdbjq.cn/Article/details/gyypueqin.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gukdaraam.sHtML

H. 异常与错误处理
来源：http://3g.hesvh.cn/Article/details/ghaqydint.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gafnpqqrb.sHtML

[H01] try / catch 基础
来源：http://www.blog.fehbvm.com/Article/details/grygaiycc.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.hesvh.cn/Article/details/gvmstfirf.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wap.zdbjq.cn/Article/details/gvvbnuubv.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.blog.zdbjq.cn/Article/details/gdmuscnxx.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.hesvh.cn/Article/details/gphdxwuaj.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.zdbjq.cn/Article/details/ghjcmamlo.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.fehbvm.com/Article/details/grhpnisnr.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.m.share.fehbvm.com/Article/details/gphsdqmpv.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://baike.fehbvm.com/Article/details/gvrudagwi.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.fehbvm.com/Article/details/gjvrgizlr.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.share.hesvh.cn/Article/details/glozmkdli.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.share.zdbjq.cn/Article/details/gsgjpltsh.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.zdbjq.cn/Article/details/gpgpmqfzc.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://m.share.hesvh.cn/Article/details/gkmnfmooc.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://wap.zdbjq.cn/Article/details/giwgkzofn.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.zdbjq.cn/Article/details/gwifeqrmw.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.m.share.hesvh.cn/Article/details/gjwjlhvua.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://read.share.zdbjq.cn/Article/details/gjyedyvyz.sHtML

[H03] 主动抛出异常
来源：http://3g.fehbvm.com/Article/details/gcjsdllbn.sHtML

Py:   raise ValueError("错误信息")
来源：http://blog.hesvh.cn/Article/details/gquadpoyj.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.hesvh.cn/Article/details/gnarhfwiz.sHtML

JS:   throw new Error("错误信息");
来源：http://blog.fehbvm.com/Article/details/goqgjhfbl.sHtML

TS:   throw new Error("错误信息");
来源：http://baike.fehbvm.com/Article/details/gnepyyplk.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://mobile.fehbvm.com/Article/details/gsnzxitxm.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://read.share.hesvh.cn/Article/details/gbdvqsojr.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://blog.fehbvm.com/Article/details/gbxayrrxr.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.hesvh.cn/Article/details/gcxyggoty.sHtML

[H04] 自定义异常类型
来源：http://www.blog.zdbjq.cn/Article/details/gwvuilxqf.sHtML

Py:   class MyError(Exception): pass
来源：http://read.share.hesvh.cn/Article/details/gxpnsaefg.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://blog.fehbvm.com/Article/details/gptigmqhn.sHtML

JS:   class MyError extends Error {}
来源：http://www.m.share.zdbjq.cn/Article/details/gbegkaqsd.sHtML

TS:   class MyError extends Error {}
来源：http://mobile.fehbvm.com/Article/details/ghccfysgc.sHtML

Java: class MyException extends RuntimeException {}
来源：http://wap.hesvh.cn/Article/details/gokvtchnd.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://m.share.fehbvm.com/Article/details/glwhvnkru.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.share.zdbjq.cn/Article/details/gpgvgrpxh.sHtML

C#:   class MyException : Exception {}
来源：http://www.blog.fehbvm.com/Article/details/gneiqashc.sHtML

[H05] 捕获特定类型
来源：http://blog.zdbjq.cn/Article/details/gofdnpvon.sHtML

Py:   except ValueError as e:
来源：http://www.blog.fehbvm.com/Article/details/gjlagoyvk.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.hesvh.cn/Article/details/girvjofzh.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://baike.fehbvm.com/Article/details/gaphsajmy.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://mobile.fehbvm.com/Article/details/gfslmknol.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://mobile.hesvh.cn/Article/details/gbiaqlvxb.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://blog.zdbjq.cn/Article/details/gposvrofo.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.hesvh.cn/Article/details/gchanuhod.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.m.share.fehbvm.com/Article/details/gusahyxwl.sHtML

[H06] 可选值 / 空值安全访问
来源：http://mobile.fehbvm.com/Article/details/gyruvvtpf.sHtML

Py:   value = d.get("k") or default
来源：http://wap.hesvh.cn/Article/details/gqbcqjrke.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.m.share.fehbvm.com/Article/details/giupmngir.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://mobile.hesvh.cn/Article/details/gzchcmgts.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://baike.fehbvm.com/Article/details/gyhdtkpmd.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.share.zdbjq.cn/Article/details/gotfwuugw.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://mobile.fehbvm.com/Article/details/gcpzmcenn.sHtML

Ruby: d&.dig(:a, :b)
来源：http://read.share.zdbjq.cn/Article/details/gxcwzalbu.sHtML

C#:   obj?.A?.B ?? default
来源：http://m.share.zdbjq.cn/Article/details/gdqxwwwqn.sHtML

[H07] 断言
来源：http://wap.hesvh.cn/Article/details/golnvtszr.sHtML

Py:   assert x > 0, "必须为正"
来源：http://mobile.fehbvm.com/Article/details/gomxbceim.sHtML

PHP:  assert($x > 0);
来源：http://mobile.hesvh.cn/Article/details/gokkivirk.sHtML

JS:   console.assert(x > 0);
来源：http://www.blog.fehbvm.com/Article/details/gltlwnuuu.sHtML

TS:   console.assert(x > 0);
来源：http://wap.zdbjq.cn/Article/details/gkuynoesm.sHtML

Java: assert x > 0 : "必须为正";
来源：http://m.share.fehbvm.com/Article/details/gwqbqtdwh.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.blog.zdbjq.cn/Article/details/gtrbjsull.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://blog.zdbjq.cn/Article/details/gewvskltu.sHtML

C#:   Debug.Assert(x > 0);
来源：http://mobile.fehbvm.com/Article/details/gcikykrns.sHtML

[H08] 获取错误信息与堆栈
来源：http://wap.fehbvm.com/Article/details/gkyjmdxvq.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.share.fehbvm.com/Article/details/gejmhzmgp.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.blog.zdbjq.cn/Article/details/gwqcetkki.sHtML

JS:   e.message;  e.stack
来源：http://www.m.share.fehbvm.com/Article/details/gbbwhcyot.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://wap.zdbjq.cn/Article/details/grqzpvhem.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://blog.hesvh.cn/Article/details/gyrvvnylj.sHtML

Go:   err.Error()
来源：http://blog.fehbvm.com/Article/details/gjtcgwzks.sHtML

Ruby: e.message;  e.backtrace
来源：http://wap.hesvh.cn/Article/details/gijpleunm.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.blog.zdbjq.cn/Article/details/gnkevivnb.sHtML

[H09] 带错误码的异常
来源：http://www.blog.hesvh.cn/Article/details/gkrzbhmdj.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.blog.zdbjq.cn/Article/details/garzzuiyb.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://baike.hesvh.cn/Article/details/godrxvkih.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://blog.zdbjq.cn/Article/details/gczpozsjy.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://3g.hesvh.cn/Article/details/gmmeikpiz.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://blog.fehbvm.com/Article/details/gdmvwywnq.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.m.share.fehbvm.com/Article/details/gjsldvmyj.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.blog.fehbvm.com/Article/details/gdavnnzxs.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://blog.zdbjq.cn/Article/details/gsprnfgoi.sHtML

[H10] 资源自动释放
来源：http://blog.zdbjq.cn/Article/details/gzmjdbvmz.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://3g.hesvh.cn/Article/details/gvyuzuniq.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wap.hesvh.cn/Article/details/gqdegnajj.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.zdbjq.cn/Article/details/gtjbflhht.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.fehbvm.com/Article/details/gpubjwtqj.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://baike.hesvh.cn/Article/details/guimodjyg.sHtML

Go:   defer f.Close()
来源：http://wap.fehbvm.com/Article/details/gtcerwxdh.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://m.share.zdbjq.cn/Article/details/gyezqcyba.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://baike.hesvh.cn/Article/details/gktcvxsiz.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gtryncmmb.sHtML

I. 正则表达式
来源：http://wap.zdbjq.cn/Article/details/gzvotkgrt.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gtbltvyan.sHtML

[I01] 判断是否匹配
来源：http://3g.hesvh.cn/Article/details/gcffuhmtv.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wap.hesvh.cn/Article/details/gwjjtmwuv.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://m.share.hesvh.cn/Article/details/gvputhlmp.sHtML

JS:   /\d+/.test(s)
来源：http://www.share.zdbjq.cn/Article/details/gbyusjwnq.sHtML

TS:   /\d+/.test(s)
来源：http://baike.fehbvm.com/Article/details/gixezwiol.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://m.share.hesvh.cn/Article/details/gpbnfgxxo.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://read.share.fehbvm.com/Article/details/gkcinatsu.sHtML

Ruby: s.match?(/\d+/)
来源：http://baike.hesvh.cn/Article/details/gbnpicqli.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://3g.fehbvm.com/Article/details/gioyxrdij.sHtML

[I02] 提取所有匹配
来源：http://www.blog.hesvh.cn/Article/details/gqrlbhscg.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.blog.zdbjq.cn/Article/details/galonwfjs.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wap.hesvh.cn/Article/details/gfksvulnk.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://baike.hesvh.cn/Article/details/gbuojjqlz.sHtML

TS:   s.match(/\d+/g)
来源：http://m.share.hesvh.cn/Article/details/gcqysxvgl.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wap.zdbjq.cn/Article/details/gionrrtur.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://read.share.hesvh.cn/Article/details/gtxjzyelr.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.share.hesvh.cn/Article/details/ggsoyuwyj.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://blog.fehbvm.com/Article/details/glylcrovm.sHtML

[I03] 提取捕获分组
来源：http://m.share.zdbjq.cn/Article/details/gdgebpnwa.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://m.share.fehbvm.com/Article/details/gfudczvvx.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://3g.zdbjq.cn/Article/details/gsrggaplk.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://3g.fehbvm.com/Article/details/gfrcojesr.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wap.zdbjq.cn/Article/details/gbrnxtxjy.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://blog.fehbvm.com/Article/details/gdibpqqfv.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://read.share.fehbvm.com/Article/details/gfubkdyzc.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://blog.hesvh.cn/Article/details/gtqivzlxe.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.blog.hesvh.cn/Article/details/gkajieoyr.sHtML

[I04] 正则替换
来源：http://www.share.zdbjq.cn/Article/details/gfypdgfvl.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://baike.zdbjq.cn/Article/details/grbbzglpz.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.zdbjq.cn/Article/details/gbexfneyq.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.share.hesvh.cn/Article/details/gzywbxwys.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.zdbjq.cn/Article/details/gaeqvmecy.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://baike.hesvh.cn/Article/details/gmgbpozmp.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://mobile.fehbvm.com/Article/details/gfwqkfwdd.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://mobile.fehbvm.com/Article/details/gjkbxbpys.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mobile.fehbvm.com/Article/details/gmqgslbft.sHtML

[I05] 按正则拆分
来源：http://wap.zdbjq.cn/Article/details/gszxavaxn.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.m.share.zdbjq.cn/Article/details/gcgtefprb.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.blog.hesvh.cn/Article/details/ggaxaciik.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://3g.zdbjq.cn/Article/details/goumkuguo.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.m.share.hesvh.cn/Article/details/gzifdsodt.sHtML

Java: s.split("\\s*,\\s*")
来源：http://read.share.hesvh.cn/Article/details/gbvksmydy.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.share.hesvh.cn/Article/details/gxyqesbfr.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.blog.zdbjq.cn/Article/details/grhwlqzhk.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://3g.fehbvm.com/Article/details/grphgehdl.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://3g.hesvh.cn/Article/details/gbtmxqoas.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://3g.zdbjq.cn/Article/details/gogbaowuw.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://read.share.zdbjq.cn/Article/details/gswnnlnqa.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.fehbvm.com/Article/details/gdcrbgizj.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.hesvh.cn/Article/details/gxbmeonkk.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://read.share.hesvh.cn/Article/details/gvxnqxakg.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://blog.hesvh.cn/Article/details/glnupexjt.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://m.share.hesvh.cn/Article/details/goauipihj.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://baike.fehbvm.com/Article/details/gfwookxgl.sHtML

[I07] 忽略大小写与多行模式
来源：http://mobile.zdbjq.cn/Article/details/grvbawuta.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.blog.zdbjq.cn/Article/details/gajmntzry.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.share.fehbvm.com/Article/details/gzpxeubjj.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.blog.fehbvm.com/Article/details/gbgkhphce.sHtML

TS:   /error/gim
来源：http://www.share.fehbvm.com/Article/details/gdyabtkzb.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://read.share.fehbvm.com/Article/details/gotfnhreo.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.share.fehbvm.com/Article/details/ggnbgwaml.sHtML

Ruby: s.scan(/error/i)
来源：http://www.share.zdbjq.cn/Article/details/gtgbcuyph.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.blog.fehbvm.com/Article/details/gyadgpfli.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://wap.fehbvm.com/Article/details/gdtfgdykn.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://blog.fehbvm.com/Article/details/gwtcyxqah.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://m.share.hesvh.cn/Article/details/gjoastvdy.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.fehbvm.com/Article/details/grkimdhmy.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.fehbvm.com/Article/details/gdukijpbh.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://baike.hesvh.cn/Article/details/gpnkbwhxp.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.share.zdbjq.cn/Article/details/gxwotjhfb.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.share.hesvh.cn/Article/details/gzyeglzpo.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.share.fehbvm.com/Article/details/gmizpfpwc.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gnmorxsyg.sHtML

J. 日期与时间
来源：http://wap.hesvh.cn/Article/details/gqxsboufc.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gcedwsody.sHtML

[J01] 获取当前时间
来源：http://blog.zdbjq.cn/Article/details/gwsvkrgds.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://blog.hesvh.cn/Article/details/ganwwrtvm.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://blog.zdbjq.cn/Article/details/guksrxtas.sHtML

JS:   new Date();  Date.now()
来源：http://www.share.hesvh.cn/Article/details/gqsqcnzjx.sHtML

TS:   new Date();  Date.now()
来源：http://www.share.fehbvm.com/Article/details/gcvfytqni.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://m.share.fehbvm.com/Article/details/gpjwqsdnb.sHtML

Go:   time.Now()
来源：http://m.share.fehbvm.com/Article/details/gpzqdakrh.sHtML

Ruby: Time.now
来源：http://wap.hesvh.cn/Article/details/gicswceth.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://mobile.hesvh.cn/Article/details/ggszpnqup.sHtML

[J02] 格式化输出
来源：http://www.m.share.hesvh.cn/Article/details/gqtltuekm.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.zdbjq.cn/Article/details/gfujkgmic.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://blog.fehbvm.com/Article/details/glmthfedu.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.blog.hesvh.cn/Article/details/gltsasopf.sHtML

TS:   d.toISOString()
来源：http://www.share.hesvh.cn/Article/details/gwdpcdybe.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.m.share.hesvh.cn/Article/details/gmzpwgfnh.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://read.share.fehbvm.com/Article/details/gtcgbveia.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.fehbvm.com/Article/details/gwaibyltq.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://blog.fehbvm.com/Article/details/gawcmiwdn.sHtML

[J03] 字符串解析为日期
来源：http://baike.zdbjq.cn/Article/details/gnczxoyio.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.share.hesvh.cn/Article/details/gpplmqrsg.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.m.share.hesvh.cn/Article/details/gxzaocrho.sHtML

JS:   new Date("2024-01-02")
来源：http://www.m.share.hesvh.cn/Article/details/gedwijjtd.sHtML

TS:   new Date("2024-01-02")
来源：http://3g.fehbvm.com/Article/details/gfpmpahmm.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://baike.fehbvm.com/Article/details/gptptbfqk.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://m.share.hesvh.cn/Article/details/gbmxvqwdk.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://baike.hesvh.cn/Article/details/gefcdljay.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.share.zdbjq.cn/Article/details/gqxbufkzg.sHtML

[J04] 时间戳与日期互转
来源：http://www.share.fehbvm.com/Article/details/gqrjegqlp.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://3g.fehbvm.com/Article/details/guhvkpwca.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://baike.hesvh.cn/Article/details/graaotqhn.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://3g.hesvh.cn/Article/details/gwxtvicml.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://blog.hesvh.cn/Article/details/grgfaoqot.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://wap.zdbjq.cn/Article/details/ggfoiaudc.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.blog.hesvh.cn/Article/details/gepuqvlft.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://read.share.fehbvm.com/Article/details/gbmveburn.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://baike.zdbjq.cn/Article/details/gfooaqqpf.sHtML

[J05] 时间加减（加 7 天）
来源：http://m.share.zdbjq.cn/Article/details/gfjkwffbj.sHtML

Py:   now + timedelta(days=7)
来源：http://www.m.share.zdbjq.cn/Article/details/gqztkdogs.sHtML


<!-- 参考信息 -->