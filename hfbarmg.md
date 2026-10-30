代发 wailian999

Ruby: attr_accessor :name
来源：http://www.m.share.fehbvm.com/Article/details/gdcowwvki.sHtML

C#:   public string Name { get; set; }
来源：http://blog.hesvh.cn/Article/details/gffvvdaoz.sHtML

[G12] 对象转字符串
来源：http://www.share.fehbvm.com/Article/details/gshubiqjs.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.zdbjq.cn/Article/details/gkuefqtyj.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.hesvh.cn/Article/details/gchhdvyir.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/guplqjaae.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.hesvh.cn/Article/details/gayloskcb.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.hesvh.cn/Article/details/gwsscpcod.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.hesvh.cn/Article/details/gpwxjfrnc.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.zdbjq.cn/Article/details/gdaklrxla.sHtML

C#:   public override string ToString() => Name;
来源：http://www.share.hesvh.cn/Article/details/gyujrphkm.sHtML

[G13] 判断对象类型
来源：http://wap.hesvh.cn/Article/details/glritcbdp.sHtML

Py:   isinstance(u, User)
来源：http://3g.fehbvm.com/Article/details/gpyuqcyzx.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.fehbvm.com/Article/details/gmegjyput.sHtML

JS:   u instanceof User
来源：http://www.share.hesvh.cn/Article/details/ghiyhoqjr.sHtML

TS:   u instanceof User
来源：http://www.share.fehbvm.com/Article/details/gjmjufgum.sHtML

Java: u instanceof User
来源：http://wap.hesvh.cn/Article/details/gwswytzxl.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.hesvh.cn/Article/details/gqemuwaif.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.zdbjq.cn/Article/details/gkytvgsng.sHtML

C#:   u is User
来源：http://read.share.hesvh.cn/Article/details/gfqocprjg.sHtML

[G14] 数据类 / record
来源：http://blog.zdbjq.cn/Article/details/gdnkfoqny.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.fehbvm.com/Article/details/grofqsacs.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.zdbjq.cn/Article/details/gkthnofah.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.fehbvm.com/Article/details/gsmnuadnd.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.zdbjq.cn/Article/details/gpvydeqld.sHtML

Java: record User(String name, int age) {}
来源：http://baike.fehbvm.com/Article/details/glaxurejp.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.zdbjq.cn/Article/details/gacxkyccf.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.zdbjq.cn/Article/details/gppjvsrze.sHtML

C#:   record User(string Name, int Age);
来源：http://read.share.zdbjq.cn/Article/details/geajamlvp.sHtML

[G15] 枚举
来源：http://www.m.share.hesvh.cn/Article/details/gjrtyzrtg.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.hesvh.cn/Article/details/ggqjgbljk.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.hesvh.cn/Article/details/gkgnsnmfl.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://read.share.fehbvm.com/Article/details/gvklwwfob.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gheioevef.sHtML

Java: enum Color { RED, GREEN }
来源：http://m.share.fehbvm.com/Article/details/gyteouicj.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.hesvh.cn/Article/details/gjnjqdlhb.sHtML

Ruby: Color = %i[red green].freeze
来源：http://read.share.zdbjq.cn/Article/details/guzbvdiwa.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.hesvh.cn/Article/details/gugzwpebp.sHtML

[G16] 对象转数组 / 字典
来源：http://www.m.share.zdbjq.cn/Article/details/gcyiyaijr.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.fehbvm.com/Article/details/gjscybzam.sHtML

PHP:  get_object_vars($obj);
来源：http://blog.hesvh.cn/Article/details/gjtvytwbq.sHtML

JS:   Object.entries(obj)
来源：http://wap.hesvh.cn/Article/details/gshepuvnb.sHtML

TS:   Object.entries(obj)
来源：http://3g.zdbjq.cn/Article/details/gvpserjpg.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.zdbjq.cn/Article/details/gojkocsff.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.fehbvm.com/Article/details/ghacwuizj.sHtML

Ruby: obj.instance_variables
来源：http://read.share.fehbvm.com/Article/details/gbndjvung.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.hesvh.cn/Article/details/gxdsfbqds.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/guirmyjrw.sHtML

H. 异常与错误处理
来源：http://blog.zdbjq.cn/Article/details/gdtetwyfg.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gozkrmifo.sHtML

[H01] try / catch 基础
来源：http://www.blog.fehbvm.com/Article/details/gbexuside.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.hesvh.cn/Article/details/gpcktbcsw.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.hesvh.cn/Article/details/gyrzmcmra.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.zdbjq.cn/Article/details/gqtenloky.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.hesvh.cn/Article/details/gspprungn.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.hesvh.cn/Article/details/gwsmuxibl.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://blog.fehbvm.com/Article/details/gwxhpmybz.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.m.share.fehbvm.com/Article/details/gnoauhplv.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.fehbvm.com/Article/details/ghmwhezdw.sHtML

[H02] finally / ensure 收尾
来源：http://mobile.fehbvm.com/Article/details/gwpjtbafa.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://read.share.fehbvm.com/Article/details/gqmarcpjc.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.share.hesvh.cn/Article/details/gamcwymmx.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://m.share.fehbvm.com/Article/details/gcjgyyoau.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.zdbjq.cn/Article/details/gvrcuktux.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://m.share.fehbvm.com/Article/details/gngkakaoi.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://read.share.zdbjq.cn/Article/details/gvznoqzgx.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.share.hesvh.cn/Article/details/gbxvfbzah.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://baike.fehbvm.com/Article/details/gfdwjxzmu.sHtML

[H03] 主动抛出异常
来源：http://www.m.share.fehbvm.com/Article/details/gsvcpasmm.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.fehbvm.com/Article/details/gjylkokgy.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blog.zdbjq.cn/Article/details/gbsodsmsk.sHtML

JS:   throw new Error("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/gtrqqynyq.sHtML

TS:   throw new Error("错误信息");
来源：http://mobile.hesvh.cn/Article/details/grgnryxgn.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.m.share.fehbvm.com/Article/details/gpwekkrcu.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.blog.zdbjq.cn/Article/details/gtmntkffm.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.fehbvm.com/Article/details/gzklbbeoo.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.fehbvm.com/Article/details/grxmgqcow.sHtML

[H04] 自定义异常类型
来源：http://www.blog.hesvh.cn/Article/details/gcpjvojae.sHtML

Py:   class MyError(Exception): pass
来源：http://read.share.fehbvm.com/Article/details/gxujmluiq.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://3g.zdbjq.cn/Article/details/gymvrhcxk.sHtML

JS:   class MyError extends Error {}
来源：http://baike.zdbjq.cn/Article/details/gbgttvnsw.sHtML

TS:   class MyError extends Error {}
来源：http://3g.fehbvm.com/Article/details/ggwlhdjpz.sHtML

Java: class MyException extends RuntimeException {}
来源：http://m.share.fehbvm.com/Article/details/gkimmvswt.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.fehbvm.com/Article/details/gozfzwqll.sHtML

Ruby: class MyError < StandardError; end
来源：http://3g.zdbjq.cn/Article/details/gnlcdjonb.sHtML

C#:   class MyException : Exception {}
来源：http://www.m.share.zdbjq.cn/Article/details/gihikzkpa.sHtML

[H05] 捕获特定类型
来源：http://read.share.fehbvm.com/Article/details/gcnjydxqq.sHtML

Py:   except ValueError as e:
来源：http://blog.fehbvm.com/Article/details/gdqycxmjs.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://baike.fehbvm.com/Article/details/gaetrxlcj.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.blog.hesvh.cn/Article/details/gshkcetjk.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.blog.fehbvm.com/Article/details/gpfjdyenp.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gnnqpnmeq.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://3g.fehbvm.com/Article/details/gevniroxw.sHtML

Ruby: rescue ArgumentError => e
来源：http://3g.fehbvm.com/Article/details/gbipkawre.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wap.hesvh.cn/Article/details/gurfqfvca.sHtML

[H06] 可选值 / 空值安全访问
来源：http://read.share.fehbvm.com/Article/details/gqycwfsli.sHtML

Py:   value = d.get("k") or default
来源：http://wap.zdbjq.cn/Article/details/grjbayeel.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.share.fehbvm.com/Article/details/gpkwslaxo.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.share.hesvh.cn/Article/details/gfjtoylgx.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://m.share.zdbjq.cn/Article/details/gyxaxcbig.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://baike.hesvh.cn/Article/details/gucjimozk.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://wap.zdbjq.cn/Article/details/gwmirbsty.sHtML

Ruby: d&.dig(:a, :b)
来源：http://wap.hesvh.cn/Article/details/glhdgdelf.sHtML

C#:   obj?.A?.B ?? default
来源：http://blog.fehbvm.com/Article/details/glomuqckp.sHtML

[H07] 断言
来源：http://3g.zdbjq.cn/Article/details/gwkwbotih.sHtML

Py:   assert x > 0, "必须为正"
来源：http://wap.zdbjq.cn/Article/details/gabykgqdh.sHtML

PHP:  assert($x > 0);
来源：http://www.m.share.fehbvm.com/Article/details/gkwbyxbsl.sHtML

JS:   console.assert(x > 0);
来源：http://baike.fehbvm.com/Article/details/gzndbpabj.sHtML

TS:   console.assert(x > 0);
来源：http://3g.fehbvm.com/Article/details/gatgqgxmq.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.zdbjq.cn/Article/details/galbgvtlj.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wap.zdbjq.cn/Article/details/gfrlvdtgi.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://mobile.zdbjq.cn/Article/details/gbqekjvpf.sHtML

C#:   Debug.Assert(x > 0);
来源：http://blog.zdbjq.cn/Article/details/gpyvcycml.sHtML

[H08] 获取错误信息与堆栈
来源：http://3g.zdbjq.cn/Article/details/grdykifje.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.blog.zdbjq.cn/Article/details/grtzmctpg.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.blog.zdbjq.cn/Article/details/gmcabbfxc.sHtML

JS:   e.message;  e.stack
来源：http://wap.zdbjq.cn/Article/details/gizvynjfs.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://read.share.zdbjq.cn/Article/details/greaklqju.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://baike.hesvh.cn/Article/details/gitoobeuu.sHtML

Go:   err.Error()
来源：http://blog.zdbjq.cn/Article/details/gpkrdscrf.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.m.share.hesvh.cn/Article/details/gfkahagpr.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.share.hesvh.cn/Article/details/gyilbrequ.sHtML

[H09] 带错误码的异常
来源：http://www.share.hesvh.cn/Article/details/guhingwaj.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://3g.fehbvm.com/Article/details/gtwjqtlou.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.blog.zdbjq.cn/Article/details/gncxesdwr.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://3g.hesvh.cn/Article/details/gcteajyyc.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://3g.fehbvm.com/Article/details/gdnntvexg.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://3g.fehbvm.com/Article/details/gaetiksda.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://m.share.hesvh.cn/Article/details/ghylzxlfu.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://read.share.hesvh.cn/Article/details/gsqdhqegh.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://3g.hesvh.cn/Article/details/gwspvpwyc.sHtML

[H10] 资源自动释放
来源：http://3g.zdbjq.cn/Article/details/gksqlnxrh.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://baike.fehbvm.com/Article/details/gnuwpzynt.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wap.zdbjq.cn/Article/details/gadpizddc.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.hesvh.cn/Article/details/ghyubmpoc.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.zdbjq.cn/Article/details/ghaxkfbco.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://baike.hesvh.cn/Article/details/gqvscmkpq.sHtML

Go:   defer f.Close()
来源：http://blog.fehbvm.com/Article/details/gvliqhhkj.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.blog.zdbjq.cn/Article/details/gguyidgou.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gkejekkcn.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gbocidqrk.sHtML

I. 正则表达式
来源：http://www.blog.hesvh.cn/Article/details/gmxmysjhh.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gmbpekqmv.sHtML

[I01] 判断是否匹配
来源：http://www.blog.zdbjq.cn/Article/details/gklreblov.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.m.share.zdbjq.cn/Article/details/glbsmvgxp.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://mobile.hesvh.cn/Article/details/giprknsdw.sHtML

JS:   /\d+/.test(s)
来源：http://wap.hesvh.cn/Article/details/gghhakklx.sHtML

TS:   /\d+/.test(s)
来源：http://mobile.zdbjq.cn/Article/details/greikqwcz.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mobile.zdbjq.cn/Article/details/gogcrivgc.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.blog.fehbvm.com/Article/details/gtspgupve.sHtML

Ruby: s.match?(/\d+/)
来源：http://m.share.fehbvm.com/Article/details/gyodrqmyb.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://3g.fehbvm.com/Article/details/ghcrbmivb.sHtML

[I02] 提取所有匹配
来源：http://m.share.hesvh.cn/Article/details/glndcsaav.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.share.zdbjq.cn/Article/details/gufkszosv.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://baike.fehbvm.com/Article/details/gzibqozyt.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.blog.zdbjq.cn/Article/details/gziecrwus.sHtML

TS:   s.match(/\d+/g)
来源：http://blog.fehbvm.com/Article/details/gfghjhzsb.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://baike.fehbvm.com/Article/details/gpvdlqvzb.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://3g.fehbvm.com/Article/details/gkileyaju.sHtML

Ruby: s.scan(/\d+/)
来源：http://mobile.zdbjq.cn/Article/details/gcewwbezv.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://3g.hesvh.cn/Article/details/gsxtyhtle.sHtML

[I03] 提取捕获分组
来源：http://mobile.fehbvm.com/Article/details/gmzygjhxo.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://m.share.fehbvm.com/Article/details/gstytrppl.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://baike.hesvh.cn/Article/details/gpruwxxsd.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://read.share.fehbvm.com/Article/details/gysuenipv.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.blog.hesvh.cn/Article/details/ghvxnavwi.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.m.share.zdbjq.cn/Article/details/gwhjjzior.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wap.zdbjq.cn/Article/details/gpjccnuky.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://read.share.hesvh.cn/Article/details/gggtnzgwv.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://blog.hesvh.cn/Article/details/gfvvwjzhg.sHtML

[I04] 正则替换
来源：http://3g.zdbjq.cn/Article/details/gbqugfzzm.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://read.share.zdbjq.cn/Article/details/gnmlwfnim.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://3g.hesvh.cn/Article/details/gphttayha.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://3g.hesvh.cn/Article/details/gfcfhfmwd.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://3g.zdbjq.cn/Article/details/gwvekcmzf.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://blog.zdbjq.cn/Article/details/gylcxanau.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.m.share.zdbjq.cn/Article/details/grnyyceec.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://mobile.zdbjq.cn/Article/details/gqajeqzud.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.m.share.zdbjq.cn/Article/details/gldsiwlfl.sHtML

[I05] 按正则拆分
来源：http://read.share.hesvh.cn/Article/details/gnltctqkk.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://wap.fehbvm.com/Article/details/gbznefhnr.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://baike.fehbvm.com/Article/details/gygfsfqfr.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://mobile.fehbvm.com/Article/details/gbgotvkxd.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://baike.zdbjq.cn/Article/details/goryrejdk.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.share.fehbvm.com/Article/details/gmtpjbegl.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://m.share.fehbvm.com/Article/details/gpbbnlzjy.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.blog.hesvh.cn/Article/details/gqnzhieqa.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://baike.zdbjq.cn/Article/details/gbqnjpwyt.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://blog.hesvh.cn/Article/details/gkgtdgfxg.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.blog.hesvh.cn/Article/details/gpbdqdjtl.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://mobile.hesvh.cn/Article/details/gnwrefpyi.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.zdbjq.cn/Article/details/gderzsxuz.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.fehbvm.com/Article/details/gasuzgcsn.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wap.zdbjq.cn/Article/details/gzqsaypiy.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wap.hesvh.cn/Article/details/gducunnrp.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.share.fehbvm.com/Article/details/gppymhcan.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://baike.zdbjq.cn/Article/details/gymjsltjd.sHtML

[I07] 忽略大小写与多行模式
来源：http://blog.hesvh.cn/Article/details/gnglinncp.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://baike.hesvh.cn/Article/details/gyqskbjrb.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.m.share.hesvh.cn/Article/details/gtvblheqa.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mobile.fehbvm.com/Article/details/gpdmnzlyl.sHtML

TS:   /error/gim
来源：http://blog.fehbvm.com/Article/details/glfrslbbd.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.m.share.fehbvm.com/Article/details/gycvzztwf.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.m.share.zdbjq.cn/Article/details/gyyfuamzk.sHtML

Ruby: s.scan(/error/i)
来源：http://www.share.zdbjq.cn/Article/details/ghpelgehl.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://read.share.hesvh.cn/Article/details/gupknuqhr.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://read.share.zdbjq.cn/Article/details/grdvicuje.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wap.hesvh.cn/Article/details/gcxwmwxda.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://baike.hesvh.cn/Article/details/gvrggpvtg.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.zdbjq.cn/Article/details/gfwcseiap.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.zdbjq.cn/Article/details/greibahoj.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://read.share.zdbjq.cn/Article/details/guootoygv.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://blog.hesvh.cn/Article/details/gyujfprdh.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.share.hesvh.cn/Article/details/gvzdkkobj.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wap.zdbjq.cn/Article/details/gqocwmorm.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gptgrgunc.sHtML

J. 日期与时间
来源：http://blog.hesvh.cn/Article/details/gfavwkdsk.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gxrzzogyf.sHtML

[J01] 获取当前时间
来源：http://3g.fehbvm.com/Article/details/gzlcyyktq.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://3g.hesvh.cn/Article/details/gajzalpec.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.share.fehbvm.com/Article/details/gevvtpgzq.sHtML

JS:   new Date();  Date.now()
来源：http://baike.zdbjq.cn/Article/details/gniedecpm.sHtML

TS:   new Date();  Date.now()
来源：http://www.m.share.hesvh.cn/Article/details/gqamyfvro.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://m.share.fehbvm.com/Article/details/gqqjkqrjc.sHtML

Go:   time.Now()
来源：http://www.blog.fehbvm.com/Article/details/gbfixitbq.sHtML

Ruby: Time.now
来源：http://read.share.zdbjq.cn/Article/details/ghtawsxtb.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://read.share.hesvh.cn/Article/details/gluecuwmb.sHtML

[J02] 格式化输出
来源：http://read.share.fehbvm.com/Article/details/gkqljrxue.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.fehbvm.com/Article/details/gxifufwlc.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mobile.zdbjq.cn/Article/details/gmtgecdfk.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://read.share.fehbvm.com/Article/details/gzndyqwan.sHtML

TS:   d.toISOString()
来源：http://m.share.fehbvm.com/Article/details/gpqjsylii.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mobile.zdbjq.cn/Article/details/gjdxlopwt.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://baike.fehbvm.com/Article/details/gamyrcljc.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.fehbvm.com/Article/details/ggzbfndgh.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://read.share.hesvh.cn/Article/details/gduygdaif.sHtML

[J03] 字符串解析为日期
来源：http://www.blog.fehbvm.com/Article/details/glpuvprol.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.blog.hesvh.cn/Article/details/getcwjjan.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.blog.zdbjq.cn/Article/details/gtmcsslpo.sHtML

JS:   new Date("2024-01-02")
来源：http://blog.fehbvm.com/Article/details/gifrspkts.sHtML

TS:   new Date("2024-01-02")
来源：http://www.share.zdbjq.cn/Article/details/gynltohkr.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://mobile.fehbvm.com/Article/details/gvnwcquuf.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://3g.zdbjq.cn/Article/details/gyfvzxrsz.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.blog.fehbvm.com/Article/details/gwauyimsa.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.blog.hesvh.cn/Article/details/gmtfnvwcp.sHtML

[J04] 时间戳与日期互转
来源：http://m.share.fehbvm.com/Article/details/gkdamnnzv.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://read.share.zdbjq.cn/Article/details/gpcjwacpq.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.share.fehbvm.com/Article/details/gnqmkayzc.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.blog.fehbvm.com/Article/details/gclyalopi.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.share.zdbjq.cn/Article/details/gwodddvme.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://mobile.fehbvm.com/Article/details/gwowzdmys.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gyxnbsvmb.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.share.zdbjq.cn/Article/details/ghxxicmgm.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.m.share.hesvh.cn/Article/details/gxzjlomsv.sHtML

[J05] 时间加减（加 7 天）
来源：http://3g.hesvh.cn/Article/details/glivjqxrz.sHtML

Py:   now + timedelta(days=7)
来源：http://www.blog.zdbjq.cn/Article/details/gidnkpser.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.blog.hesvh.cn/Article/details/gspgpmykm.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.zdbjq.cn/Article/details/gqpjngvkm.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.fehbvm.com/Article/details/gaqztveir.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://mobile.hesvh.cn/Article/details/gbcueyxjv.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://read.share.fehbvm.com/Article/details/glhrvdzzg.sHtML

Ruby: Time.now + 7 * 86400
来源：http://m.share.zdbjq.cn/Article/details/gfqvrujfx.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.m.share.zdbjq.cn/Article/details/grroxuhxe.sHtML

[J06] 计算两时间之差
来源：http://www.share.fehbvm.com/Article/details/gprtshxdm.sHtML

Py:   (end - start).total_seconds()
来源：http://blog.zdbjq.cn/Article/details/gjhzoqmqg.sHtML

PHP:  $end->diff($start)->days;
来源：http://read.share.zdbjq.cn/Article/details/gatnpqsyg.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://3g.fehbvm.com/Article/details/guoncoyje.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.share.fehbvm.com/Article/details/gtvqmmbta.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.blog.zdbjq.cn/Article/details/gqvbotgvb.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.blog.zdbjq.cn/Article/details/gxtrqtjko.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.share.hesvh.cn/Article/details/gdldlieem.sHtML

C#:   (end - start).TotalSeconds
来源：http://read.share.zdbjq.cn/Article/details/ghutwdeox.sHtML

[J07] 比较两个日期
来源：http://mobile.fehbvm.com/Article/details/gubhrmcyq.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://3g.zdbjq.cn/Article/details/gddzhdcnx.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://read.share.fehbvm.com/Article/details/gmqetekym.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://3g.zdbjq.cn/Article/details/gcwhnsoea.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://baike.zdbjq.cn/Article/details/gsbteknsf.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mobile.zdbjq.cn/Article/details/gcdergkuv.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://read.share.fehbvm.com/Article/details/gxgpcovme.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://mobile.zdbjq.cn/Article/details/gpanpkrcx.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://mobile.zdbjq.cn/Article/details/gzxqehlar.sHtML

[J08] 提取年月日与星期
来源：http://www.blog.hesvh.cn/Article/details/gcxdfowij.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wap.hesvh.cn/Article/details/ggxgyoxwp.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.share.zdbjq.cn/Article/details/gjmrosbmj.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mobile.zdbjq.cn/Article/details/gigsfpgbb.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://read.share.hesvh.cn/Article/details/glqtygkjz.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wap.fehbvm.com/Article/details/ggiqoamtq.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wap.hesvh.cn/Article/details/giamsrbnp.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://3g.zdbjq.cn/Article/details/gvhzeuydw.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://blog.hesvh.cn/Article/details/gjblgqcgb.sHtML

[J09] 时区处理
来源：http://3g.hesvh.cn/Article/details/glttvvnyw.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.share.fehbvm.com/Article/details/gnfokbcvs.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://blog.zdbjq.cn/Article/details/gwherwxrg.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.fehbvm.com/Article/details/gydtcevvr.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.hesvh.cn/Article/details/grgpgercq.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.share.hesvh.cn/Article/details/gjtvyewfi.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.share.zdbjq.cn/Article/details/gzlwbhjex.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.blog.zdbjq.cn/Article/details/gfryggbjj.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wap.zdbjq.cn/Article/details/ghojxzsyv.sHtML

[J10] 取今天 / 本月第一天
来源：http://read.share.zdbjq.cn/Article/details/gxfixbhqq.sHtML


<!-- 参考信息 -->