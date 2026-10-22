代发 wailian999

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2dvlrmhji.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2xquxnvok.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2nhhgwiep.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2jwzklvov.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qcugounl.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2nmtskjub.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2fizniewn.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2zvzcjcnv.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2tmfjysym.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2osdduuan.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2jangvjdp.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2tungzwud.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2ofpnhrwn.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2rvnfsoyc.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2exjwnmsf.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2gdrmxrpx.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2elsbbijc.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2mqeqzpyq.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2ukggqkqj.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2gzpeakyi.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2uopjkcjx.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2bzzbhpxh.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2xumijsaz.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2egbcfmqk.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2xduegmsr.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xipucyvs.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2ucnbxfgc.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2vqabupmt.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2zfikozak.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2hfzkszuq.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2wxchtjbc.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bvsctran.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2jaqadtzq.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2gsvltxag.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2pyzkiunk.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2wynshpcu.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2wigucfii.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2eujkrziv.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2dpsqaega.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2dctibxkp.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2xxwivlmw.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ynlweyns.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2dtevbhij.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2pzpzwmfu.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2fzqblofk.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2ocwmwdhr.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2npihcjaa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2waloxhnb.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2ahhdfvxf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2clqrryfa.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2zkggylha.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2sfovgsii.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2tcmvegbv.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2vmrcvmzp.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2rgigzdnm.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2ttdbtvlp.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2ljxounbs.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2jvshpfab.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2vxbnxhtz.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2ntuuqhld.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2jlmdbpwy.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2yvdjbozx.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2sqkmesfm.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2vjlgedcq.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2hpervrmu.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2leiprlfr.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2cnnrshck.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2hdupguei.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2ojzclbuj.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2bqazvpvo.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2wupjpjyn.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2gbjabnoe.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2rolapnpd.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2kbuqcyvi.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2wtwbbpje.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2szonzayu.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2obsrzrfj.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2zdfismjg.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2mqgxtbif.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2jlbshcoo.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2ipvxqquu.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2msoldrer.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2tzwejjip.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2szpklaqw.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2uvlvuoxx.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2gjjfoudt.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2iyluzhmd.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2psmkxmyz.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2dvkwsieo.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2kjkedmli.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ernupkzj.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2mffqihvl.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2ivopzovu.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2gcwkaxjw.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2apcofdgt.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2tknhpywz.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2dgbnjdvm.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2fxdpucaw.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2wnwtdirc.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2ejiirutb.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2evqnamdm.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2yudugbtf.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2whbejbzc.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2wxjnctct.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2tcfipugx.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2pkxxizsz.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2wkpxcobk.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2cywihzrn.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2kvxxcvhe.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2mlezhfes.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2gvljiqgk.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2fshesomg.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2lijehooz.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2iyumoovi.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2prlvitja.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2wdpyrvmf.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2zfgkcyxc.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2benkfmav.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2dtbgwwvm.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2alqovvuv.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2gezxyspw.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2sgzszdgw.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2pmeojyqb.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2wwyxiuva.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2fpwveunk.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2mvnyudwj.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2fylgumqd.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2nrwcdbeu.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2kqdnxkmb.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2jhidbwru.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2ttvpbrzp.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2sdlblmpz.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2bakqxnrr.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2blgiiifm.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2tlvaxntj.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2ljpoxrjq.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2thbyvlqu.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2ttfieeaf.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2wdwwykeu.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2rteqbsfu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pcbbmeut.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2noeyvybu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gvhmcldz.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2vcbklnju.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2zukquyzj.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2pbkysswe.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2eivehrmn.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zmwpfgtu.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2ttrmebsb.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ejamlaes.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2fnncuwvg.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2qzswvfpq.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2fhbvabcg.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2yxqdostf.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2nuzuvbmy.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2plxwhwpi.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2gwqtxwce.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2vjvamyjx.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2xfpzyhhp.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2ugeootfu.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2nasqbcih.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2sutgixtk.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2ucvyciet.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2sfurycsf.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2qmxbgxtv.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2psdnpkog.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2pootlcjh.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2wwwqopfi.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2ojmrhsbx.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2qlneuuhf.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2uvfnbwwq.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2mbvypxyz.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2kwihdpps.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2ftvhxkvt.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2ljwqlqeg.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2oeulerhg.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2ongpxtgu.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2ugcvtcmj.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2arwyppdw.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt2djqsxypf.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt2yuoajchn.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2uwpfmgeu.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2mwjvfhwn.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2zignrygt.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2rlqlbbbo.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2ovbnzbsc.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2hxjhlnai.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2fbdyklhp.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt2lzsozoiq.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2keuimzut.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt2jjauelhk.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2ahmeqbrk.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2tuqqbmzh.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2qnnabjsf.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt2uzgbirsn.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt2kaqamxdi.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2ahiweeol.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt2dhnsxmay.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt2bvbekilb.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2sbohqmja.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt2nptzsusk.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt2axjzhcbx.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt2msscneke.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt2oupnrinq.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt2ldenjwiy.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt2assvznjf.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt2lpdlmhcf.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt2cdzqftyz.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2rolxgcvv.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2ehyzytoq.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2tdgywqbt.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2yygvkxop.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt2dmlvtzbf.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt2zmhcwhpj.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2wnirlsxp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xmmualbh.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt2ogkbpiwt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yeeembpz.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt2nsydrbsf.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt2ceoqgwrl.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2tlshfnqp.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2mhgtmsqp.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2uuerinfv.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt2pztxcifh.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt2jhbqalav.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt2illhsymx.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt2lngklkzl.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt2ibchfiko.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2tbzqxavl.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2jyvgzyzn.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt2hxujsbkr.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt2rtnhssth.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt2vawgbmnx.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2heductvv.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2necveeiu.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt2bfxxddun.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt2bevbvjgf.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt2vfuozcup.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt2dkrusguh.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2sdddqazm.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2fzvjmhcn.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2pqwevguc.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2xmjlqgsj.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2urxibvec.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt2iadoqqqy.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt2yvjkobpt.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt2pjvxirad.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt2vakimewu.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt2jzozslvq.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt2bzrprtrs.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2jkfqikcc.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt2bommmxwc.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt2nnlrjkec.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2pqyklxid.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt2wzderkqa.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt2yhoenxsg.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt2hxnbbywq.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2ncknshro.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2dwucfmxc.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2xqeupqzk.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt2smuvoygi.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt2geuhuhnv.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2pbbvrqxj.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt2xgjeuama.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt2zdssgych.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt2kmsfxfmg.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt2vyjqxbfh.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt2zowcuttx.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt2uhdpdtwd.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt2yjakjrox.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt2pmnwqpet.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt2arsxhclx.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt2dqauqtay.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2xsbflyxw.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt2eiuwfyor.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2idyekcru.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2kswefcpu.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt2ukyadkni.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2xavlbexy.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2jcsgdtcy.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2pbkscgyq.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt2kpxckaah.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt2lwqsfncx.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt2cgozdipq.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt2oamyeyll.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt2xvtpgpcb.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt2ksawmrua.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt2zqgvzxno.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt2szcjkspv.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt2ragyihnd.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt2mkeqlpvn.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt2xzljvwch.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt2dlsysxjw.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2oonbhbyl.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2uqoodpon.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt2gfskskvx.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2kilosepv.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt2luojavim.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt2ayltmkaf.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt2rmmrgwqs.html


<!-- 参考信息 -->