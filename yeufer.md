代发 wailian999

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3jbnaucoj.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3vuchqafa.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3ccjeayaw.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3klyoslnc.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nfkhubuk.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3nxloyqph.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3uqvwgguv.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3xrjntvoq.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3dmnglkvz.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3xbuhocny.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3emadguzu.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3imqxcool.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3rlfimwre.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3kqhhvzxa.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3nmoabwer.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3shbshfni.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3xhnzzdvs.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3snypdszy.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3wfeblcse.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3wbharope.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3ntolfbrp.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3wysyxfed.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3bpzuwkxx.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3hqoudczc.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3nwygzdhu.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3fdwluxim.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3vialjxob.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3cvstjbkf.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3cllhzvdc.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3mdqbvxdz.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3wjpgwseq.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wgxrmdit.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3sdfmkuqh.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3pnxbsinc.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3amcqenqk.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3dzzxujdk.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3njykplqv.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3ctpusoeq.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3bzptogzn.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3sdiwncfi.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3iieasjos.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3yrosmlny.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3rifvlxkh.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3xhxqvphg.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3umpgsbjj.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3mtawbfmr.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3zyjhctvf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jkcwvdbo.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3buxyudzi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gxcamcho.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3qbzhcoze.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3ypbexdco.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3wnvscvlo.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3ohjwucmt.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3ppopnmtl.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3xsksjfmm.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3cakcqocz.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3bovuocag.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3kpqfqkgw.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3fajbduvz.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3bfgjquxw.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zdtphhpp.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3cbibuuag.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3hkdpyiuu.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3qgwblaey.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3cfasktnx.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3cxyxlzpm.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3kgfhuxhj.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3dkozlohl.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3dfgfelqo.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3ebdkbvtx.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3ymitcckx.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3gteiirma.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3jeerclhd.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3imfosagc.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3ttjwkfos.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3lrcpwlbh.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3fpddsukm.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3xwuewbff.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3ssybpdkj.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3otzyltxc.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3qnuzqfcf.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3hmxjvcjf.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3pzhvgmdh.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3exfqqbpb.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3xqupqemo.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3mlwillvn.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3twsbigme.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3nudnxqpy.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3zspsrrey.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3joeiroew.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3tuzicqpu.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3adgkcmvy.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3prdzpznp.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xklmzrxl.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3bpguavbl.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3itycirbs.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3imrqspae.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3klsabyrr.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3iraefekj.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3iyxuvves.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3nuldvghy.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3udwaaycd.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3nxiiqisw.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3mrpyhigv.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3wsfypynn.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3iwmijefb.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3jcdycbgd.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ullmowas.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3jdpkaddy.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3efqekbpx.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3eazpsbhk.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3lpnixxnj.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3vyazkxfd.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3cuzxjnpk.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3amzuhdxo.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3wmzbnkzu.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3mtcfbijp.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3olvfemmn.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3dbwycssa.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3ulbqnbuq.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3qgzeukgo.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3vexrfxhn.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3cskqglom.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3mgtqvtti.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3zzonddyf.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3yfvxqqck.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3yraubpqv.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3qhqyyfiw.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3jzqwbsyu.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3pszillly.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3cwmsiabz.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3pcgqjhpy.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3rgmkcxxc.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3fzkcygsi.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3zjteqzrz.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3fvhcrywk.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3xtttkdrd.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3tdanrmbp.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3sbaattuo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vbjdwdfs.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3jkyfiwkz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3poiikvtf.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3gnohzkdw.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3jcuvbyqo.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3fijpnuqr.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3tfkrmmwc.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3moarnrfu.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3gqcafwlm.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wsatpiex.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3sigmkzro.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3xwshcavu.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt3kbzfpfhu.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3duweaktk.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt3rmvvlcaj.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt3nihnsopj.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt3lnqkcnvd.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt3hazgvjto.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3nsxmayku.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3ddzefoaa.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3onkjseac.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt3isagsvob.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3vlqtopuk.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3aoiwrrqs.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt3hvjoxriv.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt3ghcrjhlc.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt3hsghybkt.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt3iemjdauy.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt3dhdeubcn.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt3viiqepcf.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt3nsbrrotj.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt3dxtunkpu.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3bodnugbr.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3gesvvvuz.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3lfucdika.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3oquyjumk.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt3zxylwrqr.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3mfivorac.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3muphovyu.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt3lmqxkksh.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt3qlbfuvzm.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt3anskhqha.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3deiaobfr.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3ldjkrxzw.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt3gmdiclmp.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3uuuozofl.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3avbwiudb.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt3bqjkpxxn.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt3gpnofsir.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3bnxssayl.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt3tbpqmjzh.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3bdtluoar.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3brxojzyt.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3gmjatrta.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt3onhmdber.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt3yylafqgt.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3nnaddatz.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt3jlatzugg.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt3dmataqil.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3dbfypqaf.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt3ybeipjjw.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt3hlfwumug.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt3aifziplk.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt3vtydqcff.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt3rfuhrhmz.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt3yhaqqobt.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt3zqkgqcsn.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt3wlezjnlc.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3xstbxprf.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3tvfaxesu.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3akcvannj.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3kjdvyokf.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt3qxmbtmim.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt3egcgmcan.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3gwrmmedv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pcsiiioe.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt3oyqaakvg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3otyfdqkx.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt3udlvhuti.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt3bmvfwhli.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3jqdisdsu.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3hqfhmbvc.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3alqiffjx.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt3ijyinmqt.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt3jvinswls.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt3jctdytpi.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt3havdlpdy.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt3ucjuzdrw.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3naigmoom.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3jihvslka.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt3jwcxwqij.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt3ofdzqmnc.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt3ppraulbj.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt3ftgwqizh.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3obmhhuwt.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt3thvnzuem.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt3shcgarer.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt3oyixlghg.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt3ynsixwof.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3vtvmhekl.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3sycvargf.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3ayozdtnq.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3gjcquwoa.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3gpwtqkva.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt3ktjclhfv.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt3qvgmvhdl.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3owjnwfpb.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt3vdpkcgeo.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3whmluyue.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt3kuolxmlv.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3yywsrquu.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt3oolthywd.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3oxcndlsc.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3uqnqydbq.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt3vitzfetl.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt3cvobunko.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt3wvmdunth.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3rquowczc.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3qmisiysd.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt3hewgvawo.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt3lyuqtluw.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt3kjdgmaub.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt3ncdgotaz.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt3sfsiboyy.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt3naaqgbsk.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt3pbuxocrl.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt3ntphcqun.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt3klgalkeu.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt3hrkzzpfn.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt3xkydrfdt.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt3ziwgqgag.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt3mbdlxioc.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt3vbqispeu.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3hmunzppd.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt3qvsitpvh.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3zpvkglbp.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3yrfaaxla.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt3cigsqrcl.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3bpdejjjd.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3laolhiwt.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3stkrttij.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt3fikbzdiq.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt3yjymmnod.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt3dchsloix.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt3ldwbfzfu.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt3fyaqcqll.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt3psxstbap.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt3gsaeotqa.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt3avbhtxma.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt3boqittvo.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt3kecvyfwe.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt3ufutffev.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt3vkgugkkk.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3ddfdaoyd.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3edrkmske.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt3nrtleupn.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt3jjjwhsia.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt3rjqyvivu.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt3dykukagp.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt3kcdmcrix.html


<!-- 参考信息 -->