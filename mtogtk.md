代发 wailian999

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2sopeosah.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2uodiyzli.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2pkyqteil.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2ycrbpjcb.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2jnxpmjoq.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2feaafujg.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2wfblenoe.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2niffiqpx.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lbjxqsta.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rppzikos.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fcvfwmkr.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kzpdmtuv.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2kuarxhxn.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2jxwdjdhl.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2kjdvcnfv.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2penucrto.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2jtfikpek.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2rdznjiiz.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2gkgswewn.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2helvjjtf.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2kvwyslun.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2vkszzztm.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2vfqstlta.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2ulczarif.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2njwbpqpt.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2nshategz.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2byjwuizb.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2mocsdcps.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2fhqxgxjs.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jtcfigqy.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2uuygrqxg.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2obxmlzrl.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2teqzjlox.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2sjwuanla.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2hgejwihr.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2dxzoxkjz.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2chafwbal.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2nuecqyia.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2lkguxqas.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2swufkwhg.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2wraomlcg.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2bcufurwo.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2hpbbnusw.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2yzkppvpj.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2tykcjyyf.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2uqwkdisz.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2uurzatdw.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2wchutkqv.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2nenyqnaq.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2xkxhegqh.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2nmqfecff.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qyalecnm.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2giwpayyw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vlgccvvw.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2oootrsid.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2wjxtjmot.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2cyxgapos.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2qlgtegni.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2qzsgpehf.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2umccdjhb.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2nogdmzxv.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2fpplrito.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2rpahkxwg.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2zkvvldfm.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2apbgxanr.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2olbxrvyj.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2olgxikrd.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2sbnmrptn.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2mckbdxjy.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2zgfdiyaw.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2osqbjazs.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2rupvbbpo.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2souacinb.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2havgvoju.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2hzkhvdmk.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2aetcobjk.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2wdqumceu.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2iiqftvns.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2mtfhvmpf.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2pyodimcp.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2kjikvovm.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2xsktvmwd.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2mzxyynyh.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2uxdlkysm.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2fydljqve.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2ntnipvmu.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2bmxaldyg.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2fjrkcsxc.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2tlrqybby.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2iooawfrl.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2kcxjxmao.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2tqbvtfda.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2ivmaoxtk.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mldvntyp.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hllopqxo.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2mapdegpl.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2dkqbuwya.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2fmewlmvd.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2kigafvpr.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2gtqikyyu.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2qprwfkff.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2sqwfeccb.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2omliqqxo.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2mcdbefoj.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2zxneqpls.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2qlzpzqol.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2zftyplrc.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2gmieptnx.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2zrrzybjk.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2kteheefz.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2okpqxhio.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2gbckfzxf.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2jkrdcwyg.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2jcrbbcrz.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2sbhznwxp.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2quujfblf.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ahzwugmj.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2mjeohkqc.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2jrzmvsgf.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2mnpawpno.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2wzllckld.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2qfbxasis.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2ngssefbd.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2rtdthuwj.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2dfuxhmxv.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2uzijiksa.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2pppvpcll.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2qmomiqxh.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2dnqqnjwn.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2tewdimuy.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2zghupalr.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2lmpsdmav.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2crirrthq.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2yohpmrgi.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2phrcrspn.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2gqgdjyho.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2pynpuphj.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2zbfdkwrc.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2vkzzvdqe.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2mvubxqho.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2ymvodcwb.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2jkhbmyis.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2kgihhpdt.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2gxfcpwvg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xxylhlsy.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2bintiqhi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jcpvozlv.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2vyjcgurm.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2lcdfuvke.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2wsbtauhe.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2gjdeekco.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2hcdsuwix.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2deglciok.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2ibeidorl.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2hpsjpnez.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2tpcethcr.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2fohnbwkl.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2iyfgvjjj.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2leddarcu.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2biepusfg.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2cwypmnyl.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2blcwzlnj.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2xaozxlsf.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2tjyzuyhh.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2cbjytubu.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2ykwltejd.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2lpiiieub.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2fqnmvlkr.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2rcjyrmol.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2izxtcvwr.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2fisjsihm.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2inqyepoo.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2rtlkrwdw.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2hhdtohka.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2lxsbkbei.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2kplyflkp.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2atgnwisx.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2oadxapnl.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2zylzxrds.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2ogsaqtcd.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2ycljrlyb.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2ymybguru.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2omhbbdjs.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt2mzwirxmx.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt2bjokflcm.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2fzrobhpa.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2riewvedf.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2rmdyeorh.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2wxulunob.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2aitnlumx.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2gmogqnbv.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2sbcbbmqc.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt2setqdcwq.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2beveeefd.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt2eoklaoba.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2xnbmwddn.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2dlnjnptm.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2xqbpphxw.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt2zbqzhmzo.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt2ielgamjs.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2gakiummi.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt2slpoodhn.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt2nmafbeob.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2jfxbjffz.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt2dlqumunn.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt2tdrhfaam.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt2ueonuqwr.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt2dcnwrzpv.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt2wkdvbipg.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt2bdkikjrk.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt2tuopkboi.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt2qjbsjdhc.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2iwvovwim.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2fhlosbnc.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2izoyhwgr.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2tvguucpy.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt2qpnzmkwz.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt2ucujsdnl.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2xsqnvwyf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wfhxunoc.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt2ajlytwtn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yudpozmn.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2vvkrnzzz.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt2obzxmzsp.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2csfzlqew.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2jkfusiwh.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2yazcnwht.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt2clvpuglj.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt2rnareuiz.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt2fnflpwnv.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt2plftkgcb.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2pjsloody.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2utynpgcu.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2gixtcnmn.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt2yqwbcedg.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt2mggrpntb.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt2hlhhtfeq.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt2pzvpwdwb.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2libnqyev.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt2eibmiepb.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt2dltewxer.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt2tgdqcehs.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt2tdvebpzq.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2hghsnniu.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2nsnsvbqt.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2kthxvelg.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2ttligzju.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2dftkcfkx.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt2qvkcdwyu.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt2tdnslfjf.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2nxvmsrqx.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt2hixpazns.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2bokgmuma.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt2dqjhczou.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt2zlyeazjx.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2yoyxgqen.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt2aoighkcm.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt2bctxliun.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt2nkmkzfgu.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt2ldujkwpx.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt2gwioyzas.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2mbtztofa.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2proshros.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt2vedobbwo.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt2bfxuyqmc.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt2dsytwghr.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt2imbwdmsx.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt2hlbkfhid.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt2lfkyeach.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt2hwkdkakh.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt2bpcpxkvg.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt2hgmlnpyn.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt2jdotmdgr.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt2wejqieun.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt2zrnuatei.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt2odmsyblf.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt2hxbjikxo.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2hqcnioeo.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt2pilkdkza.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2cccwyjvc.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2jhmnupnm.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt2astdrmda.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt2rtvmmebs.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2eenhsaga.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2kpwpyivb.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt2zjukydfx.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt2muhfdeis.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt2ysayhekk.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt2msfltxze.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt2nclnbbov.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt2edsfsfwu.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt2uztkpdte.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt2faufwihn.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt2tguehksz.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt2bvpwkegr.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2kkmmovwi.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt2eynsfuqu.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2qlgkvmxt.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2rsrpixnh.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2dxetwuno.html


<!-- 参考信息 -->