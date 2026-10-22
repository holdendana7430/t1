代发 wailian999

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zyhfplxb.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2nyoljfts.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ddlvhiaw.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2etzlgazd.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2agghozrn.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2sremobet.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2dtaxqnwt.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2xjfzaziq.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2chhmouyi.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2efxyyezr.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2wwwnzpcn.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2vrnqfnlk.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2jhpazsjt.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2zesvnxur.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2socgrlkk.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2gbuwlnte.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2devvlund.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2yroowhue.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2vclpgfjr.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2sviyukik.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2kdruwdav.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dsgtdxrc.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2thljdwkm.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2tmxwqukj.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2anhksbhe.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2lgcfiorx.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2pqnnpepy.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2dvnhqerr.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2dpaaosts.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2aonzmnhr.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2flfxktit.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2cebiogcz.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2pzimjked.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2qoooqhgm.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2bjharwvm.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2iguovskc.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2bspteejz.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2szgndrpw.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2uvgjgigd.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2hdojbozc.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2nkcastpn.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2tcedpbun.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2ptzfdvii.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lvydsimm.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2oreohljo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xavjxgnk.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2gctlncha.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2htbzffbe.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2dbjoqdpr.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2dhrxrhtk.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2gudvjicj.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2qpyeabcz.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2huhtudsu.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2jhddplgy.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2rzgjujet.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2odwvdqvx.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2tskobuzx.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ilcrczss.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2tmofnpdj.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2xjkuprtj.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2aqgachwt.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2fggujzku.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2svhotham.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ewzqtmaw.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2ajxqilyk.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2ifqcsghu.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2xvgnngaa.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2jppveoov.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2jfhtlyln.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2xepxkoat.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2qobtfzel.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2bgjqjwlp.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2eibsgvzz.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2xvnsjwfr.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2jxqnvmzi.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2iuoqkiws.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2nrjoxozm.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2xvkwggcm.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2hgvakdmq.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2smqukswq.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2zucfwjew.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2synlzkxh.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2silecpic.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2rnhkeicy.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2vkgqmfak.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2sczktbfi.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rtvmassm.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dzgtrrrt.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2gzqjsvbk.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2jonwzqlk.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ivgsddgk.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2jyeuscyb.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2trdxegvf.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2vvyfprav.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2kkgkdsqm.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2wgpoatto.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2quuoksey.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2khumfujz.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2jysnkoeb.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2ivsrdcom.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2mofwflqo.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2qaykhgee.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2pnirctcr.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2uotlfjbc.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2pcomvrwk.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2djopfqay.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2oywpnmrk.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2iohdhzae.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2nynoemws.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2ttlgtdyd.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2ormnzlsw.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2nqbgyuri.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2uzqpdmkj.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2jgdjwotm.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2echppyve.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2slvuuqur.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2xlvphfcr.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2copjyxgy.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2xqfzpiht.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2byhkzypw.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2znricwop.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2antfgtqf.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2qtxujdex.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2zpklxerm.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2agdzznws.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2bzyutved.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2xtjynaur.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2fesjulyu.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2jgpmaktj.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2svhjflcs.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2fiammpif.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2uaanbkha.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2vvfjylem.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2nnbtfkmm.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2rpmeoumy.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2qzqeokvr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ektmuqug.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2lkifdtga.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ukxtdmrh.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2ipaxjnlk.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2qpxiscqc.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2ngepckrz.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2vimclitn.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2yizsbjzg.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2aatukare.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ecvdyuom.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2xheyjgfg.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2gkcogfia.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2aaviaiog.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2fqjhjcul.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2eagqtkhg.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2xgyjmcqt.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2rblmgzzm.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2pdylunvf.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2xkqdrfbz.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2meljzpme.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2pjgtymgw.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2wgeulvod.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2hmkznrdh.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2niehqprt.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2lhfxcppc.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2aqhzntbl.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2hnuoljzk.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2xtrsjdgt.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2yocpwhpu.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2yixwhdud.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2awujhulc.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2wzdobulc.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2hpaafqbf.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2rvldqfmt.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2swbdzaih.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2uenthvmr.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2hfqwcoqy.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2hrkfjpxi.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2cvqbgaar.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt2eviydqhu.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt2npmzelgq.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ngcjrttd.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2edcankoc.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2xzqgiube.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2jiabsvct.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2uumfnkqw.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2ebknrcpy.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt2jcppdkcz.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt2bsgayypq.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2xothtyah.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt2gfedtzsl.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2tugnllvl.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2mlphbviq.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2gfvqjrsu.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt2asmcmuvr.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt2zxvtvmgw.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2asmcrwns.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt2invvzviw.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt2zunlknjf.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2amqbiyha.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt2toslsphm.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt2oufycmnz.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt2sdbwdblk.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt2tbqrmnwb.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt2iisluryw.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt2hsmajxwv.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt2wiyhdhvx.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt2jwgfowbx.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2tzqqwuql.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2jkfysogh.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2slzpkxpv.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2eiokbnvm.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt2uvcenvlz.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt2xewohflt.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2ukoxqrsl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xtqlungd.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt2lckaafxu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bnlhubiy.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2bqelnkvo.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt2fyrwzcey.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2qvmmgktv.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2jxkqqykk.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2kwhnsdei.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt2fhoxfcfb.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt2bsqnkmlf.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt2rxtknjok.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt2gujbywzf.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2ghnlgmiv.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2vdfujmti.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2qvrowfup.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt2zodgaexg.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt2tihlodac.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt2sgvtekbq.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt2lzxhqvtu.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2dodmttuk.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt2ecnihtwk.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt2ambdhfhh.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt2mfbhjxja.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt2bvwsrhok.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2rnyttgph.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2hggnqbyq.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2bgimvbcv.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2gfjmmblv.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2jwhyzvne.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt2rhbsjouy.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt2ftrhcpyz.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt2rwqxgpsq.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt2pxfelwor.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt2vlwqjyai.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt2pkjlxkye.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2pcetrqyd.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt2ggmgyrra.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt2dutnqaoy.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2qjfvgrlh.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt2gdsdaeot.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt2frnndkdk.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt2tlveygco.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2arlgvovq.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2pqaubewr.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt2aanhyump.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt2gapyqjvx.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt2ptgvzwzo.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2qpuueiym.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2xrkapgwa.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt2sefrqngt.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt2avqxgbiq.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt2nivcrowf.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt2drxesvhb.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt2dhflldhk.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt2qxpwznqi.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt2lzdbldnl.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt2cdllzimo.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2jegtosvw.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2gcqsbpsy.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt2gafbkevz.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2liypvkon.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2ngycnbdg.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2ebrsqmcc.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2oqatxitz.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2wbbzopco.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2ojsimheo.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt2wcydwnoj.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt2hjpmulja.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt2mfkdkrou.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt2uihxuxov.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt2ljrntock.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt2aedeztwm.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt2yeiiaavb.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt2uhgsbqjl.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt2sgwfpudk.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt2zsmqtiwx.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt2famzcwfa.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt2radbmgfg.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2epsgqozj.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2oqnbtwmd.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2addmonke.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt2qgkyepnz.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2snyjldaa.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt2lxmiexoa.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt2rwaongbp.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2onxmoiwi.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt2sprlckle.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2jbdqntsu.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2nebjlbrm.html


<!-- 参考信息 -->