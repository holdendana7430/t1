代发 wailian999

Ruby: super
来源：http://blog.hesvh.cn/Article/details/glvrnoadx.sHtML

C#:   base.Greet();
来源：http://3g.hesvh.cn/Article/details/gfhtfyznu.sHtML

[G08] 静态方法与属性
来源：http://3g.zdbjq.cn/Article/details/gxsnnnytd.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.hesvh.cn/Article/details/gtdkwpvyy.sHtML

PHP:  public static function f() {}
来源：http://wap.hesvh.cn/Article/details/gprzbliid.sHtML

JS:   static f() {}
来源：http://3g.hesvh.cn/Article/details/gikxyvzqk.sHtML

TS:   static f(): void {}
来源：http://mobile.fehbvm.com/Article/details/gughdjrsb.sHtML

Java: static void f() {}
来源：http://www.share.zdbjq.cn/Article/details/gmmycbrnj.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.fehbvm.com/Article/details/gbklymitx.sHtML

Ruby: def self.f; end
来源：http://mobile.zdbjq.cn/Article/details/gogevblii.sHtML

C#:   public static void F() {}
来源：http://baike.fehbvm.com/Article/details/gbjkuklzi.sHtML

[G09] 接口 / 抽象类
来源：http://3g.hesvh.cn/Article/details/gzyfcbyrz.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.zdbjq.cn/Article/details/gpslnrrug.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.zdbjq.cn/Article/details/gmybplocd.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.hesvh.cn/Article/details/grcknbmwy.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.hesvh.cn/Article/details/gxdroxccr.sHtML

Java: interface Shape { double area(); }
来源：http://3g.zdbjq.cn/Article/details/gwnrkvphi.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.fehbvm.com/Article/details/gkcguyizp.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.hesvh.cn/Article/details/gnofdtdjz.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.hesvh.cn/Article/details/guelgaqjg.sHtML

[G10] 访问控制
来源：http://blog.zdbjq.cn/Article/details/grafcragl.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.fehbvm.com/Article/details/glokusehz.sHtML

PHP:  public / protected / private
来源：http://3g.hesvh.cn/Article/details/gsluavyop.sHtML

JS:   #private 字段；其余公开
来源：http://3g.hesvh.cn/Article/details/ghogipgnb.sHtML

TS:   public / protected / private
来源：http://www.m.share.zdbjq.cn/Article/details/ggowekwxp.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.hesvh.cn/Article/details/ghogurjwd.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.hesvh.cn/Article/details/gstfpgfzq.sHtML

Ruby: public / protected / private
来源：http://mobile.zdbjq.cn/Article/details/ggxnbbqrm.sHtML

C#:   public / protected / private / internal
来源：http://wap.zdbjq.cn/Article/details/gktueuppa.sHtML

[G11] getter / setter
来源：http://blog.hesvh.cn/Article/details/gdnuzxsll.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.hesvh.cn/Article/details/ghrydzhxw.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.fehbvm.com/Article/details/ghonlmwpb.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.zdbjq.cn/Article/details/gwabotdnu.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.hesvh.cn/Article/details/gukyesyeb.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/gwrvgllec.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.zdbjq.cn/Article/details/gjyivxmmo.sHtML

Ruby: attr_accessor :name
来源：http://www.share.zdbjq.cn/Article/details/giajasdet.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.zdbjq.cn/Article/details/gzvblirhn.sHtML

[G12] 对象转字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gydcghjwq.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.zdbjq.cn/Article/details/gfvkxfkvi.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.fehbvm.com/Article/details/gzgkqkxby.sHtML

JS:   toString() { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/grylnqtdp.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/gjrohinpt.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.hesvh.cn/Article/details/gfayhrnol.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.zdbjq.cn/Article/details/gwbsvnbvz.sHtML

Ruby: def to_s; @name; end
来源：http://blog.zdbjq.cn/Article/details/gpqdimsjc.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.fehbvm.com/Article/details/gqpqvjoqo.sHtML

[G13] 判断对象类型
来源：http://read.share.zdbjq.cn/Article/details/guvhttagh.sHtML

Py:   isinstance(u, User)
来源：http://read.share.hesvh.cn/Article/details/gvluibpjs.sHtML

PHP:  $u instanceof User
来源：http://blog.zdbjq.cn/Article/details/gxunavydb.sHtML

JS:   u instanceof User
来源：http://www.blog.zdbjq.cn/Article/details/gmletbmeq.sHtML

TS:   u instanceof User
来源：http://www.share.fehbvm.com/Article/details/gyfschizq.sHtML

Java: u instanceof User
来源：http://baike.zdbjq.cn/Article/details/gpmsaijvz.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.fehbvm.com/Article/details/gbjfezxua.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.hesvh.cn/Article/details/gdznnztsf.sHtML

C#:   u is User
来源：http://www.share.fehbvm.com/Article/details/gidzhiyqg.sHtML

[G14] 数据类 / record
来源：http://wap.hesvh.cn/Article/details/gqcxesvoi.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://baike.hesvh.cn/Article/details/gycbwuzhc.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.hesvh.cn/Article/details/gkslxwzwb.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.zdbjq.cn/Article/details/gyrzajema.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.share.zdbjq.cn/Article/details/gsnhdycxw.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.hesvh.cn/Article/details/gjjqwzuos.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.hesvh.cn/Article/details/gjyvkujlx.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.zdbjq.cn/Article/details/gphthswah.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.fehbvm.com/Article/details/gktpqiuck.sHtML

[G15] 枚举
来源：http://www.blog.hesvh.cn/Article/details/gjlpwveyb.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.zdbjq.cn/Article/details/gczeaqukq.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.fehbvm.com/Article/details/gltunapdg.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.m.share.fehbvm.com/Article/details/gueiexjlm.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.hesvh.cn/Article/details/grnkbopyk.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.zdbjq.cn/Article/details/gnjqkwdww.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.hesvh.cn/Article/details/gxzfqmffn.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.fehbvm.com/Article/details/gydzajytd.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.zdbjq.cn/Article/details/gpuksrfit.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.hesvh.cn/Article/details/gwnnictnb.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.zdbjq.cn/Article/details/gktuzkflu.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.zdbjq.cn/Article/details/gulkurwny.sHtML

JS:   Object.entries(obj)
来源：http://wap.fehbvm.com/Article/details/gifhsadik.sHtML

TS:   Object.entries(obj)
来源：http://mobile.fehbvm.com/Article/details/guemxpkar.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.zdbjq.cn/Article/details/ghoapyjql.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.fehbvm.com/Article/details/gumavzufs.sHtML

Ruby: obj.instance_variables
来源：http://mobile.zdbjq.cn/Article/details/gvhunedvb.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.zdbjq.cn/Article/details/gndrpxqjv.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/goyxnacbn.sHtML

H. 异常与错误处理
来源：http://mobile.zdbjq.cn/Article/details/geimnggvi.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gzgsofqts.sHtML

[H01] try / catch 基础
来源：http://www.m.share.hesvh.cn/Article/details/giejsxory.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.fehbvm.com/Article/details/gbawufuuf.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://3g.fehbvm.com/Article/details/gspggqfua.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.zdbjq.cn/Article/details/gmhiyfqsk.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://3g.fehbvm.com/Article/details/gvdfrcoop.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.m.share.fehbvm.com/Article/details/ggqtbuxgh.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://baike.zdbjq.cn/Article/details/gtjwchtug.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.zdbjq.cn/Article/details/gjttldfgt.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://baike.zdbjq.cn/Article/details/goiaiurgt.sHtML

[H02] finally / ensure 收尾
来源：http://www.m.share.hesvh.cn/Article/details/gkdllrwck.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.fehbvm.com/Article/details/gndprztri.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://3g.hesvh.cn/Article/details/gxsifuycl.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://3g.fehbvm.com/Article/details/gmxdxkxnv.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.fehbvm.com/Article/details/gjnmadpxk.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.m.share.hesvh.cn/Article/details/gkntoxghy.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.zdbjq.cn/Article/details/gfeoiximg.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.fehbvm.com/Article/details/gtypdgeup.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://read.share.zdbjq.cn/Article/details/gfbkjzwdj.sHtML

[H03] 主动抛出异常
来源：http://read.share.fehbvm.com/Article/details/ghaqvxwgg.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.m.share.zdbjq.cn/Article/details/gzwbnljmf.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blog.hesvh.cn/Article/details/grewkefhq.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.hesvh.cn/Article/details/gurealaek.sHtML

TS:   throw new Error("错误信息");
来源：http://wap.hesvh.cn/Article/details/gjjgkmmdo.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.blog.hesvh.cn/Article/details/gwnberjhn.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.share.hesvh.cn/Article/details/gtkgtnfxo.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://wap.zdbjq.cn/Article/details/gylzpzthm.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://wap.hesvh.cn/Article/details/gzxwwpkhn.sHtML

[H04] 自定义异常类型
来源：http://m.share.hesvh.cn/Article/details/ggnkjqxvp.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.hesvh.cn/Article/details/gcoqfxjjh.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://3g.hesvh.cn/Article/details/gbwkiyexk.sHtML

JS:   class MyError extends Error {}
来源：http://www.m.share.zdbjq.cn/Article/details/gilziguoh.sHtML

TS:   class MyError extends Error {}
来源：http://baike.fehbvm.com/Article/details/gvajrokdc.sHtML

Java: class MyException extends RuntimeException {}
来源：http://m.share.zdbjq.cn/Article/details/gqaiehvbi.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.zdbjq.cn/Article/details/geobuffnw.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.share.hesvh.cn/Article/details/gwtiqqkci.sHtML

C#:   class MyException : Exception {}
来源：http://www.blog.fehbvm.com/Article/details/gfcfciyoz.sHtML

[H05] 捕获特定类型
来源：http://www.m.share.zdbjq.cn/Article/details/gwomknifw.sHtML

Py:   except ValueError as e:
来源：http://3g.zdbjq.cn/Article/details/gsstluple.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://3g.hesvh.cn/Article/details/gblzdzijq.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://baike.zdbjq.cn/Article/details/gtuxwpmsh.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://m.share.fehbvm.com/Article/details/gvmgtktcc.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://mobile.fehbvm.com/Article/details/gvayqngbv.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://3g.zdbjq.cn/Article/details/gbxujgfvu.sHtML

Ruby: rescue ArgumentError => e
来源：http://wap.fehbvm.com/Article/details/grprxbxyg.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.blog.hesvh.cn/Article/details/gtvxjxlte.sHtML

[H06] 可选值 / 空值安全访问
来源：http://mobile.zdbjq.cn/Article/details/giowuzeuu.sHtML

Py:   value = d.get("k") or default
来源：http://baike.zdbjq.cn/Article/details/gkisyfsoi.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.m.share.zdbjq.cn/Article/details/gegumiqrd.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.zdbjq.cn/Article/details/gmdwwbpuz.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.blog.hesvh.cn/Article/details/grvbztndx.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://blog.zdbjq.cn/Article/details/gkupskrlz.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.blog.hesvh.cn/Article/details/gkeekluye.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.share.fehbvm.com/Article/details/grkerlepq.sHtML

C#:   obj?.A?.B ?? default
来源：http://m.share.hesvh.cn/Article/details/gmzodbvri.sHtML

[H07] 断言
来源：http://mobile.hesvh.cn/Article/details/gzcrtcssp.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.share.hesvh.cn/Article/details/gmcgipqtb.sHtML

PHP:  assert($x > 0);
来源：http://www.share.zdbjq.cn/Article/details/ggaitghtc.sHtML

JS:   console.assert(x > 0);
来源：http://www.share.fehbvm.com/Article/details/gooogsunf.sHtML

TS:   console.assert(x > 0);
来源：http://mobile.fehbvm.com/Article/details/gdivjhpfm.sHtML

Java: assert x > 0 : "必须为正";
来源：http://m.share.hesvh.cn/Article/details/gpxmuungs.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.share.hesvh.cn/Article/details/gochgduoe.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://read.share.hesvh.cn/Article/details/ghnbptumy.sHtML

C#:   Debug.Assert(x > 0);
来源：http://mobile.hesvh.cn/Article/details/gviqrwdtf.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.blog.hesvh.cn/Article/details/gxamjjgvp.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://read.share.fehbvm.com/Article/details/gewgcbjwy.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://read.share.fehbvm.com/Article/details/gqzmrmflc.sHtML

JS:   e.message;  e.stack
来源：http://wap.fehbvm.com/Article/details/gxmsyiyqh.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://wap.fehbvm.com/Article/details/gvhqtaehb.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://mobile.hesvh.cn/Article/details/gjrksntoq.sHtML

Go:   err.Error()
来源：http://read.share.hesvh.cn/Article/details/gdvriiain.sHtML

Ruby: e.message;  e.backtrace
来源：http://wap.zdbjq.cn/Article/details/gqkzlklid.sHtML

C#:   e.Message;  e.StackTrace
来源：http://wap.hesvh.cn/Article/details/gpdgpenjk.sHtML

[H09] 带错误码的异常
来源：http://www.m.share.zdbjq.cn/Article/details/gvoopedeb.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://baike.zdbjq.cn/Article/details/gxsoxxjbe.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://wap.hesvh.cn/Article/details/gtdbuvnuu.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wap.hesvh.cn/Article/details/gegrmvalg.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.blog.hesvh.cn/Article/details/gdcsyijaw.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://m.share.zdbjq.cn/Article/details/gaccnibaf.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.share.zdbjq.cn/Article/details/ghzfdzuyb.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://baike.hesvh.cn/Article/details/gkwidgyxg.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://wap.hesvh.cn/Article/details/gvpggmxof.sHtML

[H10] 资源自动释放
来源：http://mobile.zdbjq.cn/Article/details/guybmuzai.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://wap.hesvh.cn/Article/details/gltwepjdf.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://blog.hesvh.cn/Article/details/gzlmlipva.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.hesvh.cn/Article/details/guhfvixnu.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.hesvh.cn/Article/details/gwsevqohh.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://read.share.hesvh.cn/Article/details/gsbmwoqzv.sHtML

Go:   defer f.Close()
来源：http://m.share.hesvh.cn/Article/details/gtujfdmtz.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://3g.zdbjq.cn/Article/details/ghommulho.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gsqrpyiqj.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gnoepqaxc.sHtML

I. 正则表达式
来源：http://read.share.hesvh.cn/Article/details/ggefomqbr.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/guxsbrblo.sHtML

[I01] 判断是否匹配
来源：http://m.share.zdbjq.cn/Article/details/gymdmwfnu.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://3g.zdbjq.cn/Article/details/gxrugaacg.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://m.share.fehbvm.com/Article/details/gmrehggap.sHtML

JS:   /\d+/.test(s)
来源：http://www.m.share.fehbvm.com/Article/details/gndmmankb.sHtML

TS:   /\d+/.test(s)
来源：http://www.share.hesvh.cn/Article/details/gbxwkkqpz.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://read.share.hesvh.cn/Article/details/gunfdgzjz.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://m.share.hesvh.cn/Article/details/glkluaokn.sHtML

Ruby: s.match?(/\d+/)
来源：http://blog.zdbjq.cn/Article/details/gcwbcwupu.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://3g.fehbvm.com/Article/details/gonggtrfq.sHtML

[I02] 提取所有匹配
来源：http://www.share.fehbvm.com/Article/details/gunzhnlaf.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.blog.fehbvm.com/Article/details/ggrqvvotp.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://m.share.hesvh.cn/Article/details/gbfrmdugd.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wap.zdbjq.cn/Article/details/gtnzqpwho.sHtML

TS:   s.match(/\d+/g)
来源：http://mobile.zdbjq.cn/Article/details/gqrcpwycy.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://read.share.hesvh.cn/Article/details/ggbeildli.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.m.share.fehbvm.com/Article/details/gcydhtqra.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.m.share.zdbjq.cn/Article/details/gahkmtmrc.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gubykjmlq.sHtML

[I03] 提取捕获分组
来源：http://www.m.share.fehbvm.com/Article/details/ggigmevvy.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://3g.zdbjq.cn/Article/details/gqehcayyh.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mobile.hesvh.cn/Article/details/gsricnhul.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://blog.hesvh.cn/Article/details/gbiuuqocg.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://3g.zdbjq.cn/Article/details/gbauvtizu.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.m.share.hesvh.cn/Article/details/gwjvjiutm.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://blog.hesvh.cn/Article/details/gcakfewez.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://m.share.fehbvm.com/Article/details/gwtdpyuwo.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wap.fehbvm.com/Article/details/gfprzqzjh.sHtML

[I04] 正则替换
来源：http://mobile.zdbjq.cn/Article/details/glspfigve.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://read.share.fehbvm.com/Article/details/gzhwvrioy.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.fehbvm.com/Article/details/gggancuxl.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://3g.zdbjq.cn/Article/details/gsgyunwky.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://blog.fehbvm.com/Article/details/gmwyherra.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://m.share.hesvh.cn/Article/details/gqomvkknb.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://3g.hesvh.cn/Article/details/gqgxiazow.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://wap.zdbjq.cn/Article/details/gmieuabnc.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.blog.zdbjq.cn/Article/details/gzkiibfhs.sHtML

[I05] 按正则拆分
来源：http://wap.fehbvm.com/Article/details/gczrpzvfq.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://baike.hesvh.cn/Article/details/gyxsrtpds.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://blog.fehbvm.com/Article/details/gcxicowfw.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://blog.fehbvm.com/Article/details/gxjyhvckb.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://mobile.zdbjq.cn/Article/details/ggknobgud.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.share.fehbvm.com/Article/details/guszrtrcd.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://m.share.zdbjq.cn/Article/details/gkngwrjow.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.blog.hesvh.cn/Article/details/guealiiap.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wap.zdbjq.cn/Article/details/ggclrxtsd.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.m.share.fehbvm.com/Article/details/gsyqauxzt.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.m.share.zdbjq.cn/Article/details/gckvaterb.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://m.share.fehbvm.com/Article/details/gowwdkxto.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.zdbjq.cn/Article/details/gqjberdyt.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.zdbjq.cn/Article/details/gytsaasgb.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mobile.fehbvm.com/Article/details/glyghiefg.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://baike.zdbjq.cn/Article/details/grrbevhbr.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://m.share.fehbvm.com/Article/details/gmzftwerv.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://blog.fehbvm.com/Article/details/gcubgttpr.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.share.hesvh.cn/Article/details/gonkgulrk.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://baike.fehbvm.com/Article/details/gputqshax.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://m.share.fehbvm.com/Article/details/gsgwjekiq.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://baike.fehbvm.com/Article/details/gwvpotpwp.sHtML

TS:   /error/gim
来源：http://read.share.zdbjq.cn/Article/details/gpueesmvb.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wap.zdbjq.cn/Article/details/gkytmvcxb.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mobile.hesvh.cn/Article/details/gimmtidct.sHtML

Ruby: s.scan(/error/i)
来源：http://mobile.zdbjq.cn/Article/details/gviwfvknb.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://3g.fehbvm.com/Article/details/gfjdlnfaz.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.share.hesvh.cn/Article/details/gmexqgnee.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://baike.fehbvm.com/Article/details/gfzwuqebo.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wap.fehbvm.com/Article/details/ghgxfonvd.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.hesvh.cn/Article/details/gejijzopk.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.fehbvm.com/Article/details/gtcxumhdp.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.share.hesvh.cn/Article/details/gzlxqhxlb.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://m.share.hesvh.cn/Article/details/gbnyspsix.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://blog.fehbvm.com/Article/details/gxnchypcg.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://blog.fehbvm.com/Article/details/glokxixdn.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gsytptkgw.sHtML

J. 日期与时间
来源：http://mobile.zdbjq.cn/Article/details/gzdasiwyl.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gstlfzgep.sHtML

[J01] 获取当前时间
来源：http://www.blog.hesvh.cn/Article/details/ggudybsdc.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.blog.fehbvm.com/Article/details/gljrrlnnq.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://blog.fehbvm.com/Article/details/guonksucq.sHtML

JS:   new Date();  Date.now()
来源：http://3g.hesvh.cn/Article/details/guwaqsxcx.sHtML

TS:   new Date();  Date.now()
来源：http://wap.fehbvm.com/Article/details/gjqagvmzp.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://m.share.hesvh.cn/Article/details/gfhycaenm.sHtML

Go:   time.Now()
来源：http://www.blog.zdbjq.cn/Article/details/gjjvznqrc.sHtML

Ruby: Time.now
来源：http://www.share.hesvh.cn/Article/details/gldlipzwg.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://baike.zdbjq.cn/Article/details/gzkuspyjd.sHtML

[J02] 格式化输出
来源：http://read.share.fehbvm.com/Article/details/glggfluvp.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.zdbjq.cn/Article/details/gqypkkmbu.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.blog.hesvh.cn/Article/details/gjxmumshg.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wap.hesvh.cn/Article/details/goqgpaegt.sHtML

TS:   d.toISOString()
来源：http://www.m.share.hesvh.cn/Article/details/gdrqtxjoo.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.m.share.fehbvm.com/Article/details/gepypmulu.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://mobile.hesvh.cn/Article/details/ginrxsgiy.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.zdbjq.cn/Article/details/gjzjxxpes.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://baike.hesvh.cn/Article/details/gdweznbcm.sHtML

[J03] 字符串解析为日期
来源：http://www.share.zdbjq.cn/Article/details/gaeffdall.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://m.share.fehbvm.com/Article/details/glujlyxpa.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.m.share.hesvh.cn/Article/details/gxsmqhptx.sHtML

JS:   new Date("2024-01-02")
来源：http://3g.zdbjq.cn/Article/details/gvvhsykow.sHtML

TS:   new Date("2024-01-02")
来源：http://baike.hesvh.cn/Article/details/grncqsmct.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://baike.fehbvm.com/Article/details/groztzcwz.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://m.share.zdbjq.cn/Article/details/gfrklezzq.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://read.share.fehbvm.com/Article/details/gihsgxqgm.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mobile.fehbvm.com/Article/details/gefnrtrbj.sHtML

[J04] 时间戳与日期互转
来源：http://baike.hesvh.cn/Article/details/gesusqtig.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.m.share.hesvh.cn/Article/details/gicykdmxa.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.m.share.zdbjq.cn/Article/details/gvfigvsbk.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://m.share.fehbvm.com/Article/details/gitbdrpfz.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://mobile.fehbvm.com/Article/details/gpxzpbfqi.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://baike.zdbjq.cn/Article/details/gdntgwsbh.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.m.share.fehbvm.com/Article/details/grberlrad.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.blog.zdbjq.cn/Article/details/gudkqotpu.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://read.share.fehbvm.com/Article/details/gxssmzhke.sHtML

[J05] 时间加减（加 7 天）
来源：http://blog.zdbjq.cn/Article/details/gxswkpofq.sHtML

Py:   now + timedelta(days=7)
来源：http://mobile.zdbjq.cn/Article/details/gnbpzddep.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://wap.hesvh.cn/Article/details/gdhjguygz.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.hesvh.cn/Article/details/gsyfeatcj.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.fehbvm.com/Article/details/gythxhwyf.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.blog.fehbvm.com/Article/details/gpmxlffkn.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://read.share.hesvh.cn/Article/details/glleeqzlp.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.share.fehbvm.com/Article/details/gumgalovg.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://read.share.hesvh.cn/Article/details/gyorasdmz.sHtML

[J06] 计算两时间之差
来源：http://3g.zdbjq.cn/Article/details/gkgtukyfn.sHtML


<!-- 参考信息 -->