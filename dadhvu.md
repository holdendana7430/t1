代发 wailian999

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2vciwuzgp.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2kcsimint.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2cklkxqqo.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2yhpjwtwr.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2bjvmezfk.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2lfkvefpm.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2aulozvxb.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2aqdnaeuc.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2luxhdchd.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2loyxiusa.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rjkibycp.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ynczmgnk.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2mndacgpf.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2oalwzyjx.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2qouqtsjk.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2xaebjzrm.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2cosabuwz.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2uqxbcfbk.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2ewsycqml.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2thlhvvpg.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2uvhqmqhz.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2chpssfuj.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2lvmfsppf.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2vsriequs.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2duszyklk.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2adpdheer.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2maxlepan.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2uahnybjt.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2tohuuwxi.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fajlfpzy.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2sqvliatf.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2esdnoqeg.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2xzztuarc.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2znkiqzsb.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2atojbefn.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qjaqntqg.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2vlgzknfg.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2ipkujmgf.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2dghzrzcl.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2bxldjkkq.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2lviaovwa.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2lxxgjapr.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2ctbtrszr.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2urjqrtgu.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2rokdszgq.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2ieqhzqbe.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2gqkimkeh.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2tendmfey.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2jzstloyr.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2dflqukso.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2uvwlysgu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nqqlytta.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2djgpdkps.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vqbumlfz.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2mqngylfs.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2ixegtgct.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2ygzznmuc.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2abghliok.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2asuvabkw.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2jfyocvcx.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2hrnvfnka.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2ennfzgum.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2klepnzay.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2ycpccual.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2xlxjirao.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2nsfqethj.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2plwdpcai.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2dhcpkqmb.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2qpmsvnxs.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2ikxcnqns.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2occwpbjb.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2iphyekvt.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2rsslkmuz.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2ahqiwdub.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2fkfjjtxn.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2vdmnloiw.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2qmvviqmi.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2kluismsa.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2lkdjohpd.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2aenfmnck.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2tvnwobpx.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2jifetffs.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2vbtdvfqm.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2hxvjrwxs.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2auhkaajc.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2nuonfcit.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2vdrnbfcj.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2ripjtqwz.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2uedxlcvd.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2qvgfazjl.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2jejfiugk.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2xybchtsc.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2qiucmvgc.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vobxtphi.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2owygyvdw.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2bdrozycb.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2bvbiragg.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2nkdrqwqs.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2sregwoje.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2kmcraack.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2rzfxgocb.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2wrnmvdsl.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2uoztkeeo.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2ykjhrykv.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2vvptoite.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2vzmmseas.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2wnymctxq.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2nlmkgyjx.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2foychgsg.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2owbuyemz.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2qiicdlnw.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2xpnidydq.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2vmeciowy.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2brprccjx.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2tlpdbpac.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2ahxdqdri.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2rwkmurpn.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2noebkagf.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2xmvasvnp.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2ksxfhhjo.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2fxgbkenw.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2bywbhfxb.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2tfpccpsl.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2sgwvyyhm.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2amearknt.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2cdwvwqxd.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2sqtblblq.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2eqrxgfew.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2gesddnyz.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2rntixtbd.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2wifclznw.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2ulddfsaz.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2eimlqvuo.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2xzhwxacp.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2olwmpptx.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2yhnnzpjh.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2nzkqzeuk.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2aquswlmp.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2xrkoznkm.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2irccxxbr.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2mtqrjyrd.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2gzjvvgub.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2fprjvbdq.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2pcevhdjp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dobstiul.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2cqakftqi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fjtwgjye.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2tbytncvh.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2iplsrlhs.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2itexxgic.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rixyqicu.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2rsbntdhe.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2yljglvaj.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jqxiyfio.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2qkvfbgvp.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2zrbnavep.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2wnwaufns.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2qipzsyju.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2macegsmy.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2sneacjfd.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2trlpecny.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2lfpjmotl.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2uepvzlcf.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2fanssnad.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2qemghjer.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2mjbjwccx.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2cbfshmch.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2afedumht.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2juykhquu.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2lmvzpdyk.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2vdlnhygd.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2uxaxfujm.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2daeysmtx.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2fvyjngbb.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2crvycsat.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2gfwsyqsu.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2cczhgxgj.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2fajnnkko.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2venvxnfh.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2svmzpkai.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2mtvnpjgs.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2blxieixo.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2cjktmfpw.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt2kdjzkspg.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt2zrgovuwe.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2kjnnoyma.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2yzktktkf.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2xoskclzj.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2nigrkees.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2vajezofp.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2ziuaooah.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt2drkbvqwr.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt2druxzzqj.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2fvrjohmn.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt2lgnfjqxu.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2dgfodewt.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2yogsxtyd.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2qpqdnvmq.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt2fupxwelb.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt2zjtepquk.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2tdsmfjzz.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt2yojrxvaz.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt2doanprpj.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2abqdckxp.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt2gmktyhzm.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt2lzbalohn.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt2vfohxjso.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt2hfkpolex.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt2niqggbvh.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt2kwcibojt.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt2jtpgfvqe.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt2gksxrtnm.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2iowjrcgs.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2gwqeftor.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2mutqnshy.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2ykrqkdas.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt2ntybrtim.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt2sxeqomlj.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2jqsnyido.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2stxifmwb.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt2fxpwkwkn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lpvbogmf.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt2sjcoytbe.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt2cmuetsor.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2jciwmnet.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2kikedeno.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2eajyerkn.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt2dcxdmghh.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt2qjbeluzb.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt2fffgpbdf.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt2lbpaspmh.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2urvpihfd.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2kwprkjkt.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2qtpqhjnh.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt2atexjbvi.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt2yzxwrudx.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt2awujukpr.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2pqodeowp.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2ssypeuab.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt2vygmhwbn.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt2cqrdbojc.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt2pudetmjm.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt2iuigmsrl.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2ptzjrnfu.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2rkiewdbd.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2chfedwbh.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2cirmbozu.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2qjnugdxd.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt2plggplvb.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt2tovetulr.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt2vnizuzcx.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt2bbkluroe.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2zefrtzah.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt2siebkqga.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2vxocylys.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2vbxlqbcm.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2rktalgla.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt2cncqgnfc.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt2zultptpp.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt2hrybonic.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt2qsjnjakx.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2iswrziwk.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2oyozhskt.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt2yrmbdeyq.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt2ilbmqaju.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt2zrgkkqqn.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt2yjhlzfiz.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt2btkcsrco.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt2iqnavhbd.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt2yodzabee.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt2yxqnngpc.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt2pghsrohd.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt2bqkfgomn.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt2hxgdbugy.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2lauhbjrq.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt2esxryfgt.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2bfvubudq.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2ltopylcl.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt2pwslarfs.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2imuolihs.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2psrrdirc.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2qqcgnevd.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2bnhgjzcj.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2fssiwpqu.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2uewjoxlj.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt2eobvpevt.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt2lblbesys.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt2brdbrhet.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt2hlvasezv.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt2oigzouur.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt2slaycvat.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt2gbfszxvu.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt2accxjgkc.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt2nezczvhy.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt2occmfbwu.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt2raxprseb.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt2iarlykig.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2npmnkudv.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2pvywhzrv.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt2gjptafgg.html


<!-- 参考信息 -->