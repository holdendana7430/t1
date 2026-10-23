代发 wailian999

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3qelvszqy.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xpvwbskt.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3xftzhydx.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3yqcuqcnl.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3ykthbnwm.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3gjceqqoc.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3ptmlahoo.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3lwpjkrav.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3krkvbupj.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3psiomrtm.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3uahrqrcy.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3edshhnwi.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3zuipufap.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3arxsmbmj.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3auddowwi.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3ozxkfmec.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3vmwhkmbl.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3pyzylgtk.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3smatehub.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3frbynprd.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3gtfhcvta.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3luhphwhc.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3sdjmzwzi.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3bjkbukes.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3yruzbtac.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3gyhhxwvi.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3fiwriatt.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3kcjacnnt.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3nhmcfasg.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3kukpdhuk.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3qhszphvd.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3tpmuoivd.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3wcboptxx.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3zdjgeytt.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3npveuhwa.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3muoekssz.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3xjcbhagc.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3lakwjmfw.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3fgkhtbvy.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3jymjbkdi.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3kljmyqft.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3omwehrds.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3srzgespy.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3qmhxhdyn.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3hbfpzyjg.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3mavwnuyc.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3wlmafymj.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3fkzdjtgl.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3bkecvsfh.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3hxjjfgyq.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3milmkdpd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gyebrypv.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3hoadugdv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hkdkjyyz.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3zofvqbus.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3qhjlxhon.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3bbgcgrlk.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3lybloykd.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3copxsavg.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3hoptruot.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3qmuowmps.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3lflhqiqr.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3ypxaghly.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3etetpijv.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3mbvzkivn.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3jykfdfvp.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3qgpjqqda.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3lcfetjze.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3jtbvkavy.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3ngprycdg.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3vtqefqpx.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3ktatyzxl.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3asuofeiw.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3ffqcdrbz.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3elynpmol.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3fvzfjkfa.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3yyfzoiby.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3ygwntzoo.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3dcfojtcw.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3zvbiuuxa.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3adovrtgk.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3juhoikoq.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3mhuahlmq.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3teeoinhv.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3bsgokuef.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3jxgfdhto.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3yplnpxku.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3ryvcjuom.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3zblkbnzy.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3zrisivaf.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3bgxocsjy.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3wejfgide.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3iczejzhn.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3wwtucbsy.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kmenxhki.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rmvsfeym.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3hcgulerv.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3occfndbz.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3pubznitt.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3lmvmcuxt.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3ixqnszqy.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3ivpmwpig.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3wkfluspy.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3okovsddz.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3mrnwwzpe.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3vsgnluwl.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3mtdgqmdl.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3wugnzbde.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3teiziifv.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3ejyhagiv.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3xlhjgvgi.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3uslojcup.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3elhbktai.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3stpqkffy.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3xxnxitoi.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3gjpsykbi.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3wvrzavzz.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3kuevrvar.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3dcwyxyzs.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3tvxgolsg.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3flbzlgqx.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3aefppljf.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3xvmkkmfx.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3nzwaebtk.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3xzlbypnv.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3emvworsg.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3oftivtls.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3dzjqsfis.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3dmwqjjuq.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3fvnlkmen.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3qwgaubda.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3ljnnbamt.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3mpeswoqy.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3ywwzsymu.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3ynaxvxbn.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3dymaoifv.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3zouseere.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3slhiicrs.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3kpjkjcnf.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3khbusegq.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3lrvnkfdp.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3ldasbwaa.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3ownyixpe.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3vcbzccot.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lbkuccho.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3npshhsck.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qvmoosxb.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3cuolsldy.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3ypjtwqhc.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3qukdfocl.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3glbgjbky.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3olbdwqgs.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3hpqecapx.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3bhuzwosh.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3weidgaqa.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3cviysoys.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt3iaotnewo.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3boztjmjz.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3nowgenjs.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3kwexgpjj.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3tnwianpm.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt3iwxhkdwe.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3colwtwky.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3ahsbcjcz.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3nyenwbii.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3gpzwtcnc.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3okwludgq.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3dnxoqccy.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3tbdjhprp.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt3snwqesbn.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3iolwkvye.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt3zxxddetm.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt3cujqwncz.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt3favpevia.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt3fxvhdmgc.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt3kywosvfc.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3nzmalaas.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3xvfbrbpi.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3jdnrmybe.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3ibgltlum.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3mvjsuzgs.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3akbnzyyp.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3bsldirgo.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt3ygcrjxlm.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt3whmtdpmj.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3uokvnrtb.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3gttpghvt.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3cnatvqjg.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3eypmofzp.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3hvnfazwz.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3ruqffflb.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt3hpezdulu.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt3pehgvjme.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3pjtxfblu.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt3sjdokmtg.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3xcsyzfto.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3naobsycp.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3mfxcnzuq.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt3glyjmbfr.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt3ugxrakkh.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3lkxhjaov.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt3gbvsbymm.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt3fbdkyyqy.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3hsobqhhl.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt3ssvotuao.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt3apcupozq.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt3ssrszamm.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt3aavytswm.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt3dleuviwt.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt3lilsdnch.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt3blnubpvw.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt3kzdueerw.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3opvneejr.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3bjbfomik.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3eatzuqee.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3lgxkgwsn.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt3rvlgimvi.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt3mpuvpiga.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3sswwozlv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ylxkjmae.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt3gdtquvds.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ijruojdc.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3gcgprkbb.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt3wuugsfvi.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3hlcovzak.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3aiijwivy.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3gwxjqivd.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt3kzivento.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt3lkatdujo.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt3zzhzotgu.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt3bvjtyxna.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt3ubobkely.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3pxsydbxg.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3csitxvts.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt3nynszcxl.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt3uxqyvqyr.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt3nyqhfrkk.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt3dovjfolh.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3nupdrlpl.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt3qflpnkxz.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt3hnihypzi.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt3dgstjlez.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt3ujtcjila.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3lhgmlnlp.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3tgncefyt.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3girbkhiq.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3fovlpdag.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3lzahhlqa.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt3mwysbwef.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt3emuqvjvs.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3mblbgeng.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt3qlwxsdrc.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3qhqncgjv.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3nucnjgcp.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3kumdugky.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt3oocicudd.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt3iuxgthty.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3kbjfyyff.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt3mkiotewk.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt3anhxnhcp.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt3twxsaszw.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3fotxkldf.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3srrqawyi.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3nacbrcac.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt3acdpkfrn.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt3hytpafoj.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt3bitdunpt.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt3mghpvkwt.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt3ubtjahnx.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt3qaqgywtt.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt3cqqnbytr.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt3itirnsti.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt3uesvshhd.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt3ofadkyrf.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt3lwjngzdb.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt3vxrntbeu.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt3plqliwho.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3kxfomjtd.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt3hsyalaxw.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3yowtlkgu.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3lnqxwvqy.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3mqgonrzo.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt3dcdbqcai.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3abmnpfrj.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3kxzdcjjv.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt3huferpwh.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt3vglmgfaq.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt3anjserlv.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt3xoxwccns.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt3sckwqmip.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt3bjihrcxp.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt3hlyscpix.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt3msuhtnsg.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt3pridryfh.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt3llwlynxo.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt3qmigjcct.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt3vjkyjsen.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3cftpecqj.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3yigqxqmp.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt3nbuvbmil.html


<!-- 参考信息 -->