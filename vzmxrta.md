代发 wailian999

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.hesvh.cn/Article/details/grnigtsrd.sHtML

Ruby: def self.f; end
来源：http://wap.hesvh.cn/Article/details/gmpsoxspz.sHtML

C#:   public static void F() {}
来源：http://www.blog.hesvh.cn/Article/details/gvnbaycqf.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.zdbjq.cn/Article/details/gciwpdica.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.zdbjq.cn/Article/details/gmalzkeaz.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.hesvh.cn/Article/details/grkofrubu.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.zdbjq.cn/Article/details/gjvasmfeg.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.hesvh.cn/Article/details/gbcfuivyh.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.zdbjq.cn/Article/details/gakwhhnhp.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.fehbvm.com/Article/details/gibzentaq.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.hesvh.cn/Article/details/ghvfnicmr.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.zdbjq.cn/Article/details/gimqnkclg.sHtML

[G10] 访问控制
来源：http://baike.fehbvm.com/Article/details/gnvujbhwq.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.hesvh.cn/Article/details/gbdzduuft.sHtML

PHP:  public / protected / private
来源：http://www.blog.hesvh.cn/Article/details/gsqbpafxh.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.zdbjq.cn/Article/details/gvhcolzmi.sHtML

TS:   public / protected / private
来源：http://blog.hesvh.cn/Article/details/gkgrophaq.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.fehbvm.com/Article/details/gghjuinwi.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.hesvh.cn/Article/details/ggxvtwfql.sHtML

Ruby: public / protected / private
来源：http://3g.hesvh.cn/Article/details/gmkihacrn.sHtML

C#:   public / protected / private / internal
来源：http://3g.hesvh.cn/Article/details/gaiggwmxx.sHtML

[G11] getter / setter
来源：http://blog.zdbjq.cn/Article/details/gjmdwsgrd.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.zdbjq.cn/Article/details/gszcwunsa.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.fehbvm.com/Article/details/gmcesmmgv.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.fehbvm.com/Article/details/geizblilu.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.fehbvm.com/Article/details/gctlgrhaz.sHtML

Java: public String getName() { return name; }
来源：http://wap.hesvh.cn/Article/details/gpggbrfwa.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.hesvh.cn/Article/details/gtibxsdkr.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.zdbjq.cn/Article/details/grlqnkkqz.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.fehbvm.com/Article/details/ggqskwqmx.sHtML

[G12] 对象转字符串
来源：http://www.blog.hesvh.cn/Article/details/gmrwulnsf.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.fehbvm.com/Article/details/gcvsccrmg.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.fehbvm.com/Article/details/gwpgioaey.sHtML

JS:   toString() { return this.name; }
来源：http://blog.fehbvm.com/Article/details/gyrpdjfnh.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/gzeoixniv.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.fehbvm.com/Article/details/gkjocckdc.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.hesvh.cn/Article/details/guounxwwi.sHtML

Ruby: def to_s; @name; end
来源：http://wap.zdbjq.cn/Article/details/gqkhrlhuz.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.hesvh.cn/Article/details/gvpljfchf.sHtML

[G13] 判断对象类型
来源：http://m.share.fehbvm.com/Article/details/gqlmmyilg.sHtML

Py:   isinstance(u, User)
来源：http://3g.zdbjq.cn/Article/details/gibjqhvdw.sHtML

PHP:  $u instanceof User
来源：http://baike.zdbjq.cn/Article/details/gvmzefbvu.sHtML

JS:   u instanceof User
来源：http://read.share.zdbjq.cn/Article/details/gupjlhhlg.sHtML

TS:   u instanceof User
来源：http://wap.zdbjq.cn/Article/details/gwtudythy.sHtML

Java: u instanceof User
来源：http://www.blog.zdbjq.cn/Article/details/gakuyppvi.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.hesvh.cn/Article/details/gnmivugwc.sHtML

Ruby: u.is_a?(User)
来源：http://3g.fehbvm.com/Article/details/gohcxxnvz.sHtML

C#:   u is User
来源：http://3g.zdbjq.cn/Article/details/geychiljx.sHtML

[G14] 数据类 / record
来源：http://m.share.hesvh.cn/Article/details/gxygtehyt.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.fehbvm.com/Article/details/gmvrbqdwl.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.fehbvm.com/Article/details/gizfixqpc.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.zdbjq.cn/Article/details/gvbkztrsq.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.fehbvm.com/Article/details/gclgskynn.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.fehbvm.com/Article/details/gtbsecysw.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.zdbjq.cn/Article/details/gvtdqjwqy.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.hesvh.cn/Article/details/gkstbjbld.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.fehbvm.com/Article/details/gmyzipgpr.sHtML

[G15] 枚举
来源：http://m.share.fehbvm.com/Article/details/gmygqtoxw.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.hesvh.cn/Article/details/gzeaeicvs.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.fehbvm.com/Article/details/gjtgupara.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.hesvh.cn/Article/details/gftnwexwy.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.fehbvm.com/Article/details/ghcgplqxr.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.zdbjq.cn/Article/details/gyqnldegi.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.hesvh.cn/Article/details/gunfeivww.sHtML

Ruby: Color = %i[red green].freeze
来源：http://m.share.fehbvm.com/Article/details/grptojmbt.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.fehbvm.com/Article/details/gqwytnmrj.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.hesvh.cn/Article/details/gwhmihsug.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.zdbjq.cn/Article/details/gxnxsbqeu.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.zdbjq.cn/Article/details/gjcnsqmaf.sHtML

JS:   Object.entries(obj)
来源：http://mobile.zdbjq.cn/Article/details/gvqlvgtoy.sHtML

TS:   Object.entries(obj)
来源：http://blog.fehbvm.com/Article/details/ggebwggws.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://m.share.fehbvm.com/Article/details/gsykbnhgs.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.hesvh.cn/Article/details/gcfohwovd.sHtML

Ruby: obj.instance_variables
来源：http://baike.hesvh.cn/Article/details/gldtuwzjt.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.zdbjq.cn/Article/details/ghptkhpco.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gzkylnkid.sHtML

H. 异常与错误处理
来源：http://blog.hesvh.cn/Article/details/gtkdvrpeb.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gbkgufcaw.sHtML

[H01] try / catch 基础
来源：http://3g.hesvh.cn/Article/details/gpatbwvks.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.fehbvm.com/Article/details/gywimdbrd.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.blog.hesvh.cn/Article/details/gxrgatcye.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.hesvh.cn/Article/details/gcoqzxsyo.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mobile.fehbvm.com/Article/details/glyptzaae.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.share.fehbvm.com/Article/details/gkxlblwix.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mobile.hesvh.cn/Article/details/gylbgtqtr.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.fehbvm.com/Article/details/gmzyuiabx.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.hesvh.cn/Article/details/ganafduof.sHtML

[H02] finally / ensure 收尾
来源：http://wap.hesvh.cn/Article/details/gmzzhpvvt.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.m.share.fehbvm.com/Article/details/gopcmhdyb.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/ghovjlupf.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://blog.hesvh.cn/Article/details/gqqwmbzzh.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.hesvh.cn/Article/details/gqyypuqie.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://mobile.zdbjq.cn/Article/details/ghevfepfa.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://read.share.zdbjq.cn/Article/details/geprctwox.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.hesvh.cn/Article/details/gnusqcbdl.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://baike.fehbvm.com/Article/details/gkmnchcwt.sHtML

[H03] 主动抛出异常
来源：http://baike.hesvh.cn/Article/details/gsryqlhfo.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.share.fehbvm.com/Article/details/gkxkaqyxg.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://3g.hesvh.cn/Article/details/guyhjqsit.sHtML

JS:   throw new Error("错误信息");
来源：http://wap.fehbvm.com/Article/details/gkgztcrmv.sHtML

TS:   throw new Error("错误信息");
来源：http://baike.fehbvm.com/Article/details/gdzraxnbm.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://read.share.hesvh.cn/Article/details/gktlccznk.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.zdbjq.cn/Article/details/gemousmck.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.blog.fehbvm.com/Article/details/geugaakai.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.m.share.zdbjq.cn/Article/details/gjkfyezsb.sHtML

[H04] 自定义异常类型
来源：http://www.blog.zdbjq.cn/Article/details/gybixrapl.sHtML

Py:   class MyError(Exception): pass
来源：http://read.share.fehbvm.com/Article/details/giolnrnmh.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.hesvh.cn/Article/details/gzliykpeb.sHtML

JS:   class MyError extends Error {}
来源：http://baike.hesvh.cn/Article/details/ggpckusmy.sHtML

TS:   class MyError extends Error {}
来源：http://read.share.hesvh.cn/Article/details/ggkazxiut.sHtML

Java: class MyException extends RuntimeException {}
来源：http://mobile.hesvh.cn/Article/details/gzshacyry.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://read.share.zdbjq.cn/Article/details/glfrgrdrf.sHtML

Ruby: class MyError < StandardError; end
来源：http://m.share.hesvh.cn/Article/details/gdvaszvvk.sHtML

C#:   class MyException : Exception {}
来源：http://3g.zdbjq.cn/Article/details/gkjhtdsqe.sHtML

[H05] 捕获特定类型
来源：http://www.share.fehbvm.com/Article/details/gxwyshdai.sHtML

Py:   except ValueError as e:
来源：http://read.share.fehbvm.com/Article/details/gtjuyarsh.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.m.share.fehbvm.com/Article/details/gtddmvirp.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://mobile.zdbjq.cn/Article/details/gawvotfvx.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.blog.zdbjq.cn/Article/details/glmjcisjo.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.zdbjq.cn/Article/details/gzdnazxul.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.share.zdbjq.cn/Article/details/gqfmsjyhy.sHtML

Ruby: rescue ArgumentError => e
来源：http://wap.hesvh.cn/Article/details/gkrulbuhy.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mobile.zdbjq.cn/Article/details/gfncqmpbz.sHtML

[H06] 可选值 / 空值安全访问
来源：http://mobile.fehbvm.com/Article/details/gtwpbtrfm.sHtML

Py:   value = d.get("k") or default
来源：http://blog.zdbjq.cn/Article/details/gnewummya.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.zdbjq.cn/Article/details/ggdqktfby.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://3g.zdbjq.cn/Article/details/gtdcljkwh.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.blog.fehbvm.com/Article/details/gftygshnp.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wap.fehbvm.com/Article/details/gegqgnace.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://blog.fehbvm.com/Article/details/gwewpttfd.sHtML

Ruby: d&.dig(:a, :b)
来源：http://m.share.hesvh.cn/Article/details/gcupughyg.sHtML

C#:   obj?.A?.B ?? default
来源：http://mobile.zdbjq.cn/Article/details/gvtujrhtz.sHtML

[H07] 断言
来源：http://www.share.hesvh.cn/Article/details/gikdnphlp.sHtML

Py:   assert x > 0, "必须为正"
来源：http://m.share.zdbjq.cn/Article/details/gehgmgmph.sHtML

PHP:  assert($x > 0);
来源：http://blog.zdbjq.cn/Article/details/gnqfypzfu.sHtML

JS:   console.assert(x > 0);
来源：http://wap.zdbjq.cn/Article/details/gegtfhqtu.sHtML

TS:   console.assert(x > 0);
来源：http://www.share.hesvh.cn/Article/details/garjawghc.sHtML

Java: assert x > 0 : "必须为正";
来源：http://wap.hesvh.cn/Article/details/gjmtthihq.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.share.zdbjq.cn/Article/details/gjghecqys.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://wap.fehbvm.com/Article/details/gvhavugeh.sHtML

C#:   Debug.Assert(x > 0);
来源：http://baike.fehbvm.com/Article/details/gzzqydpxc.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.m.share.hesvh.cn/Article/details/gxmbcfiyd.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://m.share.hesvh.cn/Article/details/goencazqx.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://baike.hesvh.cn/Article/details/gvobnuthc.sHtML

JS:   e.message;  e.stack
来源：http://www.share.fehbvm.com/Article/details/gjmkzcbdl.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.m.share.hesvh.cn/Article/details/gfhroxunl.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.blog.hesvh.cn/Article/details/gwvzxttbw.sHtML

Go:   err.Error()
来源：http://baike.fehbvm.com/Article/details/gxfpriowf.sHtML

Ruby: e.message;  e.backtrace
来源：http://3g.zdbjq.cn/Article/details/gbyboyxmp.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.blog.hesvh.cn/Article/details/gxobwwiju.sHtML

[H09] 带错误码的异常
来源：http://mobile.hesvh.cn/Article/details/gvlvyadff.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://read.share.hesvh.cn/Article/details/glltwcwxi.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://3g.zdbjq.cn/Article/details/gjnvchzsy.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.share.hesvh.cn/Article/details/gzqsbaoxw.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://baike.zdbjq.cn/Article/details/gaagxztpj.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mobile.hesvh.cn/Article/details/gvyllblej.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://m.share.fehbvm.com/Article/details/grkinmyee.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://3g.zdbjq.cn/Article/details/gwmjjmeof.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://read.share.zdbjq.cn/Article/details/gwwfdhrkd.sHtML

[H10] 资源自动释放
来源：http://3g.zdbjq.cn/Article/details/gcmqfhmkh.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://3g.fehbvm.com/Article/details/gyqdilrea.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://3g.fehbvm.com/Article/details/gtjcqlejc.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.hesvh.cn/Article/details/geudrqlwq.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.zdbjq.cn/Article/details/gzgzwxlqc.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.blog.hesvh.cn/Article/details/gujndyxiz.sHtML

Go:   defer f.Close()
来源：http://www.blog.fehbvm.com/Article/details/gpnwqtxyy.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://read.share.fehbvm.com/Article/details/gttwexafa.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wap.fehbvm.com/Article/details/gkhqujbkp.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gjlnlrozu.sHtML

I. 正则表达式
来源：http://www.m.share.hesvh.cn/Article/details/gsxhgffnt.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gsiflwzgv.sHtML

[I01] 判断是否匹配
来源：http://wap.zdbjq.cn/Article/details/gemfqhjcv.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://blog.hesvh.cn/Article/details/gfmcbtcoo.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://3g.zdbjq.cn/Article/details/gklrvpkel.sHtML

JS:   /\d+/.test(s)
来源：http://wap.hesvh.cn/Article/details/gyfknlnpl.sHtML

TS:   /\d+/.test(s)
来源：http://www.share.fehbvm.com/Article/details/gikacgphv.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://m.share.zdbjq.cn/Article/details/gbrwfbozr.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mobile.zdbjq.cn/Article/details/gyumoexyj.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.m.share.zdbjq.cn/Article/details/gtlictyao.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://baike.hesvh.cn/Article/details/ggsymxukp.sHtML

[I02] 提取所有匹配
来源：http://blog.hesvh.cn/Article/details/ghxsmmyxp.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.share.zdbjq.cn/Article/details/gmwnxthtc.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://3g.zdbjq.cn/Article/details/gzcmjcigz.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.blog.fehbvm.com/Article/details/ghurjwbpb.sHtML

TS:   s.match(/\d+/g)
来源：http://blog.hesvh.cn/Article/details/gfbfdqhbt.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://3g.zdbjq.cn/Article/details/gcsyhsolv.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://read.share.zdbjq.cn/Article/details/gspqtoglh.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.blog.hesvh.cn/Article/details/grtpaonee.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://blog.hesvh.cn/Article/details/gbbyhzyee.sHtML

[I03] 提取捕获分组
来源：http://mobile.zdbjq.cn/Article/details/grbjzlrru.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://m.share.fehbvm.com/Article/details/guoggzsfe.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.m.share.zdbjq.cn/Article/details/gxhiovuql.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://3g.zdbjq.cn/Article/details/gsfspqmxj.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wap.zdbjq.cn/Article/details/gciojewhu.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wap.zdbjq.cn/Article/details/gywifokqz.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.m.share.fehbvm.com/Article/details/gavfrtzog.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wap.hesvh.cn/Article/details/grmclmcxn.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.blog.zdbjq.cn/Article/details/gtqieqabk.sHtML

[I04] 正则替换
来源：http://read.share.fehbvm.com/Article/details/gdobcovvf.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.m.share.fehbvm.com/Article/details/gkccsbouc.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://read.share.fehbvm.com/Article/details/gbykrsfkj.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.fehbvm.com/Article/details/gpuntitwr.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://wap.fehbvm.com/Article/details/ggwprxrfr.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://read.share.fehbvm.com/Article/details/gzjampdli.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.m.share.fehbvm.com/Article/details/ggdshycco.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://mobile.zdbjq.cn/Article/details/gyzchdjxb.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://read.share.hesvh.cn/Article/details/gtahyjllu.sHtML

[I05] 按正则拆分
来源：http://read.share.hesvh.cn/Article/details/gblgliduv.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://baike.fehbvm.com/Article/details/gjdqrduiu.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://read.share.hesvh.cn/Article/details/gcffiggga.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.share.zdbjq.cn/Article/details/glgzzjwir.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://mobile.zdbjq.cn/Article/details/gfkueawmv.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.m.share.hesvh.cn/Article/details/ginntgupf.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://read.share.hesvh.cn/Article/details/gcordidkd.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.m.share.fehbvm.com/Article/details/gheusttpt.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://read.share.fehbvm.com/Article/details/gtkuhcrij.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mobile.fehbvm.com/Article/details/ggpsiydlp.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.m.share.zdbjq.cn/Article/details/gfgrfgimg.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://3g.hesvh.cn/Article/details/gvysxjlrg.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.zdbjq.cn/Article/details/gmvebfonj.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.fehbvm.com/Article/details/gqzqamxpo.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wap.hesvh.cn/Article/details/gfrnrjmvw.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://read.share.fehbvm.com/Article/details/gnicytutb.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.share.fehbvm.com/Article/details/gkfqcengd.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://m.share.hesvh.cn/Article/details/gneiysqbb.sHtML

[I07] 忽略大小写与多行模式
来源：http://baike.zdbjq.cn/Article/details/gywaadwwb.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://read.share.fehbvm.com/Article/details/gealvuynm.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://3g.hesvh.cn/Article/details/gkmunypgm.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://baike.hesvh.cn/Article/details/gddeuochi.sHtML

TS:   /error/gim
来源：http://read.share.zdbjq.cn/Article/details/ggconhbcv.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.blog.fehbvm.com/Article/details/giekptqgo.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://read.share.zdbjq.cn/Article/details/ghdinaoxq.sHtML

Ruby: s.scan(/error/i)
来源：http://baike.zdbjq.cn/Article/details/glxmvylwv.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://m.share.zdbjq.cn/Article/details/gumtbppoa.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.share.hesvh.cn/Article/details/gvaepcoop.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://blog.zdbjq.cn/Article/details/gdyuuywbe.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mobile.hesvh.cn/Article/details/gwmjfkfbd.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.zdbjq.cn/Article/details/grnaeffoh.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.fehbvm.com/Article/details/gavblvjwy.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://m.share.fehbvm.com/Article/details/gxflijldk.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://mobile.hesvh.cn/Article/details/gxowqjpwo.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wap.fehbvm.com/Article/details/glomvtdmw.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://3g.zdbjq.cn/Article/details/gbqpmwkwy.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gtjvndwtp.sHtML

J. 日期与时间
来源：http://www.share.hesvh.cn/Article/details/gqqcujaif.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gvgfxcgww.sHtML

[J01] 获取当前时间
来源：http://www.m.share.fehbvm.com/Article/details/goowawnhv.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.blog.hesvh.cn/Article/details/gbobshift.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://wap.hesvh.cn/Article/details/gnbktntao.sHtML

JS:   new Date();  Date.now()
来源：http://blog.fehbvm.com/Article/details/gzusgllfl.sHtML

TS:   new Date();  Date.now()
来源：http://wap.zdbjq.cn/Article/details/gyfjoucev.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.share.hesvh.cn/Article/details/gheacozqz.sHtML

Go:   time.Now()
来源：http://wap.fehbvm.com/Article/details/gzfcoiskf.sHtML

Ruby: Time.now
来源：http://read.share.zdbjq.cn/Article/details/grjoigiyr.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://mobile.fehbvm.com/Article/details/graamkzhj.sHtML

[J02] 格式化输出
来源：http://www.blog.hesvh.cn/Article/details/gkwvehvsa.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.fehbvm.com/Article/details/gapldbanv.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://3g.hesvh.cn/Article/details/gkmkmjwce.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.blog.hesvh.cn/Article/details/gnuaitgwa.sHtML

TS:   d.toISOString()
来源：http://m.share.fehbvm.com/Article/details/gvqpctaar.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://baike.zdbjq.cn/Article/details/gbnjdgtfw.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://read.share.fehbvm.com/Article/details/gdcftpitl.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.hesvh.cn/Article/details/gntwvkwiu.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://read.share.hesvh.cn/Article/details/gexnoxoor.sHtML

[J03] 字符串解析为日期
来源：http://www.share.zdbjq.cn/Article/details/gortyrzex.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.share.hesvh.cn/Article/details/gvslfhrlx.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://read.share.zdbjq.cn/Article/details/gajmpofax.sHtML

JS:   new Date("2024-01-02")
来源：http://wap.hesvh.cn/Article/details/gmjjczjro.sHtML

TS:   new Date("2024-01-02")
来源：http://3g.fehbvm.com/Article/details/gmuqybapn.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://blog.zdbjq.cn/Article/details/gcbftceku.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.share.zdbjq.cn/Article/details/gkjrkomxv.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://wap.fehbvm.com/Article/details/gkwghhorg.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wap.hesvh.cn/Article/details/gonslhjwt.sHtML

[J04] 时间戳与日期互转
来源：http://3g.fehbvm.com/Article/details/ghwdbvbqm.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://baike.fehbvm.com/Article/details/gnbjdkwsq.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wap.zdbjq.cn/Article/details/geqhvkwgq.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.blog.zdbjq.cn/Article/details/gmoywqanf.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://m.share.fehbvm.com/Article/details/guyscduml.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://mobile.zdbjq.cn/Article/details/goewuqfak.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://blog.zdbjq.cn/Article/details/gsqzuizio.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://baike.zdbjq.cn/Article/details/gmwequeej.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://mobile.hesvh.cn/Article/details/gfhqjxflv.sHtML

[J05] 时间加减（加 7 天）
来源：http://mobile.fehbvm.com/Article/details/gnpcjdqqb.sHtML

Py:   now + timedelta(days=7)
来源：http://m.share.hesvh.cn/Article/details/gifhchtlf.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://baike.fehbvm.com/Article/details/gvwjmiodc.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.fehbvm.com/Article/details/gwrdfydnh.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.hesvh.cn/Article/details/gdbnmojyx.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://wap.fehbvm.com/Article/details/gmwaevkfh.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://blog.zdbjq.cn/Article/details/gaxhiylzn.sHtML

Ruby: Time.now + 7 * 86400
来源：http://m.share.zdbjq.cn/Article/details/gqplnuxlb.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://3g.hesvh.cn/Article/details/gxixkkxep.sHtML

[J06] 计算两时间之差
来源：http://read.share.hesvh.cn/Article/details/gxxikjisv.sHtML

Py:   (end - start).total_seconds()
来源：http://www.m.share.zdbjq.cn/Article/details/gnhkogvam.sHtML

PHP:  $end->diff($start)->days;
来源：http://mobile.zdbjq.cn/Article/details/grjqhglgp.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.m.share.hesvh.cn/Article/details/gtgoumzcj.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.share.hesvh.cn/Article/details/gjbfrbonr.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://mobile.fehbvm.com/Article/details/gmfbzyaus.sHtML

Go:   end.Sub(start).Hours()
来源：http://mobile.fehbvm.com/Article/details/gxwhuryns.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.m.share.hesvh.cn/Article/details/geieecxjh.sHtML

C#:   (end - start).TotalSeconds
来源：http://read.share.hesvh.cn/Article/details/gwmnzoksq.sHtML


<!-- 参考信息 -->