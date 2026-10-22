代发 wailian999

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2twvfxftx.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2tbugkffz.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2bdnmqxhs.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2ncfdmuje.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2heohikjz.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2qfuughyd.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2cvqxyloh.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2wpgscnbq.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2jxxlabpb.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2blantxak.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2wiviymwj.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2xfvpmqtb.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2hrrbgzwr.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2yeoopuki.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2okmwdxfo.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2nerjvpmd.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2nnbhqtan.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2rmkkvjdo.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2hcfjlusy.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2ununmxst.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2fqqzqseo.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2qwbgftvg.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2nefbhoyc.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2qlrurzcm.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2oylzidpf.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2btntaocs.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2plftyfpn.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2qjbashzb.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2pptirdyb.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2xyiurkmc.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2lujxwbjv.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2sozubxsh.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2jjwxtotq.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2fhxpmclm.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2rpoilruh.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2kkwqkolm.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2rcjnmddi.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2wkafcvhr.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2mlfzefwc.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2futkkxla.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2fxwwhiel.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2drzgfhen.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2kujwpwbp.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2vctzdobr.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2vetnhpwa.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2yabuhxxj.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2xwozzinn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kfwrldng.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2enxvrngj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rzvdzpkz.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2apjudxsc.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2okisbnpv.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2axqbuajh.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2npciudde.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2safjgwba.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2ljsbhqns.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2vlegyrvu.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2kpixfhay.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2fysrnseu.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2rggtczch.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2vctslhou.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2hfihyqsb.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2fbyqvdrq.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2oefyvbgd.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2lyfjvfnm.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2ipautztr.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2mkmejozq.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2tnmmzdzc.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2ucstwyin.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2pmdrgxhj.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2qcyhvqkw.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2vzhlbcac.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2ixvlntin.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2fktzinqq.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2umlxyipr.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2xqssbexq.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2fjtbyzdp.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2rspwvxcu.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2zawedswe.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2nnligbrk.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2expkmsdh.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2urmqwgnf.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2rxhgqnjn.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2vwqpwycc.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2vbziqsad.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2qoonrcvj.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2kaeprstn.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2znxbirqk.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2hueynlms.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2znksacxu.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2ohlzlanw.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kgepjzby.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2dcfigaqf.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2nxiaunog.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hpsftxlw.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2xxigmsha.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2wrqqwlnw.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2dyzmzncr.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2nirxhdpt.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2meimaiye.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2oydthakl.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2zkmsyizi.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2zkzdhncz.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2dsujogmp.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2ffvhgyii.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2jxwxgjlv.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2xzqrhrpx.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2vjewvkfe.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2oniljblf.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2kheupwrv.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2seexitwe.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2okpnsaws.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2avdnbbnq.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2ocyqxwkk.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2jcoyxqjg.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2cwuzbvxx.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2tnjftwvm.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2emplmxdf.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2rusmwotq.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2nxeyhobu.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2ozgkqkcz.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2qethrunv.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2zfhtxnju.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2xvvddnpt.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2awiwvnnn.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2jqqvhrrs.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2moylqwaf.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2mgxniqxb.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2dqpqcyhd.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2gqvhtliv.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2hlbhjccd.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2yefhihuz.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2usfyjpde.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2ghusuunz.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2kbepnqhr.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2euuisfpx.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2zorotneh.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2uwtmhswa.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2ckmyclrp.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ubplmnwm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xgtfairl.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2rlnjwrim.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dchiwxsz.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2fmoxkzfz.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2fexmmrdv.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2prypozeh.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2mojxeoxv.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rnwugctc.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2jrcbjsys.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2gopvvapl.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2nzwntage.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2evimogja.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2tudsnabm.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2hpnsbgxw.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2ztxyemvn.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2wvryrntn.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2kqlfswyj.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2mmcpporc.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2ornhmrwp.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2vhlugtue.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2iqhfszto.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2kphlsfqx.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2ajkbjxsn.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2bunrqrer.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2uepauryp.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2rhglbvld.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2mwdmdgst.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2zejuyyen.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2rlhcbvbz.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2hbiprkah.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2zuiqpgxh.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2chkksuwu.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2uclcljxx.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2npilnlaw.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2wkvrfcxf.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2kvesoohh.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2boxfimjk.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2akikjgxw.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2bwsxozws.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt2qfyjjkrd.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt2tfftfudt.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2serirnib.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2ytvjfofv.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2ihmdshwq.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2zqqofvcp.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2mrqtlqmj.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2crjidyfb.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt2twlmrlmq.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt2mfimqrrl.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2jdoefgsw.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt2pdqdsdkt.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2hhelehlc.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2hlstdnfd.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2wwwsovsc.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt2djmjtwho.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt2mreemhao.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2cndmsysq.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt2nkwetuoo.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt2mmhaonnp.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2zbjdroml.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt2gixlbmdm.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt2nfjjsxba.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt2ahpinfdr.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt2eamxelpm.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt2mmwyqtok.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt2qylrfkno.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt2keymezdb.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt2wpnstipb.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2njladsjj.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2kwziaptu.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2awahckyz.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2iukwugva.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt2gdolcuhx.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt2wzgalduw.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2eeuoeqlp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wzebzpki.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt2iizfittm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2veuexedm.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt2ejyxvlxt.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt2eztphfsg.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2yndlrneb.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2jjgphtvi.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2afkjnyeo.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt2pxbrufhm.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt2sozswquw.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt2dtdkflhs.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt2onjfuwzv.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2uchqrggz.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2ycbmepdb.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2bceuafog.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt2rgereezf.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt2kktnzggt.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt2kezjhrvw.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2zgdguats.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2uuzcmbtw.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt2tavuplyy.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt2nmyrsbno.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt2vdhhvquc.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt2yskwvujp.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2xucsrlsh.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2omkfxfjg.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2fomvbetl.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2kmakjdrs.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2udbqqkcj.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt2tgbjwsex.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt2tzginvly.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt2sanjotzg.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt2xjzhijpx.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2kindeuwg.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2nxyggplf.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2kiqhkvkk.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt2axbdrcho.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt2ylavrfkm.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt2yvigiitd.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt2fqaykhjd.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt2sytyhshg.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt2wdqjbejb.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2pbgxjivf.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2owbjxbvl.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt2sfcjrlwh.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt2cvidupvx.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt2ysmyevkz.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt2ihkklnnj.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2hvjpumnp.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt2hyjcwhaj.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt2bofdwmvi.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt2nlcysguk.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt2igttcxek.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt2mrxcdgwd.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt2tqontvpj.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt2tqvxqehr.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt2avjaysni.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt2rfywzchk.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2xmyyjgmd.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt2mrwuygbs.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2mgdogxxj.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2qcrqmmfk.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt2whknwkaf.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt2zzppcydw.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2vgmueojm.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2mawzulnh.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt2tmxspder.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt2ilhccpto.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt2atjouryg.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt2rxochxpy.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt2gwwbauzx.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt2tiawvabz.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt2qktspziw.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt2wutcpvdd.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt2oafvpuvz.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt2vidfirtp.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt2vxmxujaf.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt2nqfygkfr.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2dttfnlzh.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2mcnxekew.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt2ieyelwub.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2ncdsbqxv.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2vniwjmdd.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt2eewvqhwg.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt2ahbkkkov.html


<!-- 参考信息 -->