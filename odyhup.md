代发 wailian999

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2avwerpxj.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2kjqykuub.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2qlqqdeha.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2lmebtqxd.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2lgeoxiqi.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2dzzswybr.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2ndprmuxp.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2yzlngvjq.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2hlxdgufh.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2rtlwasju.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2zbffbirj.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2hxjhxneu.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2cmjdcnvd.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2ilzmwyfv.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bojkpgzw.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2vrucmmof.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2rkxlnsfr.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2yarvpoku.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2xhesfxzp.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2arrjafgw.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rhyjpujp.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2rlghtvzm.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2crqmzmtb.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ztuxppbs.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2wgojktte.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2spgzsmkl.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2olqjsrej.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2cjeydbfm.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2vyefepsq.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2qwfbrahm.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2ovlonvcr.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2zqambizx.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2rfesdmmb.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2orquhaly.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2isaunjkd.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2tfdzyerx.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2tcehiewo.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2hjmjeudh.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2ydqofcta.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2clkzqpth.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2llcdofeq.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2pjpuxjpp.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2ulzwkext.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2omfunqux.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2syocysjf.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2akdolska.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2kkdmibpi.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dxicquos.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2yjgtyrty.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2ilscwxnp.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2tdhwxjae.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2htotbajq.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2ijuqcpql.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2iqbmixyt.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2kvbkmwlr.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2lfxojili.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2twdohcba.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2dlbsdjdv.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2etjyzjsc.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2wesdxrjv.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2jezdifjc.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2viupeegs.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2fqgxltka.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wqxyrdyh.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2hhyqsoxm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bqevofsd.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2tivhppjv.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2qvufeact.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2rfqtoufw.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2wuqrfaeg.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2sqazgkff.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2ingummjo.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2rattlvni.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2rjkfgbcg.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2jyfhcyvi.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2ljtcjshn.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2lnhifdcl.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2uttmrvli.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2pxfpvjlr.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2admxndoe.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2rnrbigwf.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2lyxlvrae.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2lzvtketi.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2zeoyfhvp.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2iipiqqno.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2wxcxctsg.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2svyipmpx.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2jegmgcls.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2clylxirr.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2tuceirpg.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2ohiszjkt.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2shfpjjab.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2aptzisgk.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2sgntcswc.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2htrtdxvb.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2psdddjcd.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2usriifge.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2etwtqshz.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2urtijxra.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2lcohzzhb.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2ychdkrjm.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2omqrseoy.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2iprdjwfw.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2djwimpce.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2sguuftow.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2cgipljld.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2mhejwgxs.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bztmmjob.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2kbkjhcne.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2tkljzewy.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2txgidpyx.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2wywdnsce.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2tesiexkf.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2ludnxhwb.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2rxefrewo.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2tiqmiqpq.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2pgfbuwsj.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2rtlmxlfv.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2beckgmfq.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2rgjtcurl.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2pdvprhnd.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2zivnqara.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2geuzcdis.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2jikjfgkr.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2cnyfllgq.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2ezxznger.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2utcwprjh.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2aunljfti.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2prvzlqdl.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2vzssjddg.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2jzykfyik.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2fvimgzlf.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2ftcqtbly.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2oydbdzvp.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2tfuemrho.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2axsudhno.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2fawfehxk.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2xpsukvtq.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2lnncknog.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2hycxseug.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2wxbznkkc.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2bnxtfoto.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2yjvxqnti.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2tcfhvnkw.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2xbamuujy.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2rbcjmvmq.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2brvxbknc.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2anenowdm.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2btqpnhhb.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2izmdvptm.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2jjjbvceb.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2umhdfgjq.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2wwyrrqml.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2ahzcodlr.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2qrsletsh.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2dhhktlix.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rfookvqs.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2lggotlat.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sgkfpacu.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2btrujynk.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2ssrmeswp.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2rrzabahm.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2clfgievu.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zotfqdri.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2grohukav.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2ptubrfxi.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2ryycgycs.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2lfqraawv.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2bzybqusp.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2lhlhoarf.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2ehwflcwg.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2tqnbrmsz.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2heotzyug.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2zpklshxu.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2esslvzdd.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2eodqqdbj.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2rpiwlanj.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2dxkmerzf.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2zpdkoohn.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2qrycpjfq.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2yhwqstdj.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2hhjfgpzr.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2tzxvmtae.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2eudomfrs.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2yspxqkai.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2ttyigoai.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2gevpzoox.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2autdncgv.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2kvxgzcua.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2jlgwzxnt.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2berihbsl.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2cnmzslbm.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2swvwsqur.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2jjqzxkmq.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2zrxxiaov.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt2phmgyttr.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt2qbdblqbz.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ismcmwrd.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2dxvgocra.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2fhwcjowb.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2ribefrua.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2hewwwmwq.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2zsfuavsy.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2djzifprv.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt2uqxsmudp.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2dsjlyerh.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt2quindyyb.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2ophlmoxy.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2airsdkzm.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2babirltf.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt2exuldckl.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt2ossmfqgx.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2iyucipqp.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt2attmaiqb.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt2vmgujubw.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2hbatagoc.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt2beqdgvtk.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt2boeqmxzq.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt2dbyeubjx.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt2dildwbqb.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt2oehktpul.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt2uslshfhw.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ucxljyud.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt2uowigquu.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2wbbqmknj.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2iwwyqoha.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2efrrqepq.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2fkvvdmkm.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt2iuzsrmkb.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt2tsdjunfx.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2ostrgjmo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2aatimcwt.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt2ceutbdcx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2crddayyz.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt2utnlhtpo.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt2fpvkwvpa.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2qskyarfa.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2nshngdbd.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2yqzbnbne.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt2vsvmrtki.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt2sqvvcjhf.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt2yqzxflfw.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt2kkiowguk.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2plkyetdp.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2gtkzzhpg.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2hybqipbr.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt2bzmglmqn.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt2lwoczgrl.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt2rzcrwrot.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2oaohbowt.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2dcaxxorw.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt2njvamqmm.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt2shvvkezz.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt2nofbvcvz.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt2uduovqrv.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2grjvohgm.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2istzbeju.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2hfeksyhe.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2mdmohxqs.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2clthgyig.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt2zcwtdfof.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt2gdiiglfc.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt2qwewlzec.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt2ysxadfgm.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2eoykzdmj.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2fktzjuso.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt2dstbaixf.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2aktrugpw.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2sairjwpl.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt2rqsokdwz.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt2uhnpsapa.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt2adhnrewn.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt2sahdhqjp.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2cuaoytsg.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2uctgyxrt.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt2uhfbvpvi.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt2cboneink.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt2krwzypqs.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2hmfepuxa.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt2znlpmrvn.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt2xswqyeyz.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt2lcaqiyea.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt2oehrmqzb.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt2sudklxhj.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt2jcfbthom.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt2dmtbfubq.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2kvcetabv.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt2bvcjhyft.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt2iclkmdsc.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2zbksehoc.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt2jgtewzkx.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2xriwduxi.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2jadejbub.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2tjhuutit.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2dmklxoxo.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2nvzupiza.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2gmwhpvwj.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt2zgyuykix.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt2drwvlhqs.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt2aixanqpn.html


<!-- 参考信息 -->