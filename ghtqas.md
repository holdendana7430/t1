代发 wailian999

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3ygaiytse.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3vblwiorp.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3dncwgsgp.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3khaiovhx.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zzllvfxt.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3seqegfwl.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ncqwlbcj.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3ufjafthm.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3tcqptbhl.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3aslpqugg.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3tjnbfdqz.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3dczrwizo.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hsblgyug.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ikfbrjsj.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3bexsomtl.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3icktiqnf.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3nxxiikyd.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3crqcvdmb.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3swnxamnp.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3wlmmixde.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3twwzejmx.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3eyyqfohs.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3mvqbitit.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3xwqrzcib.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3bkiloxnq.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3uxzoawcq.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3etlwodnu.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3wekvmwle.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3rphohgmj.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3wszkcjrs.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3bfpgwsaf.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3sljuatkz.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3grjrwrrb.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3bnxqmzhu.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3mqqqwifg.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3fqvvfyju.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3uaetpvan.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3dawhxfkq.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3gcctlccv.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ikwzelfv.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3gocmdswd.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3zccwwbkt.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3lhxlphru.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3wxhvftlh.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3vhzlrnhv.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3lqobbond.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3rdodjgqr.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3xgligdtt.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3oddpraod.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3obkgjlko.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3xrwgsfii.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3iwllwlxz.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3adzlipuq.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3dpabwbwj.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3fslclchf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mxwhrfbl.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3soucfgkt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3oudxlblx.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3tsfajmzk.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3bhiqgjda.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3vmdkpkaj.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3kumjkmsk.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3wbgtboew.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3wmgcdpkz.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3xlkqdvis.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3qcxgqfoe.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3yvvbnhgy.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3hjnhzwwz.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3odgtzfgs.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ylvliirq.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3pqsbhtcb.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3csjqdcoc.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3qabeeipq.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3razqiplt.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3vjvczjdj.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3nyaqbuxg.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3texatqqk.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3gpqylfgt.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3rzyqdaec.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3wuyntrci.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3rikdzppu.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3zlbyiryn.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3nprexioj.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3vguzyqli.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3qhalksey.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3vtbrbggx.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3oygfemfx.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3tweuhsoa.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3xpnfwuak.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3qugphiem.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3bvubxvkh.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3zskmhoys.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3rrkyycbq.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3jeriuvak.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3wbbkweai.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3uousadvp.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3jibltbzk.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vrbidlln.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3lbjvgztg.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3iflxrkot.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3hquuzuiu.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3cbxhpstg.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3xzthnqoo.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3ysdmkvli.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3giilpwar.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3dzjadqgf.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3ptswoiqk.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3uzgpchzm.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3iflbtvaa.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3uoxwbnha.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3eofvcylq.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3cshdfygm.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3atxyjvdy.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3efialcad.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3juomqmfk.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3civatuir.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3hevyhyjg.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3dkdbkhqu.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3oeframlq.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3dqdpkjzs.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3mfjnbzit.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3hbyeobsd.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3npdyvtri.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3omjxqvxg.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3adqjaakd.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3wzfgguoy.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3guvgdeyk.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3fcdivjfl.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3jamgfqvv.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3uzqkxxvu.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3mdavmprk.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3dnxstpki.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3gckngvmp.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3azdsrndg.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3ohemmcjm.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3kwxjqmdl.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3kcsdawjt.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3zdrtqzjo.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3yzjbqedi.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3jqqrosim.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3tgznhzom.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3vjdjrchr.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3ojrfwjcv.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3pajudefu.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3dkmjvqsv.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3wzntmveu.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3mqmmbfak.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3fawqekys.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mqgvkgmu.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3zyifmkfl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pxonoqyw.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ktmlhlhm.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3fkiboehy.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3pueppmce.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vyawzqxl.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3splzgzyd.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3xxkymfvo.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3urviojsa.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3ofzaxufs.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3giyttpdp.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3mrpstgdh.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3hraxzkdz.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt3kznzovzh.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt3hzasvtpt.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt3snvluulp.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt3byrmceij.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3mnyymzky.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3wcqskvso.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3piqzfucj.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt3ugdrqeji.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3cvcekhvs.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3hnkektla.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt3aiskclwy.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt3eabxayfe.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3qqzioktk.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt3kovmlmbr.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt3jbrodfha.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt3ppdzyfgt.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3scepizfc.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt3tkumcddr.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3dlrcdklf.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3yinswyxs.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3racsdwfh.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3ecwnhtor.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3fqvkjczj.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt3tciphrqv.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3qfxvkrco.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt3auebcder.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt3layrbxgp.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt3myapcjnh.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3lvcarqzj.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3vqqirayz.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt3oywpmwot.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3utndipjj.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3cokwtwoy.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3hryisrsx.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt3mmjcmfbx.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3fccyrvmc.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt3oefcwage.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3uxpyudyp.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3opffygdx.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3ssobidlg.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt3vszpfzec.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt3fhbzypef.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3yytnpcyy.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt3dquymufk.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt3mgwritji.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3qqoguhxe.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt3halxqmkg.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt3uxxomavg.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt3ylwsnzjc.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt3cqaygoon.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt3liotbvih.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt3ucdiwegs.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt3fvqayihw.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt3xbhvlwkx.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3twuftrrq.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3qlhhfvye.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3pxoqqqxt.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3yekdbllt.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt3yfhccvqi.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt3rsmckyun.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3mzfihnce.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zdxkukgx.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt3lflzbtii.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3smsniyvj.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt3udwimhgz.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt3uoofhldi.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3ybbauvak.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3sivnvgda.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3ojtqugzt.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt3oapzlgnz.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt3vibtblqt.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt3rehqxjle.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt3emuwyicq.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3hwcovkmn.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3cxfmgcfz.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3ahlzvdar.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt3qlzjfutx.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt3ruqbehde.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt3qqifxmyf.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt3ojltrcwx.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3nwgahqyl.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt3espmigvj.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt3ytqjrgit.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt3uyfzogzn.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt3limhgtni.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3bwttpzxu.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3vlkvmpvp.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3tkxxjzfa.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3gcooqyiw.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3xdzpgpyi.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt3ivvaoanh.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt3gzkqdytx.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt3jnvfqrdy.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt3sajujefy.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt3lrfyekte.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt3quvvevxj.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt3rhbfbzgl.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3pdiyqqbc.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3atvgzotz.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt3doemzjal.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt3lepcfroq.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt3vpfsoaxi.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt3qonlirrr.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3nutntaxt.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3bfvtoyqg.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3gisxfbyq.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt3rtagyuot.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt3lzrenugg.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3qsoohtrh.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt3mghsxvdk.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt3dvtvdupk.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt3qmcllqbs.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt3rrouozbp.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt3nwoiiaks.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt3ceiywoux.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt3rbicqpjf.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt3unrpkzrz.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt3jcdwhltf.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt3ojvcrevr.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3cmyfqrdr.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt3zuijbpfj.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3gfvmyxjd.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3hbygijsk.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt3wmfnzolx.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt3garlbqdl.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3pgqowiml.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3qyaiegpx.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt3ropafnpj.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt3xuybuita.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt3icegklss.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt3ydgsuuls.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt3mzcxerbu.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt3nxdeezxh.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt3zirvbjcb.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt3qsndywnx.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt3lkiamrqn.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt3bitiprwu.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt3pihzginy.html


<!-- 参考信息 -->