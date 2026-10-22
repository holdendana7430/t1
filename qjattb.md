代发 wailian999

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2ocxrlbvl.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qmrkofxu.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2ueevkaoo.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2kwhyppyr.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2pdcmvtau.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2ubpadvxh.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2esfmidgy.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2zwwgmrgh.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2xtgklgnw.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2lbpzxqfh.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2ftiiamgm.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2szakbhjq.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2ajezgvwc.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2ugmzgzcg.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2csyzdqta.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2xqjyjmjf.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2bqgrxbak.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2vayplpnh.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2sfktasgm.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2bfspjdrx.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2dhkrofvi.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mfjxglcf.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2hmtoswqa.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2rlamging.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2xceozeyy.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2ylkphroa.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2gqiezuxa.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2jqlbsqxf.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2jrsnsemq.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2gevimfor.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2kbzwtsgd.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2aouqbrju.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2pckclbdh.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2amrhrzbj.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2rmemjqxs.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2ivchvfwi.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2eglvhhhd.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2dxuxanre.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2cwcuhuqf.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2dtgptljv.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2mraouknz.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2bcnpuchv.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2rpdmmrah.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uvmjuaix.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2szbfxvxc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2urjmaabx.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2oltyadvk.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2euzfptrz.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2xgvipqdu.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2vzyauidb.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2tpgfvaoq.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2ovtbdqmh.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2dlrdhnml.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2phqgmqzk.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2olgrtyli.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2wfillwtq.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2cfbqgmxg.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2fedgkokw.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2xircbbpa.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2uuuwsplc.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2dkkplwpb.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2gpfuwdvo.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2rgwnwuhd.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2kwleedyr.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2qsqynvwh.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2inegjnvx.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2lfqfihfp.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2ytuajehl.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2uuhjumec.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2nsnoxkmp.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2crtvyvwx.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2pehsoxac.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2mndemqva.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2sxkooyfy.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2cwmdekjq.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2ngjcbdnf.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2cdlbncto.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2xwvzfata.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2ioouxlfn.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2tmhhcxjs.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2mwhgzego.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2lcsmdaaq.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2xodixubs.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2owrvexqv.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2qgvluyps.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2hvnlhfjt.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xwkvkvyn.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gripvcff.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2lbawebkn.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2tdppjtzb.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2nluttkbo.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2cwcnrjlw.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2ghxplrzz.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2aggirrhg.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2bduzcqrb.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2ysgquxke.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2dovyxaok.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2fuwdaxta.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2couvgqfq.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2iyxpoujd.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2bxsvpjtu.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2arayrojb.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2lmhmmufo.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ysgomukx.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2iyluurox.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2pvskptpl.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2hppkwdvt.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2onfjzfig.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2yyglcbmm.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2foxgajsr.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2wxirkstb.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2ludtkjkm.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2gbjcynsr.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2lmqrquad.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2omcwhhmt.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2weltalan.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2gpwbfqel.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2dcozvmyi.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2ogcyohdd.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2jlhehxga.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2imoasbcf.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2zqxsouyc.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2pquvhhfg.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2aeotmfrs.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2hlfzbotl.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2cjjuwcsv.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2pnjaplzw.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2dodteblo.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2tolkhjej.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2gedrcfvz.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2sjvhntba.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2pwsgskkw.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2scgckscq.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2xebdhsng.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2iqmoiiio.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2vlpbvqoh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kskbjwew.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2lazkgqbp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uhobmvej.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2kzxhnjgm.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2mzkyixtm.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2brglgjcv.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wzmxewpc.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fpqbhgfr.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2lfvsabmb.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2izdpabbv.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2pvtjuuhy.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2qpephrzy.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2nainltzp.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2gfzsntdq.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2yemgintu.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2qpptpfgm.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2iqtrksln.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2jhyhunsr.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2ugvxtrsa.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2fgwnkmwe.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2ffeuecmf.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2lnkiccuo.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2pifzqhuj.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2gikpiyjw.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2golxtmll.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2cpqitxyg.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2ffcbkimp.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2ranxgbee.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2tcojhtui.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2xjzarsii.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2xlowdjgt.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2jlabzdeb.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2cdhvgbgb.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2gpkilfti.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2ewkfyfyg.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2jljzlcpe.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2qkrvprvc.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2ukypljwd.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2vmdbemde.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt2znfhdrpy.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt2hjrehgos.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt2lvbvrxdj.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2yzdkpybm.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2avpsmgwc.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2wifshrsy.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2cwdhavuw.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2lzkcibsl.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2pxmqetut.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt2mixfhuis.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2eskwyexv.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt2lcimeeuz.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2wdkytkuu.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2thhisasl.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2tjkacbie.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt2upwpsbxw.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt2gqhkdsml.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2dkuifisw.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt2pcivfatn.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt2pztonhei.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2ulwbhimi.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt2lhobgrjn.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt2xxuugyuc.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt2vhezsbla.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt2izhudirv.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt2ssfqfswq.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt2zyssttsw.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt2mzrlztng.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt2mxrqdmid.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2yidohhij.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2lssxrkml.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2angtijmk.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2dyidtndu.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt2yxpauwmu.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt2txofypna.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2inygyllq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tmocgdtp.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt2nxxmqozj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dpagcryj.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt2dfanbzza.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt2aumscjhc.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2bzoyrdxp.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2zpdyxmey.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2qyapnwdj.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt2vnzlkokg.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt2opieuqnh.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt2rvylcbck.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt2qweamzpe.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt2dpajyacz.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2txvodcrd.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2pvlnquwb.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt2qyvycbmw.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt2nnfwasmn.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt2purbrpjv.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2ardiinxq.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2iyipwzzu.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt2qmnixuhy.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt2kbrakmjd.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt2nfbublnz.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt2iovrdzeh.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2saykpdis.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2wzmaxcbb.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2ljgjmnfb.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2gzelbsfa.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2xpykvswm.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt2lahsmbno.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt2azvdppkb.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt2dkxspfrd.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt2uofxetxs.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt2rfgvnukp.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt2zpumgsly.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt2czilsprk.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt2yppprxpa.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2qoaotrmo.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt2lskywmmg.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt2hzapsthi.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt2xhvelvgs.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt2jrpdkbuv.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2swfqtcwx.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2fzoxwuwm.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt2ajdcrbhz.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt2dxdttops.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt2arycjmfk.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt2ojyvclyr.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2gsuhihyl.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt2bxtywpyy.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt2moflnmna.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt2yfhsryny.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt2wxowguju.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt2ddtbzaib.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt2ucppdjnv.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2kygibbpw.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt2cjezlcnu.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2qcyouwtq.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2lejgtijh.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt2uqsloxez.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2pwluaobe.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2obipjxck.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2lkabkcnu.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt2yalhgbxu.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2yezjmsni.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2tujfoxbs.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt2gntuqzpc.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt2apbtrsto.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt2lbxwqdjw.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt2dnfoyfts.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt2ykftpzvp.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt2atrkdkzz.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt2wojjqdrb.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt2kbusglie.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt2rqztikyo.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt2szgjzwyn.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2qanjrulq.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt2ctgetddq.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2zojmstos.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2qihmkhpt.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt2obukraog.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2nwvockpv.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2yismgjdl.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt2rxolygpr.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt2sbdofdhr.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt2lemmxlmm.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt2xkoqfotf.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2xjyvgvng.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt2fijeutui.html


<!-- 参考信息 -->