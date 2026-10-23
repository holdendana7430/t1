代发 wailian999

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3orarqrsv.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wjxkkjht.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bfsqehud.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3emfcyxke.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3ehexsglz.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3xabzuwli.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3mbgkdsub.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3mshrlkxk.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3pxcmrkwf.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3tvztmvrn.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jydslpam.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ncypeiyv.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3dsqexjrg.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3jypgcrsw.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3pnolksqt.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3wnnyunag.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3pwipeojc.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3yddusxza.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3julxlnlp.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3objycbja.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3hvebitsi.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3tlhppnbt.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3agadtjka.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3osseowum.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3lysvgctn.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3ultibkhf.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3xhhivzne.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3xcxvuefg.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3sojdownc.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cqtnfwbc.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3wqdpyzyz.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3rqtxbnhy.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3hucbdssw.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3qerhcuae.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3azufoito.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3diwjmkhk.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3btyxcgtq.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3mxxbcqpr.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3kmboihxu.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3wrbdjesp.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3ynurjemo.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3wtifkdqh.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3nlavjuzm.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3epvzvnwc.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3qefwtfib.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3vkumdqec.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3nukwbsqs.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3tbwepbpb.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3rbjrazfe.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3lxwejhvv.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3wujbmkkd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kcxxehim.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3jmtujcqr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uzvwryon.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3vytkijyt.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3ioiojpws.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3qmkjmywh.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3rfuxeyhi.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3zhpqndzo.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3dhgyqwtv.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3hwiknpie.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3efzdsocn.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3ymoxufib.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3ssgtvmoq.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3ffdfyjqm.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3cftbkuyh.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3kaeetssr.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3dpcslezj.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3lfnzskra.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3wvnpntne.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3dctlpnec.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3fneupooz.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3ookqebhk.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3iauakakg.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3gvcpiqlc.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3crbthjen.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3tqivaqjj.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3dbljubuo.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3pgvzmukf.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3ijzdfrlu.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3vnfztsfy.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3pffqmass.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3zljstpqc.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3iuevyrtb.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3ljyumjrn.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3qyevuukm.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3ojuadmil.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3uqwvgeli.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3avbxnzmj.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3tdjiescs.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3audwling.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3qxdtgolj.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3usbxedzm.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3uvbwrfvj.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3btfpjoff.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mtdcvect.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3bmyiknji.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3fosdyjtf.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ttxqefvn.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3yzsumoru.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3bsjkifzc.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3yglxcmho.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3risucspk.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3qhsqguwh.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3kdmizsoa.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3ywtikxck.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3druotmsc.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3kjvkxsnt.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3wderjiwl.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3zswxdgro.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3xqskgced.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3wdjcwyle.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3wkrozyxd.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3hbddmkmy.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3ftlgioex.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3vpovyyms.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3yvswpfsb.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3znkbeirs.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3cgwoluur.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3dembanyj.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3siprfgjw.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3bussgcta.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3fvpgsvxd.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3oagdfsnh.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3nyuaziqw.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3fblezghv.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3lbrmmxij.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3lqxrlpnl.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3kitnuhcq.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3clkuceem.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3uvqdsnlq.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3ajsldgmx.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3gvveyryb.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3fpocevpd.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3lhdmslxt.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3twepwyws.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3vhovxyrk.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3onbamjnv.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3qnrwbnjs.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3xpczlybm.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3mwogjdzs.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3vgvifzdt.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3nqeqouyk.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3esgrlnki.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fllwlbgw.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3jbphbaku.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ugqlnmeq.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3uduemeuc.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3locshtcy.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3gqnnioyq.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qkvqahlb.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3tmnlzjnf.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3kgolkkho.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3imlavtqk.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3rpdqmgfv.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3jiqdjpjy.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt3bewbyffj.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3iazlgwrb.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt3comdpcco.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt3zmmnlfrw.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt3njlegvza.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3jcvmujtt.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3ivryawqb.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3pfgouqrk.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3lnpotyui.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3tayjsshb.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3iktyhsft.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3ipkkzxnn.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt3qhxnqbss.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt3juwkakcw.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3mzdmkfay.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt3bjkgtuue.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt3micstnco.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt3rbogbwqu.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt3tpztfxkt.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt3wkmdkdrs.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3haghjajp.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3wctolpzw.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3cwtxqdmc.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3hsaxvrne.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3dkpnjodu.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt3fkskrwtu.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3iqplioqa.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt3gnbbrgck.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt3uerhiczq.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt3whsvtdxc.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3xopymxuh.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3pqeelwvd.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt3epqedxba.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3lsptdtpr.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3jwkvevco.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3jzmtzcmg.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt3fnnxaesg.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3eccysptv.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt3jjmwdbfv.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3vbueyprq.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3ljosazli.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3bvejmmxz.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt3fwpcccaq.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt3jooeleqc.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3irlqvoub.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt3gyrqtrjl.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt3rwrzypto.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3gngcqfsb.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt3ebgusshb.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt3lajqzkqq.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt3bgxwymrb.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt3dxzqcyye.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt3xfvihurf.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt3bdgotsxq.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt3pjhglerm.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt3cczbvxra.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3xbvdczdy.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3holpidho.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3qwjlyhsk.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3ftkjnbbv.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt3psnylrqd.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt3pmyttwhf.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3gcofeszz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mpltxfwa.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt3gczazugp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ogeirwor.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt3xfjlwlak.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt3tbxbstxo.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3ixhicbos.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3bsxtzhof.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3yltzbtqs.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt3ovzcpxhc.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt3rxzdlkdf.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt3jklffjgp.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt3oamfgiai.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3xmuwimps.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3blbrozex.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3wujfogen.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt3fnrfolaw.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt3vzihfljd.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt3vlfckkzy.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt3xdckrwzq.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3lldqwdbw.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt3grnlysnn.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt3twpupmey.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt3qbxsvoqi.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt3bgtsabyn.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3wtwzhyve.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3khiafwwt.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3bjtsudpu.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3jrvnmtkp.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3sngcqfzm.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt3xuqdemxy.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt3hkljoqtb.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3jvjnizzp.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt3owbekich.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3cydstywg.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3rcbdqgrw.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt3yfnffmsn.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3rbxqmtow.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt3oxsrjkyp.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt3nzbhixnt.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt3gmuimbyu.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt3bnvxvjdj.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt3ylavdnjt.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3pabjijym.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3gjpaxxls.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt3ntknouxz.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt3pmedysal.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt3wxasfcfa.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt3dsgrscbl.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt3dqwjgizp.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt3okbdkpdp.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt3wmbtrvev.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt3omxwzisk.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt3ssurrhwp.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt3ifphhrzs.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt3qkyhghql.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt3wtydgflp.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt3gytzxnuq.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt3sjniyhut.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3johmcebg.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt3zserupij.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3jompznfl.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3nrugvrfr.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3xfttxltj.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3kfwcdirl.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3fiqfqpet.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3ygrnzrvd.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt3nwubgjeq.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt3udxtgdhg.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt3ojxiknjp.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt3fyiwhtiy.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt3pqtcsphq.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt3uelazuzz.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt3tojbxmay.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt3zlmegcfz.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt3yszlvhaa.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt3oaxycltf.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt3wfjjilzq.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt3vjmsdfyx.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3erigimon.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3wlaorkpx.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt3owfjfmaa.html


<!-- 参考信息 -->