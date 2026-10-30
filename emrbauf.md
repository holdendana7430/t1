代发 wailian999

JS:   get name() { return this._name; }
来源：http://wap.fehbvm.com/Article/details/gkybjvkgs.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gpuuenebg.sHtML

Java: public String getName() { return name; }
来源：http://m.share.hesvh.cn/Article/details/getsfnqlo.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.zdbjq.cn/Article/details/gzibotdah.sHtML

Ruby: attr_accessor :name
来源：http://3g.fehbvm.com/Article/details/gcjqlshwn.sHtML

C#:   public string Name { get; set; }
来源：http://3g.zdbjq.cn/Article/details/grolrtmmr.sHtML

[G12] 对象转字符串
来源：http://read.share.zdbjq.cn/Article/details/gignpogrb.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.zdbjq.cn/Article/details/grzxajfmv.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.zdbjq.cn/Article/details/gsfkocxkv.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.fehbvm.com/Article/details/gvbaeylkq.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/ghxyvaypj.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/gsllnvtri.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.zdbjq.cn/Article/details/gpyoeinpq.sHtML

Ruby: def to_s; @name; end
来源：http://3g.fehbvm.com/Article/details/gtkvgdtpr.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.fehbvm.com/Article/details/gezhnkqcy.sHtML

[G13] 判断对象类型
来源：http://blog.zdbjq.cn/Article/details/grqwlrpjc.sHtML

Py:   isinstance(u, User)
来源：http://www.share.zdbjq.cn/Article/details/gwhdvspmh.sHtML

PHP:  $u instanceof User
来源：http://www.share.fehbvm.com/Article/details/gqcorjyck.sHtML

JS:   u instanceof User
来源：http://mobile.fehbvm.com/Article/details/gtazvryrj.sHtML

TS:   u instanceof User
来源：http://read.share.fehbvm.com/Article/details/glfujkrgh.sHtML

Java: u instanceof User
来源：http://blog.hesvh.cn/Article/details/gqlypxmrs.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.zdbjq.cn/Article/details/gtvlkmvpe.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.fehbvm.com/Article/details/ggwjqjokb.sHtML

C#:   u is User
来源：http://baike.hesvh.cn/Article/details/ggfxolhim.sHtML

[G14] 数据类 / record
来源：http://read.share.fehbvm.com/Article/details/gxdokpaqc.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://baike.zdbjq.cn/Article/details/gqvigcjig.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.hesvh.cn/Article/details/gzrvgaiom.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.fehbvm.com/Article/details/gyncfgxrx.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.hesvh.cn/Article/details/ghuihskwe.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.fehbvm.com/Article/details/gewvtbdrq.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.hesvh.cn/Article/details/gjhdxkhtz.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.fehbvm.com/Article/details/gzjlmmbot.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.zdbjq.cn/Article/details/gqdfkhztk.sHtML

[G15] 枚举
来源：http://mobile.hesvh.cn/Article/details/gjmhlyrlu.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.fehbvm.com/Article/details/gckirnwhk.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://baike.zdbjq.cn/Article/details/gwyrdptgk.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.hesvh.cn/Article/details/gmfpjjwcz.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.hesvh.cn/Article/details/gfhbvhupe.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.zdbjq.cn/Article/details/gbcobzqqx.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://baike.hesvh.cn/Article/details/gaftoiraq.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.hesvh.cn/Article/details/gnfkughwr.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://blog.zdbjq.cn/Article/details/gdxsxrlko.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.fehbvm.com/Article/details/grndqtctc.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.hesvh.cn/Article/details/grbvjflyj.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.zdbjq.cn/Article/details/gtxqvlrcm.sHtML

JS:   Object.entries(obj)
来源：http://wap.zdbjq.cn/Article/details/gxamezqad.sHtML

TS:   Object.entries(obj)
来源：http://3g.zdbjq.cn/Article/details/gfawujgrx.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.fehbvm.com/Article/details/gwkotwuek.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.zdbjq.cn/Article/details/gljhodyrb.sHtML

Ruby: obj.instance_variables
来源：http://wap.zdbjq.cn/Article/details/ggxcxzrfc.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.zdbjq.cn/Article/details/gxvcvmjcd.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gamcwsepf.sHtML

H. 异常与错误处理
来源：http://www.blog.zdbjq.cn/Article/details/gkcttoyly.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gmkaaijxj.sHtML

[H01] try / catch 基础
来源：http://read.share.fehbvm.com/Article/details/gbgaaliru.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.fehbvm.com/Article/details/ggpgbkrpz.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.hesvh.cn/Article/details/gemnbzahu.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://m.share.zdbjq.cn/Article/details/gjsftgfby.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.fehbvm.com/Article/details/gxxixtkgl.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.fehbvm.com/Article/details/ghuggvkjm.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.fehbvm.com/Article/details/gbiagvwkc.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.hesvh.cn/Article/details/gkqcxiunf.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.fehbvm.com/Article/details/gphbguprr.sHtML

[H02] finally / ensure 收尾
来源：http://wap.fehbvm.com/Article/details/ghdkzyard.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://mobile.hesvh.cn/Article/details/gxkfiwzzx.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.zdbjq.cn/Article/details/gekazzfbu.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://mobile.fehbvm.com/Article/details/godgxnuoz.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.fehbvm.com/Article/details/gprpperwm.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://m.share.fehbvm.com/Article/details/gzncnwijc.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.share.fehbvm.com/Article/details/guugczejj.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.hesvh.cn/Article/details/gezyqxntj.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/ghwvkweuk.sHtML

[H03] 主动抛出异常
来源：http://www.blog.fehbvm.com/Article/details/gpmxsufew.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.m.share.zdbjq.cn/Article/details/gcbmwpuyh.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.blog.fehbvm.com/Article/details/gyxaqwddc.sHtML

JS:   throw new Error("错误信息");
来源：http://www.share.hesvh.cn/Article/details/gxowgujmd.sHtML

TS:   throw new Error("错误信息");
来源：http://wap.hesvh.cn/Article/details/gurucftjx.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://blog.zdbjq.cn/Article/details/gijmuuhyc.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://baike.fehbvm.com/Article/details/gjxsudycc.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://baike.fehbvm.com/Article/details/gsuagaeom.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.hesvh.cn/Article/details/gdorjajeg.sHtML

[H04] 自定义异常类型
来源：http://baike.zdbjq.cn/Article/details/gskdjqlgn.sHtML

Py:   class MyError(Exception): pass
来源：http://www.share.hesvh.cn/Article/details/gqdfjovat.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.hesvh.cn/Article/details/gntcdsgkr.sHtML

JS:   class MyError extends Error {}
来源：http://wap.fehbvm.com/Article/details/gzwplobsu.sHtML

TS:   class MyError extends Error {}
来源：http://www.share.hesvh.cn/Article/details/gbibjxbvh.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.blog.fehbvm.com/Article/details/grjdsulqo.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.fehbvm.com/Article/details/gzexsxxns.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.zdbjq.cn/Article/details/gfyjvhpzs.sHtML

C#:   class MyException : Exception {}
来源：http://3g.zdbjq.cn/Article/details/guknktfus.sHtML

[H05] 捕获特定类型
来源：http://baike.zdbjq.cn/Article/details/gkwshibnw.sHtML

Py:   except ValueError as e:
来源：http://m.share.fehbvm.com/Article/details/gelxapcnu.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://m.share.zdbjq.cn/Article/details/goxpyiabs.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.m.share.hesvh.cn/Article/details/gtzpmbxlp.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://blog.fehbvm.com/Article/details/gvhjtntqr.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://m.share.hesvh.cn/Article/details/gbvdjtayq.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mobile.zdbjq.cn/Article/details/gxnpvutua.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.m.share.zdbjq.cn/Article/details/gojphyyth.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mobile.fehbvm.com/Article/details/gzllqcxwx.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.share.fehbvm.com/Article/details/gjvikedcx.sHtML

Py:   value = d.get("k") or default
来源：http://3g.hesvh.cn/Article/details/glvgxyemx.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.hesvh.cn/Article/details/gnafzdayw.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://mobile.fehbvm.com/Article/details/gxxumeude.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://read.share.hesvh.cn/Article/details/gzxfgvhir.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://blog.fehbvm.com/Article/details/gcohffkwn.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.m.share.fehbvm.com/Article/details/ggjwwgdrp.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.blog.hesvh.cn/Article/details/girbvlten.sHtML

C#:   obj?.A?.B ?? default
来源：http://3g.zdbjq.cn/Article/details/gdpxgvcso.sHtML

[H07] 断言
来源：http://www.share.zdbjq.cn/Article/details/gvxzwupvf.sHtML

Py:   assert x > 0, "必须为正"
来源：http://baike.zdbjq.cn/Article/details/gdsxezhtz.sHtML

PHP:  assert($x > 0);
来源：http://wap.zdbjq.cn/Article/details/grrxexjao.sHtML

JS:   console.assert(x > 0);
来源：http://www.share.zdbjq.cn/Article/details/glatzqiwn.sHtML

TS:   console.assert(x > 0);
来源：http://3g.hesvh.cn/Article/details/gchetooqm.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.zdbjq.cn/Article/details/goiqctcpe.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://read.share.zdbjq.cn/Article/details/gibsazdpq.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://wap.zdbjq.cn/Article/details/ggkrgciaj.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.blog.zdbjq.cn/Article/details/gpnesizhf.sHtML

[H08] 获取错误信息与堆栈
来源：http://3g.fehbvm.com/Article/details/gtbogvsdv.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.blog.hesvh.cn/Article/details/gtwgdcfuv.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://m.share.zdbjq.cn/Article/details/gizjlqewc.sHtML

JS:   e.message;  e.stack
来源：http://blog.fehbvm.com/Article/details/gaerybpzn.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://m.share.zdbjq.cn/Article/details/gesmeqwft.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://mobile.zdbjq.cn/Article/details/gczokgish.sHtML

Go:   err.Error()
来源：http://mobile.zdbjq.cn/Article/details/gxfldrfqn.sHtML

Ruby: e.message;  e.backtrace
来源：http://blog.hesvh.cn/Article/details/gwzxoirvz.sHtML

C#:   e.Message;  e.StackTrace
来源：http://3g.hesvh.cn/Article/details/gatggqjmq.sHtML

[H09] 带错误码的异常
来源：http://www.blog.fehbvm.com/Article/details/gphafgevp.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.m.share.zdbjq.cn/Article/details/ggmxqdsnv.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://read.share.fehbvm.com/Article/details/gwhkechjv.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://3g.hesvh.cn/Article/details/gcpzqjhek.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.share.fehbvm.com/Article/details/gbskjypkf.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.m.share.fehbvm.com/Article/details/gfjouaypr.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://m.share.fehbvm.com/Article/details/gwmbatdch.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.m.share.zdbjq.cn/Article/details/gjujdzkej.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://baike.zdbjq.cn/Article/details/gibbbfsiz.sHtML

[H10] 资源自动释放
来源：http://3g.zdbjq.cn/Article/details/gjchaxdkx.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.m.share.zdbjq.cn/Article/details/gbckfgsuw.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wap.fehbvm.com/Article/details/gplzdrkks.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.zdbjq.cn/Article/details/ghpeoqvmf.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.zdbjq.cn/Article/details/ghgbvmxvh.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://m.share.zdbjq.cn/Article/details/gemydcgze.sHtML

Go:   defer f.Close()
来源：http://m.share.fehbvm.com/Article/details/gyghueyao.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.share.zdbjq.cn/Article/details/glvwqnwbi.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gmacgecjf.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gzknfeqpu.sHtML

I. 正则表达式
来源：http://m.share.zdbjq.cn/Article/details/gyzqthvzc.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gqfqdwotd.sHtML

[I01] 判断是否匹配
来源：http://www.blog.fehbvm.com/Article/details/gkejuwmja.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.share.zdbjq.cn/Article/details/ggfxopjrl.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://mobile.hesvh.cn/Article/details/gnyflegxp.sHtML

JS:   /\d+/.test(s)
来源：http://www.share.fehbvm.com/Article/details/gheedftpj.sHtML

TS:   /\d+/.test(s)
来源：http://read.share.zdbjq.cn/Article/details/gesugbvij.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.share.hesvh.cn/Article/details/gfvesgffe.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.m.share.hesvh.cn/Article/details/gkhrcmmbk.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.blog.zdbjq.cn/Article/details/glyqvskqi.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.m.share.fehbvm.com/Article/details/gykkspqkh.sHtML

[I02] 提取所有匹配
来源：http://www.m.share.hesvh.cn/Article/details/giqxjbuyy.sHtML

Py:   re.findall(r"\d+", s)
来源：http://wap.hesvh.cn/Article/details/girvdowlw.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://3g.zdbjq.cn/Article/details/ghkefrgzy.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.m.share.fehbvm.com/Article/details/gxfezldfd.sHtML

TS:   s.match(/\d+/g)
来源：http://blog.hesvh.cn/Article/details/gcyblywdj.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://read.share.hesvh.cn/Article/details/gymqirxyf.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wap.zdbjq.cn/Article/details/gskozrrau.sHtML

Ruby: s.scan(/\d+/)
来源：http://blog.hesvh.cn/Article/details/gvozcuwec.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://baike.hesvh.cn/Article/details/gwepkewmi.sHtML

[I03] 提取捕获分组
来源：http://www.share.fehbvm.com/Article/details/gwngzeclv.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://blog.zdbjq.cn/Article/details/gutqefoba.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://baike.fehbvm.com/Article/details/gydsogivu.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://baike.hesvh.cn/Article/details/gaxbdqcjk.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://baike.hesvh.cn/Article/details/gavgasyme.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.blog.fehbvm.com/Article/details/gwmqcbtej.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mobile.fehbvm.com/Article/details/gurbidkld.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wap.fehbvm.com/Article/details/ggopjikwq.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://read.share.zdbjq.cn/Article/details/gcntnfexb.sHtML

[I04] 正则替换
来源：http://3g.zdbjq.cn/Article/details/gqkhjdipq.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://3g.hesvh.cn/Article/details/gwtzdynfa.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mobile.hesvh.cn/Article/details/gcelamuwx.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://wap.hesvh.cn/Article/details/giznsuaal.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://m.share.zdbjq.cn/Article/details/ggkpcampw.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://3g.fehbvm.com/Article/details/gnpilavrg.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://blog.fehbvm.com/Article/details/gacysmlxf.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://m.share.zdbjq.cn/Article/details/gkqnkfwjs.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.m.share.hesvh.cn/Article/details/ggfvlxmpn.sHtML

[I05] 按正则拆分
来源：http://www.share.hesvh.cn/Article/details/gwnbkjnqu.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://mobile.zdbjq.cn/Article/details/gpgvhmhxj.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://baike.hesvh.cn/Article/details/grppvlwud.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.blog.zdbjq.cn/Article/details/gbnyrdxvl.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.m.share.hesvh.cn/Article/details/grfmcahsh.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.share.hesvh.cn/Article/details/ggsspmmky.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.m.share.fehbvm.com/Article/details/ghhneflfq.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://mobile.fehbvm.com/Article/details/gmwryorvu.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.share.hesvh.cn/Article/details/gzptwwhwq.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://baike.fehbvm.com/Article/details/glmzisacb.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://m.share.hesvh.cn/Article/details/gwbqdjxhy.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://baike.hesvh.cn/Article/details/ganyaobcs.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.hesvh.cn/Article/details/gwubeciwf.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.zdbjq.cn/Article/details/ggwdfhjuh.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://3g.zdbjq.cn/Article/details/gcydvhpbj.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://mobile.zdbjq.cn/Article/details/gjcqhjahx.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://3g.fehbvm.com/Article/details/gxueeemym.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.share.fehbvm.com/Article/details/gbimvtzgz.sHtML

[I07] 忽略大小写与多行模式
来源：http://baike.hesvh.cn/Article/details/gcamcinyh.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://blog.hesvh.cn/Article/details/gnxejzokw.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://read.share.hesvh.cn/Article/details/gozjvjtym.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://read.share.fehbvm.com/Article/details/gskuxobfy.sHtML

TS:   /error/gim
来源：http://baike.fehbvm.com/Article/details/grdxnejmi.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://read.share.fehbvm.com/Article/details/glkomkviy.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.m.share.fehbvm.com/Article/details/gqvxdqslu.sHtML

Ruby: s.scan(/error/i)
来源：http://mobile.hesvh.cn/Article/details/gyoeyvtzw.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.blog.zdbjq.cn/Article/details/gsqtrkzzw.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://3g.hesvh.cn/Article/details/gqxiwxvvm.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://m.share.fehbvm.com/Article/details/gumijapkj.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://3g.hesvh.cn/Article/details/gthrvokax.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.hesvh.cn/Article/details/gvuujhfbh.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.fehbvm.com/Article/details/gxxznafvh.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.m.share.fehbvm.com/Article/details/gmdzmkfcz.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.m.share.fehbvm.com/Article/details/gsyiiaofu.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://m.share.fehbvm.com/Article/details/gwyzmeuvb.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mobile.fehbvm.com/Article/details/gmpeuckpr.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gfrvyfers.sHtML

J. 日期与时间
来源：http://blog.hesvh.cn/Article/details/gcmymgpxy.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gwhcgumhp.sHtML

[J01] 获取当前时间
来源：http://baike.zdbjq.cn/Article/details/gsphgwlyi.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://read.share.zdbjq.cn/Article/details/gxkdaloek.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mobile.zdbjq.cn/Article/details/grmssqfty.sHtML

JS:   new Date();  Date.now()
来源：http://blog.zdbjq.cn/Article/details/gawkagjeo.sHtML

TS:   new Date();  Date.now()
来源：http://www.m.share.zdbjq.cn/Article/details/gcbcohaub.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://baike.hesvh.cn/Article/details/gublcmdoo.sHtML

Go:   time.Now()
来源：http://baike.fehbvm.com/Article/details/gfhckyqfr.sHtML

Ruby: Time.now
来源：http://baike.zdbjq.cn/Article/details/gytwfqjru.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.share.zdbjq.cn/Article/details/gjnnepnzk.sHtML

[J02] 格式化输出
来源：http://m.share.zdbjq.cn/Article/details/gbjweixdy.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.fehbvm.com/Article/details/ggtqtcvxt.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.share.fehbvm.com/Article/details/gqqkasdsa.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.blog.zdbjq.cn/Article/details/gcmscfwud.sHtML

TS:   d.toISOString()
来源：http://blog.zdbjq.cn/Article/details/gudlbaewt.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.blog.zdbjq.cn/Article/details/grnogmzeh.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.m.share.fehbvm.com/Article/details/gbmbtirze.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.hesvh.cn/Article/details/giwtlmlti.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.m.share.fehbvm.com/Article/details/gqsqexduw.sHtML

[J03] 字符串解析为日期
来源：http://m.share.fehbvm.com/Article/details/gsxeorvfe.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://read.share.hesvh.cn/Article/details/gpzzfdftj.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wap.zdbjq.cn/Article/details/giscoriie.sHtML

JS:   new Date("2024-01-02")
来源：http://m.share.fehbvm.com/Article/details/gctxjmojg.sHtML

TS:   new Date("2024-01-02")
来源：http://m.share.hesvh.cn/Article/details/gjrknulhz.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.share.hesvh.cn/Article/details/geqgszexv.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://m.share.zdbjq.cn/Article/details/gtagqllbs.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://baike.fehbvm.com/Article/details/ghqzvedlv.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mobile.fehbvm.com/Article/details/gmohxiyry.sHtML

[J04] 时间戳与日期互转
来源：http://blog.hesvh.cn/Article/details/gqlcrmixu.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://blog.hesvh.cn/Article/details/gnvkhstop.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://read.share.hesvh.cn/Article/details/gybijyhbn.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.share.zdbjq.cn/Article/details/guuqeqdwt.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://baike.fehbvm.com/Article/details/gmxkxaupl.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://read.share.fehbvm.com/Article/details/gaytsbqoq.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.share.hesvh.cn/Article/details/gmhbrjvsb.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wap.zdbjq.cn/Article/details/gfheiddls.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://read.share.fehbvm.com/Article/details/gsdrjvzbx.sHtML

[J05] 时间加减（加 7 天）
来源：http://read.share.hesvh.cn/Article/details/grmzqknzx.sHtML

Py:   now + timedelta(days=7)
来源：http://blog.hesvh.cn/Article/details/girjwkfpu.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://wap.zdbjq.cn/Article/details/gvouucicv.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.fehbvm.com/Article/details/gdrofkakd.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.hesvh.cn/Article/details/gwnkhskiz.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.blog.fehbvm.com/Article/details/ggjujsres.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://wap.fehbvm.com/Article/details/gvsukrtzk.sHtML

Ruby: Time.now + 7 * 86400
来源：http://3g.zdbjq.cn/Article/details/gbeqrwimw.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.blog.hesvh.cn/Article/details/gvvcwjxra.sHtML

[J06] 计算两时间之差
来源：http://3g.zdbjq.cn/Article/details/ghjyttgyf.sHtML

Py:   (end - start).total_seconds()
来源：http://baike.hesvh.cn/Article/details/gjrohptzh.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.m.share.zdbjq.cn/Article/details/gzkllxmxq.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://3g.fehbvm.com/Article/details/gvfrhlhnd.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wap.fehbvm.com/Article/details/gcmwcmgew.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.m.share.zdbjq.cn/Article/details/gctrnflvc.sHtML

Go:   end.Sub(start).Hours()
来源：http://wap.fehbvm.com/Article/details/gizrphcjl.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.blog.fehbvm.com/Article/details/glytjmlir.sHtML

C#:   (end - start).TotalSeconds
来源：http://m.share.fehbvm.com/Article/details/gtpfrnrhm.sHtML

[J07] 比较两个日期
来源：http://www.m.share.fehbvm.com/Article/details/gmfstbxtu.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://m.share.hesvh.cn/Article/details/gvdertrei.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://m.share.hesvh.cn/Article/details/gmwdrawmt.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://wap.hesvh.cn/Article/details/ghgzxmgae.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.share.hesvh.cn/Article/details/gulljkoeb.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://blog.fehbvm.com/Article/details/gpvkgbirn.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://mobile.fehbvm.com/Article/details/gamipxtrm.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.share.zdbjq.cn/Article/details/glyocmbrh.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://mobile.zdbjq.cn/Article/details/ggjajqemj.sHtML

[J08] 提取年月日与星期
来源：http://blog.fehbvm.com/Article/details/glqdyhxpc.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.share.zdbjq.cn/Article/details/giywjjxgx.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://m.share.fehbvm.com/Article/details/gelpinatx.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.m.share.fehbvm.com/Article/details/gfxwaaxoa.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://read.share.zdbjq.cn/Article/details/geqtmoezp.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://blog.fehbvm.com/Article/details/garptvpcj.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://baike.fehbvm.com/Article/details/gwkhktmqo.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wap.fehbvm.com/Article/details/gybqsmopt.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.blog.hesvh.cn/Article/details/godhsnwwa.sHtML

[J09] 时区处理
来源：http://baike.fehbvm.com/Article/details/gpharglnp.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://blog.zdbjq.cn/Article/details/gfwpjlpjr.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://read.share.zdbjq.cn/Article/details/genpxtjyv.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.zdbjq.cn/Article/details/gahnifmhy.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.zdbjq.cn/Article/details/gdfsleqvi.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.m.share.zdbjq.cn/Article/details/grxxeaedc.sHtML


<!-- 参考信息 -->