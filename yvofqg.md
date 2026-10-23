代发 wailian999

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3istqvxva.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3xvpqnwgj.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3ungkyqtu.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3lwxcersr.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3geedsiku.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3ytavojxr.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3nzktfojq.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3jhoddxvu.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3wddbxehw.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3klwuzcgv.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3ocsskolo.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lfcabktf.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3sdqzzycf.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bevrjzzq.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rsryxgwy.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3gfxpdrmu.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3gmysznri.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3ihobopnf.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3kyyomipt.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3ugaqqozn.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3yvnrdlqg.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wspupkmn.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hgjybssj.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zpeubwdk.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3abfxgsqm.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3hhexwieh.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3hwuljjms.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3cibiudnv.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3elexdwal.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3jzfdkazk.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3kgyosyrq.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3jvtsdqna.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3iikflyib.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3xyykjumv.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3lknexhqp.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3yzrvlhao.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3mbyvqrlv.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3enzjzayj.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3bvptcimz.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3zshizapg.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3tvaazkgq.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3aqcluysn.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3fvasagog.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3nirmuspv.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3xxsswcmp.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3kdnttuam.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3cqikbqnh.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3kzjxqgnt.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3aefulzqb.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3oytolhsu.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3ukikgbzc.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3aokqeyul.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3nxdagyvt.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3mkkssmrm.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3fnghboey.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3umsldwbx.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3lmkqshfd.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3gygukify.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3apdpeior.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3xxrpfjoi.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3rbqpkczw.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3hdgdabne.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3udyjhljk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rlhuoobm.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3vsyvkaqo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wqkwlauu.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3zjrklqyn.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3wmzoyrwy.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3jwkfjjnq.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3ujgulvuk.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3yvbaidnx.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3igmtseue.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3ytfdabsk.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3kctpmmcj.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3letsszkn.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3qhwqongz.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3atopsprt.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3uxtlkjjf.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3lfxilrsu.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3tfxqhcox.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3uqupiwup.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3rzwnquxm.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3sumyaxpd.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3taxeicqe.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3mxzsdvra.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3nggndfpn.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3udzsnnxu.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3fkhbsbmr.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3beemvenz.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3ffonbxic.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3gmirjdri.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3xtjmbfww.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3ktokgsju.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3akompxcj.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3uldoyyyq.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3dxbjemnt.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3jbsancoq.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3mdizimgx.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3msbamtrl.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3bmemjwts.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3euqrsfpf.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3dzpplcrb.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3qfwevibj.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3mcxcpbot.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3szsdyjli.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ofcmzofw.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gltfntya.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vbbyqvnp.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3xcbkiwru.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3dxqtilpt.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3anuslrso.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3spfdyttq.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3lysbsunw.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3qjqgzsyx.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3ltwiwxze.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3yzvgyqug.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3rgvashfg.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3qdehmuau.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3dbvmnbyk.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3rfwrocml.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3hxpibyug.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3bemrkrry.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3nezwbgni.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3wbjeuiub.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3vtgzspkn.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3dcajofgf.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3nscdrbsh.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3ewktenbd.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ulbgqrky.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3kurktocb.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3doatayzl.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3excglhgu.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3wgkmbejv.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3hbxgezfd.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3mknsiecy.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3fcveenqi.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3lppqzymv.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3szcdwuuf.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3wfcocgcb.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3emcahfhj.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3rjbaivdd.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3kxjxbimu.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3ggdukyqf.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3wxazmpnv.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3xlppmdpb.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3uguidsye.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3rzmlhyof.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3dmuvkxva.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3uzkgmbwz.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3eorvujxp.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3lpybljyz.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3zsfidlji.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3anlgtqol.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3oezvmfht.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3goqdyjwq.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3qpfzmxrh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3znhaswcb.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3aosesort.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rcegjgfg.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3wwsxqyby.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3pnzmvzzu.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3dtsedlwt.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3mkwuvbnt.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3pxnkhwki.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3yravczna.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3pvpxbdab.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3qduxawjn.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3mkkhmpme.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3rbzmhnkd.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3yvejtyps.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt3vbrsdrut.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3hbpkjhmf.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3tumxmykd.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3mkpdtgyl.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3evftqtqv.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3vidnalwn.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3ffxqqpic.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt3vdkbfulb.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt3pkibtgio.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3nqzvpvny.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt3yzyrokza.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt3beuqhhgh.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3gtfmkclk.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt3jjhlvqoc.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt3lqukmeaa.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt3pdcxbbuu.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3pagkvgyo.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3axftdyvc.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3mnsajhys.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3kmbhhllm.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3xwrrfzow.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3iraenren.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt3cssgvznb.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt3aabjsnul.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3inkgaugj.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt3cbgkgjsm.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt3lwchbtve.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ecdtrarv.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3wrvuapac.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3wibktbmm.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt3vvymijvf.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3bfnshkhl.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3fbgkrtmg.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt3ksetaguz.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt3osormrgn.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3jhjsisuw.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt3rilaxuig.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3imceuzyz.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3poizsesc.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3vcldwmer.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt3kgjcrits.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt3hfwiigrb.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3omldvtte.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt3rfhdwcuz.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt3mlvnffbv.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3bcplppnt.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt3dydaztbi.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt3ogsbqktp.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt3ajqyedvj.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt3cctnkgtu.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt3xbttvrwr.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt3fizkkaft.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt3rtnzczej.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt3xvwyruna.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3feduknhm.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3equwhadg.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3msgxxjqw.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3klzzfcii.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt3hiyhjaax.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt3bwcwkrto.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3biwseyyk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fkpizprw.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt3eiiadbii.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3psfrfefr.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt3grptmynq.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt3mcyabtvt.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3yesqykqy.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3yuraxitm.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3wpxvmqca.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt3hccxzomc.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt3rpckgosa.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt3umygfbwl.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt3avapawzi.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt3nxsdipdu.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3cfpfsdct.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3cgqfrjnu.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt3dbnhmdwu.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt3zbxbsgud.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt3qafvmebw.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt3jeenukui.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3dtkwwelj.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt3jeluwkqw.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt3ioiyxeex.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt3etdfxbpk.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt3stjxyytg.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3hrcxdsqc.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3xetxcdvo.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3raldvdoz.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3lvxsthej.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3qmhwdtzy.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt3eeahnjha.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt3vwinnwsm.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3jjapvsky.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt3cvxepgnz.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3iazxibvo.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3zahtnvno.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3hrnqlmms.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt3opqxqvko.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt3eizhiohz.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt3rvuzyffi.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt3fmmsbtiv.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt3wywjktaq.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt3dtzhjzmb.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3drjowied.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3hbnautws.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3zlsflnpl.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt3unwrakgk.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt3nycfhalk.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt3gfbwsrin.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt3wohnipul.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt3eiokxcyz.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt3etkwswgy.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt3jnnvstpk.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt3nxyjpgym.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt3ccbqgjok.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt3xixajlth.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt3ysymbaxg.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt3pmartqqg.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt3ynhfgjsy.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3mhcpfejd.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt3tdjprdte.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3ujawtavh.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3kbodjwgc.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt3cwmnriyj.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt3sfvjsixg.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3irorzksb.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3dojtljwi.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt3yqmqmpua.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt3kucpugyo.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt3xgyybxsm.html


<!-- 参考信息 -->