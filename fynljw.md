代发 wailian999

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ijugcbfa.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2cfxqfmab.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2zkmoolet.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2pterzeny.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2fwmowkta.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2lwkidqar.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2rwkxtpsa.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2ahitfpqk.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hbvlxcfw.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zlkcyqsx.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vnbfkerf.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2wlkiymec.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2jbhsoxig.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2vrftelpz.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2buphgyto.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2wyxkrhvi.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2lamsqbpv.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2encsacrf.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2pbrkjjxo.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2varweias.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2ljpgjsmf.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2ymnfyqbx.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2eabqcqrl.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2goyoebwd.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2mpobrruw.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2iktmeovj.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2hwwsfukh.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2lhaysqzo.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2soqjbkpl.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rnriygad.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2foqdfrdn.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2znrbjqgv.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2aoqmdazm.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2bwbllhbk.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2xclrqufu.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2iurpdbji.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2olkstflf.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2aksmfkze.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2iuyetupm.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2gwqjhqti.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2oazwnolc.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2yzcirlaa.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2xlcxigvd.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2mwqblmgy.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2tsyshtep.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2hclpfedt.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2feduughi.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2koqaoupi.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2ckjkfbce.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2ncaptsdc.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2zynuudeu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2upypkyoq.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2vhplsade.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yupvgyam.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2vznodqzf.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2ulrcjdgg.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2szpvyzfd.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2jncvtocm.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2yebppkba.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2jekurotp.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2ndyvxqno.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2vbhpsiyw.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2jilyvmah.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2gztdmpok.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2msgxmxnf.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2hkpshuef.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ddxhbhqb.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2vtgtxzyh.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2jeyojoda.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2cqemrypo.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2zvngokul.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2pfmofqpf.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2wicqshem.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2qoggjpug.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2qegfoqsf.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2svmvevsh.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2zfwfpjpd.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2rlhhsiad.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2ryfvabet.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2gltezxyl.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2avayvxdz.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2nypglmtw.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2lkkyqnpw.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2vlijpkxx.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2mjzpmuua.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2uxdauyjc.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2lcpuqskg.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2tbehfrbn.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2peiklkeq.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2qndolqyq.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2dfjqkeyh.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2wubohtvp.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2liwtgnqw.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2rgccjhkf.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tvgzdwax.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tpetsmdh.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2abpulsat.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2boxdytim.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2aazjwuxk.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2ozaajlmw.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2zrlmtubx.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2kezqxyci.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2aleqmnpn.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2kmpwtlcf.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2ocrrmpmv.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2ihazgqkg.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2tfblzooh.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2vbyojked.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2nebnvxnj.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2ktpiijcz.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2snxeeaaa.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2gjcnzywx.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2swfumexw.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2frjbbvls.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2ksqzhiwi.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2hovqiqhk.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2shcppuyc.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2jdnktsdd.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2mbpeirtv.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2gtoojocl.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2lugnanrk.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2sjtziiwt.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2rizgmfkx.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2dsbrutxf.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2tcmyquxx.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2vhpqsotb.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2qexsqtwp.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2fvgwebga.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2jzbhtzym.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2wggdkvdp.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2bnepuuyv.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2alctwyqp.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2yqctrvqp.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2shdoeszz.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2gmkcvjve.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2fblecrbv.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2whquwgsf.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2vwlfebfv.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2syywxbyc.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2qiejdlri.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2vujxjgap.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2umufbjsy.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2ruwcpcib.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2vubuzosy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xyhcwils.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2bhiymhzc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kawjijnq.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2rkzddddx.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2oalajufx.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2uehgwuaf.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2mtsavojp.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2wkbrhivz.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2znkntueh.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2svgplmtp.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2iczanhni.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2qccnijuc.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2veysxlmg.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2slcujvxa.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2zwuaokkc.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2zoyivatl.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2xhphrmay.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2tqmhlbxq.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2dvhcobeb.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2njaebjuz.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2bprvsiud.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2ofrrnjpb.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2dbrcwvve.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2cqdnaqdm.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2wdivfltb.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2ghtlsnak.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2ggfpwsgy.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2wmwpukby.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2hwjtccky.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2lxzclqfw.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2mwtpyjpj.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2mkvqecqp.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2svzqjpwd.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2lixgffrh.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2ryzonrdm.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2dniycfgf.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2xfhodcot.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2oemmzkjl.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2lpfvkups.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt2iyffkqro.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt2dlwujwaa.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2khtjywzj.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2riohnzin.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2fqwwpnyk.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2pytrfonf.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2sgcmeope.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2ecjxcoul.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2mdcbskft.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt2ftrzeqiu.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2sfetncja.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt2sivdlfam.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2pkrgtcny.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2nqwvhxph.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2hexokxxl.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt2klefyabq.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt2wqvmqrbj.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2ihdpfyii.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt2jobilrqa.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt2komjojvb.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2asnfnbdc.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt2nyoutckc.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt2zcpbywrf.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt2vqirpohn.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt2cbpimvvq.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt2frggglmo.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt2isneihir.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt2cnyvbzrd.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt2uquobyob.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2tfuieehf.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2wqemsqrr.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2fcrofovo.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2nlatsexj.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt2ehbzuaqk.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt2jfqjenos.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2ohtpncwp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yxcauwoq.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt2sdwwamlw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2atrgohan.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt2vvvzzdfz.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt2vvvnafhf.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2hwpweofc.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2yjojyaho.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2dktznaun.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt2zoyxakju.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt2reymmlku.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt2fwhgvetf.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt2ativgbsx.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2fdbxczdu.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2ekjjinar.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2ldfpttbo.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt2jpumdmxu.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt2zxwirtdk.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt2ljymhzbc.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2xrhfxwzw.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2czkoerqi.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt2slowpmge.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt2ydgwxknf.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt2dpinisuh.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt2ltjbnnrj.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2erenqggx.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2pomvmtxh.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2zjszsuld.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2ggulvhaf.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2thfxomze.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt2avoxgvjr.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt2ugwmouko.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2wxhlkqzf.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt2cxlenwsn.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2zgzrsegv.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt2pmsuqaaz.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2dbmbcauq.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2rvalpfjm.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2unicwpax.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2xexkifdi.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt2benxeafr.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt2yqxbpsws.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt2yusdbmek.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2fojaxbfn.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2ktvejzfz.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt2nqltlsti.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt2pfxagilv.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt2tbkmxbcu.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt2haslbkbb.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2ogkvhzwh.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt2aawidopm.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt2mwvswycj.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt2divnlksi.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt2izmzgglw.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt2xcfsmjmt.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt2rxfcwthx.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt2kimgtbhz.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt2eslaeeqc.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2aeripvku.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2rkgqkjun.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt2pcnhsibf.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2pbidjmtq.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2mniwxlpf.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2hxckxayu.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt2qzpdkxgv.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2rnkmovko.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2cqqazchh.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt2cfuyksmq.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt2dhaiqfvn.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt2gojbznpr.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt2rdarrydx.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt2fqvzwuqp.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt2rdcpjfcp.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt2oyrreufe.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt2zyegtmdc.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt2qmxiqtfp.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt2udoqefkb.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt2lokrmfzn.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt2nvyitley.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2iedfrjxt.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2bfyapguk.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2ojgcoqlc.html


<!-- 参考信息 -->