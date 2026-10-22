代发 wailian999

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2lqsdoens.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2ghsjlfnc.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2vpqnbnob.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2njbrihix.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2obayxris.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2iynkeamh.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tgtcoonc.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qjxqlksm.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2ntkdeggk.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2npflpfum.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2cwcoghju.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2txzqpuwl.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2nerwdcyl.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2gdiqujox.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2mctlgsed.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2lvesltry.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2dlscnihr.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2fbhaswhq.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2jznifscl.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2xusunqrf.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2eijxoidd.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2jiuyndad.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2yhgzuqae.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2uodaxmmk.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2dkzjkads.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2aloirsaa.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2oofiowhq.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2fqwlctff.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2nhgxdigw.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2qeaiorhp.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2lyorefna.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dysdoorl.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2pmiwtepz.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2yrvihasm.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2ewmpqqci.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2yjqcjgyg.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2usbsydvc.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2yaszupvw.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2kyalwpah.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2jjjpdqgy.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2foxaltsg.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2kvdbhaxx.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2wcmluyrs.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2pbqrupmy.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2wkkdcnfg.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2weacpbob.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2dbicvjro.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dntqovjr.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2nhqqzsbg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hiacwgyq.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2offxobhs.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2fdcdmckm.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2somshmoo.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2hzhobngo.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2qkngoyfw.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2tiozmvrg.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2wbwhkpch.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2ajbttujp.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2nlaxqvhu.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2poecbkeo.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2iitcjdti.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2qfcwzqca.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2kjblkzif.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2rwxpbdkf.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2bfvslpyt.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2qukmyezc.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2girmpncj.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2lgroqqkk.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2revpfwgl.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2zipabtzu.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2xdswxbhn.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2xauioorl.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2bowdboml.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2wtvhidxi.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2nlybbjzs.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2lvcuoavg.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2oailzmxd.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2ralbqcdg.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2rdayxxrg.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2mnmzbbgu.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2pnqxviez.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2miydfyca.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2hxotoetb.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2ppdgaknl.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2qmeulqrd.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2peycgnxv.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2qvlyvmej.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2tozqozjp.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2sxziihlm.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2amhqleze.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fdjppqns.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2saizbzzb.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2dqrpcgmx.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2xpynxvom.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nrhvtxlq.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2mshcsnlq.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2hipvsyes.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2emefpxto.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2kmidwmah.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2rhbtdqlp.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2rjpcyuax.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2puujcnnz.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2hifgsbiw.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2fpccxqkk.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2rkptxwis.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2gldishkh.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2ggtzqbtq.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2nkbrjgxy.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2xpyyspyo.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2ucpzhlvo.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2anwzlvmy.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2moiylmbk.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ppfocakq.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2gmoetdfm.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2fgonlysi.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2dkbujspb.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2zaadnqul.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2gyaiwnaq.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2hspnondg.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2fifdnbgt.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2oszkewlr.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2yycxxqms.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2batkxmwa.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2jifqfqzm.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2umnatvub.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2qlhpjcjp.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2hdmnuofd.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2cmxzctzl.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2dnvctppu.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2aukkonrj.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2pftkmchm.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2wtwsqvuq.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2xdhfnbrg.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2zipppqbc.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2pzliolyq.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2kpiabgbd.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2ygsguzyl.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2dsecnalo.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2yucbrymn.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2gprrrsyt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cjtqnxkc.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2minanwrm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2njdvjmgd.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2liwvbtcx.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2glophujp.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ubxhhdxn.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2jybdbaac.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2sewsdyrh.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2igscichk.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2ocdkoywf.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2asmugpvt.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2nxyyttti.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2byibltsw.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2mrjcwptp.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2eltdebjl.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2ipeezves.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2mejbvmfa.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2imgqokpa.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2iigfllzz.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2mkjfslct.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2aglhlsnq.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2jzjxelms.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xqoageoy.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2kzdvmzkh.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2tugifqzz.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2jlzphtwm.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2vtgwdsbt.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2eeoteqtx.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2stsjofyh.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2wxjncpgr.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2ohtbivih.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2lwcacpkg.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2nrhooqyc.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2jnrvpund.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2nrbwbiqs.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2neqdlkpu.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2ooywlqnc.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2upzxzlir.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2cntwupnd.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt2zawuezoq.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt2vsrqeusk.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt2badkebeg.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2hiyhpjti.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2wmrnbkqa.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2uwcucwcz.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2bcujbxfg.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2waskqcyv.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2amxlmlff.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt2wxsrflgh.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2hemyzdlz.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt2csxecbwg.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2dodpuong.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2clqvswat.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2wipqdevb.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt2solzsvhn.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt2xwyhfurr.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2fjzglzjz.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt2okfwgymt.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt2pbaicxof.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2daojxahw.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt2jzzttaci.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt2mputiqoi.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt2gwdwirvr.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt2xykupbmh.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt2orudqznm.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt2ukqoriqo.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt2rbduptiw.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt2brkigxnr.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2xwtqphgu.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2pqnsgbmb.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2xphxxrpr.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2viwxqpvi.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt2ogawancs.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt2krvmhimv.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2jlulwolh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wnpyxrkp.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt2iszovlwq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2euvhfenl.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt2epbkafsg.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt2bauwjvck.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2qyweptvp.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2jkuktkvs.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2zxnozuhh.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt2lhweracf.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt2cdfogugo.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt2xobhobpe.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt2kgqvfpty.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt2gpotiimv.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2qftyfugh.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2kpbqzqkb.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt2wjlqkqfk.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt2lqywqhmt.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt2mwppihdx.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt2ficvymun.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2ixuzgaer.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt2aaemnele.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt2kktizprz.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt2alsejjnb.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt2ubmektpi.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2zplsmpnd.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2gosmysfy.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2qgpmevas.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2irogyljv.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2jtihmyse.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt2ynxskpse.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt2xsmakwsd.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2goqajokh.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt2wktqsbbp.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2xntgxnat.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt2oyjxlaax.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2bnkacjbw.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2evzkosag.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt2ntjvqhnx.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt2lwuqgent.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt2mntoncuh.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt2uzksstmn.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt2qibkousw.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2kywkhvgy.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2wvfasnjh.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt2cozllkyy.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt2dfszcokf.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt2dimvhwum.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt2cdjsujxz.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2frrfdxzu.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt2qckvqylv.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt2ksdtwdqr.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt2cqbqjayk.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt2jdjikoib.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt2coityhxw.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt2qwcpzcfq.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt2gzslqcbn.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt2mzegrblq.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2xqqymjkz.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2ffeopkdr.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt2rvbkjjvp.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2pxyormdl.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2lqpltoiv.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2eonyvffp.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2ebmxzhrf.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2ftmxtkcq.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2bufbcjvk.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt2iidyziro.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt2gzpmctpi.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt2bqszuskd.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt2pazlomov.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt2ygvzcvna.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt2uzafeyur.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt2iaestfag.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt2ulgnyszp.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt2bcsfowds.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt2qqgfpumb.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt2dfoiewkk.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt2ubqnheyw.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2yyoocvvn.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2ppewzhar.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt2ljsqhwxq.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2ffxawflk.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt2jbvnajad.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt2cwqvkavs.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt2fzkskaja.html


<!-- 参考信息 -->