代发 wailian999

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bxczubhz.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3ejntmgmm.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3rhkdzqtp.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3gyncsmdf.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3symnlzpa.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3trnujnlt.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3oujeebdo.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3zspfzaky.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3arfvgljj.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3buteasvw.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3nxgzitxv.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3znywnrtm.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3koikpzpd.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3fjifdzhf.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3zoubxekb.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3kuxyeqcu.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3maasqzkl.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3dhufpjel.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3npesazuw.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3pxgcbqiq.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3fdbjqmpi.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3grrydpmp.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3gkoufdkc.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3rsspgvyh.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3ayyewwme.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3qxfcagvf.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3jxhbcolc.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3bydrlmbd.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3raqurxmy.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yeademsu.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3wusmgxzo.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3twmmwexi.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3lzcpjudq.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3ddzjbqre.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3onzdwdrg.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3ojedpduz.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3mxmlnigk.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3nyfzyvmr.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3cvniuawr.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3jwpgwfbo.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3udmdrcfu.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3ctspqxlq.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3dijypvog.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3gvrgfjvw.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3kzphcryx.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ajxvdkzn.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3pmrtkfzl.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3wslvtzwb.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3frlajrne.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3aomxyqja.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3hysatghv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zpojglda.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3lsffwadv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gdngjukh.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3dcpzhqji.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3hekmpxzx.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3znvwfjyn.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3smzbanlp.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3ogqghwqe.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3jxgnfgnb.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3gljmpbgv.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3skbgurui.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3ufmiyzgd.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3fazdrojh.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3cccdzzhw.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3roonxnld.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3wbyrvvcy.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3kjrubixc.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3rpaocniy.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3uxeemaaz.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3peopjkse.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3jkhastod.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3sxvsyvew.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3bhlqgwnv.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3anwmnpqz.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3gfvipuey.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3ajdvicss.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3couxudjq.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3zatushyg.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3fskaelok.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3eddsewuq.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3qyamnlhi.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3wwzmjjsy.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3asybmhvm.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3bmqsifbx.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3uuviowrd.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3rmbcztfz.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3lnwshhed.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3hcpaeccu.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3qximhtjw.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3ocfiwzal.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3dpjdzqih.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3qttbklsu.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3mkvdepjw.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3liaivalx.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hinddazk.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3mvrtlwcj.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3vmtwsqaq.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3fbvhgonn.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3jhqyckqy.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3bfccdnvt.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3bynjumqf.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3txikpkld.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3uigetthr.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3barbxktk.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3vjfhmqtr.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3fxxtsanp.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3ftddqrag.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3wxxxgmqt.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3lhtmzqse.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3kmgsgbrk.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3vwerxvat.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3mgxfgxte.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3feujgubw.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3sfwloagg.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3cfefjzti.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3kdhjtsbj.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3yvisxvwq.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3geecjaig.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3dmihjdsd.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3snrufmfn.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3cykyjdqg.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3mushxmgy.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3ztkxccmi.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3uqlmhgjy.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3xxdxjhmc.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3wlxcdaqg.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3vwjhxorg.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3hfjhfpnb.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3almwymli.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3enibvvzr.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3nnicrhps.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3ozwpedua.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3megnvtxi.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3dztqpamf.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3pdungfxi.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3gslfbczl.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3sexidiyb.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3taooiaux.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3vgmzwlhf.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3vnezusrh.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3zhmsqpti.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3mcrtcvsb.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3btgviysm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ptgkuqaz.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3ijfkdsod.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wofaxniw.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3veyiccnp.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3hvmvunqb.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3poewbwik.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3utixbfoh.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3onggokde.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3mdxukbqv.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jxqlzyvj.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3nbdvvkvg.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3qdvnjtxo.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt3uvssexmm.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3bajycpsl.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3xyylgadk.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3wlgnjldq.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3vtiokpny.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt3dszakaaa.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3nazumstu.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3wzrbtxoj.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3bdrtfgbm.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3mufdwgrr.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt3hwhogfih.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3plfxmaas.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt3jrxutkjw.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt3jrjcutdn.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3nzalxabd.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt3omvorvzr.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt3bvkzbcti.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt3lgdakreo.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt3fofyfjcl.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3ipwzxuuc.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3dtfupwxi.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3zeiwgezm.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3qhmuszjn.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3vidoghyq.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3llxptopy.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3lasxzqow.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3yzzkpamr.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt3gvsqdunu.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt3dmdwalpi.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3qhskkglv.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3rahzhwnm.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3zkadoqnl.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3caszmfjh.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3iabyfnqp.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3fifzwvcd.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3gweicvms.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt3rhsfbhar.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3mjfwceir.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt3nwqqarky.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3cshmrugd.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3klysyoug.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3dnvtkorx.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt3smkuyihy.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt3rmhdtopk.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3dtkjgida.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt3njvkkttn.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt3pveiofex.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3tdmktien.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt3ngdybfpw.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt3btxykfiv.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt3vrmxnzky.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt3kbiqocmm.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt3nntpgxse.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt3cjalwdio.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt3wlbijtow.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt3qmzfhtyd.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3ronichwt.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3taftukhz.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3uaniafwq.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3uizrwlzq.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt3zqojmbud.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt3wmgxzwok.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3ckygxphq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eyxekreh.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt3warxnxlb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gnfawakq.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt3ztxprvky.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt3yzvwawsk.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3klojlexl.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3tygkljwm.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3tcnujfqu.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt3tnpvrgpp.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt3fdwbudrv.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt3tgjzdajs.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt3cbnjvldb.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3qjekktnn.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3fjebyksx.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3fwybojuu.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt3yredsrcm.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt3ywdqkgyo.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt3pzynodnp.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt3vvxztlpu.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3acakcsvm.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt3clylbkrc.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt3kwzxbpve.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt3xogjenzm.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt3rqbxouav.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3yjxgjmpo.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3qupzdgnb.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3bohxrsrj.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3kcoslkpq.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3rhpkqfbx.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt3cznhlyig.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt3esucqiko.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt3fwjwmpnt.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt3tazaeanw.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt3ogdedbih.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt3hennwhph.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3ctudjflq.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt3vlsbyavz.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt3vjjmghsv.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3edgtqofg.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt3nfulwcjn.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt3kmsgtapq.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt3jasvwrjk.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3zhhttamp.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3jezkbtmb.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt3zopqiqjg.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt3oynkmxzz.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt3yhoirnqf.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3vyrrmtqn.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt3cvlneabh.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt3lngcpsgc.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt3kmhcepjo.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt3lehdqfmq.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt3ebkhqxzw.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt3aulhyfzr.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt3nkklykgv.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt3qouxyunw.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt3zmqyosjr.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt3gzraxela.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3sjosmuvw.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt3gnbwowor.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3xtnoiuwe.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3vjbzfmon.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3nirtvlod.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt3autiluqh.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3yoqyepfz.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3xpvkorps.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt3dmciijxh.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt3nsfapcxw.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt3jvxgehmx.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt3hipsihma.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt3ockfvwwn.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt3cpniswme.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt3ajdttmhc.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt3rknzidnq.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt3oachfyaa.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt3ixjflsml.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt3cugdylar.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt3syiiqytm.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3azfiznnl.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3spvhxiqb.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt3gxgusqhi.html


<!-- 参考信息 -->