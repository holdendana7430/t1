代发 wailian999

Java: interface Shape { double area(); }
来源：http://www.m.share.fehbvm.com/Article/details/gzopeyzyf.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.zdbjq.cn/Article/details/glkunxjif.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.zdbjq.cn/Article/details/gtskuddxf.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.fehbvm.com/Article/details/gvutziqys.sHtML

[G10] 访问控制
来源：http://3g.hesvh.cn/Article/details/gadordoef.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.zdbjq.cn/Article/details/gcfsuxiaf.sHtML

PHP:  public / protected / private
来源：http://m.share.fehbvm.com/Article/details/gtvwwpmtx.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.hesvh.cn/Article/details/gkhtqvmzi.sHtML

TS:   public / protected / private
来源：http://www.share.hesvh.cn/Article/details/gnadmdzrq.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.fehbvm.com/Article/details/gvzzhjsgg.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.zdbjq.cn/Article/details/gwkvgpbsb.sHtML

Ruby: public / protected / private
来源：http://baike.zdbjq.cn/Article/details/giirpdsmz.sHtML

C#:   public / protected / private / internal
来源：http://blog.hesvh.cn/Article/details/gvyvolvxy.sHtML

[G11] getter / setter
来源：http://baike.fehbvm.com/Article/details/gfylfrqid.sHtML

Py:   @property 与 @x.setter
来源：http://baike.zdbjq.cn/Article/details/gsbgdmorp.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.zdbjq.cn/Article/details/gxybyszim.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.fehbvm.com/Article/details/ghffeuhqb.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.hesvh.cn/Article/details/gcjwvtghq.sHtML

Java: public String getName() { return name; }
来源：http://3g.hesvh.cn/Article/details/gnbftweuy.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.zdbjq.cn/Article/details/gibymlbig.sHtML

Ruby: attr_accessor :name
来源：http://mobile.hesvh.cn/Article/details/gjyemdocf.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.hesvh.cn/Article/details/ghxyankyo.sHtML

[G12] 对象转字符串
来源：http://www.blog.zdbjq.cn/Article/details/gxkfxoacb.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.hesvh.cn/Article/details/gyaqkpkdg.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.zdbjq.cn/Article/details/gfwfarnzl.sHtML

JS:   toString() { return this.name; }
来源：http://baike.fehbvm.com/Article/details/geiispywj.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.hesvh.cn/Article/details/gbsjmmaxo.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/gbgfmeian.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.fehbvm.com/Article/details/gcvfebhiw.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.zdbjq.cn/Article/details/gurjlcnwu.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.zdbjq.cn/Article/details/ggnkmajrh.sHtML

[G13] 判断对象类型
来源：http://mobile.zdbjq.cn/Article/details/gjtfqgfob.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.hesvh.cn/Article/details/gpfmxisll.sHtML

PHP:  $u instanceof User
来源：http://www.blog.zdbjq.cn/Article/details/ghademoia.sHtML

JS:   u instanceof User
来源：http://www.m.share.fehbvm.com/Article/details/gxrpwvggb.sHtML

TS:   u instanceof User
来源：http://m.share.hesvh.cn/Article/details/grsthxxai.sHtML

Java: u instanceof User
来源：http://www.m.share.hesvh.cn/Article/details/gmzresvaj.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.hesvh.cn/Article/details/gktkvduaz.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.hesvh.cn/Article/details/gfyufepxi.sHtML

C#:   u is User
来源：http://baike.zdbjq.cn/Article/details/gmekgmbmj.sHtML

[G14] 数据类 / record
来源：http://read.share.fehbvm.com/Article/details/gkgfsflqa.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.hesvh.cn/Article/details/gviuijhlg.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.hesvh.cn/Article/details/gzemrdotr.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.fehbvm.com/Article/details/gwxvvlysm.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.zdbjq.cn/Article/details/gsznrlyvb.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.zdbjq.cn/Article/details/guyuhrulp.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.zdbjq.cn/Article/details/glyyejoxg.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.fehbvm.com/Article/details/gqdyvypgw.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.hesvh.cn/Article/details/gzmrhwivu.sHtML

[G15] 枚举
来源：http://www.share.fehbvm.com/Article/details/gmovandxe.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.fehbvm.com/Article/details/gyyccxgkr.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.zdbjq.cn/Article/details/gerwtgamn.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mobile.fehbvm.com/Article/details/gkitmzfaz.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.fehbvm.com/Article/details/gpswzekey.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.hesvh.cn/Article/details/gdtzbzdtr.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.zdbjq.cn/Article/details/gfmoahzdd.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.zdbjq.cn/Article/details/gyacdnnao.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.hesvh.cn/Article/details/grddocizy.sHtML

[G16] 对象转数组 / 字典
来源：http://wap.hesvh.cn/Article/details/gpvaaetep.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.fehbvm.com/Article/details/gsunlcyfd.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.zdbjq.cn/Article/details/gpmtjvazq.sHtML

JS:   Object.entries(obj)
来源：http://www.share.zdbjq.cn/Article/details/gflixmtyj.sHtML

TS:   Object.entries(obj)
来源：http://mobile.hesvh.cn/Article/details/gmnfqkydx.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.share.hesvh.cn/Article/details/gsolznkrm.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.fehbvm.com/Article/details/glfqkvvhj.sHtML

Ruby: obj.instance_variables
来源：http://mobile.zdbjq.cn/Article/details/gsnzwvoyd.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.blog.fehbvm.com/Article/details/gfvpslzqi.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gbrsjrpbm.sHtML

H. 异常与错误处理
来源：http://read.share.hesvh.cn/Article/details/grxnlvohw.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gufaffhbn.sHtML

[H01] try / catch 基础
来源：http://3g.zdbjq.cn/Article/details/ghgbmulan.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.hesvh.cn/Article/details/grjnvlnvs.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.fehbvm.com/Article/details/grswonwce.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.share.hesvh.cn/Article/details/gpbdxhzdn.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mobile.fehbvm.com/Article/details/gnfqzjlsr.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.m.share.fehbvm.com/Article/details/grfkxmxwm.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://read.share.fehbvm.com/Article/details/gxnlqhbwx.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.fehbvm.com/Article/details/gdxmzxgss.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mobile.fehbvm.com/Article/details/gedufeguf.sHtML

[H02] finally / ensure 收尾
来源：http://www.m.share.hesvh.cn/Article/details/gtdlpfuru.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.hesvh.cn/Article/details/gukbfeuek.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.zdbjq.cn/Article/details/gwfpficje.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://m.share.zdbjq.cn/Article/details/gjccjzcpc.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://m.share.hesvh.cn/Article/details/gggqqxubc.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/gzebyxozk.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.zdbjq.cn/Article/details/gpvrfjfmj.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.hesvh.cn/Article/details/gjvfbouop.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.blog.zdbjq.cn/Article/details/gqbdggfve.sHtML

[H03] 主动抛出异常
来源：http://read.share.zdbjq.cn/Article/details/geemvautj.sHtML

Py:   raise ValueError("错误信息")
来源：http://baike.fehbvm.com/Article/details/gtdzhntuj.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.hesvh.cn/Article/details/gggylmzlc.sHtML

JS:   throw new Error("错误信息");
来源：http://wap.hesvh.cn/Article/details/gcvexdwbo.sHtML

TS:   throw new Error("错误信息");
来源：http://baike.zdbjq.cn/Article/details/gvdwaepko.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.hesvh.cn/Article/details/gushsindx.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://m.share.fehbvm.com/Article/details/gdbzkhrcm.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://wap.hesvh.cn/Article/details/grurylaox.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.fehbvm.com/Article/details/gxjcbnduo.sHtML

[H04] 自定义异常类型
来源：http://m.share.zdbjq.cn/Article/details/gxfmyoklf.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.fehbvm.com/Article/details/gwvoqrtvj.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://baike.zdbjq.cn/Article/details/gijhounwn.sHtML

JS:   class MyError extends Error {}
来源：http://wap.fehbvm.com/Article/details/gsmcgjtzo.sHtML

TS:   class MyError extends Error {}
来源：http://www.share.fehbvm.com/Article/details/gqmglngfv.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.m.share.hesvh.cn/Article/details/giajqthfv.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wap.zdbjq.cn/Article/details/gwhxhgekz.sHtML

Ruby: class MyError < StandardError; end
来源：http://read.share.fehbvm.com/Article/details/ggguieuxs.sHtML

C#:   class MyException : Exception {}
来源：http://www.blog.hesvh.cn/Article/details/gpzizxwiy.sHtML

[H05] 捕获特定类型
来源：http://read.share.hesvh.cn/Article/details/gctjbyzty.sHtML

Py:   except ValueError as e:
来源：http://wap.fehbvm.com/Article/details/gbjrjapli.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.hesvh.cn/Article/details/gokpbjlhh.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://3g.hesvh.cn/Article/details/gsgcljtcd.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://read.share.fehbvm.com/Article/details/grqdltlgt.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gdenissth.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wap.fehbvm.com/Article/details/ggmthxqjx.sHtML

Ruby: rescue ArgumentError => e
来源：http://wap.fehbvm.com/Article/details/gfecombjj.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mobile.zdbjq.cn/Article/details/gkqfvnnzr.sHtML

[H06] 可选值 / 空值安全访问
来源：http://mobile.fehbvm.com/Article/details/gjnobfllh.sHtML

Py:   value = d.get("k") or default
来源：http://blog.fehbvm.com/Article/details/gwysjtkny.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.m.share.zdbjq.cn/Article/details/gwfsoxuby.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.blog.hesvh.cn/Article/details/gvcyobult.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://blog.zdbjq.cn/Article/details/gvzwrxgcf.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://3g.hesvh.cn/Article/details/gezeazimp.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://3g.hesvh.cn/Article/details/golqdpvoi.sHtML

Ruby: d&.dig(:a, :b)
来源：http://blog.fehbvm.com/Article/details/gnfjrfnrx.sHtML

C#:   obj?.A?.B ?? default
来源：http://baike.fehbvm.com/Article/details/gtpqnizgb.sHtML

[H07] 断言
来源：http://www.m.share.fehbvm.com/Article/details/gvbclyfxp.sHtML

Py:   assert x > 0, "必须为正"
来源：http://read.share.hesvh.cn/Article/details/gcmjnzwjo.sHtML

PHP:  assert($x > 0);
来源：http://blog.hesvh.cn/Article/details/gkugkgmyg.sHtML

JS:   console.assert(x > 0);
来源：http://blog.hesvh.cn/Article/details/gohldvknp.sHtML

TS:   console.assert(x > 0);
来源：http://www.blog.hesvh.cn/Article/details/gqgnwtmfw.sHtML

Java: assert x > 0 : "必须为正";
来源：http://baike.zdbjq.cn/Article/details/gllnwkran.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://baike.fehbvm.com/Article/details/gkpdeenqp.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://blog.zdbjq.cn/Article/details/gfzjwumix.sHtML

C#:   Debug.Assert(x > 0);
来源：http://baike.zdbjq.cn/Article/details/gjmzozxct.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.blog.zdbjq.cn/Article/details/gojyssshd.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://baike.fehbvm.com/Article/details/gufftokbt.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.blog.zdbjq.cn/Article/details/gdcntxfqe.sHtML

JS:   e.message;  e.stack
来源：http://wap.zdbjq.cn/Article/details/gebtytoca.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.m.share.hesvh.cn/Article/details/gvtoaztsg.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://m.share.zdbjq.cn/Article/details/gpgabuzlr.sHtML

Go:   err.Error()
来源：http://www.share.fehbvm.com/Article/details/gccqjenwr.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.blog.hesvh.cn/Article/details/gybokrkha.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.share.fehbvm.com/Article/details/gzucitiar.sHtML

[H09] 带错误码的异常
来源：http://www.blog.hesvh.cn/Article/details/gvivnytwo.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://baike.hesvh.cn/Article/details/gqzkhwoxl.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://3g.fehbvm.com/Article/details/gsftzuqvj.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.m.share.hesvh.cn/Article/details/gqqzphacm.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://3g.zdbjq.cn/Article/details/gthradrax.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://3g.zdbjq.cn/Article/details/gppxazjlb.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://read.share.zdbjq.cn/Article/details/gtlaszudd.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://blog.hesvh.cn/Article/details/gkngrsfjw.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://3g.hesvh.cn/Article/details/gjnsjktmu.sHtML

[H10] 资源自动释放
来源：http://m.share.fehbvm.com/Article/details/gyyrqqxba.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://mobile.hesvh.cn/Article/details/gdbeflpba.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.blog.zdbjq.cn/Article/details/gjdmhnknq.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.zdbjq.cn/Article/details/gkvfgfgsi.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.zdbjq.cn/Article/details/gkjxsxvls.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://read.share.hesvh.cn/Article/details/gexocjhcu.sHtML

Go:   defer f.Close()
来源：http://read.share.hesvh.cn/Article/details/gsbtwawms.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://read.share.zdbjq.cn/Article/details/gcezbwvsf.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gyniadfoq.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gnywhmspz.sHtML

I. 正则表达式
来源：http://www.blog.fehbvm.com/Article/details/gzfdjvynx.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gtujaykyb.sHtML

[I01] 判断是否匹配
来源：http://mobile.zdbjq.cn/Article/details/goddawrch.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.blog.hesvh.cn/Article/details/gqkxilype.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://read.share.fehbvm.com/Article/details/ghuozzwxs.sHtML

JS:   /\d+/.test(s)
来源：http://www.share.hesvh.cn/Article/details/gklomfcpa.sHtML

TS:   /\d+/.test(s)
来源：http://read.share.fehbvm.com/Article/details/grfzlgyxv.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wap.hesvh.cn/Article/details/ggrixdmtw.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.m.share.fehbvm.com/Article/details/gqjcskdty.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.share.hesvh.cn/Article/details/gosepnstb.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.m.share.hesvh.cn/Article/details/gsljhxgye.sHtML

[I02] 提取所有匹配
来源：http://3g.fehbvm.com/Article/details/gwiiqgqcf.sHtML

Py:   re.findall(r"\d+", s)
来源：http://m.share.zdbjq.cn/Article/details/gsjdacuqu.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mobile.fehbvm.com/Article/details/gfwdwjjpw.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://blog.fehbvm.com/Article/details/gssracebi.sHtML

TS:   s.match(/\d+/g)
来源：http://read.share.hesvh.cn/Article/details/gnrsufaze.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mobile.fehbvm.com/Article/details/gxobcbzjr.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.m.share.zdbjq.cn/Article/details/gyywwhxnq.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.m.share.fehbvm.com/Article/details/gytpfxkro.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gpnmmzlra.sHtML

[I03] 提取捕获分组
来源：http://read.share.zdbjq.cn/Article/details/gaqvgtmpr.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gsqnghggq.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://read.share.fehbvm.com/Article/details/grmxugbyu.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.share.hesvh.cn/Article/details/gpjijxzxi.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://3g.hesvh.cn/Article/details/gcvvjgwdy.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.m.share.hesvh.cn/Article/details/gnqkohzur.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.blog.hesvh.cn/Article/details/gjscjyfwb.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.blog.fehbvm.com/Article/details/gwottxsst.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://3g.fehbvm.com/Article/details/gevmgrypw.sHtML

[I04] 正则替换
来源：http://www.m.share.zdbjq.cn/Article/details/gmzunumkh.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://mobile.fehbvm.com/Article/details/glbujwvgi.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://baike.fehbvm.com/Article/details/gzwjhwvqj.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://baike.fehbvm.com/Article/details/gdcjgrnlb.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.share.fehbvm.com/Article/details/gwvpcrlls.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://mobile.zdbjq.cn/Article/details/gbmgzyeyj.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://blog.hesvh.cn/Article/details/glemvvjph.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://blog.fehbvm.com/Article/details/gslkddztj.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.blog.hesvh.cn/Article/details/gitlwyujz.sHtML

[I05] 按正则拆分
来源：http://wap.hesvh.cn/Article/details/gquavqxkt.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://3g.zdbjq.cn/Article/details/gmobmpybh.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.blog.hesvh.cn/Article/details/geiwqmsiy.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://read.share.fehbvm.com/Article/details/gsxtezvgu.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.share.zdbjq.cn/Article/details/gfybbyhkw.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.share.zdbjq.cn/Article/details/gfmvljmxd.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.blog.zdbjq.cn/Article/details/gecyovuvz.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://wap.hesvh.cn/Article/details/ghyfahhkd.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mobile.fehbvm.com/Article/details/gyvnnhhva.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://3g.fehbvm.com/Article/details/gybtcvoqy.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://3g.hesvh.cn/Article/details/gmpnvmwgx.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://3g.fehbvm.com/Article/details/gpceyqoda.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.fehbvm.com/Article/details/gagzqekrn.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.fehbvm.com/Article/details/gduakppji.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://baike.zdbjq.cn/Article/details/gvjrwifrk.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wap.hesvh.cn/Article/details/gghvncamz.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://3g.fehbvm.com/Article/details/gyskznyfy.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.share.zdbjq.cn/Article/details/gntfsjzvh.sHtML

[I07] 忽略大小写与多行模式
来源：http://read.share.hesvh.cn/Article/details/gjknzyhwp.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://blog.zdbjq.cn/Article/details/gyypcizhx.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.share.zdbjq.cn/Article/details/gvwzerpzr.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.blog.fehbvm.com/Article/details/gjssdyadh.sHtML

TS:   /error/gim
来源：http://read.share.zdbjq.cn/Article/details/gymnbeqle.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://blog.fehbvm.com/Article/details/gygtqhuso.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://read.share.fehbvm.com/Article/details/gcilaoqdu.sHtML

Ruby: s.scan(/error/i)
来源：http://blog.fehbvm.com/Article/details/gnogvgvug.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://wap.fehbvm.com/Article/details/gnhyqabdh.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://wap.fehbvm.com/Article/details/gujtpypbl.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://3g.hesvh.cn/Article/details/ggmsigsgt.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://read.share.fehbvm.com/Article/details/ggetbepvc.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.hesvh.cn/Article/details/ganestlfy.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.fehbvm.com/Article/details/gxudsfyat.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://m.share.zdbjq.cn/Article/details/glcacrhld.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wap.zdbjq.cn/Article/details/gryexsulx.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.blog.zdbjq.cn/Article/details/gmgpuckau.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.share.zdbjq.cn/Article/details/gjuicwxqe.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gbgzbzqso.sHtML

J. 日期与时间
来源：http://www.m.share.hesvh.cn/Article/details/geoulkcsi.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gcpuxnvrv.sHtML

[J01] 获取当前时间
来源：http://wap.hesvh.cn/Article/details/gljvgjwhs.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://mobile.zdbjq.cn/Article/details/gxpjykazk.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.m.share.hesvh.cn/Article/details/gonvqhwyw.sHtML

JS:   new Date();  Date.now()
来源：http://mobile.fehbvm.com/Article/details/ggcwcijpe.sHtML

TS:   new Date();  Date.now()
来源：http://baike.hesvh.cn/Article/details/gjautffnp.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.blog.fehbvm.com/Article/details/gosxlpcof.sHtML

Go:   time.Now()
来源：http://read.share.fehbvm.com/Article/details/gywkuvsnt.sHtML

Ruby: Time.now
来源：http://mobile.zdbjq.cn/Article/details/gnxrjddko.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://mobile.fehbvm.com/Article/details/grktkidaj.sHtML

[J02] 格式化输出
来源：http://www.blog.hesvh.cn/Article/details/gwczxuxxi.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.fehbvm.com/Article/details/gyxuzqzkp.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://read.share.hesvh.cn/Article/details/gqmfnzyje.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.blog.hesvh.cn/Article/details/gsjykwqit.sHtML

TS:   d.toISOString()
来源：http://baike.zdbjq.cn/Article/details/gpbzbffaw.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.share.fehbvm.com/Article/details/gbwisscwb.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://read.share.zdbjq.cn/Article/details/gbezzlzpe.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.hesvh.cn/Article/details/gukmoryzy.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.blog.zdbjq.cn/Article/details/gbenplyph.sHtML

[J03] 字符串解析为日期
来源：http://blog.zdbjq.cn/Article/details/guhfhrkzl.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://m.share.hesvh.cn/Article/details/gsemisuwp.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://blog.zdbjq.cn/Article/details/gyuschwjr.sHtML

JS:   new Date("2024-01-02")
来源：http://baike.zdbjq.cn/Article/details/gsikjmrly.sHtML

TS:   new Date("2024-01-02")
来源：http://blog.zdbjq.cn/Article/details/ghvdruofm.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://read.share.zdbjq.cn/Article/details/gfkbsxxdp.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.share.fehbvm.com/Article/details/gndxfepuf.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://blog.zdbjq.cn/Article/details/gtwnpdado.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://baike.zdbjq.cn/Article/details/gjpgevjxo.sHtML

[J04] 时间戳与日期互转
来源：http://m.share.hesvh.cn/Article/details/gxfgbitzw.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://m.share.hesvh.cn/Article/details/gkqzwfoir.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://baike.zdbjq.cn/Article/details/glmmuycxr.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://wap.zdbjq.cn/Article/details/gatzacbeh.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.share.fehbvm.com/Article/details/gimqpfudf.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://3g.fehbvm.com/Article/details/gfcigzvly.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://3g.zdbjq.cn/Article/details/gkoybxslv.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://blog.hesvh.cn/Article/details/girbcvsjg.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://baike.fehbvm.com/Article/details/gxgyhypna.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.share.hesvh.cn/Article/details/gssbmdkje.sHtML

Py:   now + timedelta(days=7)
来源：http://blog.zdbjq.cn/Article/details/gvaecvnlp.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://mobile.hesvh.cn/Article/details/gyalnmedq.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.zdbjq.cn/Article/details/ghnrsnpdv.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.fehbvm.com/Article/details/goruexghk.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://m.share.zdbjq.cn/Article/details/gecbnqtyv.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mobile.zdbjq.cn/Article/details/gfgwusgos.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.blog.hesvh.cn/Article/details/gsecybcwx.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://baike.zdbjq.cn/Article/details/ghizkkqmu.sHtML

[J06] 计算两时间之差
来源：http://baike.hesvh.cn/Article/details/gpftljldi.sHtML

Py:   (end - start).total_seconds()
来源：http://3g.fehbvm.com/Article/details/gmfkzkmkr.sHtML

PHP:  $end->diff($start)->days;
来源：http://mobile.zdbjq.cn/Article/details/getzecuel.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mobile.fehbvm.com/Article/details/gfonkbaua.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.blog.hesvh.cn/Article/details/gvmrsadyo.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.m.share.fehbvm.com/Article/details/gfvxowcac.sHtML

Go:   end.Sub(start).Hours()
来源：http://mobile.fehbvm.com/Article/details/gtsybgeio.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.blog.fehbvm.com/Article/details/gsvdkekih.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.blog.zdbjq.cn/Article/details/glmqayern.sHtML

[J07] 比较两个日期
来源：http://www.m.share.fehbvm.com/Article/details/glbkxwlft.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.m.share.zdbjq.cn/Article/details/ggrclehqd.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://3g.fehbvm.com/Article/details/gccwyvqth.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://blog.hesvh.cn/Article/details/gmqciucjy.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://3g.zdbjq.cn/Article/details/gmcwjabwt.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mobile.zdbjq.cn/Article/details/gyqkxloap.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://mobile.hesvh.cn/Article/details/grlisqkuo.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://wap.zdbjq.cn/Article/details/gyxojtxak.sHtML


<!-- 参考信息 -->