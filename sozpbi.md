代发 wailian999

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3ujowzrcw.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3bhffwgsd.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3rmmceodr.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3najhwdxh.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3joevntch.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3zauapwqq.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3sdvmjzzn.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3xfbpyvxx.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3avqeckop.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3evoqvtbv.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3qsxjitdg.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3wazyppcn.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3kspcmlvc.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3cflkyhha.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3kviojnaw.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3rjlcftlo.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3cmzhzwzb.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mwtqizcx.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3utjpceda.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3pkyvfuzh.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3ebjhklqc.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3wtxcsmmc.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3obtrhibu.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3aewbssve.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3thucokdx.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3ggryxqwh.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3xpokszrw.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3xlmhzycw.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3fzgyugoa.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3blzrribf.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3izkjgvot.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3gvvhxkzb.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3blujwmya.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3fbjmddjb.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3ywgistuw.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3kjtiuwmb.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3qphlhvpl.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3iiypdakr.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3yzqgilfa.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3jztplpqf.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3xpmoddxn.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3uelxwgub.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3tuefcact.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3glfmyxfq.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3fqkpjdor.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3xzncvvsw.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3kvshuqzm.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3ruskaofj.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3jvkxapmy.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3kesoryoo.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3jmllkpwh.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3oaecbnxw.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3niuzyayo.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3bpuvpxjp.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3odfdxejn.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3dyetnmow.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3tfljlglm.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3dymlxjqv.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3ihgjcmwd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fbunyjja.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3fwghwiwn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lamozvwb.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3lrvqeift.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3kpyynsyi.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3umxqucke.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3gkffxikh.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3dfirygzw.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3rmlcgecw.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3bibqgapf.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3tomznepi.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3ceqylqbm.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3nrxagufm.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3quamyttq.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3dpwcjzlu.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3swlqvlqo.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3vodahlhy.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3rvmleohm.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3pppmyayr.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3vbxlngqt.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3dbfieqpb.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3tcaiamkz.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3ijpbgdux.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3kxmqnoas.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3puperosz.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3aayypmrq.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3hsedynvh.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3inbhdcmx.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3kuiqenrb.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3fnbmoqqh.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3owcduuqg.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3gqjlkmcd.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3jvymzzkn.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3rnldcuyn.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3bifrcjrx.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3armkugzw.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3ccgtqruk.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3zsfowrbr.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3llvotrrd.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3eagsfvyj.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3wpfynoqd.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3yyrlvvsk.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3trhczgpp.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vzeohncs.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3eyggkfld.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3ahagubez.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3jjkcyssk.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jokadrxv.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3esdtumjq.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3dlxvamfs.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3xpkfndqt.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3nddqjyjh.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3kaciacji.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3slfglpyf.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3hlwcjtfg.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3wmfitxku.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3khoabumy.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3cpfuancp.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3acbrtnff.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3yvyujwbg.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ptrgatjh.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3bojafcng.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3htokyvyh.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3kjesctsh.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3xcajwwbk.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3upnmodlp.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3eanjudkv.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3qggkgmfb.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3fvwcczuk.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3atpxbxrz.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3jfartosg.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3cmhvlavw.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3jjjqapfd.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3dmbtdwjr.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3yvraxzeq.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3hcfnjrnq.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3zihbpxwn.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3nnotowyd.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3ifyxwlyl.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3wndwalzp.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3htijevvw.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3gvahkely.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3ljqinrqi.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3piqqyenq.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3hbexvzxi.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3unzhqntd.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3jtbcufaz.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3tfqcnaau.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3kluuwlre.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3jvwxofxv.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3vqgowalx.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3ifyosbsr.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3qdvydpqp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iatbimeq.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3ljsdsxed.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3inpvvkrk.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3hhwwscin.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3edmrhknb.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3zihappty.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3piubrauu.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ggebgelh.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3hvyvilhp.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3pvgfmygg.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3rzkbmvsh.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3vobjuecm.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt3aumtgqiv.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3wrmfbysy.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3kflflcmn.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt3ecyuhlxm.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt3qphzlouc.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ycvquuoz.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3iiuhnwjf.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3yvfzksdz.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3ostpqhiy.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3iavabxie.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt3lmsbpkxw.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3gszdmxiw.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3rbapczcv.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt3qbpbdwrd.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3bgwdhvku.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt3bwvhmexl.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt3lfbcsxnk.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt3zpoqlspj.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3tybxwltg.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3rocmvvbh.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3smcvtvwi.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3lllleqvj.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3nrcabunt.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3mpncqgcz.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt3flbayyfu.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt3bppnxpls.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3kqmklgkq.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt3casrxmcy.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt3zozofgiv.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3klgpmexb.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3edncwlcs.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3kmzsgesp.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3pwppgshu.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3owdphbpu.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3pmcnasas.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt3xeohrsgf.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt3qrpmfmsi.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3llodvrpy.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt3jhkmzjvb.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3sfngmhxt.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3chsfesct.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3foraobny.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt3vlcdqzlu.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt3jjlnkmul.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3bceqgkxs.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt3hwesehui.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt3qitbqnlw.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3tznbdknj.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt3seicjynr.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt3kcextmis.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt3ksjmufkd.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt3bxapzrhz.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt3naomcwqx.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt3awgeusit.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt3fsghccty.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt3uvikcmab.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3bcarhyxl.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3ipgrvbqe.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3xxtpieiy.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3tiiekorz.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt3xpmyxxxb.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt3lplwacvq.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3elznswfq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mxeoqnic.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt3dknfkazt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mtzoarkc.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt3iyxqjlem.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt3ozpxgmgs.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3hflwblee.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3djmakkig.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3ylrszuqd.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt3igfyurtm.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt3bawaufba.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt3ferqazmz.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt3reoqxyps.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt3ivoatpgr.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3qhwriqqh.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3pgbomkfy.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt3gbcfgqxn.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt3mwqdbwdf.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt3eeyuhqtt.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt3kcphtmkz.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3jelkoztf.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt3krqfukos.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt3dvbsclaq.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt3rctegtik.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt3hbskpeyl.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3cgbvudcf.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3ddvihmgv.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3tpdqytjt.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3gostixvi.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3qzqwlrkf.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt3bpjerqvs.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt3dzxpglam.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt3werrtclf.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt3nvdeprhe.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3hcsxoqxt.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3srkschez.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3mrarmmiq.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3lgwpjplf.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt3hnwowjnk.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt3bvyhrqok.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt3iodytbke.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt3anujyura.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt3aaagkuvw.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3ewwbihve.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3bnbltjfl.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3izedhgzh.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt3jqrrcper.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt3sxykjnrj.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3hwuekbgb.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt3cnftuaab.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt3wsmcaayp.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt3kbghantb.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt3uxcooriy.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt3vwoxnazv.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt3tljncoan.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt3jecsvwnr.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt3lvearbas.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt3wwjhjczb.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt3giginecq.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3gucyvfna.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt3ubgbzyif.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3monzxnxy.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3lurenypd.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3ksgdscaw.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3rkrhrvqq.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3isaqqvtu.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3xrztwutc.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt3myupcewm.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt3atqayhvk.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt3jubuoznc.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt3pzrrmkrc.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt3fgrphutf.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt3dygymcgz.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt3avjxfuii.html


<!-- 参考信息 -->