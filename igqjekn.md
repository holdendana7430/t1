代发 wailian999

PHP:  public static function f() {}
来源：http://3g.hesvh.cn/Article/details/gpbfotkvx.sHtML

JS:   static f() {}
来源：http://www.share.hesvh.cn/Article/details/gnehyipwx.sHtML

TS:   static f(): void {}
来源：http://read.share.zdbjq.cn/Article/details/gidtwirax.sHtML

Java: static void f() {}
来源：http://3g.fehbvm.com/Article/details/gawwqmhfc.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.fehbvm.com/Article/details/ghmtxuvqh.sHtML

Ruby: def self.f; end
来源：http://baike.fehbvm.com/Article/details/gqjfovozh.sHtML

C#:   public static void F() {}
来源：http://blog.hesvh.cn/Article/details/grsseydne.sHtML

[G09] 接口 / 抽象类
来源：http://3g.hesvh.cn/Article/details/gjaebahlw.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.zdbjq.cn/Article/details/ghmrvnjeg.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.zdbjq.cn/Article/details/gfgeaxcdu.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.zdbjq.cn/Article/details/gryztyqfq.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.zdbjq.cn/Article/details/gkzvvemkk.sHtML

Java: interface Shape { double area(); }
来源：http://3g.fehbvm.com/Article/details/gutchzhqs.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.hesvh.cn/Article/details/gcpqrtznb.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.zdbjq.cn/Article/details/gqfyqpgee.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.fehbvm.com/Article/details/goiytpufu.sHtML

[G10] 访问控制
来源：http://www.share.hesvh.cn/Article/details/gqsywopxd.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.zdbjq.cn/Article/details/gtvaqnnki.sHtML

PHP:  public / protected / private
来源：http://3g.zdbjq.cn/Article/details/gbyhbayjb.sHtML

JS:   #private 字段；其余公开
来源：http://3g.fehbvm.com/Article/details/gknddfnoh.sHtML

TS:   public / protected / private
来源：http://read.share.zdbjq.cn/Article/details/gaxflxqkp.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.zdbjq.cn/Article/details/gjqvyqvre.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.hesvh.cn/Article/details/ganaotbtj.sHtML

Ruby: public / protected / private
来源：http://baike.fehbvm.com/Article/details/gsqmsgoqw.sHtML

C#:   public / protected / private / internal
来源：http://read.share.fehbvm.com/Article/details/gldpiwwae.sHtML

[G11] getter / setter
来源：http://blog.fehbvm.com/Article/details/gevqgwqkk.sHtML

Py:   @property 与 @x.setter
来源：http://baike.hesvh.cn/Article/details/guvaltaug.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.hesvh.cn/Article/details/gsjhvnqif.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.hesvh.cn/Article/details/gradbqlij.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.zdbjq.cn/Article/details/gvytjotlq.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/gdyaqgwwh.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.hesvh.cn/Article/details/gwmhhpwrx.sHtML

Ruby: attr_accessor :name
来源：http://read.share.zdbjq.cn/Article/details/gptjqzite.sHtML

C#:   public string Name { get; set; }
来源：http://blog.hesvh.cn/Article/details/gumphzdqt.sHtML

[G12] 对象转字符串
来源：http://m.share.zdbjq.cn/Article/details/gfjkpuvpj.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.fehbvm.com/Article/details/gmivaevef.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.fehbvm.com/Article/details/gzrmjikhh.sHtML

JS:   toString() { return this.name; }
来源：http://wap.fehbvm.com/Article/details/gmzricwxs.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.zdbjq.cn/Article/details/gptzwjcib.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.fehbvm.com/Article/details/gxnawtbxo.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.fehbvm.com/Article/details/gadorzgzb.sHtML

Ruby: def to_s; @name; end
来源：http://blog.fehbvm.com/Article/details/gnquyysif.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.zdbjq.cn/Article/details/gbgkzdrkp.sHtML

[G13] 判断对象类型
来源：http://read.share.hesvh.cn/Article/details/gkyvcytvk.sHtML

Py:   isinstance(u, User)
来源：http://www.share.zdbjq.cn/Article/details/gczmnvljt.sHtML

PHP:  $u instanceof User
来源：http://www.blog.fehbvm.com/Article/details/gafqqjcok.sHtML

JS:   u instanceof User
来源：http://baike.fehbvm.com/Article/details/ghklwejzr.sHtML

TS:   u instanceof User
来源：http://3g.fehbvm.com/Article/details/gxmdowucj.sHtML

Java: u instanceof User
来源：http://www.m.share.hesvh.cn/Article/details/gsrvvfnul.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.hesvh.cn/Article/details/gclmduzvk.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.fehbvm.com/Article/details/gjzdjodiz.sHtML

C#:   u is User
来源：http://www.share.hesvh.cn/Article/details/gkrzkbiwm.sHtML

[G14] 数据类 / record
来源：http://mobile.zdbjq.cn/Article/details/gqnhcgufk.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.hesvh.cn/Article/details/gbuirzgnr.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.hesvh.cn/Article/details/gcmzwqbob.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.hesvh.cn/Article/details/glkboiekw.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.hesvh.cn/Article/details/gwpyhjuzq.sHtML

Java: record User(String name, int age) {}
来源：http://mobile.zdbjq.cn/Article/details/guthtcqva.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.zdbjq.cn/Article/details/ganbfnoxk.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.fehbvm.com/Article/details/grsxbrdzf.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.hesvh.cn/Article/details/grtlzpmvo.sHtML

[G15] 枚举
来源：http://mobile.zdbjq.cn/Article/details/gamiupfzj.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.fehbvm.com/Article/details/gytqzclxd.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.hesvh.cn/Article/details/gqkynmjji.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mobile.zdbjq.cn/Article/details/gvdzsmbyp.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.hesvh.cn/Article/details/gzoxihqnq.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.zdbjq.cn/Article/details/gupmibeas.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.blog.hesvh.cn/Article/details/goyoanacw.sHtML

Ruby: Color = %i[red green].freeze
来源：http://m.share.hesvh.cn/Article/details/gcrdshibp.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.zdbjq.cn/Article/details/gwexzgzct.sHtML

[G16] 对象转数组 / 字典
来源：http://www.blog.hesvh.cn/Article/details/gyreugyvu.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.fehbvm.com/Article/details/goldcietg.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.fehbvm.com/Article/details/gtkgkpptx.sHtML

JS:   Object.entries(obj)
来源：http://read.share.zdbjq.cn/Article/details/glihpkwzx.sHtML

TS:   Object.entries(obj)
来源：http://baike.fehbvm.com/Article/details/gbabddnzv.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.zdbjq.cn/Article/details/gjzbaomul.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.zdbjq.cn/Article/details/ggbprlgjc.sHtML

Ruby: obj.instance_variables
来源：http://read.share.zdbjq.cn/Article/details/gxovfiuwy.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.hesvh.cn/Article/details/gpokgnwpn.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gsdbnxghf.sHtML

H. 异常与错误处理
来源：http://mobile.hesvh.cn/Article/details/gexpepzlg.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gzudzqasl.sHtML

[H01] try / catch 基础
来源：http://www.share.zdbjq.cn/Article/details/gmynjogwq.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://baike.zdbjq.cn/Article/details/gphibbybs.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wap.hesvh.cn/Article/details/gbowfjvgy.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://m.share.fehbvm.com/Article/details/ggyanmghk.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.hesvh.cn/Article/details/ghavsfucj.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.fehbvm.com/Article/details/godqxpcwt.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.m.share.fehbvm.com/Article/details/gmlmrlvyq.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.m.share.fehbvm.com/Article/details/gagjnpccs.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.hesvh.cn/Article/details/gsttliirf.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.zdbjq.cn/Article/details/gnuidhujf.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://3g.fehbvm.com/Article/details/gsfbomtab.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.m.share.hesvh.cn/Article/details/genugddoj.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://baike.fehbvm.com/Article/details/gxbarjoed.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/godppipto.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.zdbjq.cn/Article/details/ghflsgxiz.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.zdbjq.cn/Article/details/guummyhid.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://blog.zdbjq.cn/Article/details/givvspjel.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://blog.hesvh.cn/Article/details/gmxpmhjaq.sHtML

[H03] 主动抛出异常
来源：http://mobile.fehbvm.com/Article/details/glqswsqbz.sHtML

Py:   raise ValueError("错误信息")
来源：http://blog.hesvh.cn/Article/details/gkfuahsmf.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blog.zdbjq.cn/Article/details/gzmpmnotb.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.zdbjq.cn/Article/details/gtfxzzhob.sHtML

TS:   throw new Error("错误信息");
来源：http://mobile.fehbvm.com/Article/details/grlnjpnck.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://mobile.fehbvm.com/Article/details/gnxxvwlom.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.hesvh.cn/Article/details/gwxkktjfa.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://blog.zdbjq.cn/Article/details/gfywxezdz.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://baike.fehbvm.com/Article/details/giadlyboy.sHtML

[H04] 自定义异常类型
来源：http://wap.fehbvm.com/Article/details/gcoskqwqm.sHtML

Py:   class MyError(Exception): pass
来源：http://www.share.fehbvm.com/Article/details/gvvmaltmc.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://wap.fehbvm.com/Article/details/gaosatfum.sHtML

JS:   class MyError extends Error {}
来源：http://wap.fehbvm.com/Article/details/gzajcmirv.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.zdbjq.cn/Article/details/gcliypbne.sHtML

Java: class MyException extends RuntimeException {}
来源：http://3g.zdbjq.cn/Article/details/gpeyzkovv.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://m.share.zdbjq.cn/Article/details/gwwfhoybj.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.m.share.zdbjq.cn/Article/details/gwnbgmjtl.sHtML

C#:   class MyException : Exception {}
来源：http://read.share.hesvh.cn/Article/details/gevhvlpve.sHtML

[H05] 捕获特定类型
来源：http://www.blog.fehbvm.com/Article/details/gmdroavkl.sHtML

Py:   except ValueError as e:
来源：http://www.share.zdbjq.cn/Article/details/ghnoynwtu.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.blog.hesvh.cn/Article/details/grzapoebn.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://baike.hesvh.cn/Article/details/ghzdocrwk.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://wap.zdbjq.cn/Article/details/gjmoovoue.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://baike.zdbjq.cn/Article/details/godhqwhjn.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://3g.fehbvm.com/Article/details/gscssdndo.sHtML

Ruby: rescue ArgumentError => e
来源：http://wap.fehbvm.com/Article/details/grkhlyffw.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://m.share.hesvh.cn/Article/details/gpwactatp.sHtML

[H06] 可选值 / 空值安全访问
来源：http://read.share.hesvh.cn/Article/details/gppvmczin.sHtML

Py:   value = d.get("k") or default
来源：http://www.blog.zdbjq.cn/Article/details/gzjjyrczs.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://blog.hesvh.cn/Article/details/gbpgaszuy.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://wap.fehbvm.com/Article/details/gzpbrfcua.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://blog.fehbvm.com/Article/details/gfvsmsnfn.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://blog.fehbvm.com/Article/details/gjbeiablt.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://mobile.hesvh.cn/Article/details/gsywjrlhp.sHtML

Ruby: d&.dig(:a, :b)
来源：http://baike.hesvh.cn/Article/details/glnhkajum.sHtML

C#:   obj?.A?.B ?? default
来源：http://read.share.fehbvm.com/Article/details/gqokukjoh.sHtML

[H07] 断言
来源：http://www.m.share.hesvh.cn/Article/details/gjdxaqbfr.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.share.hesvh.cn/Article/details/gayqhpuqm.sHtML

PHP:  assert($x > 0);
来源：http://wap.hesvh.cn/Article/details/gzqlsxwbm.sHtML

JS:   console.assert(x > 0);
来源：http://mobile.fehbvm.com/Article/details/gboqfzaqf.sHtML

TS:   console.assert(x > 0);
来源：http://www.share.fehbvm.com/Article/details/gmqgmlylx.sHtML

Java: assert x > 0 : "必须为正";
来源：http://mobile.hesvh.cn/Article/details/gkbjnpdhl.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://m.share.zdbjq.cn/Article/details/gaeajqmoy.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://m.share.fehbvm.com/Article/details/gexwolkpk.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.blog.hesvh.cn/Article/details/gcktkmjiu.sHtML

[H08] 获取错误信息与堆栈
来源：http://blog.zdbjq.cn/Article/details/gphqxludb.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://baike.fehbvm.com/Article/details/ggddunrml.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://read.share.zdbjq.cn/Article/details/gvacwwmve.sHtML

JS:   e.message;  e.stack
来源：http://www.blog.hesvh.cn/Article/details/gxrpttlza.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://baike.hesvh.cn/Article/details/gsyjcnjdr.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://baike.fehbvm.com/Article/details/gsnvkgdpe.sHtML

Go:   err.Error()
来源：http://read.share.fehbvm.com/Article/details/gwwieyvqi.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.share.fehbvm.com/Article/details/gmrsaccuo.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.blog.fehbvm.com/Article/details/gssaarofl.sHtML

[H09] 带错误码的异常
来源：http://3g.hesvh.cn/Article/details/gdwvvfbwv.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://read.share.hesvh.cn/Article/details/gnpupgknp.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://blog.hesvh.cn/Article/details/gunxjrvlc.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://m.share.fehbvm.com/Article/details/gseflvagg.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.blog.zdbjq.cn/Article/details/gjzeoggfx.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://3g.fehbvm.com/Article/details/gvrkbvzed.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mobile.zdbjq.cn/Article/details/gcpjsjxju.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.blog.hesvh.cn/Article/details/gkabfyuvg.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://mobile.fehbvm.com/Article/details/grdloxjfr.sHtML

[H10] 资源自动释放
来源：http://wap.fehbvm.com/Article/details/gpqotqojm.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://baike.hesvh.cn/Article/details/gapxwfbmn.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.blog.hesvh.cn/Article/details/gqfgqqmfq.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.hesvh.cn/Article/details/gwtmelrsp.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.zdbjq.cn/Article/details/gqkxyywnq.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.m.share.fehbvm.com/Article/details/gcxsensza.sHtML

Go:   defer f.Close()
来源：http://wap.zdbjq.cn/Article/details/gfmtskdxs.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://blog.zdbjq.cn/Article/details/gneuajbtx.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gmwbghgci.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gvoajqbmn.sHtML

I. 正则表达式
来源：http://mobile.fehbvm.com/Article/details/gkaypejdc.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/grlwklwfq.sHtML

[I01] 判断是否匹配
来源：http://www.m.share.hesvh.cn/Article/details/gdaozyotg.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mobile.hesvh.cn/Article/details/grlimnyaf.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.m.share.fehbvm.com/Article/details/gdjtdsapq.sHtML

JS:   /\d+/.test(s)
来源：http://m.share.fehbvm.com/Article/details/golihxydo.sHtML

TS:   /\d+/.test(s)
来源：http://www.share.fehbvm.com/Article/details/gnpcmspvx.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://baike.zdbjq.cn/Article/details/gvxtaxqxm.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wap.hesvh.cn/Article/details/goxiyrguu.sHtML

Ruby: s.match?(/\d+/)
来源：http://blog.fehbvm.com/Article/details/gsvamegkn.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://3g.hesvh.cn/Article/details/gkgegwued.sHtML

[I02] 提取所有匹配
来源：http://blog.zdbjq.cn/Article/details/gxsewhlkl.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.blog.fehbvm.com/Article/details/gdmtkbrsl.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://blog.fehbvm.com/Article/details/gfvkbmnqb.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.m.share.zdbjq.cn/Article/details/gupqnxjhn.sHtML

TS:   s.match(/\d+/g)
来源：http://blog.zdbjq.cn/Article/details/gxqahriuv.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://blog.fehbvm.com/Article/details/gcccrfwxt.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wap.hesvh.cn/Article/details/gtlgmweiq.sHtML

Ruby: s.scan(/\d+/)
来源：http://baike.zdbjq.cn/Article/details/ggbcasvqi.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.blog.fehbvm.com/Article/details/ggysulree.sHtML

[I03] 提取捕获分组
来源：http://m.share.hesvh.cn/Article/details/gqgdtytlv.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.blog.hesvh.cn/Article/details/gksotopxf.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mobile.fehbvm.com/Article/details/gifttrupt.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.share.fehbvm.com/Article/details/ggywsqsjs.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wap.fehbvm.com/Article/details/gvwpgpdli.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://blog.fehbvm.com/Article/details/gnpkmtflo.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://m.share.zdbjq.cn/Article/details/gwuvzfisr.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://3g.hesvh.cn/Article/details/gqgoujwoq.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://m.share.hesvh.cn/Article/details/gnjusbsfo.sHtML

[I04] 正则替换
来源：http://3g.hesvh.cn/Article/details/gmzmwmgdw.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.blog.fehbvm.com/Article/details/gestmmywh.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://3g.zdbjq.cn/Article/details/gnosirhbn.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://wap.hesvh.cn/Article/details/gwzwmvnxd.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://3g.zdbjq.cn/Article/details/gyjivvmlo.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://read.share.fehbvm.com/Article/details/gnlqeclja.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://baike.zdbjq.cn/Article/details/glscezrgt.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.share.fehbvm.com/Article/details/ggvonnscb.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://3g.zdbjq.cn/Article/details/gjrekldrf.sHtML

[I05] 按正则拆分
来源：http://wap.hesvh.cn/Article/details/gmwzsogjk.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://baike.hesvh.cn/Article/details/gbqhftcft.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://m.share.fehbvm.com/Article/details/gxwcslvki.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://mobile.hesvh.cn/Article/details/gtbwjnawb.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://blog.fehbvm.com/Article/details/gjcohgwfd.sHtML

Java: s.split("\\s*,\\s*")
来源：http://wap.fehbvm.com/Article/details/gyloeptcq.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wap.zdbjq.cn/Article/details/gwahhaglg.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://m.share.fehbvm.com/Article/details/gbquopvbn.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://3g.hesvh.cn/Article/details/gvrnumqqr.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wap.zdbjq.cn/Article/details/grqpboofh.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://mobile.fehbvm.com/Article/details/gqkleigzc.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://read.share.hesvh.cn/Article/details/grdckyaqr.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.zdbjq.cn/Article/details/gisnukdbi.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.zdbjq.cn/Article/details/gvqmmvzri.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://blog.fehbvm.com/Article/details/grwxwxusf.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://3g.hesvh.cn/Article/details/glmvubexw.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.blog.zdbjq.cn/Article/details/gcdlwrzrd.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wap.fehbvm.com/Article/details/gazxyfmbl.sHtML

[I07] 忽略大小写与多行模式
来源：http://3g.fehbvm.com/Article/details/gnolngspp.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.m.share.zdbjq.cn/Article/details/guvfroafw.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.m.share.hesvh.cn/Article/details/gtbkfwtlx.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wap.zdbjq.cn/Article/details/gkhnimlva.sHtML

TS:   /error/gim
来源：http://blog.hesvh.cn/Article/details/grynmmntv.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.share.fehbvm.com/Article/details/gqjaazdin.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://3g.zdbjq.cn/Article/details/gjjdneqgu.sHtML

Ruby: s.scan(/error/i)
来源：http://blog.zdbjq.cn/Article/details/gvsoerfmv.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.blog.zdbjq.cn/Article/details/gckcowmpb.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.share.fehbvm.com/Article/details/grsvwamwd.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.m.share.hesvh.cn/Article/details/gotvwehhz.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.share.hesvh.cn/Article/details/gyygjasop.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.hesvh.cn/Article/details/gjcsrpkbg.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.hesvh.cn/Article/details/grvaqpvvu.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://3g.zdbjq.cn/Article/details/gmimadsug.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wap.hesvh.cn/Article/details/gfqhtqcbp.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.share.zdbjq.cn/Article/details/gfwdrxefa.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mobile.zdbjq.cn/Article/details/gniypgwuf.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gnmiguvew.sHtML

J. 日期与时间
来源：http://www.share.fehbvm.com/Article/details/gymdrmwhp.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/ghgmehznm.sHtML

[J01] 获取当前时间
来源：http://www.share.fehbvm.com/Article/details/gafjvtrok.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://wap.fehbvm.com/Article/details/gsqngxioc.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://read.share.zdbjq.cn/Article/details/gqryecncg.sHtML

JS:   new Date();  Date.now()
来源：http://blog.fehbvm.com/Article/details/gyoltrmfe.sHtML

TS:   new Date();  Date.now()
来源：http://read.share.fehbvm.com/Article/details/gmsiwukps.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://mobile.hesvh.cn/Article/details/ghasvzvkk.sHtML

Go:   time.Now()
来源：http://read.share.fehbvm.com/Article/details/gghphhyzf.sHtML

Ruby: Time.now
来源：http://blog.fehbvm.com/Article/details/geeflkybg.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.blog.fehbvm.com/Article/details/gjyrvqdml.sHtML

[J02] 格式化输出
来源：http://3g.fehbvm.com/Article/details/gicrwygfw.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.fehbvm.com/Article/details/gtwbhfhbj.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://blog.zdbjq.cn/Article/details/gxwrwruoi.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://read.share.zdbjq.cn/Article/details/gynbgoyty.sHtML

TS:   d.toISOString()
来源：http://www.m.share.zdbjq.cn/Article/details/gtxqawjoo.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://wap.zdbjq.cn/Article/details/gkvcsbbuu.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://mobile.zdbjq.cn/Article/details/gycxxvtfu.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.hesvh.cn/Article/details/gvkhyyfed.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://3g.fehbvm.com/Article/details/gqlxkeape.sHtML

[J03] 字符串解析为日期
来源：http://www.m.share.zdbjq.cn/Article/details/gxmlkykkx.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.share.zdbjq.cn/Article/details/gmtynghol.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://mobile.fehbvm.com/Article/details/ghftbgrfb.sHtML

JS:   new Date("2024-01-02")
来源：http://blog.zdbjq.cn/Article/details/gydsswtnq.sHtML

TS:   new Date("2024-01-02")
来源：http://www.share.hesvh.cn/Article/details/guaroywuo.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://mobile.fehbvm.com/Article/details/geodeeqlf.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.blog.zdbjq.cn/Article/details/gmnlxuafu.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.share.fehbvm.com/Article/details/gvunqrrnw.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://3g.hesvh.cn/Article/details/gwsrykgtx.sHtML

[J04] 时间戳与日期互转
来源：http://www.share.fehbvm.com/Article/details/gjugufeqq.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.blog.zdbjq.cn/Article/details/gofrucdbz.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://mobile.hesvh.cn/Article/details/gqsjbcuie.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.m.share.hesvh.cn/Article/details/gloylpjrm.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://read.share.hesvh.cn/Article/details/gmmjtwiyz.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.blog.fehbvm.com/Article/details/gbxrlfish.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://baike.zdbjq.cn/Article/details/gbrjzfjtp.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mobile.hesvh.cn/Article/details/gnjvwlpml.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://3g.fehbvm.com/Article/details/gwltnvyes.sHtML

[J05] 时间加减（加 7 天）
来源：http://mobile.hesvh.cn/Article/details/gcqpahczw.sHtML

Py:   now + timedelta(days=7)
来源：http://www.m.share.hesvh.cn/Article/details/ginskqcbn.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://baike.zdbjq.cn/Article/details/ggiulnavr.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.fehbvm.com/Article/details/gmxrdwspx.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.fehbvm.com/Article/details/gpryrgfvd.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.m.share.zdbjq.cn/Article/details/gmwzubamf.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.share.fehbvm.com/Article/details/gbtcqohkd.sHtML

Ruby: Time.now + 7 * 86400
来源：http://3g.hesvh.cn/Article/details/gkuhusost.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.blog.hesvh.cn/Article/details/gevbrelor.sHtML

[J06] 计算两时间之差
来源：http://m.share.zdbjq.cn/Article/details/gbvnaihbb.sHtML

Py:   (end - start).total_seconds()
来源：http://read.share.fehbvm.com/Article/details/glszmwszr.sHtML

PHP:  $end->diff($start)->days;
来源：http://m.share.fehbvm.com/Article/details/gfvjxafnf.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.m.share.fehbvm.com/Article/details/gvgcgyfhs.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mobile.hesvh.cn/Article/details/gamknywqd.sHtML


<!-- 参考信息 -->