代发 wailian999

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.fehbvm.com/Article/details/getxlopwq.sHtML

Ruby: def self.f; end
来源：http://3g.hesvh.cn/Article/details/gwddzlolx.sHtML

C#:   public static void F() {}
来源：http://mobile.fehbvm.com/Article/details/glbmvlysa.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.fehbvm.com/Article/details/gylkxwxqc.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.fehbvm.com/Article/details/gxxhmigpn.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.zdbjq.cn/Article/details/gcgtiaxvi.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.hesvh.cn/Article/details/gpvonwaej.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.fehbvm.com/Article/details/gsnkozlkt.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.fehbvm.com/Article/details/ginytluoa.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.zdbjq.cn/Article/details/gvxeifgul.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.zdbjq.cn/Article/details/gvbnlqwjj.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.fehbvm.com/Article/details/gttyibvev.sHtML

[G10] 访问控制
来源：http://baike.zdbjq.cn/Article/details/ghhmxgwjn.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.zdbjq.cn/Article/details/gimnpzwal.sHtML

PHP:  public / protected / private
来源：http://mobile.hesvh.cn/Article/details/girgwxnml.sHtML

JS:   #private 字段；其余公开
来源：http://3g.fehbvm.com/Article/details/gxogbdomr.sHtML

TS:   public / protected / private
来源：http://mobile.fehbvm.com/Article/details/gjextjzem.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.hesvh.cn/Article/details/gwbnometh.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.zdbjq.cn/Article/details/grmfrxfwk.sHtML

Ruby: public / protected / private
来源：http://www.blog.hesvh.cn/Article/details/guxxyfrgj.sHtML

C#:   public / protected / private / internal
来源：http://wap.fehbvm.com/Article/details/gagafmpyo.sHtML

[G11] getter / setter
来源：http://blog.zdbjq.cn/Article/details/ghwetnkgu.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.hesvh.cn/Article/details/ghzokivkh.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.fehbvm.com/Article/details/grejyfyrx.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.zdbjq.cn/Article/details/gydkskcrv.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.hesvh.cn/Article/details/gngxtzwrv.sHtML

Java: public String getName() { return name; }
来源：http://mobile.fehbvm.com/Article/details/gfyksrtol.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.zdbjq.cn/Article/details/gcmxmywwu.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.fehbvm.com/Article/details/gfclovovb.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.zdbjq.cn/Article/details/gyvttfags.sHtML

[G12] 对象转字符串
来源：http://baike.zdbjq.cn/Article/details/gwbtiacgm.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.zdbjq.cn/Article/details/giuhvojdl.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.zdbjq.cn/Article/details/gnywicjai.sHtML

JS:   toString() { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/grwilrept.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/gjxpodbqn.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.zdbjq.cn/Article/details/gksgzrygb.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.zdbjq.cn/Article/details/gucoiaaia.sHtML

Ruby: def to_s; @name; end
来源：http://wap.hesvh.cn/Article/details/ggipwzira.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.fehbvm.com/Article/details/gbcyqvocy.sHtML

[G13] 判断对象类型
来源：http://www.blog.fehbvm.com/Article/details/gozdttykw.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.hesvh.cn/Article/details/gmubjvamb.sHtML

PHP:  $u instanceof User
来源：http://wap.fehbvm.com/Article/details/gmxupvuyh.sHtML

JS:   u instanceof User
来源：http://read.share.zdbjq.cn/Article/details/gfyxjhfdj.sHtML

TS:   u instanceof User
来源：http://m.share.hesvh.cn/Article/details/ghpzimupe.sHtML

Java: u instanceof User
来源：http://www.share.hesvh.cn/Article/details/gqlakhiqj.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.fehbvm.com/Article/details/gntcnfryw.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.zdbjq.cn/Article/details/gxmjndmsn.sHtML

C#:   u is User
来源：http://blog.fehbvm.com/Article/details/gfvtsyzmo.sHtML

[G14] 数据类 / record
来源：http://wap.hesvh.cn/Article/details/gstyosddu.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.fehbvm.com/Article/details/gqdzkiahz.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://read.share.fehbvm.com/Article/details/gezukeyba.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.hesvh.cn/Article/details/gvrhfktas.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.share.zdbjq.cn/Article/details/gynqsvfum.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.hesvh.cn/Article/details/gmecizyus.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.zdbjq.cn/Article/details/gpzbtpjvv.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.hesvh.cn/Article/details/gsjvrgkjt.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.hesvh.cn/Article/details/ggdlhhuso.sHtML

[G15] 枚举
来源：http://baike.zdbjq.cn/Article/details/gxiiliilm.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.fehbvm.com/Article/details/gxeuieyio.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.hesvh.cn/Article/details/gzsjyidzl.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.hesvh.cn/Article/details/gmsmdqfoo.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.zdbjq.cn/Article/details/gjxqmcabx.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.zdbjq.cn/Article/details/gjiesttoy.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.hesvh.cn/Article/details/grampytqw.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.hesvh.cn/Article/details/gnxjnyxti.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.hesvh.cn/Article/details/gsvyilsmd.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.fehbvm.com/Article/details/gyjoklirx.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.fehbvm.com/Article/details/gkodkbhss.sHtML

PHP:  get_object_vars($obj);
来源：http://wap.fehbvm.com/Article/details/ggcmvnxhw.sHtML

JS:   Object.entries(obj)
来源：http://baike.zdbjq.cn/Article/details/gghrhphar.sHtML

TS:   Object.entries(obj)
来源：http://mobile.hesvh.cn/Article/details/gvbgaqdld.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://blog.fehbvm.com/Article/details/gnuhpcnzx.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.fehbvm.com/Article/details/gpoavemev.sHtML

Ruby: obj.instance_variables
来源：http://m.share.fehbvm.com/Article/details/gfyawqxfx.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.hesvh.cn/Article/details/ghvwxgogw.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gogyzfjde.sHtML

H. 异常与错误处理
来源：http://baike.hesvh.cn/Article/details/gqvhcwzoq.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gpcyrhgyk.sHtML

[H01] try / catch 基础
来源：http://m.share.zdbjq.cn/Article/details/gfvhqctlq.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.fehbvm.com/Article/details/grvrragbu.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.blog.zdbjq.cn/Article/details/gwimoddje.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.hesvh.cn/Article/details/gxoxkgfmd.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.blog.zdbjq.cn/Article/details/ghfgjkapq.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.share.fehbvm.com/Article/details/gfmhzwyor.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://m.share.hesvh.cn/Article/details/gfxisqgtj.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.fehbvm.com/Article/details/gbnrzirjd.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://baike.hesvh.cn/Article/details/gvcjdaowy.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.zdbjq.cn/Article/details/gqsfabpmx.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.zdbjq.cn/Article/details/ggwixuqqv.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.blog.hesvh.cn/Article/details/glsukmfio.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/gpwldxkyf.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://blog.hesvh.cn/Article/details/gqgqlyoxs.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://wap.hesvh.cn/Article/details/geczfsugm.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://3g.fehbvm.com/Article/details/gmrymwwnw.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://blog.hesvh.cn/Article/details/gzhctmrlw.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://mobile.zdbjq.cn/Article/details/goaqdiwkp.sHtML

[H03] 主动抛出异常
来源：http://wap.hesvh.cn/Article/details/gvhibhptb.sHtML

Py:   raise ValueError("错误信息")
来源：http://wap.hesvh.cn/Article/details/gixvlvtgs.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://3g.zdbjq.cn/Article/details/gmyzjivkr.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.zdbjq.cn/Article/details/gkcarrifa.sHtML

TS:   throw new Error("错误信息");
来源：http://www.share.fehbvm.com/Article/details/gqzfmuchr.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://mobile.hesvh.cn/Article/details/gxuciwgwa.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.share.zdbjq.cn/Article/details/gqepsyphr.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.hesvh.cn/Article/details/ggxgbihso.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.share.fehbvm.com/Article/details/gnveaintv.sHtML

[H04] 自定义异常类型
来源：http://m.share.zdbjq.cn/Article/details/gflspsacf.sHtML

Py:   class MyError(Exception): pass
来源：http://www.share.hesvh.cn/Article/details/gjmxnlmon.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.m.share.fehbvm.com/Article/details/gxjgbjgkv.sHtML

JS:   class MyError extends Error {}
来源：http://baike.zdbjq.cn/Article/details/gyejlxduz.sHtML

TS:   class MyError extends Error {}
来源：http://baike.fehbvm.com/Article/details/gkuryikch.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.m.share.zdbjq.cn/Article/details/gadnuatjn.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.hesvh.cn/Article/details/gpmofoyaa.sHtML

Ruby: class MyError < StandardError; end
来源：http://blog.hesvh.cn/Article/details/gisqrdumm.sHtML

C#:   class MyException : Exception {}
来源：http://3g.fehbvm.com/Article/details/gtsjgllxu.sHtML

[H05] 捕获特定类型
来源：http://www.share.hesvh.cn/Article/details/gpygbjdia.sHtML

Py:   except ValueError as e:
来源：http://3g.zdbjq.cn/Article/details/grzvfyumw.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://blog.zdbjq.cn/Article/details/gibwocdvb.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://mobile.fehbvm.com/Article/details/gfcfjbyrv.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://m.share.fehbvm.com/Article/details/gdzwkwkcp.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://wap.fehbvm.com/Article/details/glkgnyqud.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://baike.hesvh.cn/Article/details/glzoeqwwf.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.hesvh.cn/Article/details/gnrjsgdjo.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wap.zdbjq.cn/Article/details/gktfwbyeb.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.m.share.zdbjq.cn/Article/details/gimgvkohd.sHtML

Py:   value = d.get("k") or default
来源：http://blog.fehbvm.com/Article/details/ggsrovmtw.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.m.share.hesvh.cn/Article/details/geytyfqff.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.fehbvm.com/Article/details/ggylcixeo.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.blog.hesvh.cn/Article/details/gfoifaank.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.blog.hesvh.cn/Article/details/ghcsijaqv.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://baike.fehbvm.com/Article/details/gkuduzdmp.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.m.share.zdbjq.cn/Article/details/glyooaxfv.sHtML

C#:   obj?.A?.B ?? default
来源：http://baike.fehbvm.com/Article/details/gsuieetic.sHtML

[H07] 断言
来源：http://baike.fehbvm.com/Article/details/guepoxogn.sHtML

Py:   assert x > 0, "必须为正"
来源：http://mobile.zdbjq.cn/Article/details/gohrjpjra.sHtML

PHP:  assert($x > 0);
来源：http://blog.fehbvm.com/Article/details/gdfftifop.sHtML

JS:   console.assert(x > 0);
来源：http://baike.zdbjq.cn/Article/details/gamiyfbyb.sHtML

TS:   console.assert(x > 0);
来源：http://wap.zdbjq.cn/Article/details/gsgvijsyq.sHtML

Java: assert x > 0 : "必须为正";
来源：http://m.share.fehbvm.com/Article/details/gwommiyef.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.m.share.fehbvm.com/Article/details/gsqwwyyfl.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://baike.hesvh.cn/Article/details/guqeexovl.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.share.hesvh.cn/Article/details/gyicraxkg.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.blog.hesvh.cn/Article/details/gqjhdsgay.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://mobile.zdbjq.cn/Article/details/gqtfwbcmv.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.m.share.zdbjq.cn/Article/details/gtqmxumti.sHtML

JS:   e.message;  e.stack
来源：http://blog.hesvh.cn/Article/details/gqqxuutet.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://blog.hesvh.cn/Article/details/grhatdzuo.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://mobile.hesvh.cn/Article/details/gdncocxev.sHtML

Go:   err.Error()
来源：http://mobile.hesvh.cn/Article/details/gjorxrash.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.m.share.fehbvm.com/Article/details/gviilbyma.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.m.share.zdbjq.cn/Article/details/grqpxrbdb.sHtML

[H09] 带错误码的异常
来源：http://www.share.hesvh.cn/Article/details/gpuflvlxi.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.blog.fehbvm.com/Article/details/gwvlzuzwj.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.blog.fehbvm.com/Article/details/gogvqrlvl.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://blog.hesvh.cn/Article/details/gcfqpvton.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.blog.hesvh.cn/Article/details/gynhgrpiu.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mobile.fehbvm.com/Article/details/gvpodojhb.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://3g.fehbvm.com/Article/details/gcaqgskbe.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://3g.fehbvm.com/Article/details/gdgraibdl.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.share.hesvh.cn/Article/details/gorvftyus.sHtML

[H10] 资源自动释放
来源：http://blog.zdbjq.cn/Article/details/ggetjvsjf.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://m.share.zdbjq.cn/Article/details/gasdyraua.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wap.hesvh.cn/Article/details/ghwrrbjtb.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.hesvh.cn/Article/details/gtbmmohry.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.fehbvm.com/Article/details/gobhmeshs.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.m.share.hesvh.cn/Article/details/goayxzdje.sHtML

Go:   defer f.Close()
来源：http://m.share.hesvh.cn/Article/details/gzgvjekvq.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mobile.hesvh.cn/Article/details/gicslqwoa.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/goxghledn.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gkrnlmfwk.sHtML

I. 正则表达式
来源：http://www.blog.zdbjq.cn/Article/details/ghjzrukqi.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/grxdzfilu.sHtML

[I01] 判断是否匹配
来源：http://blog.hesvh.cn/Article/details/gkauaymom.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://baike.zdbjq.cn/Article/details/guygiizoh.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://mobile.hesvh.cn/Article/details/gixtiepmc.sHtML

JS:   /\d+/.test(s)
来源：http://www.share.hesvh.cn/Article/details/gwgclzrxm.sHtML

TS:   /\d+/.test(s)
来源：http://m.share.zdbjq.cn/Article/details/gnahvkhkx.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wap.fehbvm.com/Article/details/gxuorlvlf.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.m.share.fehbvm.com/Article/details/gtxjhuihk.sHtML

Ruby: s.match?(/\d+/)
来源：http://blog.hesvh.cn/Article/details/gldjaxjhk.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://blog.hesvh.cn/Article/details/gujqkexuk.sHtML

[I02] 提取所有匹配
来源：http://www.share.zdbjq.cn/Article/details/gwmrkrdqn.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.share.hesvh.cn/Article/details/gyxfdijdi.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://read.share.fehbvm.com/Article/details/gmyopmdny.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://baike.hesvh.cn/Article/details/gxsjplzde.sHtML

TS:   s.match(/\d+/g)
来源：http://www.m.share.zdbjq.cn/Article/details/gczdluzwf.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://3g.fehbvm.com/Article/details/gljtjhyqi.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.blog.zdbjq.cn/Article/details/gesydzwds.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.m.share.hesvh.cn/Article/details/ghbliyiiq.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://m.share.hesvh.cn/Article/details/gzpbobwsj.sHtML

[I03] 提取捕获分组
来源：http://read.share.hesvh.cn/Article/details/gdisxeldv.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wap.fehbvm.com/Article/details/gvtmaffvd.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.blog.fehbvm.com/Article/details/gbjngsgwa.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://read.share.hesvh.cn/Article/details/gsqvpmffm.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.blog.fehbvm.com/Article/details/gncfccaxf.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://blog.hesvh.cn/Article/details/gyuxgiyut.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://baike.fehbvm.com/Article/details/gwxaauszv.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.share.fehbvm.com/Article/details/giutcsblf.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.blog.zdbjq.cn/Article/details/ggqjozhqw.sHtML

[I04] 正则替换
来源：http://m.share.fehbvm.com/Article/details/gmyyocuaa.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://baike.fehbvm.com/Article/details/gsyjqawdb.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wap.hesvh.cn/Article/details/gnjodunzt.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://blog.hesvh.cn/Article/details/gnnycwtkh.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://wap.zdbjq.cn/Article/details/gwtibuumt.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.blog.zdbjq.cn/Article/details/gttsmedhl.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.blog.hesvh.cn/Article/details/gofwrizga.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://m.share.hesvh.cn/Article/details/gbkhqkynn.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://read.share.fehbvm.com/Article/details/gifberzzd.sHtML

[I05] 按正则拆分
来源：http://read.share.zdbjq.cn/Article/details/gwsmsbdke.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.m.share.fehbvm.com/Article/details/gxbvegmsn.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://baike.zdbjq.cn/Article/details/gbgbrvaxp.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://3g.fehbvm.com/Article/details/gbptpmhdl.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.m.share.fehbvm.com/Article/details/gzkbimqno.sHtML

Java: s.split("\\s*,\\s*")
来源：http://m.share.zdbjq.cn/Article/details/gvpawwffv.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.m.share.fehbvm.com/Article/details/gemuwlkwm.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.share.hesvh.cn/Article/details/goygccftd.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.m.share.zdbjq.cn/Article/details/gkimqcttg.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wap.hesvh.cn/Article/details/gjzxndroj.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://mobile.fehbvm.com/Article/details/gosvpwbem.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.m.share.hesvh.cn/Article/details/gdohbgadz.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.hesvh.cn/Article/details/gayjfflwg.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.zdbjq.cn/Article/details/gkyypqbza.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wap.zdbjq.cn/Article/details/gcntnhxsy.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://m.share.zdbjq.cn/Article/details/gdpfzvxnp.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://3g.fehbvm.com/Article/details/gzbaovuay.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.m.share.zdbjq.cn/Article/details/gkllprrbb.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.blog.fehbvm.com/Article/details/gozdfhdim.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wap.fehbvm.com/Article/details/gsckqflvz.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://read.share.hesvh.cn/Article/details/gccxoeftq.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://m.share.fehbvm.com/Article/details/gzqlaraah.sHtML

TS:   /error/gim
来源：http://read.share.zdbjq.cn/Article/details/gcaftmwtz.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://3g.fehbvm.com/Article/details/gqlrgfteq.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://3g.fehbvm.com/Article/details/ghjmunsmm.sHtML

Ruby: s.scan(/error/i)
来源：http://read.share.hesvh.cn/Article/details/gggqlxeyv.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.m.share.zdbjq.cn/Article/details/gxsdreayd.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://m.share.zdbjq.cn/Article/details/gcairphin.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://baike.hesvh.cn/Article/details/gjonuvitz.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.m.share.zdbjq.cn/Article/details/gqrievhlc.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.zdbjq.cn/Article/details/ggekmotbr.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.zdbjq.cn/Article/details/ggfoexzub.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://m.share.hesvh.cn/Article/details/gxegysmlr.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://mobile.zdbjq.cn/Article/details/gzsaqitqc.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://m.share.fehbvm.com/Article/details/gcynkidzb.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.m.share.zdbjq.cn/Article/details/giognfbdy.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gzrzyeexk.sHtML

J. 日期与时间
来源：http://wap.hesvh.cn/Article/details/gampwifuj.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gikygdhxa.sHtML

[J01] 获取当前时间
来源：http://m.share.hesvh.cn/Article/details/gutuxomda.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://blog.zdbjq.cn/Article/details/gchkvuief.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://wap.fehbvm.com/Article/details/gskzfqljh.sHtML

JS:   new Date();  Date.now()
来源：http://www.m.share.zdbjq.cn/Article/details/gabdlbjnl.sHtML

TS:   new Date();  Date.now()
来源：http://read.share.zdbjq.cn/Article/details/gomqamcmp.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.share.zdbjq.cn/Article/details/ggbsnhevi.sHtML

Go:   time.Now()
来源：http://3g.hesvh.cn/Article/details/gteptfcbl.sHtML

Ruby: Time.now
来源：http://baike.zdbjq.cn/Article/details/gzbvykaot.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.m.share.fehbvm.com/Article/details/ggchaapgp.sHtML

[J02] 格式化输出
来源：http://read.share.zdbjq.cn/Article/details/gpxzrykrd.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.hesvh.cn/Article/details/gqovqcldq.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.m.share.hesvh.cn/Article/details/gwrmeugha.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://blog.zdbjq.cn/Article/details/gkyifnkma.sHtML

TS:   d.toISOString()
来源：http://www.share.zdbjq.cn/Article/details/gozdmtryk.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://blog.hesvh.cn/Article/details/gqctabmks.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://m.share.zdbjq.cn/Article/details/gkesjlwot.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.hesvh.cn/Article/details/gnzkroymc.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.m.share.fehbvm.com/Article/details/gwoytkubb.sHtML

[J03] 字符串解析为日期
来源：http://www.m.share.fehbvm.com/Article/details/gincihiqn.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wap.hesvh.cn/Article/details/grepebeus.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wap.hesvh.cn/Article/details/gxkerrond.sHtML

JS:   new Date("2024-01-02")
来源：http://m.share.zdbjq.cn/Article/details/gjplpnnni.sHtML

TS:   new Date("2024-01-02")
来源：http://wap.hesvh.cn/Article/details/gqegrsfmb.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://read.share.fehbvm.com/Article/details/gpjowyigw.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://blog.zdbjq.cn/Article/details/gakexheaz.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://mobile.zdbjq.cn/Article/details/gagylrwha.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wap.fehbvm.com/Article/details/gsrknfrgt.sHtML

[J04] 时间戳与日期互转
来源：http://www.share.hesvh.cn/Article/details/gdjkvbycz.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://m.share.fehbvm.com/Article/details/grpehadah.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.m.share.fehbvm.com/Article/details/guofwsdzo.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://blog.fehbvm.com/Article/details/gvmesgojt.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.blog.zdbjq.cn/Article/details/gtffkvrmb.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://wap.zdbjq.cn/Article/details/girezmnyu.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wap.hesvh.cn/Article/details/genvgwfep.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mobile.hesvh.cn/Article/details/gxmshynfj.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://blog.hesvh.cn/Article/details/gweubnoyr.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.m.share.hesvh.cn/Article/details/gdcvxhoot.sHtML

Py:   now + timedelta(days=7)
来源：http://baike.zdbjq.cn/Article/details/guoxpxjmr.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://m.share.zdbjq.cn/Article/details/gzftnksux.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.zdbjq.cn/Article/details/gmhofmddo.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.fehbvm.com/Article/details/gzzmdihhf.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.share.fehbvm.com/Article/details/gunboadal.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.m.share.hesvh.cn/Article/details/gqdqfptft.sHtML

Ruby: Time.now + 7 * 86400
来源：http://wap.fehbvm.com/Article/details/gcteovtjn.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://m.share.hesvh.cn/Article/details/gjmokuteg.sHtML

[J06] 计算两时间之差
来源：http://read.share.hesvh.cn/Article/details/gpeiapyvd.sHtML

Py:   (end - start).total_seconds()
来源：http://www.m.share.fehbvm.com/Article/details/ghysotgzy.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.m.share.fehbvm.com/Article/details/gyrmolhzh.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://read.share.hesvh.cn/Article/details/ghdagqfmt.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://m.share.fehbvm.com/Article/details/gumywvnzh.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://wap.zdbjq.cn/Article/details/gsvmlipnt.sHtML

Go:   end.Sub(start).Hours()
来源：http://baike.fehbvm.com/Article/details/gciwuvrqd.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.m.share.zdbjq.cn/Article/details/gkstouxnl.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.m.share.hesvh.cn/Article/details/gwcsigiol.sHtML


<!-- 参考信息 -->