代发 wailian999

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2dyheblzn.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2qdlgusdz.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2atytyhxn.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2illgjaxs.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2cvgzwrfm.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2spworloh.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rgrtbgzq.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2hpzbtnzj.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2efjotthj.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2ioafezby.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2uvsbpawt.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2prspoxkd.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jwtdurrr.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mmermuvi.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2oqsppdbs.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2afnzslht.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2eyenkhnt.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2yroimzas.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2hjozipvy.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2xcsonoin.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2hwjhgrec.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2szansmfc.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2hpcghdtf.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2robrumot.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2wstrlvau.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2yizencnk.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2rrpudvht.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2owqqpqwj.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2dzlwiedq.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2onbdyhyu.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2oomfwzgn.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2qfmhncgj.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2majyuowx.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2zjzsewox.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2iecxikoq.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2kmqvpskx.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2aejezfgy.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2givmokoq.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2klilkxxs.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2iweucowh.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2qikbrkah.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2ctipvsvl.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2sizodqdu.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2ftkxnjqi.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2ouuuovka.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2rmwvehkc.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2caolwuod.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2ribtbnav.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2pddwtedz.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2wklattfe.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2dhthdkrh.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2sudwtymu.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2twgdlyqy.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2tcvthvlo.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2ocavioyf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yykaymec.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2dxtzwsik.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nzhezuic.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2xfjivsvl.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2saxyehou.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2fknkeqwm.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2azpsmppw.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2crmftexj.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2gdnrsnfy.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2zzkzarun.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2cwefslan.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2wtdrhhdg.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2mdpnovwi.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2nphdujqn.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2ocbvmhdq.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2vbkdxgad.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2tcrdocoj.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2rpshefgz.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2ykqggcoj.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2tctoiinf.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2oqiflnau.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2yyfgmuqp.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2cypmclfu.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2yhdqnyox.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2klzsmexy.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2jvauouxi.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2nsdcgheu.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2axsiuwex.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2uhkbicyl.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2kwpdlxfg.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2hewojthi.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2jupqyxls.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2yxjyllal.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2chzhcqaj.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2jkbixlen.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2ptbmmwlr.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2qegdfhtg.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2vsrditqd.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2pwqaefiw.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2zcqwdjyy.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2phqrizeh.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2fiqemliz.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2toyymyao.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2uvlxfgeb.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2gzjtrtxd.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2fntbdwwc.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2iczcnpig.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2vftthlcs.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2wzgfgesa.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2whuedcau.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2zgvebprx.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2qlgdalee.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2gweitybk.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2fqjdxonq.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2hovmklmo.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2yhtmgtkw.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2yxmjhcph.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2cdgqmnpa.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2fwhmlazp.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2plvcqvqu.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2hcfenill.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2jmdqltwu.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2dbvzxarf.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2xgmvzkkf.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2xoomoqig.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2xzhmszro.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2lvyxbtwn.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2lkunthqn.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2khnwmeam.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2bgbpijpy.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2luofotkh.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2jubgrvnt.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2vbwiyuut.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2mqtzzhad.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2wmaojpxi.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2nlutuwdr.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2bgjzelhr.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2oinafsfc.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2rnvzdjcw.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2mdavrbxo.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2ayyhumwp.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2hhfacagg.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2jqssumgo.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2ctebmtof.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2acvtqodb.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2rutgrpzf.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2zumfmyyd.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2jaepuduk.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2sckdmobw.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2ksxbeblf.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2ebycufnv.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2qonmfjrq.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2sflzxybz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fqiizthe.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2cgilonxp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2czmlqgsc.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2lfkeoqlq.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2tdimaglo.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2mzzmmdql.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2mqzkzxjo.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2lucfobpr.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2jwrlfdty.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2lxwifbkk.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2jzywggox.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2ncmxfwof.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2fxbrkwju.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2bpdoaezf.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2xubsfdss.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2qceefwfa.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2miezuioq.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2pwdfzoou.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2nflhyetx.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2zouqawjg.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2jtdzgbpu.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2qsrlaxtp.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xytndnuj.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2jgxilwez.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2zkadeybp.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2huedbltx.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2zaaufplq.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2slgkhhps.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2lsvnmkeg.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2geapzido.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2napatnvf.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2annictid.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2mepctysr.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2bbgsefln.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2uqvyxfos.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2pducxglk.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2plnuamkf.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2rjxpyctb.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2hvjhnqqw.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt2bhyestjh.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt2uysqanvy.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt2ulgqmvqt.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2foysmktb.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2hguoxxgl.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2flcwogbx.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2rkyszmzg.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2idkvngsv.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2itbswcef.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt2dixpxful.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2nzxfqcus.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt2cacmemnm.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2mvmokrkg.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2fjrddcgm.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2djsurkve.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt2bgbgubyw.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt2lzbrokzj.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2dxahlzus.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt2uzuhbrhq.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt2dhppqwxq.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2kpecsjxm.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt2gberljml.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt2lgwqfntd.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt2jpmngnce.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt2sewizcgp.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt2sizoimck.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt2mxztndia.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt2wxkcforg.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt2ykuvabab.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2rvezybnm.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2klfaraus.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2knjbvonn.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2kmjowkeo.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt2icxljuoj.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt2ojtgxsho.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2efzsflpe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jfmyrybh.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt2bhlrzxui.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ujiwiskr.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt2cshfaljp.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt2pxeqlnyf.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2nihjhnme.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2qvnwblld.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2zenovrdb.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt2ilfpanve.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt2nacgdqrm.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt2hdgpugnt.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt2hjzzhlsv.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt2dzinyrpe.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2xvysiier.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2gzsncjsz.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt2caiiupuh.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt2pskltelv.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt2yqsfuniq.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2clxfjgck.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2invnpcud.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt2kqzkwuoh.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt2yasztaqd.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt2mrlzwmei.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt2nacdaxjr.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2bbjnhxhk.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2kkggepyz.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2lygrczez.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2oodvuldl.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2apqukpvh.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt2lucwihbn.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt2kwavzojf.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt2utxtnjao.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt2urvuerrl.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt2pfjfrjdy.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2jziukalo.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt2ioiohqib.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2arzwttgq.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt2xfbgwyml.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2vzseoehf.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt2vfyklsow.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt2gypazcbh.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt2nxkxtwyw.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2vklguynn.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2pohekbzh.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2ggscpyqa.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt2mkzutegg.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt2tccyvfgs.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2ymnvslee.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2qaonsdzv.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt2dbrkmlai.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt2nctdsgsr.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt2tlbegacv.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt2fvipuwfi.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt2xqdmmrjp.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt2ufrvfltn.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2rzihplyi.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt2ndnackej.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt2ldxogwgm.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2qttiqinu.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt2qbmfiiyg.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2zqitafuq.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2jqludzyu.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt2obvtzgfa.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt2hkxrbjae.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2zbhjjwzx.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2ckmdmjrv.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt2lrtvotih.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt2shnolqux.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt2lqzpbwfa.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt2ohcykjqp.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt2gbywwvwn.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt2hmwvsfsq.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt2ffswjchg.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt2zcgqbcek.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt2gpnkmzsz.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt2ppkcdgef.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2hqgshejm.html


<!-- 参考信息 -->