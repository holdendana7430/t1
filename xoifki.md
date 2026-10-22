代发 wailian999

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2nwiszydb.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2lrnswflr.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ynuhaswt.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2cflkjxso.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ljxxrkng.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2bhkwqdcy.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2falnqncw.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2xxekwbwt.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2xsbhmhvt.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2qefffuwv.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2sqpfofob.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2twkfoyiy.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2jjykvwnu.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2prbpoxgq.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2wjjaqlpw.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2eyvausdj.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2pusflstx.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2bdltwbzg.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2pdbirsby.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2ngkkajhj.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2febsggwk.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2gpqypykz.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2vzttjxei.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2xdtjuqwf.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2vveeixye.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tkzggzcy.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2trcourqb.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2fqgqezvm.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2rextcxxu.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2cnhgjixi.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2kqdkxubd.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zkcdgrkc.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2swsrcfhg.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2drpffnuw.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2wktxvizm.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2kevieunw.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2pihvfing.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2yxmsmqeg.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2ybzjdhsw.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2teoozbrr.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2quznqkam.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2rzoocagr.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2xioqklhy.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2udanacyb.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2uwzseosf.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2dspnypkg.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2hmydyqmm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ppgsoqvq.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2fvrjvvdz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xqhhfxwj.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2zlhrheda.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2zrvfsfqb.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2hetpunqq.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2vgorgfda.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2sfodtplh.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2uhypmeyn.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2ldixeavz.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2ixgupivn.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2qpsbvgpi.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2cqhzddep.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2ovpchmby.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2ychjfszr.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2smixrlsu.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2fffxbgmb.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2bdxjcxob.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2yabcfacw.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2exrxkfaz.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2waobbnng.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2eeswkhqe.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2gmkgufqw.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2ujjwgwln.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2wovoxslg.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2pcbfmokb.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2ssxfpebh.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2ussypncq.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2ifdwdvlb.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2extxnsqp.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2mdvpparb.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2ccppvcoy.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2dlduiila.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2nexonaer.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2viunekth.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2ebtuluvz.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2lpcillan.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2cjwopypv.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2thgjtxwu.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2qadmfrmd.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2ghuaybld.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2mtbcklam.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2phfivfdv.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2eydkvwgj.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ranxdnwi.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2nfsjkirr.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2tcdetjzy.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hhostxhk.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2oggzfjwz.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2rbihdizn.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2ycligavc.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2glzsoplb.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2znammpcj.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2apwpcsnw.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2eydyfcoa.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2jwwnfrrm.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2zjymipns.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2holqnhst.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2lnhmztxx.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2urbadlkq.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2vavlabkn.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ealwpsqd.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2hlqefkpg.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2eecxkkgr.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2xrbtzryd.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2xkcrfokn.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2yyckyklx.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2gmxugfyx.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2nkyuzpmy.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2hbtjmrmz.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2hhoohpnl.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2tsntuxwa.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2iufvvnmx.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2jkxglcbw.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2elthckhh.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2kiajbfto.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2qfjcmyxn.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2urnozpms.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2lmjsenza.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2ikbdraff.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2engdgmpk.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2hgkyeuat.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2xvknfyox.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2uwuqvmxe.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2odafwhoj.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2ghtzwmgu.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2vzatltoe.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2gkufdmfo.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2qrhcmokq.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2ykgyukhi.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2iregtazz.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2javcekuh.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2jrpvuqow.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fzkbtlmi.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2frdterbx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ebgbjblp.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2rsfcyutf.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2yeifqgky.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2lqimuorb.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rsznakwd.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2owxxgvve.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2qeyfvdum.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2towxziyd.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2lxphjscz.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2htjtmcju.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2jvzusvcx.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2isniqlva.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2whmchpwc.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2lzyzwdbi.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2xcexqklv.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2suctmtfm.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2zevxszhw.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2omzditug.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2tupbbxjg.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2frdnfhdy.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2ylwnegsk.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2qgpxlsby.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2wbfegoam.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2loqnbcsm.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2zvpnpjkj.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2ofwdzhdg.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2xujidaku.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2oemqiebz.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2tfsdwlym.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2rlhzuoku.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2jmtyudep.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2ypuwmdrc.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2tegkycyl.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2bercmthg.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2hdjpocjn.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2xbhietaf.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2bxsylzep.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt2ibgkhvqg.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt2dgedevnk.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt2mswufzed.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2serpvxib.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2ozficvbn.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2dfratjdt.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2zrjufsdy.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2bpmjkybd.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2rbbytzhw.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt2plccztsz.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2wugcofgt.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt2ynrebbuf.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2upknndpm.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2zvcivtts.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2mjvdmlmq.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt2mvdczier.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt2efouqzgx.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2xyndpklq.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt2jrlimnjb.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt2zgtvzuap.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2jpestfjg.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt2leqcxfnd.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt2nasvlkyq.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt2jnktcrgn.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt2fmgzwktb.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt2luhdsatj.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt2msvhvpkt.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt2cvmorppm.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt2fwgavczs.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2ffvysaho.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2qtbhbxqq.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2edeevrkv.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2luboecsb.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt2germhuff.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt2heqsvyon.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2svosvefh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ezxavjeb.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt2hgjuzheq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zdxadomy.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt2dxtecuxw.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt2rtovglsk.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2lbsiaacx.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2tfrqcdka.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2tboqimdr.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt2kdvuqsdz.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt2bjqydypg.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt2ebcwefaf.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt2dhatpilb.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt2rcvsktrc.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2ntmlivzn.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2nfyaidyo.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt2bizyfupb.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt2ijtpradj.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt2fgmlcxdf.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt2udkkrvqu.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2rdrszeio.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt2vhocywxa.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt2fhmsdrxd.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt2usrsordt.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt2twonrtgl.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2kalnwxxl.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2cuqdhfci.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2tvhcjsvc.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2gdnaalxg.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2yyhtbseh.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt2iocaruxz.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt2rnyoxcha.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt2xfsqjits.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt2yrzwqhjk.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2lfgjheom.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt2uimsrhps.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2fvbutgkm.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2worvphit.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2axlbzyim.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt2hibmqigq.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt2bcckthla.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt2aeqpmqcx.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt2ykqoxwti.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2qnqyltig.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2kytmjges.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt2opngkcrz.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt2yrgjkxui.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt2yynbbcbb.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2rnuzybfi.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2scdxfinr.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt2iliamaqg.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt2sbfmnbgb.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt2ajlttixx.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt2bqkyltbl.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt2wyqbrwny.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt2bxnjiumq.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2mtmskvzh.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt2kgyotaux.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2txxidnmz.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2ndsyyyff.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt2puqvwarb.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2aqzxntkp.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2kradsjbe.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt2qdoldjao.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt2nwipswsj.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2tvurovou.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2ohgmyptk.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt2igyauyva.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt2fgkvrzfe.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt2gkbesifv.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt2labqyrmb.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt2eafgthnv.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt2zuquanty.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt2ywkmgwfy.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt2jzqukzzz.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt2axetlfpj.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt2uffqwdwh.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt2mmvkxhqh.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt2fxiqufpa.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2arqsjhey.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2zosqlbvy.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2pxtsetwe.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt2iebxcwzs.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2taxcjpcf.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt2cttjrcdl.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt2zirwyrbd.html


<!-- 参考信息 -->