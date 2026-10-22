代发 wailian999

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2ozdyjbqx.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2odvouryz.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2xrjcznpd.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2wjtottjs.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2lmiccsiy.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2zzqmueak.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2uclkarxk.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2wglkejgq.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2qthbcyts.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2dcjggerm.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2srytwpaq.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2vhfutndg.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2pknrxecw.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jzawrgwo.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qahzchlv.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2bobmbdof.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2slcsxnxq.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2edzambnp.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2rpiqdosi.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2nyrtarbw.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fgxuejrt.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2umxgvqkt.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vsrckjii.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2zmpjfdnm.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2kgikryux.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2qibmrtab.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2ybrgvkit.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2kuvkizkq.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2vgbudnpc.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2wboobzhh.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2uyphnoio.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2akiprbqg.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2kajvdumx.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2dtkjdkic.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2ydgikeee.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2aiwmsuga.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2wrvixqsw.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2xmhsdows.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2njgmtehi.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2zvfheexp.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2luskhknf.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2asftrcjl.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2amkwfbku.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2hlkxbcgi.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2kvajeuie.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2pvvugqtc.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2jzepbyxb.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bvolcsrw.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2nglinoox.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2xrqdpzst.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2aatbjflt.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2xpaobjeq.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2lpvqngoy.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2synlsyht.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2zdicpqkk.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2grnrgnzi.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2hglrvodu.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2utivsxke.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2jkcxmbfx.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2ucdifaxr.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2hjepyojo.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2rtdvviqu.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2ifabnbua.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2idqyfqle.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2amcdjmbg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uqntinut.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2xbvjpwex.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2ubukcrei.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2bdqewplw.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2isegmnjp.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2xcgawcew.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2brmelciz.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2qlbatrsa.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2yslzkoiy.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2audjekzo.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2gckgpmwd.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2djgxfmrt.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2mlispbdf.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2yqxjzaji.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2xnyrqnrx.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ovjblfid.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2pdfoamiq.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2fcdnkrfh.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2dsodhsmp.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2hgjggxhq.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2xoxjqiwz.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2kezzohrv.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2aybfeqwo.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2udjzvkeg.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2xztxbffq.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2vuvndpes.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2ydqwgkob.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2egnsobba.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2rharwref.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2uisgfxeo.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2azssgfwz.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2sdiebreo.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2zwcrxwjy.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2jiqggjri.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2nomabcnb.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2chqopcsj.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2ijsawhwb.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2elzveuba.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2brsqcxxi.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2lppmdumq.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2oxbubauf.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2hmowrpit.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2ualydiry.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2punwzoer.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2secykacq.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kfrriysg.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2wcqmooys.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2egdubezk.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2chxhwauc.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2anlgpuft.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2adfoynhf.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2zqfiifbm.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2cttrrxlb.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2bfjygpbm.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2wmldhwio.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2xhliyvft.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2qjltiehm.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2hajzllgb.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2tisekacs.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2itpwzqcc.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2gpydvwti.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2dzmlfrpc.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2dgnjszmf.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2impqjosj.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2lrsdvbog.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2vnkjcftj.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2bzqzixmh.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2arxjqfse.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2utahuman.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2igwwylsa.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2fdcqqunt.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2nerbsvhn.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2dvijrlae.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2nkrxzslx.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2uddilafj.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2yjclqysv.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2oegbuind.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2qrtalkdv.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2sunehfsy.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2xjvzehkz.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2svgfelam.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2ysugufdg.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2gzwabnhk.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2kmdzcyxs.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2ppovohpg.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2ikzcbfuz.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2pyvdurbv.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2tmgouuxl.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2kvvpocjm.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2uwiphnxv.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2czxanrsc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2opaqvdpm.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2fuhburph.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zodfoykc.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2xspdjale.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2erqwifjt.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2tgdtsdjg.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2ousftkrx.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2itqufkux.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2pospyrey.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2vpyfoiph.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2jwktfozc.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2nhwodixu.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2taimpjjj.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2trpfxvlt.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2mtgzuypf.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2ltvbwinv.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2eiosawya.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2omwtidtl.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2phivzecj.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2uixezrmm.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2urlwyvvj.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2fhxwysed.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2iyegxtde.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2mgyzxvxg.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2rxxcsrpm.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2eorrkgbg.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2jmyznzxz.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2hsxirwiv.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2ogejixkr.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2ykdjgann.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2koirsnfn.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2ctnnmtyg.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2nkrnxuxa.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2mknpvwim.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2awcuumzr.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2xueefeva.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2zznrfzfl.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2mghlworq.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2tywiuzgd.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt2lnjwiizr.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt2tzxvzztr.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt2ruspivug.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2smzzdqvm.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2lpyrqgqm.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2vokixwey.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2hqnyhcku.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2ogjcwnyr.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2vhfmpeyf.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt2dhuuwxbn.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2hcbzeyjo.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt2lbrvphks.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2ctmszsls.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2rsidlkme.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2jxtdddwt.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt2kwcftdmf.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt2rxiqccll.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2bdycvzzo.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt2bsgozmnw.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt2mbywjpcw.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2jcpxkqvs.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt2xpxhjmsx.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt2kyempyox.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt2dubocztb.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt2ntrskgzy.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt2jvavkyem.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt2iuohtqxv.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt2qaokahdw.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt2yqypljug.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2tmakahpa.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2pqxxqtub.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2hhdnyblz.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2iazkrhkq.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt2oqqkpyeg.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt2dfghcpey.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2kwglgbag.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2guyajaas.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt2zibopgau.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xmnxfdec.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt2txehsmpp.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt2apgsqsee.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2gqtdsuzy.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2phravhnv.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2obtbmfmn.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt2ruhpovgr.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt2fweygsir.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt2vtsakbbb.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt2lbhuoqaz.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2ethhpjig.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2bxvqwpso.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2knyjyitc.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt2svoqgfxh.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt2mxczzlbq.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt2zzbksnsu.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt2tkytbiwy.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2ripvqflz.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt2kxgipfty.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt2bwsvrptk.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt2yojxjzcc.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt2wfgpcate.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2wwagxxlm.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2nmkyhjki.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2lqncqvts.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2pxbslfvn.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2xmdedmao.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt2zynadlip.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt2xjbsatah.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt2uuaqcliu.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt2gchgbjcn.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt2bdaksihk.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2eymaclyk.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt2zoipsbpo.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt2zfgnlbex.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt2oqmzpspi.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2osbkjrdq.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt2fhmcleld.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt2qybrvlos.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt2iuzlkzde.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2yyjplpfh.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2bnjqpjvb.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt2fmcwfljk.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt2gbrzsgch.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt2ibgufrnp.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt2nmblcnlu.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt2yypdoyuq.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt2vdkjtxuh.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt2sexhgjxw.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt2xsqkizqb.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt2pnjiqypw.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt2tcrwjcgm.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt2rvlowpxz.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2vbxmqzjx.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt2slmljwyx.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2hlwrmrze.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2ubfcrklr.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt2vgefrkso.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2tyclscth.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2ccgjrjsb.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt2ypgilglr.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2uetinpxd.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2ersuwxtu.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2chtmzden.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt2phuclzqp.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt2uvfnuowk.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt2xzggwcvr.html


<!-- 参考信息 -->