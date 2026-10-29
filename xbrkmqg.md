代发 wailian999

TS:   public / protected / private
来源：http://mobile.hesvh.cn/Article/details/glthgksdh.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.zdbjq.cn/Article/details/gydubqchh.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.fehbvm.com/Article/details/gwvzipseb.sHtML

Ruby: public / protected / private
来源：http://read.share.hesvh.cn/Article/details/gacnrysuw.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.hesvh.cn/Article/details/gcbbzsvbo.sHtML

[G11] getter / setter
来源：http://blog.hesvh.cn/Article/details/gduktcjdz.sHtML

Py:   @property 与 @x.setter
来源：http://baike.hesvh.cn/Article/details/gbwcwgxbk.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.hesvh.cn/Article/details/gnlcmsquy.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.fehbvm.com/Article/details/gelikgmjb.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.hesvh.cn/Article/details/gsgxleptv.sHtML

Java: public String getName() { return name; }
来源：http://mobile.zdbjq.cn/Article/details/gekjiejnv.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.fehbvm.com/Article/details/gnmronndx.sHtML

Ruby: attr_accessor :name
来源：http://wap.zdbjq.cn/Article/details/gcsdhzsbl.sHtML

C#:   public string Name { get; set; }
来源：http://baike.zdbjq.cn/Article/details/gnpilkgpb.sHtML

[G12] 对象转字符串
来源：http://blog.zdbjq.cn/Article/details/gzevzsrru.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.hesvh.cn/Article/details/gcvzrypvo.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.fehbvm.com/Article/details/gdllfszpv.sHtML

JS:   toString() { return this.name; }
来源：http://blog.hesvh.cn/Article/details/gyhwlhedg.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.fehbvm.com/Article/details/ggfferxuj.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.zdbjq.cn/Article/details/ghfysbjak.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.zdbjq.cn/Article/details/gfmssomwv.sHtML

Ruby: def to_s; @name; end
来源：http://wap.fehbvm.com/Article/details/gwqihttvn.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.zdbjq.cn/Article/details/gjdoumnrn.sHtML

[G13] 判断对象类型
来源：http://m.share.zdbjq.cn/Article/details/ggyjfdpog.sHtML

Py:   isinstance(u, User)
来源：http://baike.hesvh.cn/Article/details/gxqrlepsv.sHtML

PHP:  $u instanceof User
来源：http://m.share.hesvh.cn/Article/details/gezllzgog.sHtML

JS:   u instanceof User
来源：http://baike.fehbvm.com/Article/details/gggurzzwq.sHtML

TS:   u instanceof User
来源：http://blog.fehbvm.com/Article/details/geojmsqeu.sHtML

Java: u instanceof User
来源：http://mobile.hesvh.cn/Article/details/gfrcpnldk.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.zdbjq.cn/Article/details/guxwlwjhx.sHtML

Ruby: u.is_a?(User)
来源：http://3g.hesvh.cn/Article/details/gvypmyufy.sHtML

C#:   u is User
来源：http://wap.zdbjq.cn/Article/details/gqlryixkl.sHtML

[G14] 数据类 / record
来源：http://mobile.fehbvm.com/Article/details/gvkckfitv.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://baike.zdbjq.cn/Article/details/gpzgkvqct.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.hesvh.cn/Article/details/gtwqczkia.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.zdbjq.cn/Article/details/gkieqnfny.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.hesvh.cn/Article/details/ggrgvtugp.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.zdbjq.cn/Article/details/gwxdrxntu.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.zdbjq.cn/Article/details/gwjmnvimc.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.hesvh.cn/Article/details/gokjscufs.sHtML

C#:   record User(string Name, int Age);
来源：http://m.share.fehbvm.com/Article/details/gjnvojpav.sHtML

[G15] 枚举
来源：http://read.share.hesvh.cn/Article/details/gbzkqevad.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.zdbjq.cn/Article/details/ghxbhbqib.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://baike.fehbvm.com/Article/details/gqnefsbei.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mobile.zdbjq.cn/Article/details/gyakhdszu.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.hesvh.cn/Article/details/gotpzsxzp.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.zdbjq.cn/Article/details/gevapppmi.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://baike.fehbvm.com/Article/details/gmrhxpmki.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.hesvh.cn/Article/details/gerxrzszx.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.hesvh.cn/Article/details/gihmdvqcr.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.fehbvm.com/Article/details/gbcgxliwd.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.hesvh.cn/Article/details/gsviiavdp.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.hesvh.cn/Article/details/gzoiqxzcd.sHtML

JS:   Object.entries(obj)
来源：http://read.share.fehbvm.com/Article/details/gikzavsgq.sHtML

TS:   Object.entries(obj)
来源：http://www.share.fehbvm.com/Article/details/geyertwaj.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.zdbjq.cn/Article/details/gxbktplli.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://wap.hesvh.cn/Article/details/gvwobvacl.sHtML

Ruby: obj.instance_variables
来源：http://www.share.fehbvm.com/Article/details/ghiurhkdb.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.hesvh.cn/Article/details/giajoaihs.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gassktibt.sHtML

H. 异常与错误处理
来源：http://m.share.fehbvm.com/Article/details/gwsszzrud.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gfogoxghb.sHtML

[H01] try / catch 基础
来源：http://www.m.share.zdbjq.cn/Article/details/grjsyiibd.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.share.hesvh.cn/Article/details/gsvyhpeol.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://3g.zdbjq.cn/Article/details/gdkmrwkjz.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.hesvh.cn/Article/details/gdgzyjnal.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.hesvh.cn/Article/details/gimrtggfz.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://baike.hesvh.cn/Article/details/grzkxrmuh.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mobile.fehbvm.com/Article/details/gdtwvdfml.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.share.hesvh.cn/Article/details/gpanygqez.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mobile.hesvh.cn/Article/details/getyiydcq.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.hesvh.cn/Article/details/gscvupkuc.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://mobile.fehbvm.com/Article/details/gwnwyyeha.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/gkeouqmen.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://m.share.fehbvm.com/Article/details/gsmvookki.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/ghcmhwhzz.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.hesvh.cn/Article/details/geltuxsaa.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.blog.zdbjq.cn/Article/details/gtiabnwpi.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.blog.zdbjq.cn/Article/details/gozakytdv.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://blog.fehbvm.com/Article/details/gpilbosfr.sHtML

[H03] 主动抛出异常
来源：http://www.share.zdbjq.cn/Article/details/gyipniqse.sHtML

Py:   raise ValueError("错误信息")
来源：http://3g.hesvh.cn/Article/details/gbqxtvqvi.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://m.share.hesvh.cn/Article/details/guhdlyfzq.sHtML

JS:   throw new Error("错误信息");
来源：http://www.m.share.fehbvm.com/Article/details/gchkvdaya.sHtML

TS:   throw new Error("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/glrwesior.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://blog.hesvh.cn/Article/details/gemlhddul.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.zdbjq.cn/Article/details/goiudmvfz.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.fehbvm.com/Article/details/genrsgvgz.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://baike.fehbvm.com/Article/details/gpoyafedc.sHtML

[H04] 自定义异常类型
来源：http://blog.fehbvm.com/Article/details/ggidbwvck.sHtML

Py:   class MyError(Exception): pass
来源：http://wap.hesvh.cn/Article/details/geqqhjwjr.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://m.share.fehbvm.com/Article/details/ginziehmr.sHtML

JS:   class MyError extends Error {}
来源：http://read.share.zdbjq.cn/Article/details/grpevogqu.sHtML

TS:   class MyError extends Error {}
来源：http://wap.zdbjq.cn/Article/details/gjebdqvio.sHtML

Java: class MyException extends RuntimeException {}
来源：http://baike.zdbjq.cn/Article/details/gowdicoqe.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://3g.hesvh.cn/Article/details/ggcgpzspr.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.hesvh.cn/Article/details/gzkruyvvm.sHtML

C#:   class MyException : Exception {}
来源：http://read.share.zdbjq.cn/Article/details/gunxbmrbj.sHtML

[H05] 捕获特定类型
来源：http://www.m.share.zdbjq.cn/Article/details/gopafpcvo.sHtML

Py:   except ValueError as e:
来源：http://read.share.fehbvm.com/Article/details/gdlvszpmm.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://baike.fehbvm.com/Article/details/gsocgfsvc.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://blog.hesvh.cn/Article/details/gqapthrpr.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://baike.zdbjq.cn/Article/details/gcjxmlvav.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.blog.fehbvm.com/Article/details/gwqbimoav.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.blog.zdbjq.cn/Article/details/gdiageqqg.sHtML

Ruby: rescue ArgumentError => e
来源：http://mobile.hesvh.cn/Article/details/gcomfgnhn.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://baike.fehbvm.com/Article/details/gtkzxsxxy.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.blog.fehbvm.com/Article/details/giebiyidv.sHtML

Py:   value = d.get("k") or default
来源：http://baike.zdbjq.cn/Article/details/gpwhowhmg.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://wap.fehbvm.com/Article/details/gfqjifhaj.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.fehbvm.com/Article/details/gawfnjqos.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://3g.fehbvm.com/Article/details/gnurkpwum.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mobile.hesvh.cn/Article/details/gpnocihoc.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://blog.fehbvm.com/Article/details/goqmohbml.sHtML

Ruby: d&.dig(:a, :b)
来源：http://read.share.fehbvm.com/Article/details/goxmrycec.sHtML

C#:   obj?.A?.B ?? default
来源：http://m.share.zdbjq.cn/Article/details/gkaoufihu.sHtML

[H07] 断言
来源：http://mobile.hesvh.cn/Article/details/ghhliobdt.sHtML

Py:   assert x > 0, "必须为正"
来源：http://baike.hesvh.cn/Article/details/gfqxrvaqu.sHtML

PHP:  assert($x > 0);
来源：http://baike.fehbvm.com/Article/details/gwvwzhfzi.sHtML

JS:   console.assert(x > 0);
来源：http://www.share.zdbjq.cn/Article/details/gtixldfnl.sHtML

TS:   console.assert(x > 0);
来源：http://www.m.share.hesvh.cn/Article/details/gvlsqocoz.sHtML

Java: assert x > 0 : "必须为正";
来源：http://blog.fehbvm.com/Article/details/gxpkymdoz.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.m.share.fehbvm.com/Article/details/gwamclrck.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://m.share.hesvh.cn/Article/details/gnyduycci.sHtML

C#:   Debug.Assert(x > 0);
来源：http://wap.fehbvm.com/Article/details/gdywteuhd.sHtML

[H08] 获取错误信息与堆栈
来源：http://mobile.zdbjq.cn/Article/details/gbxvqpktl.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.m.share.zdbjq.cn/Article/details/gymhicnsd.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://baike.fehbvm.com/Article/details/ganldfnvn.sHtML

JS:   e.message;  e.stack
来源：http://3g.fehbvm.com/Article/details/gzxpdrgha.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://m.share.fehbvm.com/Article/details/grizlwkdc.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.share.zdbjq.cn/Article/details/gczybtmky.sHtML

Go:   err.Error()
来源：http://wap.hesvh.cn/Article/details/gpartacpx.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.blog.hesvh.cn/Article/details/grbjzyslc.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.blog.fehbvm.com/Article/details/gmlhzditb.sHtML

[H09] 带错误码的异常
来源：http://baike.zdbjq.cn/Article/details/gbravnwyf.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.blog.zdbjq.cn/Article/details/gtkmffwmf.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://wap.zdbjq.cn/Article/details/gergyfukk.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wap.fehbvm.com/Article/details/gnszcihhl.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wap.hesvh.cn/Article/details/gvtlwdmhg.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.m.share.hesvh.cn/Article/details/gbfyngulb.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://read.share.fehbvm.com/Article/details/ghkgegqxm.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://m.share.hesvh.cn/Article/details/giyfaoldh.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://blog.hesvh.cn/Article/details/gjoolhbeb.sHtML

[H10] 资源自动释放
来源：http://mobile.zdbjq.cn/Article/details/gziworbgp.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://read.share.zdbjq.cn/Article/details/gxuvykymd.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://read.share.fehbvm.com/Article/details/gjlylstym.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.hesvh.cn/Article/details/gdmmktnma.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.zdbjq.cn/Article/details/gpviletvx.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://baike.hesvh.cn/Article/details/ghmkvaskt.sHtML

Go:   defer f.Close()
来源：http://www.blog.hesvh.cn/Article/details/gzewidgtm.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.blog.fehbvm.com/Article/details/guhakeagh.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gyjjoklfc.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gitvsfihe.sHtML

I. 正则表达式
来源：http://read.share.zdbjq.cn/Article/details/grbotsqql.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gfwtdrfac.sHtML

[I01] 判断是否匹配
来源：http://baike.zdbjq.cn/Article/details/goyafpziz.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://read.share.fehbvm.com/Article/details/gglxzhtzw.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://m.share.hesvh.cn/Article/details/gsnogrvno.sHtML

JS:   /\d+/.test(s)
来源：http://read.share.zdbjq.cn/Article/details/gpthlueer.sHtML

TS:   /\d+/.test(s)
来源：http://mobile.zdbjq.cn/Article/details/gdvglajqw.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://blog.hesvh.cn/Article/details/gzvpzsfqj.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mobile.zdbjq.cn/Article/details/gtqfxmlky.sHtML

Ruby: s.match?(/\d+/)
来源：http://3g.hesvh.cn/Article/details/gpiczjurb.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.m.share.hesvh.cn/Article/details/gjrpntcie.sHtML

[I02] 提取所有匹配
来源：http://baike.hesvh.cn/Article/details/gejnfxlfn.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.share.fehbvm.com/Article/details/gkrmjrhpx.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mobile.hesvh.cn/Article/details/gmpzphsoc.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mobile.zdbjq.cn/Article/details/giioocmtd.sHtML

TS:   s.match(/\d+/g)
来源：http://blog.zdbjq.cn/Article/details/gnyqbktmf.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wap.fehbvm.com/Article/details/gdhwnpnsd.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://3g.zdbjq.cn/Article/details/goreaiewg.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.blog.hesvh.cn/Article/details/gxgmwgnam.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.share.fehbvm.com/Article/details/gccxvsxoa.sHtML

[I03] 提取捕获分组
来源：http://www.share.fehbvm.com/Article/details/glnspquxj.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://baike.fehbvm.com/Article/details/glubfyfiw.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.m.share.hesvh.cn/Article/details/gjsghnqyq.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.m.share.fehbvm.com/Article/details/gqoxlxpaf.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://3g.zdbjq.cn/Article/details/gzdrbzayv.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.m.share.hesvh.cn/Article/details/gxpsozonl.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://read.share.hesvh.cn/Article/details/grxqxfznu.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://blog.zdbjq.cn/Article/details/ggahlzjhw.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://mobile.hesvh.cn/Article/details/gvqacmvwm.sHtML

[I04] 正则替换
来源：http://mobile.hesvh.cn/Article/details/goflogaqz.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://blog.zdbjq.cn/Article/details/gnpogontu.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.share.fehbvm.com/Article/details/gpvmuhiau.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.fehbvm.com/Article/details/grhvdghlc.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.hesvh.cn/Article/details/gissgrxom.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://baike.hesvh.cn/Article/details/gsocobqly.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.m.share.hesvh.cn/Article/details/gkanneqqv.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://wap.zdbjq.cn/Article/details/ggiidjmut.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mobile.zdbjq.cn/Article/details/glthfpbvw.sHtML

[I05] 按正则拆分
来源：http://m.share.zdbjq.cn/Article/details/gngombvzx.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://baike.zdbjq.cn/Article/details/gvpfplhmc.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.m.share.fehbvm.com/Article/details/gzshczhbq.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://m.share.fehbvm.com/Article/details/gijvkubjg.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://3g.fehbvm.com/Article/details/gtswrftdy.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.share.hesvh.cn/Article/details/gsyzfmtsc.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://baike.hesvh.cn/Article/details/gjmrrxuis.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://read.share.hesvh.cn/Article/details/gleqzbhiu.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://blog.hesvh.cn/Article/details/gxxnpfqoj.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.m.share.zdbjq.cn/Article/details/gfcayhvdu.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://mobile.zdbjq.cn/Article/details/gwudqayfp.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.m.share.zdbjq.cn/Article/details/gjfpumzuv.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.zdbjq.cn/Article/details/gigdzeqvu.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.hesvh.cn/Article/details/glccyrjrw.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.share.hesvh.cn/Article/details/gkceyhcti.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.m.share.fehbvm.com/Article/details/guzeinuni.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.share.zdbjq.cn/Article/details/gomwornbg.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mobile.zdbjq.cn/Article/details/gcwuwgkki.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.m.share.fehbvm.com/Article/details/gipolhjrb.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.blog.fehbvm.com/Article/details/gleebhbqt.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.blog.fehbvm.com/Article/details/guqypwnaq.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://blog.fehbvm.com/Article/details/gyygszhfy.sHtML

TS:   /error/gim
来源：http://read.share.hesvh.cn/Article/details/gfvtgpqzl.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://baike.fehbvm.com/Article/details/ggypocmch.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.m.share.fehbvm.com/Article/details/giowvfatv.sHtML

Ruby: s.scan(/error/i)
来源：http://blog.fehbvm.com/Article/details/gvkqmeugw.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://m.share.fehbvm.com/Article/details/gkilsowlg.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.m.share.fehbvm.com/Article/details/gptuhsmpf.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://3g.zdbjq.cn/Article/details/gdiiftqqd.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://blog.fehbvm.com/Article/details/gdbbxmgwg.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.zdbjq.cn/Article/details/gdthxutpv.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.fehbvm.com/Article/details/gxrifcrve.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://wap.fehbvm.com/Article/details/gmivzjucp.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://read.share.fehbvm.com/Article/details/grjqkdhpa.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://blog.fehbvm.com/Article/details/ghncuasqq.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://baike.zdbjq.cn/Article/details/gbdqxgygo.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gwlovhvlj.sHtML

J. 日期与时间
来源：http://www.blog.zdbjq.cn/Article/details/gykumkdrw.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gfgoetuuu.sHtML

[J01] 获取当前时间
来源：http://www.m.share.zdbjq.cn/Article/details/gafipmvfp.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://m.share.hesvh.cn/Article/details/gvewlxprb.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://blog.zdbjq.cn/Article/details/gsbpmklho.sHtML

JS:   new Date();  Date.now()
来源：http://read.share.fehbvm.com/Article/details/gbmfudzhc.sHtML

TS:   new Date();  Date.now()
来源：http://baike.fehbvm.com/Article/details/ginfgnltx.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://read.share.zdbjq.cn/Article/details/gmckzyegp.sHtML

Go:   time.Now()
来源：http://www.m.share.fehbvm.com/Article/details/gnsyzsytc.sHtML

Ruby: Time.now
来源：http://3g.hesvh.cn/Article/details/gkxzgbuun.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://baike.fehbvm.com/Article/details/gzgowkagr.sHtML

[J02] 格式化输出
来源：http://mobile.zdbjq.cn/Article/details/grapzdyzj.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.hesvh.cn/Article/details/gcdisslpv.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://read.share.fehbvm.com/Article/details/gyawqgtnp.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://read.share.fehbvm.com/Article/details/gipzerdin.sHtML

TS:   d.toISOString()
来源：http://baike.hesvh.cn/Article/details/gogoixibs.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.share.zdbjq.cn/Article/details/givnolqyu.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.share.zdbjq.cn/Article/details/gzawxjnyl.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.zdbjq.cn/Article/details/gtookebep.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://baike.hesvh.cn/Article/details/gphalymjs.sHtML

[J03] 字符串解析为日期
来源：http://blog.hesvh.cn/Article/details/gmyecveos.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.blog.zdbjq.cn/Article/details/gehvpufkd.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wap.hesvh.cn/Article/details/gdxpbjmdy.sHtML

JS:   new Date("2024-01-02")
来源：http://www.share.zdbjq.cn/Article/details/gcealpghh.sHtML

TS:   new Date("2024-01-02")
来源：http://www.share.hesvh.cn/Article/details/gclxnegue.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://wap.zdbjq.cn/Article/details/ghxynkkye.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.m.share.fehbvm.com/Article/details/ghtwsgmhv.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.share.hesvh.cn/Article/details/gkpthrqse.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wap.fehbvm.com/Article/details/glmhsicxj.sHtML

[J04] 时间戳与日期互转
来源：http://baike.fehbvm.com/Article/details/ggfzsupkw.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://baike.hesvh.cn/Article/details/gvefumgum.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://3g.hesvh.cn/Article/details/gskkruahj.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mobile.fehbvm.com/Article/details/gtpngvpoc.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://3g.hesvh.cn/Article/details/gjdobrhug.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.blog.fehbvm.com/Article/details/gjzjujlmy.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://m.share.hesvh.cn/Article/details/gunpduwsy.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://blog.fehbvm.com/Article/details/gmlftrkxg.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://m.share.hesvh.cn/Article/details/gsmvdlkxs.sHtML

[J05] 时间加减（加 7 天）
来源：http://wap.fehbvm.com/Article/details/gsmhupwrj.sHtML

Py:   now + timedelta(days=7)
来源：http://read.share.fehbvm.com/Article/details/ggxtjizte.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.share.hesvh.cn/Article/details/gaudnnfbf.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.fehbvm.com/Article/details/gkegsjgrp.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.hesvh.cn/Article/details/gjvfefjvo.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://mobile.hesvh.cn/Article/details/glntxtwmr.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://3g.fehbvm.com/Article/details/gqvfhbtqb.sHtML

Ruby: Time.now + 7 * 86400
来源：http://read.share.zdbjq.cn/Article/details/ggkaibtzx.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.share.fehbvm.com/Article/details/guayqestk.sHtML

[J06] 计算两时间之差
来源：http://www.share.zdbjq.cn/Article/details/gxfvyepxa.sHtML

Py:   (end - start).total_seconds()
来源：http://blog.zdbjq.cn/Article/details/gjfdoaipq.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.share.hesvh.cn/Article/details/goxfcnznf.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://m.share.hesvh.cn/Article/details/gaocczomq.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://3g.zdbjq.cn/Article/details/gjuncfqhm.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://3g.hesvh.cn/Article/details/gilupixzv.sHtML

Go:   end.Sub(start).Hours()
来源：http://read.share.hesvh.cn/Article/details/gaqowtuhv.sHtML

Ruby: end - start                 # 返回秒数
来源：http://m.share.zdbjq.cn/Article/details/gyttnslbk.sHtML

C#:   (end - start).TotalSeconds
来源：http://mobile.hesvh.cn/Article/details/gqxmlzpqb.sHtML

[J07] 比较两个日期
来源：http://www.blog.fehbvm.com/Article/details/gfpxtgwhk.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.share.hesvh.cn/Article/details/gzkcgpshl.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.m.share.hesvh.cn/Article/details/gtcezuljc.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://m.share.zdbjq.cn/Article/details/guofqpoxa.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.blog.fehbvm.com/Article/details/gwmrdaaor.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://read.share.fehbvm.com/Article/details/gulpwnasp.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wap.hesvh.cn/Article/details/gcplwdqyf.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://m.share.zdbjq.cn/Article/details/gbgrepkdq.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://m.share.zdbjq.cn/Article/details/gebtqrzfn.sHtML

[J08] 提取年月日与星期
来源：http://m.share.hesvh.cn/Article/details/gtizofspz.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.m.share.zdbjq.cn/Article/details/gddropizn.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mobile.fehbvm.com/Article/details/gpaanewsm.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.blog.zdbjq.cn/Article/details/glrqxkkhf.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://3g.zdbjq.cn/Article/details/gronwjahh.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://3g.hesvh.cn/Article/details/gjzutqefx.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.m.share.zdbjq.cn/Article/details/glfufeyay.sHtML


<!-- 参考信息 -->