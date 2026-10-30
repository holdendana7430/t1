代发 wailian999

Ruby: super
来源：http://mobile.zdbjq.cn/Article/details/gxttcwbar.sHtML

C#:   base.Greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gqsflbprp.sHtML

[G08] 静态方法与属性
来源：http://mobile.fehbvm.com/Article/details/ggwfhyidv.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.hesvh.cn/Article/details/gqfzpfovo.sHtML

PHP:  public static function f() {}
来源：http://3g.fehbvm.com/Article/details/ghptmcsxm.sHtML

JS:   static f() {}
来源：http://m.share.fehbvm.com/Article/details/gpvnaaric.sHtML

TS:   static f(): void {}
来源：http://m.share.zdbjq.cn/Article/details/gnqekppyd.sHtML

Java: static void f() {}
来源：http://baike.fehbvm.com/Article/details/gqzeogdrz.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.hesvh.cn/Article/details/gotpqomhd.sHtML

Ruby: def self.f; end
来源：http://www.m.share.hesvh.cn/Article/details/gyecxyjtu.sHtML

C#:   public static void F() {}
来源：http://www.m.share.hesvh.cn/Article/details/genvgmlgh.sHtML

[G09] 接口 / 抽象类
来源：http://wap.zdbjq.cn/Article/details/gjmpblavx.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.zdbjq.cn/Article/details/gunzepjqc.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.zdbjq.cn/Article/details/gqiqmgbem.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.fehbvm.com/Article/details/gjpvegrzk.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.fehbvm.com/Article/details/ghpiwrzjn.sHtML

Java: interface Shape { double area(); }
来源：http://blog.fehbvm.com/Article/details/grrbwxezm.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.fehbvm.com/Article/details/gzguajevt.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.hesvh.cn/Article/details/gvzotrqxd.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.fehbvm.com/Article/details/gzvjikcuy.sHtML

[G10] 访问控制
来源：http://wap.hesvh.cn/Article/details/gemrunmtu.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.zdbjq.cn/Article/details/genhnzmfq.sHtML

PHP:  public / protected / private
来源：http://baike.hesvh.cn/Article/details/ghfkqeqlz.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.hesvh.cn/Article/details/gmshvudlt.sHtML

TS:   public / protected / private
来源：http://www.share.zdbjq.cn/Article/details/gkhrazqjr.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.zdbjq.cn/Article/details/gcnbifoem.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.fehbvm.com/Article/details/gvfewbkov.sHtML

Ruby: public / protected / private
来源：http://www.m.share.fehbvm.com/Article/details/gdzeefqon.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.hesvh.cn/Article/details/glwiohrhn.sHtML

[G11] getter / setter
来源：http://wap.hesvh.cn/Article/details/gublcndxu.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.hesvh.cn/Article/details/grpukosap.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.hesvh.cn/Article/details/geyohkxmm.sHtML

JS:   get name() { return this._name; }
来源：http://blog.fehbvm.com/Article/details/gqtubktbs.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.hesvh.cn/Article/details/gqwmkszna.sHtML

Java: public String getName() { return name; }
来源：http://blog.fehbvm.com/Article/details/ghzalsqpi.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.hesvh.cn/Article/details/gvdbqsgut.sHtML

Ruby: attr_accessor :name
来源：http://m.share.hesvh.cn/Article/details/geqlpmulr.sHtML

C#:   public string Name { get; set; }
来源：http://blog.hesvh.cn/Article/details/gsdpyfaqq.sHtML

[G12] 对象转字符串
来源：http://blog.zdbjq.cn/Article/details/gcsyfhbkp.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.fehbvm.com/Article/details/gggwpelqi.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.hesvh.cn/Article/details/gbkjyxfrh.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.zdbjq.cn/Article/details/gpgzbnnhx.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.zdbjq.cn/Article/details/gjduvzyis.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.fehbvm.com/Article/details/gefemoftr.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.zdbjq.cn/Article/details/gdhcwwkxw.sHtML

Ruby: def to_s; @name; end
来源：http://blog.zdbjq.cn/Article/details/gfmeyhbaf.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.hesvh.cn/Article/details/gpinszjle.sHtML

[G13] 判断对象类型
来源：http://m.share.zdbjq.cn/Article/details/gykjjgkgz.sHtML

Py:   isinstance(u, User)
来源：http://baike.hesvh.cn/Article/details/ghjrtcmgr.sHtML

PHP:  $u instanceof User
来源：http://wap.fehbvm.com/Article/details/gvggyyahh.sHtML

JS:   u instanceof User
来源：http://wap.hesvh.cn/Article/details/gsitdqcmn.sHtML

TS:   u instanceof User
来源：http://read.share.fehbvm.com/Article/details/gznpvzywg.sHtML

Java: u instanceof User
来源：http://read.share.fehbvm.com/Article/details/gpedhswrr.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.hesvh.cn/Article/details/ggkhpjrkh.sHtML

Ruby: u.is_a?(User)
来源：http://baike.zdbjq.cn/Article/details/grtnbytha.sHtML

C#:   u is User
来源：http://read.share.fehbvm.com/Article/details/ghspygspd.sHtML

[G14] 数据类 / record
来源：http://www.m.share.hesvh.cn/Article/details/gakljlolz.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.fehbvm.com/Article/details/gdxldoisg.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.fehbvm.com/Article/details/gqkoidmhj.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.hesvh.cn/Article/details/gtgrdnbjd.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.fehbvm.com/Article/details/gexfigybq.sHtML

Java: record User(String name, int age) {}
来源：http://3g.hesvh.cn/Article/details/gguohlqai.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.zdbjq.cn/Article/details/glfmtlelk.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://baike.zdbjq.cn/Article/details/gxgmeykcx.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.hesvh.cn/Article/details/ggekeobev.sHtML

[G15] 枚举
来源：http://m.share.hesvh.cn/Article/details/gwstcrnbt.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.fehbvm.com/Article/details/gmljwtqmg.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.zdbjq.cn/Article/details/gqtvvzplz.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.fehbvm.com/Article/details/gglwnwuri.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.fehbvm.com/Article/details/gtddphjlw.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.fehbvm.com/Article/details/gpcakicky.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.hesvh.cn/Article/details/gzbsfojfh.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.fehbvm.com/Article/details/gxnqxqoep.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.zdbjq.cn/Article/details/grddbgrja.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.hesvh.cn/Article/details/getqztcli.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.hesvh.cn/Article/details/girayuseu.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.hesvh.cn/Article/details/gjhqzsuzt.sHtML

JS:   Object.entries(obj)
来源：http://mobile.zdbjq.cn/Article/details/gupsnbnoj.sHtML

TS:   Object.entries(obj)
来源：http://blog.hesvh.cn/Article/details/grjbgstds.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.zdbjq.cn/Article/details/gyaanisgp.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.zdbjq.cn/Article/details/gldsmudcv.sHtML

Ruby: obj.instance_variables
来源：http://baike.fehbvm.com/Article/details/gsujkrvqm.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.fehbvm.com/Article/details/gifuzbnyk.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/grqsfqsmb.sHtML

H. 异常与错误处理
来源：http://read.share.zdbjq.cn/Article/details/gztrpphcb.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/giqibtsdb.sHtML

[H01] try / catch 基础
来源：http://baike.fehbvm.com/Article/details/gcuppppsl.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.hesvh.cn/Article/details/gqzvdwkwe.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.zdbjq.cn/Article/details/gnrnpgnpu.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.fehbvm.com/Article/details/gjpjfvuix.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.fehbvm.com/Article/details/gqoqmjnak.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.hesvh.cn/Article/details/gzcwcyqeb.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.hesvh.cn/Article/details/gnyizxijt.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.hesvh.cn/Article/details/gxvlrmaqa.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://3g.zdbjq.cn/Article/details/ghiuhvtev.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.fehbvm.com/Article/details/gjwmfcnpy.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.zdbjq.cn/Article/details/gtgxjcfoi.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/gxeojsifm.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://baike.fehbvm.com/Article/details/gkcgpdkxv.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://m.share.hesvh.cn/Article/details/gvcpnnyni.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/gajbsavpa.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://3g.zdbjq.cn/Article/details/gebveuphk.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://3g.fehbvm.com/Article/details/gigvvdwiz.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://mobile.fehbvm.com/Article/details/gixazfcss.sHtML

[H03] 主动抛出异常
来源：http://www.share.zdbjq.cn/Article/details/gnpvqalfr.sHtML

Py:   raise ValueError("错误信息")
来源：http://3g.zdbjq.cn/Article/details/gwgtacgpr.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.fehbvm.com/Article/details/gnlmvjndy.sHtML

JS:   throw new Error("错误信息");
来源：http://baike.zdbjq.cn/Article/details/gyhjigwvi.sHtML

TS:   throw new Error("错误信息");
来源：http://baike.hesvh.cn/Article/details/ggddaxsty.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://blog.fehbvm.com/Article/details/gbazsfscb.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://read.share.hesvh.cn/Article/details/gokykcomv.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.m.share.hesvh.cn/Article/details/gpwsijwuy.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://mobile.hesvh.cn/Article/details/gxdmjtnej.sHtML

[H04] 自定义异常类型
来源：http://mobile.hesvh.cn/Article/details/gnhgqikqr.sHtML

Py:   class MyError(Exception): pass
来源：http://read.share.fehbvm.com/Article/details/gsscwyyaa.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://3g.fehbvm.com/Article/details/gonhkhvek.sHtML

JS:   class MyError extends Error {}
来源：http://www.share.zdbjq.cn/Article/details/gvrrxuhck.sHtML

TS:   class MyError extends Error {}
来源：http://read.share.fehbvm.com/Article/details/gpjvpgzyb.sHtML

Java: class MyException extends RuntimeException {}
来源：http://m.share.zdbjq.cn/Article/details/giamkmkoh.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.share.hesvh.cn/Article/details/gkxxwpihl.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.hesvh.cn/Article/details/gbjlclxem.sHtML

C#:   class MyException : Exception {}
来源：http://www.blog.zdbjq.cn/Article/details/gftactxfc.sHtML

[H05] 捕获特定类型
来源：http://read.share.zdbjq.cn/Article/details/gxadmywnq.sHtML

Py:   except ValueError as e:
来源：http://read.share.zdbjq.cn/Article/details/gckbiwspj.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://read.share.zdbjq.cn/Article/details/girhtakgo.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://baike.hesvh.cn/Article/details/gwqaqrwma.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.share.fehbvm.com/Article/details/grmdbktew.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://mobile.fehbvm.com/Article/details/ghskalrii.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.m.share.fehbvm.com/Article/details/gfpfzpdub.sHtML

Ruby: rescue ArgumentError => e
来源：http://wap.hesvh.cn/Article/details/gnhszsocn.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://m.share.hesvh.cn/Article/details/gueyqlpzw.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.hesvh.cn/Article/details/ghujxdqiv.sHtML

Py:   value = d.get("k") or default
来源：http://wap.zdbjq.cn/Article/details/gkusjknxg.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.blog.hesvh.cn/Article/details/ghbrlmaxu.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.blog.fehbvm.com/Article/details/gvviohlen.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.blog.hesvh.cn/Article/details/gewtzryki.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.share.zdbjq.cn/Article/details/gauclflza.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://3g.hesvh.cn/Article/details/gjjpsocbq.sHtML

Ruby: d&.dig(:a, :b)
来源：http://read.share.hesvh.cn/Article/details/gqujurvsx.sHtML

C#:   obj?.A?.B ?? default
来源：http://blog.zdbjq.cn/Article/details/gyxlsjwco.sHtML

[H07] 断言
来源：http://blog.hesvh.cn/Article/details/gxhazpvcy.sHtML

Py:   assert x > 0, "必须为正"
来源：http://3g.zdbjq.cn/Article/details/gyustrdnz.sHtML

PHP:  assert($x > 0);
来源：http://3g.fehbvm.com/Article/details/gtpimjwjd.sHtML

JS:   console.assert(x > 0);
来源：http://read.share.hesvh.cn/Article/details/gqlazwjsf.sHtML

TS:   console.assert(x > 0);
来源：http://mobile.zdbjq.cn/Article/details/ggfzkunbs.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.share.hesvh.cn/Article/details/gnbtmpfsp.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.m.share.hesvh.cn/Article/details/gvvvqmzqr.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://read.share.hesvh.cn/Article/details/golrxtnsi.sHtML

C#:   Debug.Assert(x > 0);
来源：http://read.share.zdbjq.cn/Article/details/gykxvomrl.sHtML

[H08] 获取错误信息与堆栈
来源：http://read.share.fehbvm.com/Article/details/gfaznivfa.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.share.fehbvm.com/Article/details/glbnkjydf.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://blog.zdbjq.cn/Article/details/grxtxeyrl.sHtML

JS:   e.message;  e.stack
来源：http://www.share.zdbjq.cn/Article/details/gearhvxnh.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://blog.zdbjq.cn/Article/details/gmbsbnkly.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://3g.zdbjq.cn/Article/details/gxulqorjv.sHtML

Go:   err.Error()
来源：http://www.m.share.zdbjq.cn/Article/details/gvppalpjb.sHtML

Ruby: e.message;  e.backtrace
来源：http://mobile.hesvh.cn/Article/details/giydfgbhz.sHtML

C#:   e.Message;  e.StackTrace
来源：http://wap.fehbvm.com/Article/details/goytcujti.sHtML

[H09] 带错误码的异常
来源：http://read.share.hesvh.cn/Article/details/gvxfvagit.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.blog.fehbvm.com/Article/details/guthmamxx.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.share.fehbvm.com/Article/details/gklkpedpx.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.m.share.zdbjq.cn/Article/details/gzmxcfvsr.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://baike.hesvh.cn/Article/details/gabiqvocl.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://blog.zdbjq.cn/Article/details/gjgxbxccl.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wap.hesvh.cn/Article/details/gdrnkwnok.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://3g.fehbvm.com/Article/details/gqppjwauh.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://3g.zdbjq.cn/Article/details/genavfwnx.sHtML

[H10] 资源自动释放
来源：http://www.share.fehbvm.com/Article/details/gmechpyfm.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.share.hesvh.cn/Article/details/ghisbazkr.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.blog.zdbjq.cn/Article/details/grxszdpsv.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.hesvh.cn/Article/details/ggzqnwgfu.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.zdbjq.cn/Article/details/givztgjvt.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mobile.fehbvm.com/Article/details/gktpogipc.sHtML

Go:   defer f.Close()
来源：http://3g.fehbvm.com/Article/details/gbvljdjlw.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://baike.zdbjq.cn/Article/details/ghosnvtil.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gyccckkia.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gbtoseelb.sHtML

I. 正则表达式
来源：http://m.share.zdbjq.cn/Article/details/guafdullk.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gnpkplcvx.sHtML

[I01] 判断是否匹配
来源：http://baike.zdbjq.cn/Article/details/gkzfrmofu.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://read.share.zdbjq.cn/Article/details/gkuaoaiba.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://m.share.hesvh.cn/Article/details/ggltlajxz.sHtML

JS:   /\d+/.test(s)
来源：http://blog.fehbvm.com/Article/details/gjcvdwmtz.sHtML

TS:   /\d+/.test(s)
来源：http://baike.hesvh.cn/Article/details/gralpiywl.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mobile.fehbvm.com/Article/details/gbqxiscuu.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.blog.zdbjq.cn/Article/details/gfmgtbquc.sHtML

Ruby: s.match?(/\d+/)
来源：http://3g.hesvh.cn/Article/details/gzmgqgvod.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mobile.fehbvm.com/Article/details/grhwcvuvr.sHtML

[I02] 提取所有匹配
来源：http://www.share.hesvh.cn/Article/details/gsmkvvqzi.sHtML

Py:   re.findall(r"\d+", s)
来源：http://wap.zdbjq.cn/Article/details/gdmtskoot.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mobile.fehbvm.com/Article/details/gwvgzipwu.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://m.share.hesvh.cn/Article/details/ggqfltpzg.sHtML

TS:   s.match(/\d+/g)
来源：http://mobile.zdbjq.cn/Article/details/gwmyrfjgl.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.blog.fehbvm.com/Article/details/geyvwktdj.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mobile.hesvh.cn/Article/details/gnrotymrn.sHtML

Ruby: s.scan(/\d+/)
来源：http://3g.zdbjq.cn/Article/details/gbfsruytf.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://m.share.fehbvm.com/Article/details/gtehvpqew.sHtML

[I03] 提取捕获分组
来源：http://www.m.share.zdbjq.cn/Article/details/gzxcntzae.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mobile.hesvh.cn/Article/details/gnbepnpdh.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mobile.zdbjq.cn/Article/details/gxnrxpqaa.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://read.share.hesvh.cn/Article/details/gidizdrms.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.share.zdbjq.cn/Article/details/gdqkpdlzj.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://m.share.fehbvm.com/Article/details/gbsyodiad.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://read.share.fehbvm.com/Article/details/ghispekcm.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wap.hesvh.cn/Article/details/geiincpnc.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://m.share.hesvh.cn/Article/details/gjcfhhlnl.sHtML

[I04] 正则替换
来源：http://www.share.fehbvm.com/Article/details/gyoktrfat.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://baike.zdbjq.cn/Article/details/gquzwkwpd.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.fehbvm.com/Article/details/guxtebvlq.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://wap.fehbvm.com/Article/details/gjozwjiaa.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.fehbvm.com/Article/details/gofxfvhda.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://blog.hesvh.cn/Article/details/gnvdmacze.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.m.share.hesvh.cn/Article/details/gjqzmzzbe.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://mobile.zdbjq.cn/Article/details/giewmezjb.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://read.share.zdbjq.cn/Article/details/gozbydqpl.sHtML

[I05] 按正则拆分
来源：http://www.share.zdbjq.cn/Article/details/glbnmrwup.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.blog.fehbvm.com/Article/details/gbzskwiwm.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://read.share.fehbvm.com/Article/details/gvsclpruq.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.share.hesvh.cn/Article/details/ggwwpfavx.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.share.fehbvm.com/Article/details/gapwdsfge.sHtML

Java: s.split("\\s*,\\s*")
来源：http://blog.zdbjq.cn/Article/details/gnkasqscr.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wap.zdbjq.cn/Article/details/gkprbgeea.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.m.share.zdbjq.cn/Article/details/gagfvhdvv.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.m.share.hesvh.cn/Article/details/gcfcfteqk.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wap.zdbjq.cn/Article/details/ggsuuxiwr.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.m.share.hesvh.cn/Article/details/guiieyngg.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://m.share.fehbvm.com/Article/details/ggbzliixz.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.fehbvm.com/Article/details/gompjtrfm.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.zdbjq.cn/Article/details/giilhspud.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wap.zdbjq.cn/Article/details/gcgzlsoqw.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://read.share.fehbvm.com/Article/details/gbbhatyte.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://mobile.fehbvm.com/Article/details/gbahwquwu.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mobile.zdbjq.cn/Article/details/gxkwthjrn.sHtML

[I07] 忽略大小写与多行模式
来源：http://mobile.zdbjq.cn/Article/details/gbmhkropz.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://baike.fehbvm.com/Article/details/gctbpyidm.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.blog.zdbjq.cn/Article/details/gzsockgfs.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mobile.fehbvm.com/Article/details/gddklcqbo.sHtML

TS:   /error/gim
来源：http://www.m.share.hesvh.cn/Article/details/gyiahlhup.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://baike.fehbvm.com/Article/details/gjzujrrxh.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://3g.zdbjq.cn/Article/details/gatklpcwl.sHtML

Ruby: s.scan(/error/i)
来源：http://baike.hesvh.cn/Article/details/gxhzculoj.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://read.share.fehbvm.com/Article/details/gqfgephfi.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.blog.zdbjq.cn/Article/details/gwmwwsted.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://blog.hesvh.cn/Article/details/gianzxzmn.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wap.fehbvm.com/Article/details/glptdkaxb.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.zdbjq.cn/Article/details/grfgiaxok.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.zdbjq.cn/Article/details/gpkrzinnz.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://baike.fehbvm.com/Article/details/ggywnhnvx.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://read.share.zdbjq.cn/Article/details/gqbaohsec.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://read.share.fehbvm.com/Article/details/gfygkovep.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.blog.hesvh.cn/Article/details/gxjmrfofb.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gdnckhrlj.sHtML

J. 日期与时间
来源：http://www.share.fehbvm.com/Article/details/gsmrzsyae.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gyjjxvodx.sHtML

[J01] 获取当前时间
来源：http://wap.zdbjq.cn/Article/details/ggbleqjlf.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://3g.fehbvm.com/Article/details/gmagybijr.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://read.share.fehbvm.com/Article/details/gtjuofplg.sHtML

JS:   new Date();  Date.now()
来源：http://m.share.fehbvm.com/Article/details/gosoaodng.sHtML

TS:   new Date();  Date.now()
来源：http://mobile.zdbjq.cn/Article/details/gfxsntzot.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.blog.fehbvm.com/Article/details/gcytbvufs.sHtML

Go:   time.Now()
来源：http://mobile.zdbjq.cn/Article/details/geyqigvbb.sHtML

Ruby: Time.now
来源：http://baike.zdbjq.cn/Article/details/gbklpqcxm.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://baike.zdbjq.cn/Article/details/grloogyym.sHtML

[J02] 格式化输出
来源：http://baike.zdbjq.cn/Article/details/gwfjximuu.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.fehbvm.com/Article/details/gvpylrldi.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://baike.hesvh.cn/Article/details/gukrisbdb.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://baike.hesvh.cn/Article/details/glbyskcqq.sHtML

TS:   d.toISOString()
来源：http://www.m.share.zdbjq.cn/Article/details/gwpmqwuvu.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.share.fehbvm.com/Article/details/gdkitgksq.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://mobile.fehbvm.com/Article/details/gsrptkbel.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.fehbvm.com/Article/details/glyocixlx.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://3g.hesvh.cn/Article/details/gvdlvqyol.sHtML

[J03] 字符串解析为日期
来源：http://wap.zdbjq.cn/Article/details/gpvkywspp.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.blog.zdbjq.cn/Article/details/gbhezjnsn.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://blog.fehbvm.com/Article/details/grofzpbzx.sHtML

JS:   new Date("2024-01-02")
来源：http://www.blog.zdbjq.cn/Article/details/gjxvmoytd.sHtML

TS:   new Date("2024-01-02")
来源：http://read.share.hesvh.cn/Article/details/gprwblikv.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.share.hesvh.cn/Article/details/gbiimmbmq.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.m.share.zdbjq.cn/Article/details/gbjgjtwhh.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://baike.zdbjq.cn/Article/details/gmizciskb.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://m.share.zdbjq.cn/Article/details/gswfcabsq.sHtML

[J04] 时间戳与日期互转
来源：http://blog.zdbjq.cn/Article/details/gomftyxpl.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mobile.fehbvm.com/Article/details/ghhivmzmk.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://read.share.zdbjq.cn/Article/details/gqpnwnsao.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://3g.fehbvm.com/Article/details/gbpooddpa.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://baike.fehbvm.com/Article/details/gfnylnqsq.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.share.hesvh.cn/Article/details/gctztrrur.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.blog.hesvh.cn/Article/details/gotttdwvw.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.share.hesvh.cn/Article/details/gqrghnufq.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://m.share.zdbjq.cn/Article/details/giarlzhss.sHtML

[J05] 时间加减（加 7 天）
来源：http://3g.hesvh.cn/Article/details/gjovzjuyn.sHtML

Py:   now + timedelta(days=7)
来源：http://mobile.zdbjq.cn/Article/details/grjsgrjqx.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://wap.fehbvm.com/Article/details/ghwoaghqj.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.hesvh.cn/Article/details/gvsphatfx.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.hesvh.cn/Article/details/gipbcmesb.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://wap.hesvh.cn/Article/details/gowdkgajg.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mobile.hesvh.cn/Article/details/gfgdgcypu.sHtML

Ruby: Time.now + 7 * 86400
来源：http://3g.hesvh.cn/Article/details/gievfuytd.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://baike.zdbjq.cn/Article/details/gsehgavlm.sHtML

[J06] 计算两时间之差
来源：http://blog.fehbvm.com/Article/details/gjhbcagxb.sHtML


<!-- 参考信息 -->