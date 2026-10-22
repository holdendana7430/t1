代发 wailian999

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ifixdouy.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jfjnzpcf.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2ibpdaozm.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2rruuayap.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2ovdxnxop.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2zzlyumgh.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2zgumvykd.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2hwnskdse.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2zdfxikif.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2sqbksgpk.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2bxvuxkqq.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2aqdeawmo.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2txbolhzf.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2qzumfcth.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2wtabppph.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2gspqglni.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2dmbmakrb.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2fujtgxyr.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2obtyifet.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2jwljdfzn.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2duuipjwp.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2qykfwtuy.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2zqvtclet.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2hjivuuyt.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2gvvwklfb.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2rtrbvaie.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2leegbxvd.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ofopkloj.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2gvyyfrby.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2kobrijua.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2pgzsxzip.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2nsplaryt.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2ajdajvey.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2hpndvnbi.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2epkszfzq.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2wlapuofx.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2cxyzxplh.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2uaihvrlz.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2dqavqksb.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2yqkcpxfe.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2hckqkygs.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2ltbbyrut.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2kefmrxob.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vvnpilzs.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2rxqnkepn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rokxiwjs.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2iauhpizt.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2vwcjzxcg.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2hjljmsfl.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2xmkykrwg.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2fwrvezoq.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2bxqmfpfp.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2luvgodvi.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2otbdhthh.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2efvulxgs.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2aberyeyx.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2ccudqjie.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2qscucwxr.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2xrqamywg.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2spmhxlgi.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2bhfrqzbi.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2mfubacbq.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2exglirpn.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ypmmrbgu.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2tjlzbpks.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2fhquyxtx.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2mwxtvzfv.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2plokfrzu.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2mpengsqm.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2npfrkejv.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2pwxsdgwk.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2epbvjbos.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2lhtnmjqe.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2omnuwitd.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2evxitagr.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2nnntdwec.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2mzfueuqb.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2ezcrdkzx.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2poovurpl.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2cunjuimx.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2kxxkefle.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2nxxgbusk.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2uztemhtf.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2akgzbhri.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2xqhrcrlx.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xcxkyngi.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2ibxsfrcl.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hapgyuvm.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2ihmjshva.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2lzoqfuve.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2ofzgjbso.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2aomslacx.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2vbmhqcbr.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2fcuyquxx.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2rridyiet.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2egeyzzkb.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2xxjpsfwh.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2nqreswjh.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2yjalsbxl.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2kytnioui.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2aedyfmkt.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2pfouzmdp.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2tgdzdtqf.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2jvlphzcu.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2hlkdflae.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2wsyirfti.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2wwfayhdz.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2bfyjuqkd.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2bpzwvkez.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2hkicbmye.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2rruyuyff.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2ykmdhrpn.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2gfxetzeh.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2ywxpruem.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2pvvoovip.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2oppnglwv.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2vqdjlitb.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2nluiduex.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2yywtjktu.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2yecotrfi.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2mxnskbwy.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2zvyjyppg.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2nrduuzyd.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2auhpjnib.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2aeqgrgly.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2uoqrbumg.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2hviobeou.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2ffccmuej.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2qytigyxo.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2gthfredo.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2besrgcer.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2dgcwnvvb.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2sklczmfx.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2worwbijb.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2naxjscuz.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2qkwrfdwj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bhtmuhhk.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2uvgunqof.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wvahvauy.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2ycwxgxvr.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2xusilldd.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2kmsgeksa.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2mvceodmn.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2maacsloq.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2hyntnwfc.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2axzjnmel.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2naalhpsr.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2sbfdxrqy.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2uzgxljti.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2gobcjcnn.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2zsfjdzrf.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2ffbvefuw.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2ycikrliw.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2lkfbsmwj.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2wcnizxay.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2esoftfdr.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2tfydhemr.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2kidkfnjd.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2izljdmhi.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2lxktwsoi.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2azpcaply.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2smnkducn.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2fylsgecl.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2juvsafvt.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2cwksbiar.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2sulgqlzm.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2dbyyyyfr.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2yvoutvuk.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2drhdirql.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2cunvmcod.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2szcqzrya.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2skyjatbi.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2pyavdwwr.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2rvslldpi.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2vzzwuhob.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt2ecymfknu.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt2ihdprecu.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt2ytlxohyt.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2ypvpvpeu.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2xyxujsmw.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2gbjhooby.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2vvvuxgyy.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2qjtzmuli.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2dxorzyle.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt2eokoadzj.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2meagmaxi.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt2vxmmvybh.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2jnpgsyld.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2vmqsywmc.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2nwtkbuxh.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt2owwanuuo.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt2grpwsikx.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2afzeqvyp.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt2oabuxkbx.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt2jhxubasp.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2vnpyxccs.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt2cvvlzxmr.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt2inkcsxlo.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt2gndkihch.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt2vgewqqlm.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt2ehpqgwof.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt2fwbmqcvo.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt2zuobqvfi.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt2tqedipcx.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2fuqsdldp.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2zsvhaxsj.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2ycyegwea.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2ffuumavi.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt2pmgowypr.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt2gtgxmqrr.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2nwrwkqgl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2maxodapi.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt2velpilng.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dxhajbgq.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2wkjtjtfb.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt2hrmyucgk.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2vdcladyu.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2uhbdobfh.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2xdefjyct.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt2pasbnkzj.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt2awhztftr.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt2wlvikcxk.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt2lvoaegqa.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2evgyhuml.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2ndnwnkjs.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2tewmfmnv.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt2bsofxqop.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt2gqhzpfoh.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt2vxgrpgri.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt2tlpkxgem.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2hammcqar.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt2idxndcxe.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt2semmuevh.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt2mkdcgkpq.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt2wuzouiel.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2ixitzcrz.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2ahmelgwp.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2nbtpjgyo.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2mjzrzytd.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2jsmntuyn.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt2ogfkklxw.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt2dbrtndpj.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2tpnlhnao.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt2bhkqvrkv.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2fosfczkd.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2lazaxrwu.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2rivqvleg.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2bntiqyku.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt2zbsngpuk.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2hfdbksak.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt2rcvkkswk.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt2jpvnnikz.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt2sotqtuqv.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2hocabgrd.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2poesewgw.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2tacgxcsg.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt2sxgefums.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt2hodavfci.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2cbxdhutl.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt2hywrhcod.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt2rmwghmof.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt2qqaaliqb.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt2oiybrxsn.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt2ayjavvft.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt2laonufvm.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt2emlmmfda.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2rjshvfnz.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt2kxhwmvuf.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2qfnozotr.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2grwwlzyy.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt2ipquejad.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2jlstckpz.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2fjxwmybs.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt2pkvqqulg.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt2dlhrbtce.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2fcywnrhu.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2bwihehur.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt2fcqhnaac.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt2hmaygcfr.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt2xgfhciov.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt2hqnwaaxo.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt2etbqjqqi.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt2ylzuyfto.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt2wvvnpvio.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt2fzuqnxna.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt2wumsuxqw.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt2cmlbbdfv.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt2pwpbjlax.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt2ppxszbvz.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2pixtwuyc.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2kvxnqogy.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2bncwitqr.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2pakfczdq.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2yvsxbumo.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt2qdqxndzv.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt2tqcprrpx.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt2bkrkkeph.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt2obsfnfud.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2vrpccivk.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2htxzbszo.html


<!-- 参考信息 -->