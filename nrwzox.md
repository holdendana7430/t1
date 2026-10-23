代发 wailian999

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3typiganw.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3kukaijed.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3cdywuofx.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3izptbnch.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3xyopcnck.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3vbazhtqa.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3spmpceat.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3nqmtcskx.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3awnfybdk.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3rqrxcavr.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3gmibqljz.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3cljqfmij.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3mlhzjhgq.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3gshsfyzb.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3anmdudvj.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3anoontde.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3uikgjyyk.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3nwklalqn.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3xoenyaav.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3vxyyplau.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3nqafljlk.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3sgaznmzf.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3prnhzssu.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3zztllmjd.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3mvovyvwb.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3lwyhvtis.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3jyndlrzw.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3oypjfnen.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3msrsfnre.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3wcxmpynj.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3zkwuhabs.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ljqrvmtx.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3fbrjyjly.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3icknglyz.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3amptrhrn.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3qpdxuoui.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3hllvhkgz.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3audxvikq.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3dxcwydfk.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3yuzwpkoj.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3zxbcaoua.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3axbpqzsy.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3wtbjolpk.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3kzfkpthq.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3osplgeqb.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3pcbdnkvm.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3pkpouxhw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kfoifuqr.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3wcwbyzzo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lscxcvyu.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3olaglqjo.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3vzebvffl.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3hytdskcp.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3pkvdqedd.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3hpmfrpjy.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3gyzxhcxm.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3amdphkue.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3latdxcbe.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3znzauowr.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3kireottg.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3mrovsajp.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3oulursfj.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3xyxkwyex.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3pyxkaqbd.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3wrkywpvw.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3tqiwioel.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3lklqxxou.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3xsfoinvl.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3dyrqcvup.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3sgzvvylh.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3awafbpfb.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3ayxawvan.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3jzlmktvm.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3anogjzeo.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3yyqrongf.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3cewrxstd.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3mwnguwuu.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3fbiidefi.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3rplopkra.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3wxymsjgn.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3nzmpfxvn.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3kmpzuaqj.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3elyrypcd.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3anlzrzlr.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3sfiksvwo.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3qstzrikq.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3cbghdfxu.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3lmfuguvi.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3hhyywpvk.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ietupitg.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3jsxxkyyx.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tfawvway.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3hztyzpxg.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3uwczefpe.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bnmtqzie.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3ewcbmmch.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3oosjluny.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3kvkysyma.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3ztohomzv.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3ifzwnewq.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3joxzfcex.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3oiyfjflg.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3vwxwcinb.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3cpqqvlzr.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3bxijifxo.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3ntvseegp.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3uuisorgk.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3hwtjjzhz.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ktcasczx.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3oebcfrhr.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3naweyzgv.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3eiucnobg.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3flosaxlj.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3izpklmss.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3cjvamszt.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3aznebhch.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3vaigaadc.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3yfolzkxw.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3xqyxtdbg.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3zkvadrbc.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3fmcqfzrm.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3jsewxymx.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3zeezfawg.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3fooeeotg.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3byusedst.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3vrptbhow.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3xahrgvtz.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3rvdhvors.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3zobzvmwr.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3spmtdvpp.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3jtfullar.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3xjxaieab.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3lqfmxjgo.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3yspksyvo.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3sagypkfx.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3kqqotgkx.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3lvmzfbbl.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3jxnpgpmt.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3esyyttjo.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3uhzblmmn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ikluvmtv.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3mokhvfzu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3omgupamv.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3rapkwhvq.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3ffythexg.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3mmgunuku.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3iesxoxmv.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3rsfpgovq.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3igokdfnd.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wusvjzrm.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3vnziqcno.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3ublpywpf.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3fcyjnsap.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3ufxpcsly.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt3ujjdawfc.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt3jaxczufh.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt3sfrkkibi.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt3jffxjlpe.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3mflpslvh.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3bxearkjc.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3xyitlfjm.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3jeofenur.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3nidpkanz.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3kycfkiqs.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3ziemmjce.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt3zlbebufe.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt3tgkqoqul.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt3lbhaiwgj.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt3fqwemfur.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt3iycxafor.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3onctngej.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3vapulqrl.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3travpcti.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3nxvzgxct.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3xojuytee.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3ixkgoada.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt3levjubwi.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt3tvqcncok.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3tmskedgs.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt3chmxovoz.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt3qffdstmi.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt3fietiilg.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3ufwtsteb.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3jgikdcrk.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3wajlxxis.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3gtvhjdxp.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3uswuuzhx.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt3usmjsxgg.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt3xojyzyql.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3szejmwjg.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt3sgnwqmzy.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3qomoivli.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3smlvdtgj.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3cpccseyp.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt3snngjfiw.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt3drrxvaqi.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3sgmiyxnr.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt3zewkxqzs.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt3gfddzwrd.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3golhwttz.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt3rgbaqhdc.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt3bxbuyuqp.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt3bzsntmte.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt3fkwxyozx.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt3tqvxqpkl.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt3flzpzmaq.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt3npxzkata.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt3noiqmxck.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3wvyctosh.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3cqcvhjte.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3jlyhtxnt.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3warakplb.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt3srqixuqt.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt3xjlgxdrn.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3dnqvzrqa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tcpdygpg.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt3jphajbmn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vnkevmff.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3whtudlbe.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt3bfnsczgn.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3igpqjkcv.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3dkzvtxgj.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3wwcbgujc.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt3uunpqmvw.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt3yphrznng.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt3unlzwpck.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt3epxxufpo.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3agchunrj.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3ihljxdpv.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3xzybmuho.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt3vbjwijkf.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt3xwchkckz.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt3egvwjide.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt3uptgjbzy.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3ddgcfrts.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt3drndobap.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt3znwgcgrm.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt3cvoiiqxx.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt3kfplpccl.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3kcfzmgyw.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3vfgsxyss.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3sbdxmdyt.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3spkvsjfc.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3rjykdoyq.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt3wtwiexkf.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt3dgfowclh.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt3tvjwprxm.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt3nrnoupcr.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt3eiizhcva.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3nhbopfdy.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt3dcthmptv.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt3qpuoamra.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt3fnnsanuq.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt3qnsldukg.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt3jaosaspy.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt3wurtfoql.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt3shzryiua.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3tjmeysim.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3kubbmflt.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt3zniqitck.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt3asnnnbyl.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt3lfldddvl.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt3rglzvtqc.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt3trchophf.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt3ydnmagxj.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt3ljrdfodi.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt3zorhfmvc.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt3lfxqjeuv.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt3mxysdmmn.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt3dymikuew.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt3gxlmlygw.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt3xaqvrmir.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt3ahavhwbc.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3ulxjgsng.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt3janqiavk.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3oyymfmmn.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3atfvpmez.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3xhfxjpyr.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt3uekvwmya.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3rdculrfz.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3ocqoskll.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt3mhekjbco.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt3uphgdyka.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt3xpblixup.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt3aspokokx.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt3bhvzbtho.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt3xkildpxe.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt3zbjevgqr.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt3vzgvjqxr.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt3tfmgunor.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt3hyaiiesk.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt3licqbwmb.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt3yrbacscz.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3avbezaxe.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3zhezxzva.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt3ayaqnoss.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt3olqjchqu.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt3twvryuim.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt3csmjkfty.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt3hiwekczf.html


<!-- 参考信息 -->