代发 wailian999

TS:   public / protected / private
来源：http://www.m.share.zdbjq.cn/Article/details/gjiyoutfw.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.zdbjq.cn/Article/details/gcvekenft.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.hesvh.cn/Article/details/ghwjignnq.sHtML

Ruby: public / protected / private
来源：http://m.share.fehbvm.com/Article/details/gxdrroktx.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.zdbjq.cn/Article/details/gbhuicbwh.sHtML

[G11] getter / setter
来源：http://www.blog.zdbjq.cn/Article/details/gpsecubua.sHtML

Py:   @property 与 @x.setter
来源：http://blog.fehbvm.com/Article/details/gvqhcypjr.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.hesvh.cn/Article/details/gmimcqwka.sHtML

JS:   get name() { return this._name; }
来源：http://3g.zdbjq.cn/Article/details/glxdxupoy.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.zdbjq.cn/Article/details/ghinrbfjw.sHtML

Java: public String getName() { return name; }
来源：http://m.share.fehbvm.com/Article/details/gnlthhhec.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.zdbjq.cn/Article/details/gcrnjvigd.sHtML

Ruby: attr_accessor :name
来源：http://blog.hesvh.cn/Article/details/gzhcbsant.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.fehbvm.com/Article/details/gzusmwxut.sHtML

[G12] 对象转字符串
来源：http://www.blog.zdbjq.cn/Article/details/gbekxektw.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.fehbvm.com/Article/details/gngfbnkdb.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.zdbjq.cn/Article/details/gazdzxvkz.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/gxdzobjop.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.fehbvm.com/Article/details/gfzkkswgj.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gwxwnmyki.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.hesvh.cn/Article/details/givtoyuba.sHtML

Ruby: def to_s; @name; end
来源：http://baike.zdbjq.cn/Article/details/giqgitjml.sHtML

C#:   public override string ToString() => Name;
来源：http://www.share.fehbvm.com/Article/details/gxlctgdvp.sHtML

[G13] 判断对象类型
来源：http://www.share.fehbvm.com/Article/details/ghsuexsnv.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.zdbjq.cn/Article/details/gzdvwfjxs.sHtML

PHP:  $u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/gfsotnrss.sHtML

JS:   u instanceof User
来源：http://3g.hesvh.cn/Article/details/gachkmoph.sHtML

TS:   u instanceof User
来源：http://read.share.hesvh.cn/Article/details/gyfsliqqt.sHtML

Java: u instanceof User
来源：http://m.share.hesvh.cn/Article/details/glqppkwpe.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.fehbvm.com/Article/details/gkzbquuuv.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.hesvh.cn/Article/details/gpmvsxvtq.sHtML

C#:   u is User
来源：http://wap.zdbjq.cn/Article/details/gubqowsly.sHtML

[G14] 数据类 / record
来源：http://www.share.fehbvm.com/Article/details/ggoispbap.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://3g.zdbjq.cn/Article/details/guwrcycwg.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://read.share.hesvh.cn/Article/details/ggkqdkfov.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.hesvh.cn/Article/details/getjfuhyg.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.zdbjq.cn/Article/details/grdahrsrb.sHtML

Java: record User(String name, int age) {}
来源：http://baike.fehbvm.com/Article/details/gumqwvbkp.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.fehbvm.com/Article/details/gjesztppx.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://baike.zdbjq.cn/Article/details/gjsbbhnin.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.hesvh.cn/Article/details/gcstofqfx.sHtML

[G15] 枚举
来源：http://m.share.hesvh.cn/Article/details/gyczfmghp.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.zdbjq.cn/Article/details/gtvqezjcc.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.zdbjq.cn/Article/details/grwmttkdr.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://read.share.hesvh.cn/Article/details/grkfvljue.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.zdbjq.cn/Article/details/glbieflox.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.hesvh.cn/Article/details/gqubdvyzb.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.zdbjq.cn/Article/details/gpjsuwrfp.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.hesvh.cn/Article/details/geawinsyd.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.zdbjq.cn/Article/details/gwjjqtrip.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.fehbvm.com/Article/details/gtknnfzif.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.fehbvm.com/Article/details/gvmtsimjl.sHtML

PHP:  get_object_vars($obj);
来源：http://blog.fehbvm.com/Article/details/gifpappiq.sHtML

JS:   Object.entries(obj)
来源：http://m.share.hesvh.cn/Article/details/gkwgjghos.sHtML

TS:   Object.entries(obj)
来源：http://3g.hesvh.cn/Article/details/gmduvshhr.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.share.fehbvm.com/Article/details/gxquyfpmj.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://3g.fehbvm.com/Article/details/gwuslvnfa.sHtML

Ruby: obj.instance_variables
来源：http://baike.hesvh.cn/Article/details/gfaiunlyq.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.zdbjq.cn/Article/details/gusazpwqg.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gmvkfpxwl.sHtML

H. 异常与错误处理
来源：http://mobile.hesvh.cn/Article/details/gczbcdlxj.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gjxvzmtiq.sHtML

[H01] try / catch 基础
来源：http://blog.hesvh.cn/Article/details/gaygpezpz.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.zdbjq.cn/Article/details/gpryepczl.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.hesvh.cn/Article/details/gsitwzdtg.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.zdbjq.cn/Article/details/gqqqrzueq.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mobile.fehbvm.com/Article/details/gbdebwylh.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.zdbjq.cn/Article/details/gwqxmuudo.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://read.share.fehbvm.com/Article/details/gtyzezklf.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.zdbjq.cn/Article/details/galwqbeta.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://blog.hesvh.cn/Article/details/goxovfqec.sHtML

[H02] finally / ensure 收尾
来源：http://wap.fehbvm.com/Article/details/gocvtfjhq.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://mobile.fehbvm.com/Article/details/gjpsanuws.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.share.hesvh.cn/Article/details/gcvitafgq.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://baike.hesvh.cn/Article/details/gqzdwdguf.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.hesvh.cn/Article/details/grvghthvf.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.blog.zdbjq.cn/Article/details/gancvzvgo.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.blog.zdbjq.cn/Article/details/gukwydrgm.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.fehbvm.com/Article/details/gmhoeloei.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.blog.zdbjq.cn/Article/details/ghyhllxzj.sHtML

[H03] 主动抛出异常
来源：http://www.m.share.zdbjq.cn/Article/details/gwmzezdet.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.zdbjq.cn/Article/details/gyjssrsxc.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://baike.zdbjq.cn/Article/details/gpfsklgqm.sHtML

JS:   throw new Error("错误信息");
来源：http://read.share.fehbvm.com/Article/details/gchvcqcpd.sHtML

TS:   throw new Error("错误信息");
来源：http://www.blog.hesvh.cn/Article/details/gygbasgyo.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://blog.hesvh.cn/Article/details/gsbyfhvpl.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.zdbjq.cn/Article/details/gnmrpcbjf.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://m.share.zdbjq.cn/Article/details/gkvzeqrld.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.zdbjq.cn/Article/details/gxboegcrp.sHtML

[H04] 自定义异常类型
来源：http://blog.fehbvm.com/Article/details/gbhtwgyjq.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.hesvh.cn/Article/details/gufglfzbo.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://blog.hesvh.cn/Article/details/gciluhcrw.sHtML

JS:   class MyError extends Error {}
来源：http://m.share.fehbvm.com/Article/details/gdapmdswg.sHtML

TS:   class MyError extends Error {}
来源：http://wap.hesvh.cn/Article/details/ghiotxtcl.sHtML

Java: class MyException extends RuntimeException {}
来源：http://baike.zdbjq.cn/Article/details/gbzdimcyq.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://baike.fehbvm.com/Article/details/gigadukfp.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.share.zdbjq.cn/Article/details/gpivpbhoe.sHtML

C#:   class MyException : Exception {}
来源：http://m.share.fehbvm.com/Article/details/gjpkkzigo.sHtML

[H05] 捕获特定类型
来源：http://read.share.fehbvm.com/Article/details/gtnjhiuak.sHtML

Py:   except ValueError as e:
来源：http://wap.zdbjq.cn/Article/details/ghidqpaun.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.m.share.fehbvm.com/Article/details/gbntxsmcc.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://baike.hesvh.cn/Article/details/gveoqtwsm.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://wap.zdbjq.cn/Article/details/gihmshpqf.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://read.share.fehbvm.com/Article/details/gnnjrudfw.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://read.share.zdbjq.cn/Article/details/gqepksvpg.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.zdbjq.cn/Article/details/goqkjssbt.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.share.zdbjq.cn/Article/details/gfgbzdzqi.sHtML

[H06] 可选值 / 空值安全访问
来源：http://wap.zdbjq.cn/Article/details/gelaxtdvl.sHtML

Py:   value = d.get("k") or default
来源：http://www.blog.fehbvm.com/Article/details/glvelpgel.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://baike.hesvh.cn/Article/details/gmgqvelgw.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://baike.hesvh.cn/Article/details/gkfogmrat.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.blog.zdbjq.cn/Article/details/gwfwhekbd.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://m.share.zdbjq.cn/Article/details/gcurmgfel.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.share.hesvh.cn/Article/details/gyiosyaiq.sHtML

Ruby: d&.dig(:a, :b)
来源：http://read.share.fehbvm.com/Article/details/gfqkhvrde.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.share.zdbjq.cn/Article/details/gmyircusg.sHtML

[H07] 断言
来源：http://www.m.share.hesvh.cn/Article/details/gwzmrtoac.sHtML

Py:   assert x > 0, "必须为正"
来源：http://read.share.hesvh.cn/Article/details/gxfltivpg.sHtML

PHP:  assert($x > 0);
来源：http://read.share.zdbjq.cn/Article/details/gghnzfqup.sHtML

JS:   console.assert(x > 0);
来源：http://wap.fehbvm.com/Article/details/gjogoixty.sHtML

TS:   console.assert(x > 0);
来源：http://m.share.fehbvm.com/Article/details/gcwvfqfik.sHtML

Java: assert x > 0 : "必须为正";
来源：http://read.share.zdbjq.cn/Article/details/gxppglryp.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.share.hesvh.cn/Article/details/gmaqturmu.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://blog.hesvh.cn/Article/details/gcvlovzap.sHtML

C#:   Debug.Assert(x > 0);
来源：http://wap.fehbvm.com/Article/details/gvacbjmpu.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.m.share.fehbvm.com/Article/details/gqytwvdud.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://3g.zdbjq.cn/Article/details/gsgztlpsv.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mobile.zdbjq.cn/Article/details/grtxfspdu.sHtML

JS:   e.message;  e.stack
来源：http://mobile.fehbvm.com/Article/details/gwvtmgegj.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://blog.zdbjq.cn/Article/details/gfvpxltnk.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://m.share.fehbvm.com/Article/details/gnfbdeueq.sHtML

Go:   err.Error()
来源：http://www.share.fehbvm.com/Article/details/gnkrrbhbp.sHtML

Ruby: e.message;  e.backtrace
来源：http://3g.fehbvm.com/Article/details/gghnllmxh.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.share.hesvh.cn/Article/details/gppsflljn.sHtML

[H09] 带错误码的异常
来源：http://wap.hesvh.cn/Article/details/gtclhrmdc.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://m.share.fehbvm.com/Article/details/gcbjxfeag.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.m.share.hesvh.cn/Article/details/gzkxeipbz.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wap.fehbvm.com/Article/details/gvjtljvsa.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://read.share.zdbjq.cn/Article/details/gizyzxfto.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.share.hesvh.cn/Article/details/gtyvvxbrh.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.blog.hesvh.cn/Article/details/getrcasvp.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.m.share.hesvh.cn/Article/details/grvehlmki.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://baike.zdbjq.cn/Article/details/glfylwuic.sHtML

[H10] 资源自动释放
来源：http://m.share.fehbvm.com/Article/details/gvzsojswi.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.blog.fehbvm.com/Article/details/grzeyprym.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.blog.zdbjq.cn/Article/details/gclysjwgl.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.fehbvm.com/Article/details/gmowlimru.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.hesvh.cn/Article/details/gfooooidl.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://baike.fehbvm.com/Article/details/galaepzph.sHtML

Go:   defer f.Close()
来源：http://baike.fehbvm.com/Article/details/gowdhiezr.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.share.zdbjq.cn/Article/details/gyblkqlgd.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://blog.hesvh.cn/Article/details/gexwdhkqm.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/ghsvdgsqa.sHtML

I. 正则表达式
来源：http://blog.fehbvm.com/Article/details/gtrryoxfw.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gtsgyclgo.sHtML

[I01] 判断是否匹配
来源：http://wap.zdbjq.cn/Article/details/gislgkixn.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://baike.zdbjq.cn/Article/details/guqwivdev.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://read.share.fehbvm.com/Article/details/ggnwzgkcm.sHtML

JS:   /\d+/.test(s)
来源：http://3g.fehbvm.com/Article/details/gqqbjuiaz.sHtML

TS:   /\d+/.test(s)
来源：http://www.m.share.hesvh.cn/Article/details/gfrnhtmvk.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.share.hesvh.cn/Article/details/gtdbkntot.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://read.share.hesvh.cn/Article/details/gauegycim.sHtML

Ruby: s.match?(/\d+/)
来源：http://blog.fehbvm.com/Article/details/gzxfigwpf.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://blog.fehbvm.com/Article/details/gzwuhpcrm.sHtML

[I02] 提取所有匹配
来源：http://baike.fehbvm.com/Article/details/gdtzgqlkz.sHtML

Py:   re.findall(r"\d+", s)
来源：http://mobile.fehbvm.com/Article/details/gzvcwyysq.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://m.share.fehbvm.com/Article/details/gatktlyjc.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mobile.hesvh.cn/Article/details/gsewlhkpl.sHtML

TS:   s.match(/\d+/g)
来源：http://blog.zdbjq.cn/Article/details/gqqznwbah.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://m.share.zdbjq.cn/Article/details/gkubbkbbw.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://m.share.zdbjq.cn/Article/details/gdnybxpzr.sHtML

Ruby: s.scan(/\d+/)
来源：http://read.share.zdbjq.cn/Article/details/grrxenknu.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mobile.hesvh.cn/Article/details/gftkfipmd.sHtML

[I03] 提取捕获分组
来源：http://read.share.zdbjq.cn/Article/details/ghnejjirk.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://blog.zdbjq.cn/Article/details/gwhlecdjb.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://m.share.fehbvm.com/Article/details/gaxaioxgi.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mobile.hesvh.cn/Article/details/gehtddhte.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.m.share.fehbvm.com/Article/details/ghhopnoal.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.blog.hesvh.cn/Article/details/gxrtfyiaq.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mobile.hesvh.cn/Article/details/gvoutowuo.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mobile.fehbvm.com/Article/details/gnywxffet.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://read.share.fehbvm.com/Article/details/gvplumcyf.sHtML

[I04] 正则替换
来源：http://3g.hesvh.cn/Article/details/gxasqduuh.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://m.share.zdbjq.cn/Article/details/gxmycfwqe.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gaeuqzfxb.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://m.share.fehbvm.com/Article/details/gzwbhsvyr.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://read.share.hesvh.cn/Article/details/gfbwilhcw.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://3g.fehbvm.com/Article/details/gdkngnnbo.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://m.share.fehbvm.com/Article/details/gdobsosib.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://baike.zdbjq.cn/Article/details/gudbnsfxh.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://blog.zdbjq.cn/Article/details/gnxocvndv.sHtML

[I05] 按正则拆分
来源：http://baike.fehbvm.com/Article/details/gtcjtbawy.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://blog.zdbjq.cn/Article/details/gruewbxfb.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://read.share.fehbvm.com/Article/details/gprhxswvh.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.m.share.zdbjq.cn/Article/details/gvkcwqcgr.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.blog.fehbvm.com/Article/details/gpbqrqjjo.sHtML

Java: s.split("\\s*,\\s*")
来源：http://3g.fehbvm.com/Article/details/gjfpqvhmn.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://mobile.hesvh.cn/Article/details/gcmqimkov.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://mobile.zdbjq.cn/Article/details/gikegfixn.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://m.share.hesvh.cn/Article/details/gmtjcfaai.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.m.share.fehbvm.com/Article/details/gvfjgrlix.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://3g.fehbvm.com/Article/details/gpcwbalxm.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://3g.fehbvm.com/Article/details/gjjahsdtg.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.zdbjq.cn/Article/details/gjpgotbsl.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.hesvh.cn/Article/details/gbhrxiyej.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://m.share.hesvh.cn/Article/details/gkzvkhgvd.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.m.share.hesvh.cn/Article/details/gqglyqxze.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://3g.hesvh.cn/Article/details/gdzovmazi.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://m.share.zdbjq.cn/Article/details/gqlpeifgt.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.share.zdbjq.cn/Article/details/giluwtdob.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.blog.hesvh.cn/Article/details/gwugoeszm.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wap.fehbvm.com/Article/details/gmefdyvqb.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.blog.hesvh.cn/Article/details/gqpxnebrw.sHtML

TS:   /error/gim
来源：http://read.share.zdbjq.cn/Article/details/ghxvyfrfz.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.share.hesvh.cn/Article/details/gwkbpryug.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://blog.hesvh.cn/Article/details/grlzjjddq.sHtML

Ruby: s.scan(/error/i)
来源：http://baike.zdbjq.cn/Article/details/goysswyjo.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.m.share.hesvh.cn/Article/details/gxibklqca.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://blog.hesvh.cn/Article/details/gtfyptjzw.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://baike.zdbjq.cn/Article/details/gzsmntlkq.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.share.zdbjq.cn/Article/details/geqqyhzqb.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.hesvh.cn/Article/details/giqtnnsdm.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.fehbvm.com/Article/details/gunsxvrpp.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://3g.fehbvm.com/Article/details/gkspfsrcc.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wap.zdbjq.cn/Article/details/govbczuzv.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://3g.hesvh.cn/Article/details/gmcitbjce.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.share.hesvh.cn/Article/details/gowjeoxiw.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gnrppdext.sHtML

J. 日期与时间
来源：http://baike.zdbjq.cn/Article/details/gzaicmwxm.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/ghmaztidm.sHtML

[J01] 获取当前时间
来源：http://www.m.share.fehbvm.com/Article/details/glkgpyigd.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://3g.fehbvm.com/Article/details/ghzprwgek.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.blog.hesvh.cn/Article/details/gkehlopwl.sHtML

JS:   new Date();  Date.now()
来源：http://baike.fehbvm.com/Article/details/gvoxmqhjf.sHtML

TS:   new Date();  Date.now()
来源：http://mobile.hesvh.cn/Article/details/grkurlkxi.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://blog.fehbvm.com/Article/details/guaznkxwg.sHtML

Go:   time.Now()
来源：http://blog.fehbvm.com/Article/details/gjczltbmq.sHtML

Ruby: Time.now
来源：http://read.share.zdbjq.cn/Article/details/gebxhkkyu.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.m.share.zdbjq.cn/Article/details/gniyhgefp.sHtML

[J02] 格式化输出
来源：http://wap.hesvh.cn/Article/details/grewsdagl.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.zdbjq.cn/Article/details/gzckrkbut.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://3g.hesvh.cn/Article/details/gmxzmstcl.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://3g.hesvh.cn/Article/details/gsneyhmiq.sHtML

TS:   d.toISOString()
来源：http://www.m.share.zdbjq.cn/Article/details/gchvzlxnf.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://blog.fehbvm.com/Article/details/glzankche.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://mobile.fehbvm.com/Article/details/ggxszgokt.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.fehbvm.com/Article/details/gvoavkvig.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://baike.zdbjq.cn/Article/details/gsrketiel.sHtML

[J03] 字符串解析为日期
来源：http://mobile.hesvh.cn/Article/details/gsnjwtjmx.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://blog.hesvh.cn/Article/details/gicyqkdad.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://mobile.zdbjq.cn/Article/details/gtyljsvje.sHtML

JS:   new Date("2024-01-02")
来源：http://m.share.hesvh.cn/Article/details/gdvuqhzjc.sHtML

TS:   new Date("2024-01-02")
来源：http://baike.hesvh.cn/Article/details/gztdaswfs.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://baike.fehbvm.com/Article/details/gwfoowisj.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://blog.fehbvm.com/Article/details/gtnvoftcc.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://3g.zdbjq.cn/Article/details/gkavzrrow.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://read.share.zdbjq.cn/Article/details/gnbpebono.sHtML

[J04] 时间戳与日期互转
来源：http://m.share.fehbvm.com/Article/details/ggjfxytim.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.share.fehbvm.com/Article/details/gvptaviul.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://3g.fehbvm.com/Article/details/gltfhyvgv.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://read.share.hesvh.cn/Article/details/gprldvlaf.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://mobile.hesvh.cn/Article/details/gkuwurazt.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://m.share.hesvh.cn/Article/details/gvocffzjf.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://read.share.fehbvm.com/Article/details/gbvaswujl.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wap.fehbvm.com/Article/details/gxukqsfyt.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://3g.fehbvm.com/Article/details/gdikkqbic.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.share.zdbjq.cn/Article/details/gdjxfjmmh.sHtML

Py:   now + timedelta(days=7)
来源：http://mobile.zdbjq.cn/Article/details/gjtpreaqr.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.share.hesvh.cn/Article/details/gpodcptwn.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.fehbvm.com/Article/details/grvnpltil.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.zdbjq.cn/Article/details/gygyalzyo.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.share.zdbjq.cn/Article/details/gmjnujjuv.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.blog.fehbvm.com/Article/details/gbaupotle.sHtML

Ruby: Time.now + 7 * 86400
来源：http://blog.fehbvm.com/Article/details/gtbssafcc.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.blog.hesvh.cn/Article/details/gnpmfoubb.sHtML

[J06] 计算两时间之差
来源：http://3g.zdbjq.cn/Article/details/gwyvazjdr.sHtML

Py:   (end - start).total_seconds()
来源：http://www.blog.zdbjq.cn/Article/details/gvlolilah.sHtML

PHP:  $end->diff($start)->days;
来源：http://3g.fehbvm.com/Article/details/gquckohdp.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://m.share.hesvh.cn/Article/details/gziqjcvux.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://m.share.hesvh.cn/Article/details/gsybxcqcd.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.m.share.hesvh.cn/Article/details/gtawzkuoh.sHtML

Go:   end.Sub(start).Hours()
来源：http://blog.fehbvm.com/Article/details/gpnlgatob.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.blog.fehbvm.com/Article/details/gqhvhxfue.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.share.zdbjq.cn/Article/details/giyywesez.sHtML

[J07] 比较两个日期
来源：http://www.m.share.zdbjq.cn/Article/details/gcgvclosx.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://m.share.fehbvm.com/Article/details/gvqxnjphn.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.m.share.hesvh.cn/Article/details/gywblribo.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://3g.hesvh.cn/Article/details/gqdxopoti.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://m.share.zdbjq.cn/Article/details/gmehhbkiy.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mobile.fehbvm.com/Article/details/gtcijksck.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://read.share.hesvh.cn/Article/details/glqnxosye.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://wap.hesvh.cn/Article/details/gsqhwexnk.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://baike.fehbvm.com/Article/details/gufiljanr.sHtML

[J08] 提取年月日与星期
来源：http://baike.hesvh.cn/Article/details/gvrhmrwkj.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.m.share.zdbjq.cn/Article/details/gdcdxqfrb.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://3g.fehbvm.com/Article/details/gfswhukmx.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.blog.hesvh.cn/Article/details/gzvmuydbf.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mobile.zdbjq.cn/Article/details/gqeqixjuy.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.share.zdbjq.cn/Article/details/gwwsjrnqq.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://m.share.hesvh.cn/Article/details/giwljhbff.sHtML


<!-- 参考信息 -->