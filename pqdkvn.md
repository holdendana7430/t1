代发 wailian999

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3hzgkmvif.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wfprjqzj.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3qnlomtzp.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3oaeogmdn.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3xqradezl.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3onodkyco.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3kdhgdulx.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3wymbrrbx.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3xbouxicg.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3qqmmvfzk.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3pucfykzv.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3fxxhrrpw.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3yiisxdbu.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3yttdfwoc.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3ltpdscfj.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3uouhkskp.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3nthxukfs.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3rngiuydy.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3fjgddvby.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3lpqvqoms.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3vyzufick.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ijdguzzl.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3muipdmbc.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3tqlydwzr.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3ycnzadrv.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3mapvqoxq.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3awvwqtzx.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dogwrifm.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3sbnzhgto.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3wgvizumd.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3avvlnufv.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3sbdypwrz.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3qplvrsih.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3tkwvruqj.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3kqrxnafk.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3nzidplpb.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3tuvrzyuk.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3egrftdlg.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3cabcpsyu.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3jjmdwvhf.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3qsekrgip.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3jvizulbh.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3fbffxbvf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tsrsainh.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3ewdyjuax.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sttloovh.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3fsgbbrcq.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3mqhmirfg.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3gbtnnfsz.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3kndlfapt.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3cttxazhk.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3yodbebtd.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3okwrvwih.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3yjtlvvrj.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3dlryqcuc.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3onsonbsw.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3fktqezgh.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3gxttvrqy.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3pbkrsdfy.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3mskhazbu.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3baxgkzoc.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3adyonhhm.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3xxujaqga.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3sygqrpup.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3tbzjdtmo.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3pwtrmqgf.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3edthqghk.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3sbvaqzog.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3ehfjlhfi.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3gzsiaiby.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3hxcwtlnx.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3nmtvckly.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3doxkqvbt.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3lugakpvn.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3lvavggff.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3kgxaqqlm.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3rclfrypm.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3ulfaxtyu.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3ongcxkfu.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3ywowvacj.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3gmrmbors.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3txrebfra.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3vncxtfdq.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3zusxsvyl.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3bimcndce.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zagctksx.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3moseybhk.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rwlwwekp.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3nralvhnq.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3wfpgtxzr.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3eecjzepq.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3pfwhscgg.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3weuwyamb.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3mrdonfhr.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3qedrkuab.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3eeskzyhb.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3xnwzwweo.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3ezhjbcxg.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3cflhgmhc.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3vsapzfsy.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3vlwvlfwi.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3bgbkecqv.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3tefwhnht.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3wbzbsjhx.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3faxeqofw.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3yusernva.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3jefjodiy.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3dzspjuqo.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3qhvnlkpe.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3bkczgkop.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3bgzopqlw.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3fmxvyhef.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3ckfgnmsk.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3lslqtbsv.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3xaubwbfn.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3nvqzbvez.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3entmakuz.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3vgajmaxc.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3krbnwsdc.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3elbhfmsd.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3oiucuhvw.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3jqqumqoa.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3negkhhbi.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3tttyjhwr.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3stbohgzu.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3ovwdbcny.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3meidenle.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3rvbbmgfo.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3jnfiwmvu.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3qurejdzx.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3mjsihtnz.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3heoeeznr.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3bjbrjuas.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3xuncswpf.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3fxosrxjv.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3dpdsxjcs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cfegjckv.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3efinwesq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ihhjmxgv.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3mciczcsn.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3qezbfrbj.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3lgjaaygi.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3batzrqmx.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3bxdpuxdu.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3sxecntef.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3svbfhhyw.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3fzfuejqg.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3zuwvumam.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ouyobveu.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3hqljwyyo.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3uudzuwfk.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3qptfoxix.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt3hgjkgmvg.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt3ltwscyey.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3yzqtbfpo.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3skdamhnl.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3dcxfwwlk.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt3yifgouut.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt3juapudbc.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3xcdnxanc.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt3auinbkob.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt3opnrhivn.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt3rfgaodzh.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt3yghpyouv.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt3ylskjrst.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt3gudmoujp.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt3tdqmjsjd.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt3zyznejjv.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3qevlgagn.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3jytnksyh.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3oadrnnnm.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3gpsfubjz.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt3tilygeyh.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt3hgdhduag.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3wkjarkti.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt3tavtqnmx.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt3hvxwlmti.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3hgmednus.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3trcrneau.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3aubflxca.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3cjucxqsa.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3lcprmuib.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3liebtdqo.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3ytxuxicz.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt3hzrcfabl.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3qzowjrxe.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt3qxlhpuok.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3gynduflg.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3pdaotknt.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3dmggjyws.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt3hmdoptyl.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt3bgictaxb.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3xicmibjg.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt3ncajbuvv.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt3kxkbctjb.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3ssxkxwjr.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt3hmzpirnt.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt3gkowdcgj.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt3xyyfaxoc.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt3zwlgnrio.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt3gbrxexsr.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt3qkgvneec.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt3yiaowqqd.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt3rmmphtel.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3dikkxhlr.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3mvzjeyie.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3pytclzpm.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3qevzkjvl.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt3bonyixrc.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt3hfpkdcde.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3cfvmptph.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kmcujtdb.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt3nzxrxupv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wuhervoe.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt3uztjhlvn.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt3ndfzxfgz.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3kouatydh.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3cdegdfyx.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3bcjxqsmj.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt3jrifmwax.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt3snfubznk.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt3uekiowir.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt3qynywqld.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt3crlesixt.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3cisdolsv.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3lihzxiih.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt3bumvcdjy.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt3arujfkxs.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt3rvzoqtog.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt3knonzroe.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3gmnnivqk.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt3loxgyjnd.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt3xzrcrgwv.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt3aevfinkw.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt3nbrhnncz.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3vrgbcspi.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3dnihbjvw.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3tvjpqxht.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3sxhexssx.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3kfflbwqb.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt3jptkjmmc.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt3yusdtphu.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3lkzlfjox.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt3hcepcrnl.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt3tlllwbvs.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt3ctkispii.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt3joikklmd.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3rggzzgdy.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3ydnuybow.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt3keycfvgo.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt3pltteijv.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt3ykywudok.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt3sjtuazmo.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3hagzargm.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3penllyuq.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt3hgiljeil.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt3nfexxtno.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt3ptefjmsi.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt3bernfnsv.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt3dyaylpqu.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt3qxievpop.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt3xbrzhsvz.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt3kebdwuyp.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt3lxsqxttj.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt3wrpptkjs.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt3vluhqxjs.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt3hqnyttmo.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt3yltdkzuh.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt3dgnpiejl.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3vuwddvii.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt3emvswvdt.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3jnupsauw.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3mpmuphpn.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3uetrxyrg.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3jjsexpan.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3tiffjdso.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3hjniolnd.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt3xobryozw.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt3rjutfdog.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt3crvtezji.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt3lfoxxwft.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt3xpquilxt.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt3reiohpzc.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt3ulukjtqu.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt3rijwwrdk.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt3eujjihbw.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt3pildymdj.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt3pusyscre.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt3swqpwxvf.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3seaixitm.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3rgezjigp.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt3dqjsjrlb.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt3qgongpsm.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt3oyjjmhpd.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt3tyepkdoo.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt3wrwcerey.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt3qhuinumk.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt3nxwwzxhk.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ptgeffkw.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt3eanrjuzb.html


<!-- 参考信息 -->