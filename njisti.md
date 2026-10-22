代发 wailian999

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2mbybnbcn.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2ekoboknm.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2tvyrbrmd.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qdzehmrs.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2jfzwuqnl.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2mfhvlztq.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hryvrvnq.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2tpchpuur.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2xdyyxjpp.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2reihayqt.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2oidkgefp.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2iauuxmfg.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hafrzmto.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2khuvosde.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2zkybizsz.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2prkhvlvl.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2dxdtfabg.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2kdofpqvp.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2xorahdlg.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2destgogz.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2nhyblqci.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2mtuvydwt.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2caubrpgb.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2xvnblzlx.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2ywnyxegz.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2njypqfre.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2nffkixlf.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2wcwsdewl.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2uwcfzvqy.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2xorbauxn.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2coujwzxf.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2bhpbtjho.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2lbhpwyav.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dxdcqcfh.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2gwoylrgc.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2myyivrmz.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2ixyarrtj.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2ttwppyhb.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2qyqnxxgt.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2uspmbmsf.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2ykfxbeuz.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2gcsywyst.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2lozgokyq.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2arxrblyz.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2brqybsqb.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2iheurrit.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2xacbesba.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2gqcyjcur.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2pycktciv.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2vbwxeuep.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2yymrotwd.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2lebtmhfx.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2pspkliia.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2hkoqafov.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2dhtmppem.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2aaaefrpx.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2cqubvoyd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gynhhjqs.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2rdsbgezf.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2xmtcojqx.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2avbudygc.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2esnqaznr.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2byaxdjgl.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2sncbqkpd.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2xqucshnl.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2epxfbvcv.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2dtdevqaw.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2zzqdbjif.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2bfigurqk.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2hzufkfma.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ubhnowgs.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2gmmynpcn.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2tosujlfm.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2vduwlgca.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2wtrirrdx.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2rfyybxqd.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2xcvzdqht.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2mxleaazx.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2iyuhqndw.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2maaanupi.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2bchbigvf.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2jyfzrmbo.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2vrmnjalj.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2ruxfuqyq.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2ndvtwhht.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2pbdljvlv.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2gxnlkgoh.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2ewsqvjjn.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2ozpuocds.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2qbyskctb.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2chngnkbb.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2bgrpnhqb.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2sfkqnniw.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2wqlfmlsf.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2vevkyysq.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2coptuawq.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2akhbsave.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2wnpfejvu.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bjfhvvet.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2qrnxwgmk.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2ygvuofew.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2cbdxjtgz.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2whnabijm.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2pjtokcwb.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2ysefuyyb.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2uklrukuq.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2upkqiwlh.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2rbvkxgfb.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2ukzezeke.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2rgruxoyi.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2fkiejina.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2lunpcvup.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2ozuxnoht.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2vvsvwruy.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2epbrxpfx.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2jewlmjom.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2lgmikbtf.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2aibafbwy.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2zyyuewmw.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2foydlpxa.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2ztwboicg.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2msizyjcc.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2wdldpxno.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2wqlhetpr.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2kzzeeito.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2umqqknum.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2ztlhsdwi.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2zipiblyt.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2lpmluzpc.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2lpqihxcc.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2hmtdilgz.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2ostzofiw.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2bqbotdhu.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2japmlndv.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2wesitdcq.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2krjzcgwn.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2rdddgnjm.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2jclbtizb.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2vudithrc.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2vubrskmq.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2pkibazwm.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2wgidjtsh.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2fahvfolm.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2eahjfosh.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2bplrqmuu.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2wqvyfaqd.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2oqunxyyx.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ommxikjc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2euikymlv.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2ytvbmwap.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fkwfwyrf.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ynjipjgp.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2qeulhbte.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2twlfvzcz.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2fdbzdyop.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dgiciagn.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2srkphqne.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2fdzwmuqv.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2dhwbhjia.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2rvekvhky.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2hnymznqm.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2rmtabaqk.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2hwjutbom.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2lswjunkx.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2tdqezfrk.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2cdekoqyx.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2cyxkjndo.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2qbbirvnu.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2naqrfjbm.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2dnfgvwtq.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2sbxbgmci.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2hxwhuhci.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2mxmceqsh.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2wicioirs.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2ccawecwn.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2fzmacrch.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2yuhqhkno.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2cnibzdkp.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2apjtfvgc.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2lwcaawsm.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2iakunuog.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2bxevlazf.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2recpemtv.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2rtmiknkk.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2jaziodag.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2tzkvbeky.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2hzsityrg.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt2xunqdhne.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt2ypjnvwbx.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt2qyiyeuwe.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2ltbjfsyk.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2tzuoncmt.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2aeroebbi.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2shoijfks.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2bpikkzvu.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt2iimnfzmg.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt2ykomyova.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2gwdexpks.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt2exfhgmbl.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2eqezmcld.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2wlrhprep.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2hfeaqzhz.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt2ugrlicjx.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt2bmdsxrvq.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2qduettqp.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt2fpztrmva.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt2dopzwfai.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2exwiwfax.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt2wvppyldi.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt2cuxjapmt.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt2fpbhyrah.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt2obwoadta.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt2qzcgwsma.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt2moiieeao.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt2meeboriy.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt2vxhuylxg.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2uhofryav.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2fujrkads.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2rdpopmxb.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2hsaezujj.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt2awtyfwgn.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt2ixraylio.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2osvylfzh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2swjfgxni.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt2uvvbspij.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2djwzxoxp.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2jucfzbwg.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt2qabzzmwb.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2zjlubvvf.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2cvywahwc.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2jargudci.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt2kpnykekz.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt2ixrxqowv.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt2kecwxxlz.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt2fhswvglf.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt2bowtvnna.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2dwnmdifg.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2lyhltbvd.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt2kmqboilv.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt2mcrvccdc.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt2equdcvoq.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2zbtuqyno.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2fjdzjnua.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt2ibcqfsfp.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt2mhelkgyy.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt2wwjqfkuc.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt2eohmowgq.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2dorlrtnf.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2aueonirs.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2mcgfdnru.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2nlqrciun.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2yvaldefr.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt2jutmykzh.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt2glwoawas.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2ykfmebnv.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt2uxdclpko.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2ookbvvif.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt2ktmucxdy.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2nthdcpkf.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ocltrfwz.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2clqeehpe.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt2efkyxwbw.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt2rcevrraa.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt2lnvvbtxi.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt2uadqvevh.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2cjplkcje.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2kuzoonkf.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt2ulqnrukt.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt2trxxhpox.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt2xyfsboaj.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2qihyluwy.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2uwhfpddv.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt2wkscgvio.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt2vrawpert.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt2bmyrorrh.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt2axrwhgsg.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt2axqhfvxu.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt2vpsgqtlk.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2ryjnxfbm.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt2ljxxaxbq.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt2szklfuca.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2ejzihvwf.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt2wlhcbjug.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2vwynhuvm.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2oddzrehq.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2eqlxwhsc.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2sjoehjwb.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2vbmwzqoi.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2ydkbyunc.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt2ljjsfsie.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt2hvhehvfw.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt2jhwycvwh.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt2cknsifbe.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt2saffghha.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt2czpacesn.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt2veisdhqj.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt2vcqoyhvv.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt2klbufpva.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt2pfbpftys.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2debahbxv.html


<!-- 参考信息 -->