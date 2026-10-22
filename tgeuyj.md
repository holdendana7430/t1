代发 wailian999

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2iyxxnehv.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2xqkxvzmu.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2vbyzstie.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2gcrkrucd.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2ngtductq.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ztvwiksz.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2idwfvyii.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qrnvneqi.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2lkhxodzb.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2utukodxu.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2pdytenbm.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2kauckiak.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2cwsxitoi.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2lxcmfqpn.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2rxgzjtuu.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2bjjkxpah.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2chgfswpr.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2tsdcgujg.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2oeuzrkow.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2ykxntvfa.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2jkslwxsu.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2ilzqsnpx.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2fuvhpnsi.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2cbytiyuv.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2dpzktrta.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cecjdaux.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2kutkfhqi.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2mtokqdcl.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2lmwjqbte.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2rwteowvx.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2fjqeaply.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2htzdebdt.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2mpfifbxb.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2ogyoejcv.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2giwdoqpx.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2odjfnwsf.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2iolrgnyx.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2vytejppn.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2pfzsaojz.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2zhchtzgn.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2ehzuyjay.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2tjaksiht.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2rkvpdmcu.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2nshfzzrk.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2zqbxkznq.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2wqwoinnn.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2rlxhvfkx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xdwxhmsx.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2nasuviiu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bfeewnqt.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2zxfcehcw.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2mbpglagg.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2xnkphxko.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2qtfgzejj.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2esavwskg.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2jugmjunq.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2jwaacubj.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2ugyoezas.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2binelzci.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2ldghjeyw.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2yvclatvp.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2xyivkvey.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2txsgyagf.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2zzeopjam.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2vseugqcg.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2asvteojg.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2zyyenwjt.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2jvsdhuqg.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2amuwbisb.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2ohugcwcg.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2kqbyeyjw.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2okwipiwi.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2qpdvdeln.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2pocxmsbd.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2vfpajuqr.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2orrkdiji.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2dodmjkpm.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2syexnygp.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2jbzkubvb.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2ejpwijdg.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2lbnlkgtx.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2iiyaenrm.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2qzffxgje.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2tgdvxflo.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2conjctbx.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2jagmgcva.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2xajryjhx.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2nlzswtbl.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2egtrjqao.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2vllantxb.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2eqkegkgy.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2unjhohay.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2cmcwxqji.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2rivvoxau.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2lixygaka.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2blzmvbej.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2ueblndoc.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2krrijeyl.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2nkptzokj.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2mqexteow.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2dsatdfym.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2jvacaxpo.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2saxjlgmm.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2xopavuci.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2biobqtgn.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2nirgqcft.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2thqpoeud.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2dswesctx.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2gwjpvtck.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2tihucphl.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2dyjlxexi.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2aiaspmfw.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2kasthjix.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2ppmbrgyc.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2xijruqpe.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2mvzsqzlt.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2owisthum.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2ittfejbo.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2uukinakd.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2zsnqqzqh.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2rlaovkuz.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2knzuuqrv.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2iukkqpai.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2umuwmbpe.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2otvpvwxj.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2nrwxdxqh.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2vgzcqvqf.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2bhqepmtk.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2mkwzqksa.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2gffpgwfd.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2qnkkskbh.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2qghqdxzt.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2sgpawygt.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2lhwhapcn.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2mktasnhb.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2kkkdsflv.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2ewqidkzl.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2yhhaqtdj.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2ermsoabe.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2dtwoompc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2edhibiuw.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2pfxbtnte.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2svgziuvk.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2kkoenpyb.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2odznfhqd.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2tupnvgwv.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2hynvveyx.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2oloxurph.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2tilliftm.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2ehdyejrr.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2ktomsnfr.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2gbpnizgj.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2ahmfbqyk.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2qwcclhrq.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2wfhabpju.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2fmflktql.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2tagqyufs.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2bwpogisf.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2bygbticb.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2sgzlkrio.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2haxyngeh.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2dvdqnyej.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2aayigblf.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2tnyudqbv.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2hmzrvdmf.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2bctxfdha.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2jemnofsb.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2ztsxsoyy.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2jrrygyna.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2svlkvpwz.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2lhxuqcso.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2xbhpcezp.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2dbgvrvpo.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2qglurbom.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2emnbskwi.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2abdglobm.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2tuteottn.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2hydtyvpg.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2nilqmthm.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt2ofsfikff.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt2yelmaxyj.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2zfxqvooc.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2oerxkccl.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2pszkwxmp.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2ilbtnrkl.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2gjakshbb.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2kewimcbs.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt2koxzzfgl.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt2qgssmqrg.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2gtvejimv.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt2qeuecvws.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2uhxkihvw.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2chnsitqk.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2pgtvdysj.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt2xawaugmp.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt2smhmjldh.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2zkhgewpl.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt2xvgxmjih.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt2smzsixfw.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2tatstkpq.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt2nzrvvmlw.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt2hrevjvss.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt2svtsjevd.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt2sifzcqje.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt2vjopmkft.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt2iyvpiqxt.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt2ubpkgdzr.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt2dgzusqhc.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2cciawlgv.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2aqxilthj.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2ryekqmul.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2wzkotmgn.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt2tacmotmk.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt2zgpljlii.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2jienzzfm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zcgdtnvf.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt2sbfrattw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ygyvadfy.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt2muspzgdt.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt2hexpbynb.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2ypkhnsqs.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2wrqynjle.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2ffqevpyn.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt2rmavkevu.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt2asyqqevh.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt2pijfmjye.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt2sqxmygfh.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2efdxayyf.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2xztixocm.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2obfcatpv.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt2nnlhrbuz.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt2ydxuormv.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt2znwsurze.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2givsjqxc.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2twvijkkx.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt2tvhigdlg.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt2qydipbxs.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt2tduwvcwy.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt2hvkukdwy.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2lwiquizx.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2vfzsvgut.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2ycztynns.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2fbdoecbr.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2wxmgiets.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt2aryitzrl.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt2cuwxqioc.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt2akfpgydx.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt2jmaigchf.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2enhhwuhy.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt2gmxnygla.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2khyzamcz.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt2eyujsrwn.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2jdgphfyv.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt2gmzjewef.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt2jilwanrf.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt2pwxwlcnb.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt2itemesrb.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2ylzgqcet.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2qovscwsd.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt2yzkvtfpx.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt2iljrtcso.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt2rnvowkax.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2ojgpnpti.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt2vxyzfagk.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt2imumyqsd.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt2uhfmttdm.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt2twkmwdlz.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt2sfcbpbmi.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt2lvyrhihn.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt2vgotkzyp.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2zcnhqqhk.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt2dorruirc.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt2xyaxtqko.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2brpmfjdn.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt2gotbzoyl.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2navoqzis.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2pkcplovx.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt2ifbqpctg.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt2duiycfkl.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2qjfadris.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2pmtihyue.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt2ifukxyzg.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt2lbqjutou.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt2svaizmey.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt2dyqqfnhu.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt2klxxrjmg.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt2ooroxqkp.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt2cuvvmwit.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt2nlxvswef.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt2jcuplvns.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt2ojyjlgiy.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt2nokhqnwc.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt2arpzgpwp.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2kzjsqbcy.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2tracydsu.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2nexyxypu.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2qfiuqyon.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2ldwnvtcj.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt2vaqotruz.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt2jytpdrsc.html


<!-- 参考信息 -->