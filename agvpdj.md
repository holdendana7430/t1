代发 wailian999

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2klnxdlpb.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2jtmbzswh.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2hqbuliuy.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2sgskrcsf.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2cnfhvsfm.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2ujgacwmd.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2mefjgjqo.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2eoekjfwq.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2vxvnmlek.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cpjxabsg.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2djfpdict.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2bngpuscf.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2uysfexrf.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2ibxcouwl.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2kaepfqgp.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2uuqbnhpw.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2tcdokavi.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2svgrgqqy.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2rxeosebk.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2cnuhjgxe.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2arkdnlij.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2ytvuuabd.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2eiisyypi.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2qvhfibjk.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2apuomzxr.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2gwixubav.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2axtsfhvz.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2yeaqxjce.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2gqcucvwp.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2urskrmef.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2vblkxgwl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2itmreuuu.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2qsonqwrg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ebvvrpgk.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2bdodltxu.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2spcchxaj.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2pzacwpau.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2fwrpcueo.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2chizghxv.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2fwetkfmg.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2hmubopda.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2oqkmfqlm.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2eciodqeo.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2papansgk.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2tnubokgm.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2igegeoec.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2owdkteze.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2yffhvosk.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2zisdctgm.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2sbkjumgg.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2yfitsncv.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2cegcvqly.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2cwpivswx.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2gzbrdqjg.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2sdciwded.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2herkllip.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2ksvxvllu.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2kcjhgvji.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2ldjfuzth.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2pcmnrpqu.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2unabcrcy.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2chnfqaoi.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2pihnfokl.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2gyrapgis.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2duwemdwd.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2cugigyaw.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2wgixnazn.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2prnrlpql.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2itkhustl.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2ffpxpmsv.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2ahzzsnlf.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2sjcwvdyk.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2eqrsywhe.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pziilkvp.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2fnzzluxp.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tghfmnlc.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2ngeugzud.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2mdayhgcw.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rxtrwxzo.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2kdmtyues.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2rcxkfrdf.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2letgkcdy.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2nolaioft.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2xwxwoobd.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2pnoyrula.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2mgyyvcmc.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2yasvhwed.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2fnmcalfl.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2fqbghsoi.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2mimhvrlh.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2jqliyoaj.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2xtvtivgw.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2nafgxcjo.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2ckqbmcrm.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2sjegnyou.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2lqgcivpc.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2uwvvfoyx.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2aohrdozp.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2humjzwao.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2skrksxom.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2abddsmzr.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2bamsuwzn.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2momkwwhm.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2izvxcazo.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2aovhqnjo.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2fgcjcrvd.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2fmgtklws.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2jbwwlbum.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2tpynfaqb.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2nvjckaan.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2twoluymv.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2vgdwyxaq.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2pzqgytsy.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2urjslmdf.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2unmelfby.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2brmuvozi.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2drnasxth.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2wffteohb.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2oyzwoqld.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2sgaonaed.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2xhhwfihp.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2qgkdmdbe.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2bzojzrdc.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2aadsmmyg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2taeuapqk.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2aistskdf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ypmqfvqo.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2mjuysikh.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2hyqrzvqw.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2xeikjzjl.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2kbblsene.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2nilvpmll.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2fbgihqop.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2kreoepkn.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2uzcbujhc.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2sjajvtuc.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2mjxzurgs.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2golwcpxy.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2wcdpsisa.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2dbcevipg.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2tcsawdry.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2kvzbvcml.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2alwgjnwa.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2tktlknik.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2zczkpfpm.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2mktaqggb.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2wcyxoyie.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2sxqjrncy.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2lqbnkqvl.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2gooqfjwn.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2fbwectqn.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2yptyabun.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2kngcysxf.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2nywgprfl.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2dzndynsk.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2khqqbkix.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2ycapzryv.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2bpqwexso.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2puirdbjg.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2jrmdlots.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2hzjxntve.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2darhvxfh.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2elaykcqd.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt2mmnabtfq.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt2tjbckxur.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2cfkplezs.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2qcqgvldg.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2kmljabdc.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2fpbwxwjk.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2ibhwoyec.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2aeegnwub.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2ykhhlchv.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt2ijaloszd.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2xipbdbdw.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt2hjoavgcw.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2qzdkswvo.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2cqrtaumb.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2cgghcsyf.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt2mfyzanyh.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt2qowsuhxm.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2tohnxmcy.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt2ljamoboq.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt2uixtwvxp.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2etkbkcsw.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt2obqygasv.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt2wheyfyua.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt2ymfcedgm.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt2erdjnvic.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt2ayzrwlru.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt2fnhhshro.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt2azuuubce.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt2xuplnxux.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2anibqshi.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2xufocnqs.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2vgmoxatt.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2xcxxkwhr.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt2ndipqlzf.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt2lzkpwgit.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2wdoobqse.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2eendxxpp.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt2mpdfbqqn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fkdkxtbw.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2jqtmdmrb.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt2oivjsdzl.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2vovevpom.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2rlcindjr.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2epcagtem.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt2bowwwffa.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt2gqlhcsjm.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt2shgjtuxo.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt2xwbzpazp.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt2lbukakjf.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2smhfvcby.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2kjzeqrmy.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt2jauscvtd.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt2tpyuxqwq.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt2yvnvjjxv.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt2dmdnqrtb.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2slsucmdq.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt2hcwsjvms.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt2sqxozdnr.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt2rdrphwuz.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt2eskcajjp.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2oopjydov.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2lwsyscai.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2lqazzkpl.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2nzhysonx.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2ocoupfdz.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt2nhjlltxe.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt2diregfor.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2uqwqqduv.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt2lsawqipt.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2ywfmwvwe.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt2bnfduoke.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2yqunlyhu.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt2chdqtadt.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt2ysjneheb.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2fclkzojo.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt2lvyorhwp.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt2kygiavuz.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt2wnbdllcp.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2lzqrbsjj.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2vkfxvzgc.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2jimjvzah.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt2jlxqqpyw.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt2majvlmgk.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2dwxxjpph.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt2ehwqxcrp.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt2ayxlxvuq.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt2vylmjsxy.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt2ppitizmo.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt2jhmcmtdw.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt2strnzbqq.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt2pzybmcrk.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2ogfjxgwc.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt2wmmksowc.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2buhdcrkf.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2budzmwzh.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt2ytztyvlw.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2eqkunkbg.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2ndplhxuj.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2jhuzktkz.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2xpbwdkwk.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2dyplkjla.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2qvkzchkf.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt2thkrwhyq.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt2izrvoyks.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt2xgbfhrqd.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt2gbdcihek.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt2nkbxkphm.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt2dgckcvvy.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt2cikibely.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt2eqeaxafs.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt2mshfpbbz.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt2pkpglhuz.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2nllcfins.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt2innleeet.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2myrjxujo.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2fkjkikcb.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt2szjxthln.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2lxzudaqm.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2cwqkseou.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt2lhhtfbzv.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt2ovarxtxt.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt2rdzrqeco.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt2kcfhkcit.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt2gaxvewpd.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2cswtjana.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt2ccmfqcbn.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt2wddeklvf.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2culkcone.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2eernccys.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ozoinist.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt2bdqlqmcv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ghjlzzgk.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt2yzwybogc.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2zpxjeqdj.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2jguwmlbj.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2wkpxertj.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2kolmvvcu.html


<!-- 参考信息 -->