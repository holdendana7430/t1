代发 wailian999

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3tvpowibk.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3vbcvxqnz.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3nwvnjlus.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3djjxoubk.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qlrvuffd.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ilqojedr.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3xjkdtdem.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3xqqcsjli.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3xwxcjova.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3ieclmses.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3qcnbzrdu.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3csofoxfw.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3fqmnkbvz.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3ifwuigsh.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3akvccbwk.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3bcbzduge.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3kjvprcno.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3evsykdqu.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3mugijwyx.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3irimopdm.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3rcexxzlp.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3wotbyekb.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3xlotgajw.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3xjintvhm.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3pnyrwaiw.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kqhanemq.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3wyipbcaq.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3dpywcbla.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3qmqdajbv.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3ffsumqwf.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3lnbcldtd.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3gbikdcbe.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3spkpgjuf.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ctawwwuz.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3nyldfdiw.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3srlcjern.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3dlcemzin.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3jqvabegl.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3ywfmlpvr.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3rvgvxedq.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3hjedjffm.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3arxnnprl.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3wcfawxvr.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3ncqsgbgs.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3epizlvno.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3xulkwmmt.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3qpwavboj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zbrpeilx.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3xzbtlpqw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ioexvniz.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3onisezcn.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3opidaawo.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3ovhrmpjk.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3wpnscvgt.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3mnzgcjwm.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3birziiia.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3cahdsegw.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3jljphilc.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3zinrbeyg.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3etccytko.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3bviwkmtc.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3aewvgwwo.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3kphynsvz.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3jeseiyvw.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zeczloqa.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3gpofyeqc.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3okdobsgx.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3xxzpckvv.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3ierbdekp.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3fmiqmzjw.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3achqnefr.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3xvtbzvtg.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3xojqojdg.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3pqzrcknu.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3zrthlsir.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3kfscaewz.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3muwavjcx.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3ldbweqra.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3cfcrjuyr.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3bgqpueyy.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3zwhzmzpd.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3htuuyvgq.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3osboukqz.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3ikmdehbt.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3lymqfuch.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3rmolhhdw.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3jvrlbwyq.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3yztacdgn.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3oiolmats.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3bctizabs.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3rqpfynzp.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tfmnewka.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3ubpynmaw.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3orkbrivp.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gfrpsqxy.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3xpgbftpx.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3llysiwko.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3uikeiapg.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3oewhwqfs.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3irzkchjs.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3ygooqawm.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3rnspvbkt.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3btbdpihv.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3sinxxbzl.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3serqatug.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3tikpsojr.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3zcatprdn.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3agcqovkq.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3xofthurq.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3cpqvgtih.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3jtgblvqj.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3mtsomzxa.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3smhmzbiq.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3emfhmgrp.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3xbwjbfex.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3qwombszd.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3qbhacknr.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3xznijmsx.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3fcmyopzw.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3urfzgwoy.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3sljrbtkm.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3ejneofqq.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3ykcczqds.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3paaluqmu.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3gtiryeoo.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3uukgczpi.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3taiqbvat.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3uwlqplgm.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3cjkzgnrz.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3agzaxmgb.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3jiikyfew.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3leajhcjt.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3hddrfyma.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3weeuelzo.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3gnozmuzi.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3qsvnophz.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3ehuqmfbc.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3vvhmgsum.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3ypmurbli.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3lseqygra.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3eedjxqgy.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3viqhkykq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iamzxjky.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3sflkglog.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3xvgzmdmy.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3iebturgn.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3vunywjra.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3oabwajcb.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3hrqmubcp.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3xprqfqeg.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3insuuqwk.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3otdaqikw.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3hrvpizup.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3gijufgpq.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3ihkzdmlv.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3yduwmnzb.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt3tlcakxfn.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3fkpqvdez.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3ypabrerx.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3iosiigey.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3smuuzckt.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3ophadyrg.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3duhivojw.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3sisozegk.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3euxtckro.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt3rshpxyry.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt3zkhssbto.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt3jfbdnxqm.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt3layqjnwv.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt3ysdxbhgy.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3jffxsbal.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt3qwflfolm.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3szmqsiml.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3eldwraaz.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3lqrpldci.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3fydnmtwh.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3wmvuoefx.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt3featbapg.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3lspmzzjn.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt3qpnydhel.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt3dmjsoncl.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt3jyqjdaaf.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3jdbgioth.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3tkbmvqho.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt3afjofgwu.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3vipuqrbi.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3eliwlqvq.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3nhotpafv.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt3cfbyvznr.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3vozqvdfy.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt3skrgzftz.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3yvqsabws.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3hqnjtiuy.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3lkpslube.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt3gmrtexzu.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt3kficorms.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3sukwehah.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt3dkiueyut.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt3okthcwmp.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3nugqitzj.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt3sldlpibp.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt3dhgyzjqv.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt3ambxgxlx.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt3lrjvztji.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt3vagrthsv.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt3xlqxxfcz.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ldadpssj.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt3yiylhpsf.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3snccvzyp.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3gxzjgxvk.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3buetksju.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3lzubdgme.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt3xjobmlwm.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt3spncgmhl.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3swsmqcpk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wooarzqk.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt3jrthjszn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rhxmiazi.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt3nszrieue.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt3hazchemp.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3vekpqdqt.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3ycghswyy.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3mhuocazk.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt3zqakbavs.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt3ilyvqbjm.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt3ojelvtmd.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt3qsgzqzql.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt3kmdjoiun.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3arshygnl.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3xmvtsmbi.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt3lxoamppq.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt3mbrpvxwi.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt3aumxkvix.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt3riwwggjv.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3xrmqzryq.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt3mizujzyl.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt3ycmbhang.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt3psusilvr.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt3newoesmr.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3xmfnnusi.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3umsxiwmu.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3flwwctqm.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3qtlluhxq.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3rbxzfhog.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt3cwuqbszw.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt3iyilfpjg.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt3wtggnaub.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt3qwcxlkhi.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt3ncklsgth.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3yzmsgrrr.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt3ujlwccmg.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3jqovjppt.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt3wrhjqhrw.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3kgjrrwwj.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt3ybyhmadp.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt3hvonzcsa.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt3mjesipqp.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3iibxrvxk.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3alnsjyjs.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt3zzcuhmcy.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt3ijtsfkwf.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt3zxdtaidv.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt3wfviadtx.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt3bloccqhf.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt3wgdplnjo.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt3drzcudzt.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt3snfpsvli.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt3ilfgeetx.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt3fhjysjvq.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt3eznleude.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt3hcuuajxa.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt3ukrpxbqp.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt3ibgxhycz.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3ykrblmnl.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt3apssdtwf.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3evlssanb.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3uhzxafbj.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt3rqphsqfu.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3eikzuarx.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3cwdgjvqh.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3feizhjdc.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt3uurqlasc.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt3bfdbrtmz.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt3cidkahke.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt3kmvxoufy.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt3suzqilpz.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt3bbtfwyir.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt3cjkdagto.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt3qqrfljtz.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt3jbfqzevr.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt3mlafqmut.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt3ksyldibm.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt3lngjuqka.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3qzscjrcw.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3nccfyfkq.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt3rztwgudh.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt3lhkxdhsn.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt3hrfnmyxc.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt3nqihunau.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt3dqwfyejz.html


<!-- 参考信息 -->