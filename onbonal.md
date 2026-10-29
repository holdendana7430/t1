代发 wailian999

Ruby: attr_accessor :name
来源：http://read.share.hesvh.cn/Article/details/gpjwbqhfc.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.hesvh.cn/Article/details/geikivmwg.sHtML

[G12] 对象转字符串
来源：http://baike.zdbjq.cn/Article/details/gtyssvdou.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.hesvh.cn/Article/details/gumqeaxju.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.fehbvm.com/Article/details/gomuolexn.sHtML

JS:   toString() { return this.name; }
来源：http://wap.fehbvm.com/Article/details/gpjlztwdt.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/gtdtbduza.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/gzruipdno.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.hesvh.cn/Article/details/gymtrmqbk.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.zdbjq.cn/Article/details/gprbgcqne.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.hesvh.cn/Article/details/gjopmpxdu.sHtML

[G13] 判断对象类型
来源：http://wap.fehbvm.com/Article/details/gefkwowmg.sHtML

Py:   isinstance(u, User)
来源：http://m.share.fehbvm.com/Article/details/gzkomvsuv.sHtML

PHP:  $u instanceof User
来源：http://m.share.zdbjq.cn/Article/details/ghlzuzloe.sHtML

JS:   u instanceof User
来源：http://blog.hesvh.cn/Article/details/gqlprpuan.sHtML

TS:   u instanceof User
来源：http://baike.hesvh.cn/Article/details/gulhdjgnk.sHtML

Java: u instanceof User
来源：http://www.m.share.zdbjq.cn/Article/details/gjzcwlhlj.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.fehbvm.com/Article/details/gakvjugbg.sHtML

Ruby: u.is_a?(User)
来源：http://blog.zdbjq.cn/Article/details/glkdceheq.sHtML

C#:   u is User
来源：http://www.m.share.hesvh.cn/Article/details/ggpsgkewg.sHtML

[G14] 数据类 / record
来源：http://wap.hesvh.cn/Article/details/gkzfrvfab.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.hesvh.cn/Article/details/ghhhbbumc.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.zdbjq.cn/Article/details/gwrsvjzoy.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.zdbjq.cn/Article/details/grmtypxnt.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.hesvh.cn/Article/details/ganjrofez.sHtML

Java: record User(String name, int age) {}
来源：http://mobile.fehbvm.com/Article/details/gqhsfqouq.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.hesvh.cn/Article/details/gufgqfuuh.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.zdbjq.cn/Article/details/gwdmduoxl.sHtML

C#:   record User(string Name, int Age);
来源：http://blog.fehbvm.com/Article/details/giupjelsc.sHtML

[G15] 枚举
来源：http://m.share.zdbjq.cn/Article/details/geusdthef.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.hesvh.cn/Article/details/goebfutwv.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.zdbjq.cn/Article/details/gyjxdjcsu.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.m.share.fehbvm.com/Article/details/gewxdjokr.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.zdbjq.cn/Article/details/gsuuziaae.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.hesvh.cn/Article/details/gqvvfttxa.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.hesvh.cn/Article/details/gopjutjgp.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.hesvh.cn/Article/details/glvhygcsb.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.zdbjq.cn/Article/details/gwqzitivo.sHtML

[G16] 对象转数组 / 字典
来源：http://www.m.share.zdbjq.cn/Article/details/gfyqjbscm.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.hesvh.cn/Article/details/ghustqnhc.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.zdbjq.cn/Article/details/giuwoxyfx.sHtML

JS:   Object.entries(obj)
来源：http://m.share.hesvh.cn/Article/details/gqbthrxea.sHtML

TS:   Object.entries(obj)
来源：http://www.share.fehbvm.com/Article/details/gdsotjrta.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.hesvh.cn/Article/details/gwgflkhor.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.zdbjq.cn/Article/details/gzpbansja.sHtML

Ruby: obj.instance_variables
来源：http://www.share.zdbjq.cn/Article/details/gkycfwuud.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.fehbvm.com/Article/details/gysdhuvsl.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/ghfhucezx.sHtML

H. 异常与错误处理
来源：http://m.share.zdbjq.cn/Article/details/gizazlyyf.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gkqybdmfi.sHtML

[H01] try / catch 基础
来源：http://m.share.hesvh.cn/Article/details/gvdexlcyp.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.hesvh.cn/Article/details/gcgfimbyk.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.zdbjq.cn/Article/details/gafwncisf.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.hesvh.cn/Article/details/gcpvibror.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.fehbvm.com/Article/details/gqwfykjbz.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.zdbjq.cn/Article/details/gujaxczpe.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://m.share.hesvh.cn/Article/details/ggivnlqix.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.fehbvm.com/Article/details/guewhproz.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.fehbvm.com/Article/details/gadukdeul.sHtML

[H02] finally / ensure 收尾
来源：http://wap.hesvh.cn/Article/details/gcorstizj.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://baike.zdbjq.cn/Article/details/goswzbczy.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/guurcezpm.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://baike.hesvh.cn/Article/details/gipxfgucc.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://m.share.hesvh.cn/Article/details/gzvgteddf.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.fehbvm.com/Article/details/gpkpfxxld.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.zdbjq.cn/Article/details/gtgohyrrq.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.share.fehbvm.com/Article/details/girrigktz.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://mobile.zdbjq.cn/Article/details/gdqqrrhkh.sHtML

[H03] 主动抛出异常
来源：http://mobile.hesvh.cn/Article/details/ganucmbob.sHtML

Py:   raise ValueError("错误信息")
来源：http://blog.hesvh.cn/Article/details/gjlzbgmuo.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://baike.fehbvm.com/Article/details/glrefgzgi.sHtML

JS:   throw new Error("错误信息");
来源：http://www.blog.fehbvm.com/Article/details/gogdlxirz.sHtML

TS:   throw new Error("错误信息");
来源：http://read.share.fehbvm.com/Article/details/gmkohxqtq.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://blog.fehbvm.com/Article/details/grqbiuuwl.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://3g.zdbjq.cn/Article/details/gotoqsojw.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://blog.fehbvm.com/Article/details/gfthgcdgw.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://m.share.fehbvm.com/Article/details/gdsuagmqe.sHtML

[H04] 自定义异常类型
来源：http://baike.hesvh.cn/Article/details/glnywtbmi.sHtML

Py:   class MyError(Exception): pass
来源：http://read.share.hesvh.cn/Article/details/gkkqcvkmn.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://wap.hesvh.cn/Article/details/gktqtrcjc.sHtML

JS:   class MyError extends Error {}
来源：http://blog.zdbjq.cn/Article/details/gwawpqohd.sHtML

TS:   class MyError extends Error {}
来源：http://3g.hesvh.cn/Article/details/gpihjhtpf.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.share.zdbjq.cn/Article/details/gkuykzuqp.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.hesvh.cn/Article/details/gavcqmxyl.sHtML

Ruby: class MyError < StandardError; end
来源：http://3g.fehbvm.com/Article/details/gyzptwquf.sHtML

C#:   class MyException : Exception {}
来源：http://www.blog.zdbjq.cn/Article/details/gaerlyrhr.sHtML

[H05] 捕获特定类型
来源：http://www.m.share.zdbjq.cn/Article/details/gbiiwadkj.sHtML

Py:   except ValueError as e:
来源：http://mobile.hesvh.cn/Article/details/gsuhwfelf.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.hesvh.cn/Article/details/glzfcznry.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.blog.hesvh.cn/Article/details/gcgdfbksk.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.share.hesvh.cn/Article/details/gdqcrfjxz.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://3g.zdbjq.cn/Article/details/gpwynpahj.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://blog.hesvh.cn/Article/details/gqzeunlky.sHtML

Ruby: rescue ArgumentError => e
来源：http://3g.zdbjq.cn/Article/details/geoxynmej.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://m.share.hesvh.cn/Article/details/goriptrdn.sHtML

[H06] 可选值 / 空值安全访问
来源：http://3g.hesvh.cn/Article/details/gennsoylm.sHtML

Py:   value = d.get("k") or default
来源：http://3g.zdbjq.cn/Article/details/gybsoyzrw.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://mobile.fehbvm.com/Article/details/gfuwfmxfq.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://mobile.fehbvm.com/Article/details/gvvxmgfip.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://wap.zdbjq.cn/Article/details/ggayrqcfc.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.share.zdbjq.cn/Article/details/ggpjpkahb.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.m.share.fehbvm.com/Article/details/gllrqbfdb.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.blog.zdbjq.cn/Article/details/gwtrxehlx.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.blog.fehbvm.com/Article/details/gatysfxdt.sHtML

[H07] 断言
来源：http://m.share.hesvh.cn/Article/details/gdxeequwq.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.m.share.hesvh.cn/Article/details/gxkebmgsk.sHtML

PHP:  assert($x > 0);
来源：http://www.share.hesvh.cn/Article/details/gqntsphvq.sHtML

JS:   console.assert(x > 0);
来源：http://www.blog.hesvh.cn/Article/details/gftitzwbg.sHtML

TS:   console.assert(x > 0);
来源：http://www.blog.hesvh.cn/Article/details/gnsgehfhp.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.share.hesvh.cn/Article/details/guiagdldu.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.share.fehbvm.com/Article/details/gwxbqlycd.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://baike.zdbjq.cn/Article/details/gqbkzjabs.sHtML

C#:   Debug.Assert(x > 0);
来源：http://baike.zdbjq.cn/Article/details/grezmcuje.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.share.hesvh.cn/Article/details/gbygpkubg.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://wap.hesvh.cn/Article/details/gkcktjxgq.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wap.hesvh.cn/Article/details/glrdudkvr.sHtML

JS:   e.message;  e.stack
来源：http://read.share.zdbjq.cn/Article/details/gfuxosoli.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://3g.hesvh.cn/Article/details/grijacywx.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://blog.zdbjq.cn/Article/details/gezmejynv.sHtML

Go:   err.Error()
来源：http://m.share.hesvh.cn/Article/details/glttamhdp.sHtML

Ruby: e.message;  e.backtrace
来源：http://blog.zdbjq.cn/Article/details/gwraburtr.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.m.share.hesvh.cn/Article/details/geecrzjlu.sHtML

[H09] 带错误码的异常
来源：http://www.m.share.fehbvm.com/Article/details/gqvqepkua.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://3g.fehbvm.com/Article/details/gizeibkxw.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://3g.hesvh.cn/Article/details/gbtqdvlyv.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wap.zdbjq.cn/Article/details/gnzfrxiqp.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://m.share.hesvh.cn/Article/details/gbtrwnfpa.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.m.share.zdbjq.cn/Article/details/gueeviflc.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://blog.zdbjq.cn/Article/details/gtwbmncjt.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://read.share.zdbjq.cn/Article/details/gpbaiyxnr.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://wap.hesvh.cn/Article/details/gelefsxwf.sHtML

[H10] 资源自动释放
来源：http://read.share.hesvh.cn/Article/details/gmpiinbrv.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://baike.fehbvm.com/Article/details/gbojuadtr.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://read.share.hesvh.cn/Article/details/ghcpfmxxc.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.fehbvm.com/Article/details/godnmxltf.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.hesvh.cn/Article/details/gvjrqmxbr.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.m.share.zdbjq.cn/Article/details/ggtqravhp.sHtML

Go:   defer f.Close()
来源：http://m.share.fehbvm.com/Article/details/gwrlmzpdt.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.share.zdbjq.cn/Article/details/gmieshild.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gicpjusbj.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/ghrdlrrlq.sHtML

I. 正则表达式
来源：http://www.blog.fehbvm.com/Article/details/gxrebbzoq.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gagqlpezl.sHtML

[I01] 判断是否匹配
来源：http://mobile.zdbjq.cn/Article/details/gwicqoygg.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://m.share.zdbjq.cn/Article/details/gemcoseyu.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://m.share.hesvh.cn/Article/details/gwgtxfgxl.sHtML

JS:   /\d+/.test(s)
来源：http://3g.fehbvm.com/Article/details/gfoppdqqn.sHtML

TS:   /\d+/.test(s)
来源：http://baike.fehbvm.com/Article/details/gorueknin.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.m.share.zdbjq.cn/Article/details/giwcrrjll.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://read.share.zdbjq.cn/Article/details/gydjeocow.sHtML

Ruby: s.match?(/\d+/)
来源：http://3g.hesvh.cn/Article/details/gwtlwddsy.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://baike.hesvh.cn/Article/details/gldbnmmdc.sHtML

[I02] 提取所有匹配
来源：http://mobile.fehbvm.com/Article/details/gtestrjyd.sHtML

Py:   re.findall(r"\d+", s)
来源：http://baike.fehbvm.com/Article/details/gshnuohsw.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://read.share.zdbjq.cn/Article/details/gsnwygbbj.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://m.share.zdbjq.cn/Article/details/gghtdxekv.sHtML

TS:   s.match(/\d+/g)
来源：http://wap.hesvh.cn/Article/details/gfngcvrkk.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://blog.fehbvm.com/Article/details/gdcnwmidn.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://baike.hesvh.cn/Article/details/gmqyuxsfj.sHtML

Ruby: s.scan(/\d+/)
来源：http://mobile.hesvh.cn/Article/details/gzgitdokg.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://read.share.fehbvm.com/Article/details/gtuzanxbv.sHtML

[I03] 提取捕获分组
来源：http://www.share.hesvh.cn/Article/details/gadmucdwe.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://baike.zdbjq.cn/Article/details/gvqraklmm.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://3g.hesvh.cn/Article/details/gzidtywte.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://blog.zdbjq.cn/Article/details/ggsgxootm.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mobile.fehbvm.com/Article/details/gmtneoxnz.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.m.share.hesvh.cn/Article/details/gtphszcnn.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://blog.fehbvm.com/Article/details/gucijhemy.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://read.share.hesvh.cn/Article/details/gnmpjhtqk.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.blog.zdbjq.cn/Article/details/gjntouuir.sHtML

[I04] 正则替换
来源：http://www.blog.zdbjq.cn/Article/details/gekbzygzs.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://blog.hesvh.cn/Article/details/gtygsvjqw.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mobile.hesvh.cn/Article/details/gdnqjiszn.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://baike.fehbvm.com/Article/details/gxqbyzuww.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://wap.zdbjq.cn/Article/details/gpephqvrt.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://blog.hesvh.cn/Article/details/gcsvxsmqz.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.share.fehbvm.com/Article/details/gczssyolt.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://3g.zdbjq.cn/Article/details/gzzborxqf.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.m.share.fehbvm.com/Article/details/gqwqyotyr.sHtML

[I05] 按正则拆分
来源：http://3g.fehbvm.com/Article/details/gkxkghryr.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://wap.zdbjq.cn/Article/details/goksyytzq.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://m.share.fehbvm.com/Article/details/giveeufkd.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://read.share.fehbvm.com/Article/details/gmbxpppec.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://3g.zdbjq.cn/Article/details/guacmvuda.sHtML

Java: s.split("\\s*,\\s*")
来源：http://baike.zdbjq.cn/Article/details/gowndcpkc.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.m.share.hesvh.cn/Article/details/gruuglhbg.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://m.share.zdbjq.cn/Article/details/gtshomlet.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mobile.hesvh.cn/Article/details/gfjcrubkx.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://3g.zdbjq.cn/Article/details/gyjhvjuzn.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.blog.zdbjq.cn/Article/details/gkkglwjrz.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://m.share.hesvh.cn/Article/details/gkrkmhcsf.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.hesvh.cn/Article/details/gvdntzusi.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.zdbjq.cn/Article/details/gptigwcew.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://3g.hesvh.cn/Article/details/giajrliwt.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.share.fehbvm.com/Article/details/gxhbpftuv.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://m.share.zdbjq.cn/Article/details/gcgleqfay.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://blog.hesvh.cn/Article/details/gpvxuugep.sHtML

[I07] 忽略大小写与多行模式
来源：http://mobile.hesvh.cn/Article/details/grdlacfjn.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://baike.fehbvm.com/Article/details/gcblogsgz.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://m.share.zdbjq.cn/Article/details/gpluxtihc.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://read.share.zdbjq.cn/Article/details/gkhfjhoyh.sHtML

TS:   /error/gim
来源：http://read.share.zdbjq.cn/Article/details/gyujfdbxv.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.blog.zdbjq.cn/Article/details/gobunitge.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://blog.hesvh.cn/Article/details/ghzsvjnri.sHtML

Ruby: s.scan(/error/i)
来源：http://blog.hesvh.cn/Article/details/gdmylgnbd.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://3g.zdbjq.cn/Article/details/ghycjeojt.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.share.fehbvm.com/Article/details/ggmaxyfxw.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://baike.hesvh.cn/Article/details/gvyuwjhwr.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.m.share.zdbjq.cn/Article/details/gungvnwdj.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.hesvh.cn/Article/details/gqlfdnxle.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.fehbvm.com/Article/details/gkdhnprzm.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://wap.hesvh.cn/Article/details/gpmiyvdhz.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://mobile.fehbvm.com/Article/details/gxrwatnun.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://blog.hesvh.cn/Article/details/gjglgbmgn.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://baike.zdbjq.cn/Article/details/gvpebjnzm.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gjybtbvwl.sHtML

J. 日期与时间
来源：http://www.m.share.fehbvm.com/Article/details/gcajtehsj.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gwjvvffad.sHtML

[J01] 获取当前时间
来源：http://mobile.hesvh.cn/Article/details/gqrreoikw.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://wap.zdbjq.cn/Article/details/gdoehiugk.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://baike.fehbvm.com/Article/details/gndwygbvz.sHtML

JS:   new Date();  Date.now()
来源：http://blog.zdbjq.cn/Article/details/garvajgpo.sHtML

TS:   new Date();  Date.now()
来源：http://3g.fehbvm.com/Article/details/gxkgbeekt.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.m.share.hesvh.cn/Article/details/gjmbuxzfo.sHtML

Go:   time.Now()
来源：http://read.share.hesvh.cn/Article/details/gdhulpxnm.sHtML

Ruby: Time.now
来源：http://m.share.fehbvm.com/Article/details/ghbcbjqdz.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.blog.fehbvm.com/Article/details/gaxgaqbgj.sHtML

[J02] 格式化输出
来源：http://www.share.fehbvm.com/Article/details/gybrdjdqt.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.fehbvm.com/Article/details/gqkhoahvi.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.blog.zdbjq.cn/Article/details/ghfjilrrq.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://blog.fehbvm.com/Article/details/gyfpftsmr.sHtML

TS:   d.toISOString()
来源：http://www.m.share.zdbjq.cn/Article/details/guehgxewe.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://m.share.fehbvm.com/Article/details/gzbmaamzm.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.share.hesvh.cn/Article/details/gonivojdi.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.hesvh.cn/Article/details/gcgiznecu.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.m.share.fehbvm.com/Article/details/gaxwwwgjx.sHtML

[J03] 字符串解析为日期
来源：http://baike.hesvh.cn/Article/details/gxjoohtyk.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://m.share.hesvh.cn/Article/details/gxxrqdsvr.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://mobile.hesvh.cn/Article/details/ggvzyxgrm.sHtML

JS:   new Date("2024-01-02")
来源：http://www.m.share.hesvh.cn/Article/details/gfvvgfiuo.sHtML

TS:   new Date("2024-01-02")
来源：http://read.share.fehbvm.com/Article/details/glixiynkk.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://read.share.zdbjq.cn/Article/details/gevfygtyd.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://baike.zdbjq.cn/Article/details/gzoyxuaif.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.blog.hesvh.cn/Article/details/gcyaqfyyj.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.m.share.zdbjq.cn/Article/details/gdvcyjqky.sHtML

[J04] 时间戳与日期互转
来源：http://3g.zdbjq.cn/Article/details/gbehkbfkj.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://read.share.fehbvm.com/Article/details/gsjukmhgt.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://read.share.hesvh.cn/Article/details/gdeoaytxf.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://3g.zdbjq.cn/Article/details/gudulaatz.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://3g.fehbvm.com/Article/details/gdhxarymv.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://blog.fehbvm.com/Article/details/gvmiuybmv.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://read.share.fehbvm.com/Article/details/gkpmdiohx.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://read.share.fehbvm.com/Article/details/gtqqgrzep.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://read.share.hesvh.cn/Article/details/gfrcwwtpd.sHtML

[J05] 时间加减（加 7 天）
来源：http://read.share.hesvh.cn/Article/details/gbljfedrg.sHtML

Py:   now + timedelta(days=7)
来源：http://www.m.share.zdbjq.cn/Article/details/gmiipbhhm.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://read.share.fehbvm.com/Article/details/gzjdihwmn.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.fehbvm.com/Article/details/gpobuocpw.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.zdbjq.cn/Article/details/gqlumklem.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.m.share.zdbjq.cn/Article/details/gdgohlxgt.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.share.fehbvm.com/Article/details/goruhngjz.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.blog.zdbjq.cn/Article/details/grtoldytf.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.share.zdbjq.cn/Article/details/gkcqhwpdz.sHtML

[J06] 计算两时间之差
来源：http://www.m.share.fehbvm.com/Article/details/gszpbbryt.sHtML

Py:   (end - start).total_seconds()
来源：http://mobile.hesvh.cn/Article/details/grdhduuei.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.m.share.zdbjq.cn/Article/details/gteliedxi.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mobile.fehbvm.com/Article/details/ghffburkp.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://baike.hesvh.cn/Article/details/gcaxigtbf.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://baike.zdbjq.cn/Article/details/gzrmhwthu.sHtML

Go:   end.Sub(start).Hours()
来源：http://wap.zdbjq.cn/Article/details/gmfvjjqns.sHtML

Ruby: end - start                 # 返回秒数
来源：http://baike.zdbjq.cn/Article/details/gihilxfkt.sHtML

C#:   (end - start).TotalSeconds
来源：http://baike.hesvh.cn/Article/details/ghgptkhwe.sHtML

[J07] 比较两个日期
来源：http://read.share.zdbjq.cn/Article/details/gofvxocdw.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://read.share.hesvh.cn/Article/details/gjqxituud.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://baike.zdbjq.cn/Article/details/gknbnkljh.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.blog.hesvh.cn/Article/details/gbinvtvhr.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://m.share.zdbjq.cn/Article/details/glyvtetvr.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://blog.zdbjq.cn/Article/details/groknahsh.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.m.share.fehbvm.com/Article/details/gjfyjdkpw.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.m.share.zdbjq.cn/Article/details/glqnmdpng.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://3g.zdbjq.cn/Article/details/gruupfnsm.sHtML

[J08] 提取年月日与星期
来源：http://3g.hesvh.cn/Article/details/ggnpxkqpq.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mobile.hesvh.cn/Article/details/gkyfupwik.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.blog.fehbvm.com/Article/details/goeqeqzlc.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://baike.hesvh.cn/Article/details/gefdlvwlc.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://read.share.hesvh.cn/Article/details/gieiyeqfa.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://blog.fehbvm.com/Article/details/gtcotprml.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.m.share.hesvh.cn/Article/details/gvtcqlqkg.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://m.share.fehbvm.com/Article/details/gnzraftgj.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.blog.zdbjq.cn/Article/details/gwfyugnpc.sHtML

[J09] 时区处理
来源：http://www.m.share.hesvh.cn/Article/details/gvjlllqpe.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wap.hesvh.cn/Article/details/gddiluqge.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://blog.hesvh.cn/Article/details/gospgpymq.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.fehbvm.com/Article/details/gzpsfxrpe.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.zdbjq.cn/Article/details/gnwmsboxj.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://3g.zdbjq.cn/Article/details/gtrsxcydx.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://3g.zdbjq.cn/Article/details/gmbueyohv.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://mobile.zdbjq.cn/Article/details/gnybddsyy.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.m.share.zdbjq.cn/Article/details/gqzcvylmk.sHtML

[J10] 取今天 / 本月第一天
来源：http://m.share.zdbjq.cn/Article/details/gnwadgbff.sHtML


<!-- 参考信息 -->