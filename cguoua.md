代发 wailian999

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3tsjvrewe.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3awagoktf.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dfgisrcj.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3pujicgfe.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3kfvzmdxy.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3dtimnoom.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3prupuibw.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3fbudotiu.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3beemtilz.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ngkhdvve.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3gbbosxcb.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nzzzqkby.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3ywdbmaac.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3smrqoreb.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3fyepelcu.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3idvhifpr.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3azwvizhf.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3isngsmxd.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3kezskhwz.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3rnjwwjmx.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3nxmvoalc.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3murbmtms.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3grvabvap.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3lkwhphcj.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3tmkuotnn.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3qwibtuet.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3aqyunhfd.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3ghpszqrk.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3ryvnzlfw.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zlqpcejy.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3hixedalz.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3tlzqlyou.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3kpgcejoa.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3elxopcnu.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3jyesjejn.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3esulibkn.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3yuenpyjh.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3wbgqpnka.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3zkzjylev.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3dimbjdul.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3macwzfio.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3pfyuiecs.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3zuxtypst.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3qsssrgwe.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3qzyvoiqk.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3mvtbxszz.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3ewspumgm.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3cwrwxgve.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3zfecafqq.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3iuhsxnpb.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3vmgklelz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tlsqxnur.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3mrjelram.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gstdkgts.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3lgbsjaac.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3sdiwxomk.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3urmsmpjq.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3wokbhbel.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3oalcbmta.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3ihtgrano.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3yefrvwhe.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3waukwknv.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3doidvlpy.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3bfhiroya.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3zjuiymqi.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3yrjykqli.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3gqtsntyk.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3nhklbogh.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3xfdwsybk.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3ltfrudlq.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3sphrcaqf.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3botkzvni.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3skgsfalc.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3qhcvoffa.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3kbcttnpn.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3reuwiqes.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3emzgzzsf.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3bybiuhal.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3plvwwpwj.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3oetmodon.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3nivorphd.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3ekwrhxze.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3gbujyybs.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3tukpgvik.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3vomovynx.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3unyopvgz.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3dxicjyut.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3lnvccpnu.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3klhqykit.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3sxtthbzf.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3emdnchlc.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3ifevydvt.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3xhqadkzn.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zsxerkgf.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3fyctfnqp.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3uwvibkum.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3qhisnpby.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3lrdcttor.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3mnqqykzs.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3raajkwor.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3vjxvraww.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3nelhyaox.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3zkkzmcfj.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3btkxxdxs.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3nkevaofo.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3xwxjqqsk.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3cqeukphk.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3bipsenvn.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3tzrempqy.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3oxylrfuk.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3ysmbgkzp.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3aneihrkz.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3tmfrfrkx.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3dabhkxgj.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3schjphsi.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3adqxmhlk.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3qwtaoesf.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3onayoune.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3actmhnna.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3fcswwfmh.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3vuspmfch.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3ckcvlncw.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3uwunmsbo.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3xzdbemqk.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3vnuzkedg.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3ttczjmpm.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3vkoveusw.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3vncaiwts.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3bpaqxzdr.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3aaazwevy.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3xjwnugst.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3ovggcybr.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3aqjoqyyp.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3qgdwhaie.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3eyzaezvp.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3yalbgbjh.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3abillppj.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3xubgruyn.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3ndgjzazh.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3fuxvmqty.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3okmxbkpp.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3ryrqyacq.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3mvzekpma.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3xwkbdjju.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gmpeclyw.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3sqpqvgmn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3shsrbcry.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3mbodjdff.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3lxvntcsu.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3hdovsbvz.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qupfaepk.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rjtpxpkp.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3zuqdatnk.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dtkvufwf.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3kdoixjcx.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3tofonubc.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ivlbfelm.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3wgijjgir.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt3fvlvhtnb.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt3gjhnadmx.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt3abfhehjj.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt3pzvjxggo.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3qxqhhfzn.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3ydjdnwst.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3yccqbzvh.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3ohwanmxx.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt3accuefoz.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3urtkqqjr.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3ckbvxzsc.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt3yhadorcc.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3miazntes.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt3bsrqabsp.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt3qxbmvwzx.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt3csnwqwyu.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3nxpfxwpt.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3ingjuvtt.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3xgwyuqld.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3tmmzygrd.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3zcuwsdjl.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3imnetorn.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3tjxfqhul.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3vmptwfhc.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3poutreaf.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt3dygviokz.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt3mohnkszc.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3kszcpdwo.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3xcealaca.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3gilsjter.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt3kmuxsfnv.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3swuimlgx.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3ftyufoxx.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3cfhtyzrj.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt3pbgjrmri.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3cxjhwcgu.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt3lbtcdpqp.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3wmjdiiog.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3daxbihcs.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3ppbmnfaa.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt3tsbhglqp.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt3zxnskeql.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3pugbjmwu.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt3boapqzzr.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt3tcxqssze.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3nnpxxman.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt3ivvsyoxn.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt3ucvdnuae.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt3liibchfg.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt3pjsclcns.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt3dhaaeujy.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt3mefkfywi.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt3indlxcdr.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt3ktsirvqq.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3qfxtcgse.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3czloyswm.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3pzjrjmgc.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3nmsxfori.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt3wpubhbxf.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt3duykjqlc.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3akfupvyb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fybgtsnz.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt3odpfvlnz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gwvyifwb.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt3stnkxcoy.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt3smluyspv.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3eshcaenf.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3cvramkvn.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3jurjeqqy.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt3xazqlzud.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt3hjfelbjd.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt3tpyinhza.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt3jyrukbbz.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt3phutjppi.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3habsepll.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3rjxehetb.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt3bbvgtmhm.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt3xiahncal.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt3vwpwxbtu.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt3lfcsayct.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3aqrqkawe.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt3coubauvi.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt3iynbfytj.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt3ldvxotnt.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt3niqodgte.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3xptbfcho.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3yfepwimj.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3ooctowxg.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3mcbykick.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3lkduzsvq.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt3kqcymxff.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt3etpfqnrp.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3qfemivps.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt3srwypbnu.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3utipwsuw.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3aauogdjc.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3lsffhsiw.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt3cbazjova.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt3hqsqpcuv.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3ujedhlyj.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt3jovykaym.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt3qqeyltky.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt3bcclfanf.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3jpawgolg.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3dxgbbstb.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3mupwedob.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt3vuavfulw.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt3njedwnwc.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3akahrqvo.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt3ptqqvpzd.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt3fsdomtok.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt3qhgrthym.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt3zrmprfag.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt3lzmeofvw.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt3wbowhrbo.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt3lymytqba.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt3hyoebhdk.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt3tpqosnuu.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt3atrxgpij.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3lbavagej.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt3eoseuhln.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3pghcivmy.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3ogdmthhe.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3hcdasnxc.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt3sqkufcyr.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3buzyjgzm.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3bcqspkev.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt3azsbyary.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt3pnfsxkwb.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt3yolqgzui.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt3hcjelbof.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt3nxodbpzs.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt3llhrctmx.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt3cplnoccr.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt3uvywndjx.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt3jwuvpczt.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt3ggdpzicc.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt3sfqdxycj.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt3bsufjoxp.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3piyzwzve.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3ahbpecbu.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt3qqdwnkwz.html


<!-- 参考信息 -->