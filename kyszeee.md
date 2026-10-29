代发 wailian999

[G10] 访问控制
来源：http://wap.zdbjq.cn/Article/details/gdbknylgp.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.fehbvm.com/Article/details/gtjbdzssw.sHtML

PHP:  public / protected / private
来源：http://mobile.fehbvm.com/Article/details/gayxrjywl.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.fehbvm.com/Article/details/gyyimquna.sHtML

TS:   public / protected / private
来源：http://read.share.fehbvm.com/Article/details/gphsuzyzk.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.hesvh.cn/Article/details/gfeiuqpzk.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.fehbvm.com/Article/details/ghqhbtysc.sHtML

Ruby: public / protected / private
来源：http://www.share.fehbvm.com/Article/details/giytruevj.sHtML

C#:   public / protected / private / internal
来源：http://www.share.zdbjq.cn/Article/details/gdonvaeji.sHtML

[G11] getter / setter
来源：http://www.m.share.hesvh.cn/Article/details/gobfpufgy.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.fehbvm.com/Article/details/gafbkooob.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.hesvh.cn/Article/details/gyzbodaaf.sHtML

JS:   get name() { return this._name; }
来源：http://3g.hesvh.cn/Article/details/gqvurtghn.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.fehbvm.com/Article/details/gafdcxthf.sHtML

Java: public String getName() { return name; }
来源：http://mobile.fehbvm.com/Article/details/gofrzkefh.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.fehbvm.com/Article/details/gspbywzeo.sHtML

Ruby: attr_accessor :name
来源：http://baike.hesvh.cn/Article/details/gmgcsecez.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.zdbjq.cn/Article/details/gkqzgkkmi.sHtML

[G12] 对象转字符串
来源：http://3g.fehbvm.com/Article/details/gxqogkqte.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.fehbvm.com/Article/details/gsuqqcuia.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.zdbjq.cn/Article/details/gpcpvxgjm.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.hesvh.cn/Article/details/gzzwutdkh.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.hesvh.cn/Article/details/ggrrgdsmm.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.hesvh.cn/Article/details/gpitttvbn.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.zdbjq.cn/Article/details/grkhzcuhk.sHtML

Ruby: def to_s; @name; end
来源：http://blog.fehbvm.com/Article/details/ghcrbkenk.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.fehbvm.com/Article/details/ghauymqrz.sHtML

[G13] 判断对象类型
来源：http://mobile.zdbjq.cn/Article/details/gspyytznv.sHtML

Py:   isinstance(u, User)
来源：http://mobile.fehbvm.com/Article/details/gnaxvznuu.sHtML

PHP:  $u instanceof User
来源：http://baike.fehbvm.com/Article/details/gynwbuonz.sHtML

JS:   u instanceof User
来源：http://3g.fehbvm.com/Article/details/guhiprwns.sHtML

TS:   u instanceof User
来源：http://www.m.share.zdbjq.cn/Article/details/gtrdrfcuh.sHtML

Java: u instanceof User
来源：http://read.share.zdbjq.cn/Article/details/guabiehoq.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.zdbjq.cn/Article/details/gixpfxcig.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.zdbjq.cn/Article/details/gevoiuxgp.sHtML

C#:   u is User
来源：http://www.share.zdbjq.cn/Article/details/gzomcezvk.sHtML

[G14] 数据类 / record
来源：http://blog.hesvh.cn/Article/details/giechhwff.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.zdbjq.cn/Article/details/gqixhuslu.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.hesvh.cn/Article/details/gnpjspszn.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.zdbjq.cn/Article/details/gytfxopoc.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.share.zdbjq.cn/Article/details/gygjowhvv.sHtML

Java: record User(String name, int age) {}
来源：http://read.share.fehbvm.com/Article/details/glqxsfvqq.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.zdbjq.cn/Article/details/gfjdchwjl.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.fehbvm.com/Article/details/gsyzjhgrg.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.hesvh.cn/Article/details/gefrfjbrs.sHtML

[G15] 枚举
来源：http://mobile.fehbvm.com/Article/details/gitdnqsuh.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.hesvh.cn/Article/details/gmhxyoogr.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.fehbvm.com/Article/details/garaaqjoz.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.zdbjq.cn/Article/details/guufcryby.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://3g.fehbvm.com/Article/details/gamgbowlt.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.fehbvm.com/Article/details/gggnablsk.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.zdbjq.cn/Article/details/gtajfjrrd.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.fehbvm.com/Article/details/gofhbvdxx.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.fehbvm.com/Article/details/gqusnmgsk.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.fehbvm.com/Article/details/grdhfiqnb.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.hesvh.cn/Article/details/giotvzbeb.sHtML

PHP:  get_object_vars($obj);
来源：http://3g.hesvh.cn/Article/details/gujnosjur.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gcyifyeam.sHtML

TS:   Object.entries(obj)
来源：http://mobile.fehbvm.com/Article/details/gdstrsxrx.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.hesvh.cn/Article/details/gdhtkwxnd.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.zdbjq.cn/Article/details/gjszqlgyg.sHtML

Ruby: obj.instance_variables
来源：http://www.m.share.fehbvm.com/Article/details/gsxqfmccf.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.hesvh.cn/Article/details/glnxtirpx.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gtfaoaxes.sHtML

H. 异常与错误处理
来源：http://www.share.fehbvm.com/Article/details/gihimakte.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gqusvmvwq.sHtML

[H01] try / catch 基础
来源：http://wap.fehbvm.com/Article/details/gvqsqlzcf.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.zdbjq.cn/Article/details/glvpujplv.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mobile.fehbvm.com/Article/details/glwelslps.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.hesvh.cn/Article/details/gdohwvpvx.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://m.share.zdbjq.cn/Article/details/gnnocorts.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.blog.hesvh.cn/Article/details/gmyvnkhmb.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.zdbjq.cn/Article/details/gnesefzmr.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.share.hesvh.cn/Article/details/gvaupvcwg.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.hesvh.cn/Article/details/gkiafpyvr.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.fehbvm.com/Article/details/gzldsqjje.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.hesvh.cn/Article/details/gitrclbhp.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.share.hesvh.cn/Article/details/gwsoddzzl.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://mobile.zdbjq.cn/Article/details/gkdilaksu.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.fehbvm.com/Article/details/gbfiqjxos.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://m.share.hesvh.cn/Article/details/gsvcgxrgn.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://blog.fehbvm.com/Article/details/gdidpeius.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.hesvh.cn/Article/details/gnamcwgwe.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/girmeiqpn.sHtML

[H03] 主动抛出异常
来源：http://read.share.hesvh.cn/Article/details/gdhvapagj.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.fehbvm.com/Article/details/grvrzqnul.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.m.share.fehbvm.com/Article/details/gqzsphaxg.sHtML

JS:   throw new Error("错误信息");
来源：http://read.share.fehbvm.com/Article/details/gshtmaune.sHtML

TS:   throw new Error("错误信息");
来源：http://mobile.hesvh.cn/Article/details/gbctqtaqi.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://blog.fehbvm.com/Article/details/gvncspzmu.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.m.share.zdbjq.cn/Article/details/gposohchh.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.share.hesvh.cn/Article/details/gfkebhfcu.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.share.hesvh.cn/Article/details/glneshjos.sHtML

[H04] 自定义异常类型
来源：http://mobile.hesvh.cn/Article/details/gemnlthej.sHtML

Py:   class MyError(Exception): pass
来源：http://wap.fehbvm.com/Article/details/gddhnjunv.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://baike.zdbjq.cn/Article/details/gehvidjbo.sHtML

JS:   class MyError extends Error {}
来源：http://mobile.fehbvm.com/Article/details/gxqkbwmox.sHtML

TS:   class MyError extends Error {}
来源：http://read.share.hesvh.cn/Article/details/gkxoracab.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.hesvh.cn/Article/details/geylagseh.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.blog.zdbjq.cn/Article/details/gqmmztptd.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.m.share.fehbvm.com/Article/details/gdtlfhfaa.sHtML

C#:   class MyException : Exception {}
来源：http://blog.hesvh.cn/Article/details/gnbwnfydb.sHtML

[H05] 捕获特定类型
来源：http://www.share.zdbjq.cn/Article/details/gwtlzetwq.sHtML

Py:   except ValueError as e:
来源：http://www.m.share.fehbvm.com/Article/details/gvjezufiz.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.blog.zdbjq.cn/Article/details/gatfqnqha.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://3g.fehbvm.com/Article/details/gmuuxpusm.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.share.hesvh.cn/Article/details/gxfryipuf.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.zdbjq.cn/Article/details/gggdauqsa.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.m.share.fehbvm.com/Article/details/gmomanrnz.sHtML

Ruby: rescue ArgumentError => e
来源：http://read.share.fehbvm.com/Article/details/gtrwjsdck.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://baike.fehbvm.com/Article/details/gjkyzlylr.sHtML

[H06] 可选值 / 空值安全访问
来源：http://mobile.zdbjq.cn/Article/details/gthizuclq.sHtML

Py:   value = d.get("k") or default
来源：http://baike.fehbvm.com/Article/details/gsohvlfex.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.m.share.fehbvm.com/Article/details/gwyugjvty.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://wap.fehbvm.com/Article/details/gfixmkwht.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://blog.fehbvm.com/Article/details/gdewveyfc.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.blog.fehbvm.com/Article/details/gytfywjvc.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://mobile.fehbvm.com/Article/details/glctvesgs.sHtML

Ruby: d&.dig(:a, :b)
来源：http://read.share.zdbjq.cn/Article/details/gmboyvrnd.sHtML

C#:   obj?.A?.B ?? default
来源：http://read.share.fehbvm.com/Article/details/gvwsymqxv.sHtML

[H07] 断言
来源：http://www.blog.fehbvm.com/Article/details/gnsbltsuy.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.share.hesvh.cn/Article/details/glupenbmo.sHtML

PHP:  assert($x > 0);
来源：http://wap.zdbjq.cn/Article/details/gvgcebhti.sHtML

JS:   console.assert(x > 0);
来源：http://m.share.zdbjq.cn/Article/details/gcbkmuwvu.sHtML

TS:   console.assert(x > 0);
来源：http://wap.fehbvm.com/Article/details/gwsxreycn.sHtML

Java: assert x > 0 : "必须为正";
来源：http://mobile.fehbvm.com/Article/details/gljofaafi.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.m.share.zdbjq.cn/Article/details/gjefrdfcv.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://mobile.zdbjq.cn/Article/details/gqzbbemoj.sHtML

C#:   Debug.Assert(x > 0);
来源：http://wap.fehbvm.com/Article/details/giwaauhtk.sHtML

[H08] 获取错误信息与堆栈
来源：http://mobile.hesvh.cn/Article/details/ghlxlviby.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.m.share.hesvh.cn/Article/details/gmzpyefpj.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://read.share.zdbjq.cn/Article/details/gilfpqshj.sHtML

JS:   e.message;  e.stack
来源：http://m.share.fehbvm.com/Article/details/ghiplqwju.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.blog.hesvh.cn/Article/details/goblfibcc.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.share.zdbjq.cn/Article/details/gvnvckifc.sHtML

Go:   err.Error()
来源：http://baike.fehbvm.com/Article/details/gvqrooyzx.sHtML

Ruby: e.message;  e.backtrace
来源：http://read.share.hesvh.cn/Article/details/gdkynbnmd.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.m.share.hesvh.cn/Article/details/gpvpeexlh.sHtML

[H09] 带错误码的异常
来源：http://baike.zdbjq.cn/Article/details/gvelbsrvh.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mobile.hesvh.cn/Article/details/gzhhbhnsd.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.m.share.zdbjq.cn/Article/details/grocnyuul.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.blog.fehbvm.com/Article/details/gbihyicsg.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.share.fehbvm.com/Article/details/gcaydopvk.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.blog.hesvh.cn/Article/details/gfxpvkejd.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.m.share.hesvh.cn/Article/details/gzgynsnrj.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://3g.fehbvm.com/Article/details/gyktdzklr.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://3g.fehbvm.com/Article/details/gyebhdnnl.sHtML

[H10] 资源自动释放
来源：http://m.share.fehbvm.com/Article/details/garhfcgus.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://wap.hesvh.cn/Article/details/gvqpjplgt.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mobile.hesvh.cn/Article/details/gekmvdxbb.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.fehbvm.com/Article/details/gkqkzoolv.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.fehbvm.com/Article/details/gbimtvwat.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://read.share.zdbjq.cn/Article/details/gswwpyuec.sHtML

Go:   defer f.Close()
来源：http://3g.fehbvm.com/Article/details/gbyttasjl.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mobile.fehbvm.com/Article/details/gvzvghtdi.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/geantleii.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gqudlbyjb.sHtML

I. 正则表达式
来源：http://read.share.hesvh.cn/Article/details/gmyrmhnvw.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gzitmziog.sHtML

[I01] 判断是否匹配
来源：http://www.blog.zdbjq.cn/Article/details/gvlqygzlj.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mobile.zdbjq.cn/Article/details/gckobqdfj.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://blog.hesvh.cn/Article/details/gghdiohcx.sHtML

JS:   /\d+/.test(s)
来源：http://www.blog.hesvh.cn/Article/details/gswqcystq.sHtML

TS:   /\d+/.test(s)
来源：http://baike.hesvh.cn/Article/details/gqhztqxzo.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://3g.hesvh.cn/Article/details/gamqaheak.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://m.share.hesvh.cn/Article/details/gfpductjb.sHtML

Ruby: s.match?(/\d+/)
来源：http://m.share.hesvh.cn/Article/details/giwtdxryp.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://read.share.fehbvm.com/Article/details/glpmkwgkd.sHtML

[I02] 提取所有匹配
来源：http://baike.hesvh.cn/Article/details/gjxminymy.sHtML

Py:   re.findall(r"\d+", s)
来源：http://baike.hesvh.cn/Article/details/geyzgazdg.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://baike.zdbjq.cn/Article/details/geztqhhaw.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://baike.hesvh.cn/Article/details/gvnsiepzx.sHtML

TS:   s.match(/\d+/g)
来源：http://mobile.fehbvm.com/Article/details/gefsqeuwh.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://m.share.hesvh.cn/Article/details/gkcfmfpfs.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.m.share.zdbjq.cn/Article/details/gblbmlcqd.sHtML

Ruby: s.scan(/\d+/)
来源：http://3g.zdbjq.cn/Article/details/gjpxfvquu.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://baike.fehbvm.com/Article/details/gaanjllgl.sHtML

[I03] 提取捕获分组
来源：http://mobile.zdbjq.cn/Article/details/gvkbxergn.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.m.share.hesvh.cn/Article/details/gqrupudmz.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.blog.fehbvm.com/Article/details/gyukweqts.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wap.hesvh.cn/Article/details/gtwimscyn.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.blog.zdbjq.cn/Article/details/gihgpnwon.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wap.zdbjq.cn/Article/details/giaidvkzf.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://m.share.fehbvm.com/Article/details/gdtkypucy.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://m.share.fehbvm.com/Article/details/gcategoib.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://blog.zdbjq.cn/Article/details/gvzpphjzc.sHtML

[I04] 正则替换
来源：http://mobile.fehbvm.com/Article/details/gwfubxnnw.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://3g.zdbjq.cn/Article/details/gmkrfgsuc.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://blog.fehbvm.com/Article/details/gvlmltfvh.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://mobile.zdbjq.cn/Article/details/gjzgxprru.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://mobile.hesvh.cn/Article/details/gpsxrrftk.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://baike.fehbvm.com/Article/details/gtkudtomd.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://mobile.fehbvm.com/Article/details/gcpzadyql.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://3g.fehbvm.com/Article/details/gticsiuby.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.share.zdbjq.cn/Article/details/gbqrrjwcv.sHtML

[I05] 按正则拆分
来源：http://www.blog.hesvh.cn/Article/details/gqhhkezxe.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.share.hesvh.cn/Article/details/gnbhbijmj.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mobile.fehbvm.com/Article/details/gqawhqqhg.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://m.share.zdbjq.cn/Article/details/guzkejgdj.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://m.share.fehbvm.com/Article/details/gvoloewha.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.m.share.fehbvm.com/Article/details/gfxmphvwi.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://mobile.fehbvm.com/Article/details/gejarplbb.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://m.share.fehbvm.com/Article/details/gxxvlzcyj.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://3g.fehbvm.com/Article/details/gmfqddjvx.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.share.zdbjq.cn/Article/details/gjtijnvgx.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.m.share.zdbjq.cn/Article/details/goxnrhadu.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://read.share.zdbjq.cn/Article/details/gdozrbbcz.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.fehbvm.com/Article/details/gealoahra.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.hesvh.cn/Article/details/ghawtwlsd.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://baike.hesvh.cn/Article/details/gemvosnvb.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.m.share.fehbvm.com/Article/details/gxionnput.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://blog.hesvh.cn/Article/details/gvjeqiqlb.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://read.share.zdbjq.cn/Article/details/gbguwbqxa.sHtML

[I07] 忽略大小写与多行模式
来源：http://baike.hesvh.cn/Article/details/ghvlxodyv.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mobile.hesvh.cn/Article/details/gtmoueepp.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://m.share.hesvh.cn/Article/details/gcdyscgaq.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://m.share.zdbjq.cn/Article/details/gfvauyzle.sHtML

TS:   /error/gim
来源：http://www.share.fehbvm.com/Article/details/gdcbxxoml.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://blog.zdbjq.cn/Article/details/gmmjndrzq.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mobile.hesvh.cn/Article/details/gyauicimr.sHtML

Ruby: s.scan(/error/i)
来源：http://www.m.share.fehbvm.com/Article/details/gbycvqwhb.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://baike.hesvh.cn/Article/details/ggnxawpyt.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://3g.fehbvm.com/Article/details/gysmirnri.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://3g.fehbvm.com/Article/details/gbzmvtqxw.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://3g.zdbjq.cn/Article/details/gwybczvcf.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.fehbvm.com/Article/details/ghlbziyrv.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.zdbjq.cn/Article/details/ggnevkekp.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.m.share.zdbjq.cn/Article/details/gzgcsyhho.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.share.zdbjq.cn/Article/details/grfhyphwo.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.share.hesvh.cn/Article/details/glfrvgtag.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mobile.zdbjq.cn/Article/details/gpoihftpk.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gxfjekybh.sHtML

J. 日期与时间
来源：http://wap.zdbjq.cn/Article/details/gmjbfkeca.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/grpjzcprs.sHtML

[J01] 获取当前时间
来源：http://mobile.zdbjq.cn/Article/details/gdwmleadf.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://baike.fehbvm.com/Article/details/gpericwyr.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://wap.zdbjq.cn/Article/details/gchyuwdco.sHtML

JS:   new Date();  Date.now()
来源：http://baike.zdbjq.cn/Article/details/ggqpaypzi.sHtML

TS:   new Date();  Date.now()
来源：http://blog.hesvh.cn/Article/details/gbrkbfikw.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://baike.fehbvm.com/Article/details/glfctwrvl.sHtML

Go:   time.Now()
来源：http://m.share.hesvh.cn/Article/details/gtgbuvzhb.sHtML

Ruby: Time.now
来源：http://3g.zdbjq.cn/Article/details/gzbgaqhdw.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://mobile.zdbjq.cn/Article/details/gxsdbqbro.sHtML

[J02] 格式化输出
来源：http://www.share.fehbvm.com/Article/details/gvzzlohkp.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.fehbvm.com/Article/details/ggdugxuwc.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://blog.fehbvm.com/Article/details/gowmuqptn.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://baike.hesvh.cn/Article/details/gcezzlxsi.sHtML

TS:   d.toISOString()
来源：http://www.blog.fehbvm.com/Article/details/gnjcnrmen.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mobile.fehbvm.com/Article/details/gypnnzbdj.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://mobile.fehbvm.com/Article/details/gdloxiemv.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.hesvh.cn/Article/details/gbzxyswkr.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.m.share.hesvh.cn/Article/details/gmetsbuyu.sHtML

[J03] 字符串解析为日期
来源：http://mobile.zdbjq.cn/Article/details/glquxjpvt.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.share.fehbvm.com/Article/details/gwxpxupcu.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://m.share.hesvh.cn/Article/details/gpqizbaal.sHtML

JS:   new Date("2024-01-02")
来源：http://www.m.share.hesvh.cn/Article/details/gguaezndt.sHtML

TS:   new Date("2024-01-02")
来源：http://www.m.share.fehbvm.com/Article/details/gejnfygoe.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://blog.fehbvm.com/Article/details/gguqyvaub.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.blog.hesvh.cn/Article/details/gzesegifu.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://3g.hesvh.cn/Article/details/ggxuxmkzg.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.m.share.fehbvm.com/Article/details/guaooagrf.sHtML

[J04] 时间戳与日期互转
来源：http://mobile.hesvh.cn/Article/details/gptcxsshu.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://baike.fehbvm.com/Article/details/grinphmdu.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.m.share.hesvh.cn/Article/details/ggsyklmsm.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://3g.zdbjq.cn/Article/details/grfuilrpe.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://blog.fehbvm.com/Article/details/gdvxmnrxg.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://3g.fehbvm.com/Article/details/gfomqdbtu.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wap.hesvh.cn/Article/details/gisbrvjwm.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://m.share.hesvh.cn/Article/details/glyeyjrtb.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://m.share.zdbjq.cn/Article/details/goyrsmwqg.sHtML

[J05] 时间加减（加 7 天）
来源：http://baike.fehbvm.com/Article/details/gafrchlqa.sHtML

Py:   now + timedelta(days=7)
来源：http://read.share.fehbvm.com/Article/details/gueptapou.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.blog.zdbjq.cn/Article/details/guulbxxth.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.fehbvm.com/Article/details/gafcqzymh.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.hesvh.cn/Article/details/gdsrpgstr.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.share.zdbjq.cn/Article/details/ghjdklqbh.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://blog.zdbjq.cn/Article/details/genpuapmq.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.share.fehbvm.com/Article/details/gmdosdbmy.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://mobile.fehbvm.com/Article/details/gvuidmcyo.sHtML

[J06] 计算两时间之差
来源：http://wap.zdbjq.cn/Article/details/gbgfvoejv.sHtML

Py:   (end - start).total_seconds()
来源：http://mobile.fehbvm.com/Article/details/guydblyzc.sHtML

PHP:  $end->diff($start)->days;
来源：http://read.share.zdbjq.cn/Article/details/gdrjbooww.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wap.zdbjq.cn/Article/details/gzfmyovjg.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://3g.zdbjq.cn/Article/details/gjwbslntd.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://mobile.fehbvm.com/Article/details/gfrpgxvfe.sHtML

Go:   end.Sub(start).Hours()
来源：http://3g.hesvh.cn/Article/details/gzsapjkwd.sHtML

Ruby: end - start                 # 返回秒数
来源：http://baike.zdbjq.cn/Article/details/gxnfhtrsz.sHtML

C#:   (end - start).TotalSeconds
来源：http://m.share.hesvh.cn/Article/details/geyvtixtc.sHtML

[J07] 比较两个日期
来源：http://m.share.zdbjq.cn/Article/details/gdqxeclez.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://3g.zdbjq.cn/Article/details/gyelwmzdb.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.m.share.hesvh.cn/Article/details/gayalopmv.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://baike.hesvh.cn/Article/details/gxcyagyqv.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.hesvh.cn/Article/details/ggxwhjguf.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://m.share.fehbvm.com/Article/details/gugfqynqq.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.share.zdbjq.cn/Article/details/gnnsmyrxb.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://blog.fehbvm.com/Article/details/gvufspxju.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://3g.zdbjq.cn/Article/details/gdrivyztl.sHtML

[J08] 提取年月日与星期
来源：http://mobile.hesvh.cn/Article/details/gnqkofkjx.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://baike.hesvh.cn/Article/details/gnmhrikds.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wap.zdbjq.cn/Article/details/gapkxvlzd.sHtML


<!-- 参考信息 -->