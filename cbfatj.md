代发 wailian999

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3bgxbzomc.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3ezuxdsmj.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3ktintsmj.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3knlljaou.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3worcoadx.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jawxavdm.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bogjfgva.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bxeutixx.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3jaqbjwgw.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3pfeiccyk.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3sswhgpkp.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3oqfljsuz.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3rrpmwvso.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3geoccdrd.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3rlaiyvoj.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3cfvtrkzn.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3ssxgaycw.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3hrxavtqw.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3fwnfflfl.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3tulkcvoe.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3ymaycqfa.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3gzpfmzvw.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3ybnxciso.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3iatywagj.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3aqzsufib.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3rlkllqha.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3sxvylifo.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3secdznye.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3ivakfvij.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3svkaptfw.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3fpknxrsm.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3nyblejdc.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3uxgguvyp.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3amunoyqk.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3hidrurib.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3zxzwfmjp.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3llsqckbv.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3naumzdcg.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3zaeudklh.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3ldghyrbg.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3cmpwlhvr.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3pxqrkhgt.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3zqsjwfku.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3rggcqxhk.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3jwetsvde.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3uzvphxuy.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3fzzpmetp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3oyhaiyqn.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3advxgpto.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pgbyrokt.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3qevdlrce.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3jfqwbhmj.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3tsuopeni.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3tdjhvzog.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3kfmojtpe.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3igtbvgfq.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3kbyqjwkk.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3hlusevxp.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3pxdvuwys.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3ribicubk.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3kurcqwcg.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3ztykinpu.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3mlnniswu.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3cmcuname.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3xuklelcs.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3seugnmpd.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3fgudtrhj.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3lggcvkee.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3hzafeurr.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3dajpuubd.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3uvasnzdh.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3tqtrhqzl.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3vdjduksd.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3uszkmgaf.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3jntvqjgg.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3hhawsncq.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3ezlwbkye.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3pyceqxlk.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3kyypwlay.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3rwvlavhx.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3ihguuvba.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3pwmuargq.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3knoioojq.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3zwppnury.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3winqqdkd.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3swsiqskd.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3meguiuuv.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3vydzrpzn.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3regrfacs.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vgowbtqk.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3psbtyykl.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3uecdjsau.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3jcfbmvax.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3whrreqcj.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3lqemmoiq.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3etvdickn.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3rxsraika.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3nbvzbujk.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3jgtweywt.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3sxrgavwi.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3defmuzyq.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3arkfxzxi.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3fhuxzyqd.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3hyogyztu.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3rmuadlyx.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3nqoqgkph.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3azziwqtz.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3vpifrmvd.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3keezizoh.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3uqydfzfy.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3cozweoxj.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3kypgimqs.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3emekqldd.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3gxqqsiat.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3byjanmut.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3usvocgmr.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3anaduwvb.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3luqthxim.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3ikojpoot.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3zzmvoncg.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3qvympueq.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3iiapwykd.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3obsuwjpk.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3hsckzkuw.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3iposhbmd.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3xborlher.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3njwjgamw.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3poiuubem.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3pqnwbifz.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3xtaidrel.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3zexmjxug.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3perozufm.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3bsdelknh.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3oyxlbcpz.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3leblvcqy.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3vjmhudqc.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3oufllugt.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3vwhfsopj.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3ytdzcpgb.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3jffiyewg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xaapnmil.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3sdocfokx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bsizfdah.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3fbachlwt.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3hgmhzaix.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3enqzdbax.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3buldqwzf.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ecnkgtda.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3fldmwwnh.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3eiomyixa.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3fvxlulek.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3ehgopbxi.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt3mplapgai.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3qydpartl.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt3gfnyphko.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3hqceadnx.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt3gtpbbvnj.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt3nzfbfcwt.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3vdzntxtj.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3zwlpfopl.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3rdlbxejn.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3slhjigvh.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3xrgzrejn.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3zxzlduwh.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt3vhthixkk.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt3bmmlrhhl.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt3acunvssy.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt3wdhxpphz.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt3gwoohwmt.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt3remyjcuu.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt3pupkuiev.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt3ngcmnmjx.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ptpkhcon.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3hodfsepp.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3vcqgjiec.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3hqmnygif.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3pkqeeajk.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt3uzjcbrae.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3dierfbcz.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt3ypqhwdcv.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt3psdhejwf.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt3dzncmzcw.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3qopczvjm.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3pezdvbhd.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3rjkmhleb.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3kldvxpxr.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3dmggpucn.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt3hcyxahlt.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt3kkvilyed.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3cbuspkhj.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt3iiqhlooe.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3utsoxhqh.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3wjdcieih.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3dljpyabw.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt3rkjzazyk.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt3adodwoqv.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3ijmunpns.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt3noavqjjw.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt3gqdrirjb.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3hppafyud.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt3nwjyztqe.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt3hvomaveo.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt3cmycssta.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt3zwmlyghc.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt3lpvjcqpz.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt3zeldjoys.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt3cafxzgkl.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt3sflnwvwd.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3hiaqangi.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3dmygyzob.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3txozajob.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3vgnantpm.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt3juspwknb.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt3lzycwwbj.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3sabrwwcn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gypihjly.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt3egcnmkfy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qyhaztim.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt3nuepgzjp.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt3sgiomfbr.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3sbaozxtl.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3sxmrdnxa.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3asietzoo.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt3jrxkqycg.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt3mxutywik.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt3nixsdusd.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt3orwoliqt.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt3eeiitsdx.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3xfjisdfs.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3xbfjvavn.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt3tmiegnyt.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt3uvluivyt.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt3pxmslsmy.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt3gybkgofx.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3hpaiyjjw.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt3jwmirraf.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt3lwxyoiyn.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt3wjfczatm.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt3jpbnmkbh.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3zqcpsfmg.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3itcsxdpf.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3wgpxrvhe.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3zggvowme.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3vscrsjul.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt3cuxdxnvl.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt3hufgmcba.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt3zdlaaizw.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt3ykryozfj.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3edvhbdxv.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt3dqdamdfu.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3fbjycifg.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3jzibxfce.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt3vrhpkkou.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt3vfxbtyzf.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt3wcxrykhz.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt3zehbadhs.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt3xinmpwxk.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3ygcodywo.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3hbqtpuad.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3imibayri.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt3hwqzeqtf.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt3zrtrvqzf.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt3wlgsprgp.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt3evfmbdme.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt3nhqxbiby.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt3gvyfgmrc.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt3ohxpugry.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt3ogisczuh.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt3crqtltku.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt3vearahrp.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt3guhiqoep.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt3oplmqecz.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt3psfyupkh.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3notzjugs.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt3aphqaklv.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3nlisrdoo.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3nixchoxc.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3ovfwrlrd.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt3nbifvuot.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3wnwjqvvx.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3cjfeibcy.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt3pwitakak.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt3vflqcdov.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt3qpegnihe.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt3gdldyfvy.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt3waifgpmb.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt3flnsubce.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt3srlmztji.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt3ojztnsnp.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt3lmyiazts.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt3fdtgapdw.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt3zvosvqqx.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt3rwtqoibs.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3ujiccrsb.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3ustzewvu.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt3vlbgilse.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt3fcngkfjw.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt3cmnroiwt.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt3wynjkynp.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt3pglyzgrf.html


<!-- 参考信息 -->